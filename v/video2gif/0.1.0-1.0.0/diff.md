# Comparing `tmp/video2gif-0.1.0.tar.gz` & `tmp/video2gif-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video2gif-0.1.0.tar", max compression
+gzip compressed data, was "video2gif-1.0.0.tar", max compression
```

## Comparing `video2gif-0.1.0.tar` & `video2gif-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34523 2017-09-30 07:16:25.000000 video2gif-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-07-08 23:35:40.530776 video2gif-0.1.0/README.md
--rw-r--r--   0        0        0      494 2023-07-10 14:21:33.711634 video2gif-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-08 23:35:40.530776 video2gif-0.1.0/video2gif/__init__.py
--rw-r--r--   0        0        0     1666 2023-07-10 05:33:54.748338 video2gif-0.1.0/video2gif/main.py
--rw-r--r--   0        0        0      417 1970-01-01 00:00:00.000000 video2gif-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2017-09-30 07:16:25.000000 video2gif-1.0.0/LICENSE
+-rw-r--r--   0        0        0      248 2023-07-10 16:26:35.138429 video2gif-1.0.0/README.md
+-rw-r--r--   0        0        0      615 2023-07-10 17:57:13.088588 video2gif-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-08 23:35:40.530776 video2gif-1.0.0/video2gif/__init__.py
+-rw-r--r--   0        0        0     2204 2023-07-10 17:54:51.762697 video2gif-1.0.0/video2gif/main.py
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 video2gif-1.0.0/PKG-INFO
```

### Comparing `video2gif-0.1.0/LICENSE` & `video2gif-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `video2gif-0.1.0/video2gif/main.py` & `video2gif-1.0.0/video2gif/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,55 @@
 import argparse
+import datetime
 import ffmpeg
 import os
-import yt_dlp
 import validators
+import yt_dlp
 
 parser = argparse.ArgumentParser()
 parser.add_argument("video", help="url or path of the video you'd like to gif-ify")
-parser.add_argument("start", type=int, help="start time in seconds")
-parser.add_argument("end", type=int, help="end time in seconds")
+parser.add_argument("start", type=lambda d: datetime.datetime.strptime(d, '%M:%S'), help="start time in minutes:seconds")
+parser.add_argument("end", type=lambda d: datetime.datetime.strptime(d, '%M:%S'), help="end time in minutes:seconds")
 args = parser.parse_args()
 
+start_sec = int(datetime.timedelta(minutes=args.start.minute, seconds=args.start.second).total_seconds())
+end_sec = int(datetime.timedelta(minutes=args.end.minute, seconds=args.end.second).total_seconds())
+
 if validators.url(args.video):
     URLS = [args.video]
     if os.path.exists("result/inter.mp4"):
         os.remove("result/inter.mp4")
     ydl_opts = {'final_ext': 'mkv',
-                'download_ranges': yt_dlp.utils.download_range_func([], [[args.start, args.end]]),
+                'download_ranges': yt_dlp.utils.download_range_func([], [[start_sec, end_sec]]),
                 'format': 'bv*[ext=mp4]+ba[ext=vorbis]/b[ext=mp4] / bv*+ba/b',
                 'outtmpl': {'default': 'result/inter.mp4'}}
 
     with yt_dlp.YoutubeDL(ydl_opts) as ydl:
         ydl.download(URLS)
     stream = ffmpeg.input('result/inter.mp4')
 else:
     stream = ffmpeg.input(args.video)
-    
-        
-# stream = ffmpeg.input('result/inter.mkv')
+
 stream = ffmpeg.filter(stream, 'scale', height=300, width=-2).output('result/inter-scale.mp4').run(overwrite_output=True)
 stream = ffmpeg.input('result/inter-scale.mp4').filter('palettegen', stats_mode='full').output('result/palettegen_full.png')
 stream = ffmpeg.run(stream, overwrite_output=True)
 stream = ffmpeg.filter(
          [
             ffmpeg.input('result/inter-scale.mp4'),
             ffmpeg.input('result/palettegen_full.png'),
-         
+
          ],
          filter_name='paletteuse',
          dither='heckbert',
          new='False',
          )
-stream = ffmpeg.output(stream, 'result/output.gif',framerate=30)
+stream = ffmpeg.output(stream, 'result/output.gif', framerate=30)
+
 
 def run() -> None:
     stream.run(overwrite_output=True)
+    if os.path.exists("result/inter.mp4"):
+        os.remove("result/inter.mp4")
+    if os.path.exists("result/inter-scale.mp4"):
+        os.remove("result/inter-scale.mp4")
+    if os.path.exists("result/palettegen_full.png"):
+        os.remove("result/palettegen_full.png")
```

