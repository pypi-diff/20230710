# Comparing `tmp/yt_helper-0.2.8-py3-none-any.whl.zip` & `tmp/yt_helper-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7219 bytes, number of entries: 10
--rw-rw-r--  2.0 unx     9721 b- defN 21-Apr-19 22:16 yt_helper/__init__.py
+Zip file size: 7215 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx     9713 b- defN 21-Apr-19 22:43 yt_helper/__init__.py
 -rw-rw-r--  2.0 unx      455 b- defN 20-Aug-08 21:00 yt_helper/legacy.py
 -rw-rw-r--  2.0 unx        0 b- defN 20-Aug-08 21:00 yt_helper/scripts/__init__.py
 -rw-rw-r--  2.0 unx     1595 b- defN 21-Apr-19 22:16 yt_helper/scripts/download.py
--rw-rw-r--  2.0 unx      608 b- defN 21-Apr-19 22:24 yt_helper-0.2.8.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     2669 b- defN 21-Apr-19 22:24 yt_helper-0.2.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 21-Apr-19 22:24 yt_helper-0.2.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       65 b- defN 21-Apr-19 22:24 yt_helper-0.2.8.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       10 b- defN 21-Apr-19 22:24 yt_helper-0.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      818 b- defN 21-Apr-19 22:24 yt_helper-0.2.8.dist-info/RECORD
-10 files, 16033 bytes uncompressed, 5811 bytes compressed:  63.8%
+-rw-rw-r--  2.0 unx      608 b- defN 21-Apr-19 22:48 yt_helper-0.2.9.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     2641 b- defN 21-Apr-19 22:48 yt_helper-0.2.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 21-Apr-19 22:48 yt_helper-0.2.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       65 b- defN 21-Apr-19 22:48 yt_helper-0.2.9.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       10 b- defN 21-Apr-19 22:48 yt_helper-0.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      818 b- defN 21-Apr-19 22:48 yt_helper-0.2.9.dist-info/RECORD
+10 files, 15997 bytes uncompressed, 5807 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: yt_helper/scripts/__init__.py
 Comment: 
 
 Filename: yt_helper/scripts/download.py
 Comment: 
 
-Filename: yt_helper-0.2.8.dist-info/LICENSE.txt
+Filename: yt_helper-0.2.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: yt_helper-0.2.8.dist-info/METADATA
+Filename: yt_helper-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: yt_helper-0.2.8.dist-info/WHEEL
+Filename: yt_helper-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: yt_helper-0.2.8.dist-info/entry_points.txt
+Filename: yt_helper-0.2.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: yt_helper-0.2.8.dist-info/top_level.txt
+Filename: yt_helper-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: yt_helper-0.2.8.dist-info/RECORD
+Filename: yt_helper-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yt_helper/__init__.py

```diff
@@ -175,15 +175,15 @@
                     hash_id,
                     url=url,
                     vid=vid,
                     audio=audio,
                     queries_in=queries_in,
                     dirname=dirname,
                 )
-        if QUERIES is not None and query is not '':
+        if QUERIES is not None and query != '':
             try:
                 QUERIES.add(
                     query=query,
                     basenames=[basename],
                 )
             except AssertionError:
                 hash_id = QUERIES.get_hash_id_for_unique_value(query)
@@ -194,15 +194,15 @@
                 )['basenames']
                 if basename not in basenames:
                     basenames.append(basename)
                 QUERIES.update(
                     hash_id,
                     basenames=basenames
                 )
-        if URLS is not None and url is not '':
+        if URLS is not None and url != '':
             domain = get_domain(url)
             try:
                 URLS.add(
                     url=url,
                     domain=domain,
                     basenames=[basename],
                 )
```

## Comparing `yt_helper-0.2.8.dist-info/LICENSE.txt` & `yt_helper-0.2.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `yt_helper-0.2.8.dist-info/METADATA` & `yt_helper-0.2.9.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: yt-helper
-Version: 0.2.8
+Version: 0.2.9
 Summary: Light wrapper to youtube-dl
 Home-page: https://github.com/kenjyco/yt-helper
 Author: Ken
 Author-email: kenjyco@gmail.com
 License: MIT
-Download-URL: https://github.com/kenjyco/yt-helper/tarball/v0.2.8
+Download-URL: https://github.com/kenjyco/yt-helper/tarball/v0.2.9
 Keywords: youtube-dl,youtube,download
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
@@ -24,21 +24,19 @@
 Install
 -------
 
 Install system av tools
 
 ::
 
-   % sudo apt-get install -y sox rtmpdump
-   % sudo apt-get install -y libav-tools
-   % [[ $? -ne 0 ]] && sudo apt-get install -y ffmpeg
+   % sudo apt-get install -y ffmpeg sox rtmpdump
 
    or
 
-   % brew install libav sox rtmpdump
+   % brew install ffmpeg sox rtmpdump
 
 Install with ``pip``
 
 ::
 
    % pip3 install yt-helper
 
@@ -62,14 +60,15 @@
                                240.. default 720)
      -p, --playlist            Allow downloading entire playlist
      -t, --thumbnail           Download thumbnail image of video
      -d, --description         Download description of video to a file
      -s, --subtitles           Embed subtitles in the downloaded video
      -a, --audio-only          Don't keep the video file if one was downloaded
      -m, --mp3                 Convert downloaded audio to MP3 file
+     -v, --verbose             Show extra debugging output
      --help                    Show this message and exit.
 
 Optional Installs
 -----------------
 
 Collections/models (QUERIES, URLS, FILES, COMMENTS)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```

## Comparing `yt_helper-0.2.8.dist-info/RECORD` & `yt_helper-0.2.9.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-yt_helper/__init__.py,sha256=8Hx-49rjONotXAb-d1I4XjBRhEsedEmXTVZoFyvoTpY,9721
+yt_helper/__init__.py,sha256=GeLOVsJGU8QwCsyANrFX8SH_ZDGe2ZGKP2iCxokLJA0,9713
 yt_helper/legacy.py,sha256=yYK0lf44xO1QLBFl04i-Ye9hVNq7cwn5ncfHLkfx83g,455
 yt_helper/scripts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 yt_helper/scripts/download.py,sha256=ljCYRy01xWEkVufzfXlGpEZyAFo1l9q5EmoVV3HvNfY,1595
-yt_helper-0.2.8.dist-info/LICENSE.txt,sha256=qkd6gO3_mhiG9TiDq5tJieC-1f64xFSpep3GBsIfNr0,608
-yt_helper-0.2.8.dist-info/METADATA,sha256=t8W8p8hYaORlrI9SbKs5tr88CfucD2KGm7XB9OxYw18,2669
-yt_helper-0.2.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-yt_helper-0.2.8.dist-info/entry_points.txt,sha256=uegThYT3D5-qFtBXZHjLN8WoSfhvRrDukrLa0cTQ7Hs,65
-yt_helper-0.2.8.dist-info/top_level.txt,sha256=EDIsHl1qz4yz0OZQ50TRkE2c7jmmINBqnF17U0Q5pAo,10
-yt_helper-0.2.8.dist-info/RECORD,,
+yt_helper-0.2.9.dist-info/LICENSE.txt,sha256=qkd6gO3_mhiG9TiDq5tJieC-1f64xFSpep3GBsIfNr0,608
+yt_helper-0.2.9.dist-info/METADATA,sha256=VLQ1D0eHMX_t0xtcJwGuY5cW5uMA32HIT6LV3cr_qdk,2641
+yt_helper-0.2.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+yt_helper-0.2.9.dist-info/entry_points.txt,sha256=uegThYT3D5-qFtBXZHjLN8WoSfhvRrDukrLa0cTQ7Hs,65
+yt_helper-0.2.9.dist-info/top_level.txt,sha256=EDIsHl1qz4yz0OZQ50TRkE2c7jmmINBqnF17U0Q5pAo,10
+yt_helper-0.2.9.dist-info/RECORD,,
```

