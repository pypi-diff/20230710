# Comparing `tmp/mocp-0.4.8-py3-none-any.whl.zip` & `tmp/mocp-0.4.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5161 bytes, number of entries: 6
--rw-rw-r--  2.0 unx     7426 b- defN 21-Dec-12 04:43 moc/__init__.py
--rw-rw-r--  2.0 unx     2240 b- defN 22-Apr-10 15:56 mocp-0.4.8.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     1801 b- defN 22-Apr-10 15:56 mocp-0.4.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Apr-10 15:56 mocp-0.4.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        4 b- defN 22-Apr-10 15:56 mocp-0.4.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      446 b- defN 22-Apr-10 15:56 mocp-0.4.8.dist-info/RECORD
-6 files, 12009 bytes uncompressed, 4357 bytes compressed:  63.7%
+Zip file size: 5322 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx     7424 b- defN 22-Apr-12 19:38 moc/__init__.py
+-rw-rw-r--  2.0 unx     2240 b- defN 22-Apr-12 23:32 mocp-0.4.9.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     2261 b- defN 22-Apr-12 23:32 mocp-0.4.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Apr-12 23:32 mocp-0.4.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        4 b- defN 22-Apr-12 23:32 mocp-0.4.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      446 b- defN 22-Apr-12 23:32 mocp-0.4.9.dist-info/RECORD
+6 files, 12467 bytes uncompressed, 4518 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: moc/__init__.py
 Comment: 
 
-Filename: mocp-0.4.8.dist-info/LICENSE.txt
+Filename: mocp-0.4.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: mocp-0.4.8.dist-info/METADATA
+Filename: mocp-0.4.9.dist-info/METADATA
 Comment: 
 
-Filename: mocp-0.4.8.dist-info/WHEEL
+Filename: mocp-0.4.9.dist-info/WHEEL
 Comment: 
 
-Filename: mocp-0.4.8.dist-info/top_level.txt
+Filename: mocp-0.4.9.dist-info/top_level.txt
 Comment: 
 
-Filename: mocp-0.4.8.dist-info/RECORD
+Filename: mocp-0.4.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## moc/__init__.py

```diff
@@ -92,15 +92,15 @@
     if 'fatal_error' in current_info:
         return ''
     elif 'timeout' in current_info:
         return ''
     elif current_info.get('state') == 'STOP':
         return ''
 
-    # add_current_to_FILES()
+    add_current_to_FILES()
     return make_string(current_info)
 
 
 def find_audio(*paths):
     """Return a list of audio files from the given paths
 
     - paths: filename and dirname globs that either are audio files, or contain
```

## Comparing `mocp-0.4.8.dist-info/LICENSE.txt` & `mocp-0.4.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `mocp-0.4.8.dist-info/METADATA` & `mocp-0.4.9.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mocp
-Version: 0.4.8
+Version: 0.4.9
 Summary: A Python library to control the MOC (music on console) audio player
 Home-page: https://github.com/kenjyco/mocp
+Download-URL: https://github.com/kenjyco/mocp/tarball/v0.4.9
 Author: Ken
 Author-email: kenjyco@gmail.com
 License: MIT
-Download-URL: https://github.com/kenjyco/mocp/tarball/v0.4.8
 Keywords: moc,mocp,cli,command-line,console audio,mp3 player,kenjyco
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
@@ -18,14 +18,16 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE.txt
 Requires-Dist: bg-helper
 Requires-Dist: input-helper
+Provides-Extra: extras
+Requires-Dist: yt-helper[redis-helper] ; extra == 'extras'
 
 Install
 -------
 
 Install the actual `MOC player/server <https://moc.daper.net/>`__
 
 ::
@@ -38,14 +40,34 @@
 
 Then install this package with ``pip``
 
 ::
 
    % pip3 install mocp
 
+Optional Installs
+-----------------
+
+redis-helper and yt-helper
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+If redis-helper and yt-helper are installed, the FILES collection will
+be updated with the basename of the the current playing file whenever
+``moc.info_string()`` is called
+
+Install with ``pip``
+
+::
+
+   % pip3 install "yt-helper[redis-helper]"
+
+   or
+
+   % pip3 install "mocp[extras]"
+
 Usage
 -----
 
 .. code:: python
 
    In [1]: import moc
```

