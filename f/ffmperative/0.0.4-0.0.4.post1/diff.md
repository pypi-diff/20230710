# Comparing `tmp/ffmperative-0.0.4-py3-none-any.whl.zip` & `tmp/ffmperative-0.0.4.post1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 12762 bytes, number of entries: 11
+Zip file size: 12851 bytes, number of entries: 11
 -rw-r--r--  2.0 unx     1532 b- defN 23-Jul-06 23:04 ffmperative/__init__.py
 -rw-r--r--  2.0 unx      824 b- defN 23-Jul-06 00:34 ffmperative/cli.py
--rw-r--r--  2.0 unx    12892 b- defN 23-Jul-10 04:10 ffmperative/extras.py
+-rw-r--r--  2.0 unx    12911 b- defN 23-Jul-10 05:17 ffmperative/extras.py
 -rw-r--r--  2.0 unx    15005 b- defN 23-Jul-06 23:04 ffmperative/tools.py
 -rw-r--r--  2.0 unx      871 b- defN 23-Jul-06 23:04 ffmperative/utils.py
--rw-rw-r--  2.0 unx     1065 b- defN 23-Jul-10 04:18 ffmperative-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     4247 b- defN 23-Jul-10 04:18 ffmperative-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 04:18 ffmperative-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Jul-10 04:18 ffmperative-0.0.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Jul-10 04:18 ffmperative-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      892 b- defN 23-Jul-10 04:18 ffmperative-0.0.4.dist-info/RECORD
-11 files, 37478 bytes uncompressed, 11254 bytes compressed:  70.0%
+-rw-rw-r--  2.0 unx     1065 b- defN 23-Jul-10 05:18 ffmperative-0.0.4.post1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4253 b- defN 23-Jul-10 05:18 ffmperative-0.0.4.post1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 05:18 ffmperative-0.0.4.post1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Jul-10 05:18 ffmperative-0.0.4.post1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-10 05:18 ffmperative-0.0.4.post1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      928 b- defN 23-Jul-10 05:18 ffmperative-0.0.4.post1.dist-info/RECORD
+11 files, 37539 bytes uncompressed, 11271 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: ffmperative/tools.py
 Comment: 
 
 Filename: ffmperative/utils.py
 Comment: 
 
-Filename: ffmperative-0.0.4.dist-info/LICENSE
+Filename: ffmperative-0.0.4.post1.dist-info/LICENSE
 Comment: 
 
-Filename: ffmperative-0.0.4.dist-info/METADATA
+Filename: ffmperative-0.0.4.post1.dist-info/METADATA
 Comment: 
 
-Filename: ffmperative-0.0.4.dist-info/WHEEL
+Filename: ffmperative-0.0.4.post1.dist-info/WHEEL
 Comment: 
 
-Filename: ffmperative-0.0.4.dist-info/entry_points.txt
+Filename: ffmperative-0.0.4.post1.dist-info/entry_points.txt
 Comment: 
 
-Filename: ffmperative-0.0.4.dist-info/top_level.txt
+Filename: ffmperative-0.0.4.post1.dist-info/top_level.txt
 Comment: 
 
-Filename: ffmperative-0.0.4.dist-info/RECORD
+Filename: ffmperative-0.0.4.post1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ffmperative/extras.py

```diff
@@ -146,15 +146,15 @@
                     end_time_srt = self.convert_to_srt_time(segment["end"])
 
                     words = []
                     for word_timing in segment["words"]:
                         words.append(word_timing["word"])
 
                     highlighted_text = " ".join(
-                        ["<u>" + word + "</u>" if word == w else w for w in words]
+                        ["<u>" + word + "</u>" if j == idx else word for j, word in enumerate(words)]
                     )
 
                     # Write to SRT file
                     outfile.write(
                         "{}\n{} --> {}\n{}\n\n".format(
                             idx + 1, start_time_srt, end_time_srt, highlighted_text
                         )
```

## Comparing `ffmperative-0.0.4.dist-info/LICENSE` & `ffmperative-0.0.4.post1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ffmperative-0.0.4.dist-info/METADATA` & `ffmperative-0.0.4.post1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmperative
-Version: 0.0.4
+Version: 0.0.4.post1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pillow
 Requires-Dist: opencv-python
 Requires-Dist: ffprobe-python
 Requires-Dist: ffmpeg-python
```

## Comparing `ffmperative-0.0.4.dist-info/RECORD` & `ffmperative-0.0.4.post1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ffmperative/__init__.py,sha256=AXShixp1GHDzduK8D3dKtxz4dNzb0d_UzksCZ-RGpuA,1532
 ffmperative/cli.py,sha256=zWNAPc4C2PDh1bsiXS8EdaZTB3FXFLLPUudupJ7lWos,824
-ffmperative/extras.py,sha256=tjvI6NE-q-HWVjVqOH7qsHh_AZ8D1rehy2D39slPqkM,12892
+ffmperative/extras.py,sha256=-I0ly79_Za5CybAWT7RZCom2SIjQfs2bw1hylo_A_hU,12911
 ffmperative/tools.py,sha256=aNG9Zx2CqzfrYPNBJ6pLL-sdj0JvOZcI00nM_BHbcIQ,15005
 ffmperative/utils.py,sha256=3gQgMH5r_lAMHd1RL27zVuH9zFHt_sgQda-beLGTZ3k,871
-ffmperative-0.0.4.dist-info/LICENSE,sha256=08y6UINXSwNc7rrPXbxA230VfE0-lkbr8zGvSqanfmk,1065
-ffmperative-0.0.4.dist-info/METADATA,sha256=F6C-V5d_0X3UikJzsLcPrarBOvPiNs-9Exucv9V5wEk,4247
-ffmperative-0.0.4.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-ffmperative-0.0.4.dist-info/entry_points.txt,sha256=5VG0BRql3f4fUVawJbLCMCqR_miu4qBwdD1xHXRTkXA,46
-ffmperative-0.0.4.dist-info/top_level.txt,sha256=phfS7dNhucv5MTBeH67o-vzt6OSYjgxuFVEA6-mbTxY,12
-ffmperative-0.0.4.dist-info/RECORD,,
+ffmperative-0.0.4.post1.dist-info/LICENSE,sha256=08y6UINXSwNc7rrPXbxA230VfE0-lkbr8zGvSqanfmk,1065
+ffmperative-0.0.4.post1.dist-info/METADATA,sha256=3hY2M6P3OXr_zqrP205rBq4ybIXaM5pNPpZtcdyxvDY,4253
+ffmperative-0.0.4.post1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+ffmperative-0.0.4.post1.dist-info/entry_points.txt,sha256=5VG0BRql3f4fUVawJbLCMCqR_miu4qBwdD1xHXRTkXA,46
+ffmperative-0.0.4.post1.dist-info/top_level.txt,sha256=phfS7dNhucv5MTBeH67o-vzt6OSYjgxuFVEA6-mbTxY,12
+ffmperative-0.0.4.post1.dist-info/RECORD,,
```

