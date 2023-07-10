# Comparing `tmp/showcues-1.0.7.tar.gz` & `tmp/showcues-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "showcues-1.0.7.tar", last modified: Mon Jun 26 08:33:59 2023, max compression
+gzip compressed data, was "showcues-1.0.9.tar", last modified: Mon Jul 10 21:28:41 2023, max compression
```

## Comparing `showcues-1.0.7.tar` & `showcues-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-26 08:33:59.238585 showcues-1.0.7/
--rw-r--r--   0 a         (1000) a         (1000)      593 2023-06-26 08:33:59.238585 showcues-1.0.7/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)        0 2023-06-20 17:59:12.000000 showcues-1.0.7/README.md
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-26 08:33:59.234585 showcues-1.0.7/bin/
--rwxr-xr-x   0 a         (1000) a         (1000)       86 2023-06-20 17:41:41.000000 showcues-1.0.7/bin/showcues
--rw-r--r--   0 a         (1000) a         (1000)       38 2023-06-26 08:33:59.238585 showcues-1.0.7/setup.cfg
--rw-r--r--   0 a         (1000) a         (1000)     1096 2023-06-25 18:07:35.000000 showcues-1.0.7/setup.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-26 08:33:59.238585 showcues-1.0.7/showcues.egg-info/
--rw-r--r--   0 a         (1000) a         (1000)      593 2023-06-26 08:33:59.000000 showcues-1.0.7/showcues.egg-info/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)      202 2023-06-26 08:33:59.000000 showcues-1.0.7/showcues.egg-info/SOURCES.txt
--rw-r--r--   0 a         (1000) a         (1000)        1 2023-06-26 08:33:59.000000 showcues-1.0.7/showcues.egg-info/dependency_links.txt
--rw-r--r--   0 a         (1000) a         (1000)       50 2023-06-26 08:33:59.000000 showcues-1.0.7/showcues.egg-info/requires.txt
--rw-r--r--   0 a         (1000) a         (1000)        9 2023-06-26 08:33:59.000000 showcues-1.0.7/showcues.egg-info/top_level.txt
--rw-r--r--   0 a         (1000) a         (1000)    14262 2023-06-26 08:18:34.000000 showcues-1.0.7/showcues.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-07-10 21:28:41.349184 showcues-1.0.9/
+-rw-r--r--   0 a         (1000) a         (1000)      593 2023-07-10 21:28:41.349184 showcues-1.0.9/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)        0 2023-06-20 17:59:12.000000 showcues-1.0.9/README.md
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-07-10 21:28:41.345184 showcues-1.0.9/bin/
+-rwxr-xr-x   0 a         (1000) a         (1000)       86 2023-06-20 17:41:41.000000 showcues-1.0.9/bin/showcues
+-rw-r--r--   0 a         (1000) a         (1000)       38 2023-07-10 21:28:41.349184 showcues-1.0.9/setup.cfg
+-rw-r--r--   0 a         (1000) a         (1000)     1096 2023-06-25 18:07:35.000000 showcues-1.0.9/setup.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-07-10 21:28:41.349184 showcues-1.0.9/showcues.egg-info/
+-rw-r--r--   0 a         (1000) a         (1000)      593 2023-07-10 21:28:41.000000 showcues-1.0.9/showcues.egg-info/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)      202 2023-07-10 21:28:41.000000 showcues-1.0.9/showcues.egg-info/SOURCES.txt
+-rw-r--r--   0 a         (1000) a         (1000)        1 2023-07-10 21:28:41.000000 showcues-1.0.9/showcues.egg-info/dependency_links.txt
+-rw-r--r--   0 a         (1000) a         (1000)       50 2023-07-10 21:28:41.000000 showcues-1.0.9/showcues.egg-info/requires.txt
+-rw-r--r--   0 a         (1000) a         (1000)        9 2023-07-10 21:28:41.000000 showcues-1.0.9/showcues.egg-info/top_level.txt
+-rw-r--r--   0 a         (1000) a         (1000)    14662 2023-07-10 21:28:08.000000 showcues-1.0.9/showcues.py
```

### Comparing `showcues-1.0.7/PKG-INFO` & `showcues-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showcues
-Version: 1.0.7
+Version: 1.0.9
 Summary: showcues displays HLS CUE-IN and CUE-OUT tags with wallclock time
 Home-page: https://github.com/futzu/showcues
 Author: Adrian of Doom.
 Author-email: spam@iodisco.com
 Platform: all
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `showcues-1.0.7/setup.py` & `showcues-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `showcues-1.0.7/showcues.egg-info/PKG-INFO` & `showcues-1.0.9/showcues.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showcues
-Version: 1.0.7
+Version: 1.0.9
 Summary: showcues displays HLS CUE-IN and CUE-OUT tags with wallclock time
 Home-page: https://github.com/futzu/showcues
 Author: Adrian of Doom.
 Author-email: spam@iodisco.com
 Platform: all
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `showcues-1.0.7/showcues.py` & `showcues-1.0.9/showcues.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,34 +96,36 @@
 class CuePuller:
     MEDIA_COUNT = 111
 
     def __init__(self):
         self.cues = []
         self.media = []
         self.media_count = 101
-        self.sidecar_file = "cp_sidecar.txt"
+        self.sidecar = "sidecar.txt"
         self.base_uri = None
         self.iv = None
         self.key_uri = None
         self.last_iv = None
         self.last_key_uri = None
         self.event_id = 1
         self.break_timer = None
         self.break_duration = None
-        self.m3u8 = "cp.m3u8"
+        self.m3u8 = "index.m3u8"
         self.lines = []
         self.reload = True
         self.sleep_duration = 0
         self.window_size = None
         self.sliding_window = None
         self.cue_state = None
         self.last_cue = None
         self.headers = []
         self.pts = None
         self.hls_pts = "HLS"
+        with open(self.sidecar, "w+") as sidecar:  # touch sidecar
+            pass
 
     def chk_aes(self, line):
         """
         chk_aes checks for AES encryption
         """
         if "#EXT-X-KEY" in line:
             tags = TagParser([line]).tags
@@ -136,71 +138,76 @@
                     self.iv = tags["#EXT-X-KEY"]["IV"]
 
     def six2five(self, cuein):
         """
         six2five converts Time Signals (type 6)
         to SpliceInserts (type 5)
         """
-        upid_starts = [0x34, 0x36, 0x38]
-        upid_stops = [0x35, 0x37, 0x39]
+        seg_starts = [0x22, 0x30, 0x32, 0x34, 0x36, 0x38, 0x3A, 0x3C, 0x3E, 0x44, 0x46]
+        seg_stops = [0x23, 0x31, 0x33, 0x35, 0x37, 0x39, 0x3B, 0x3D, 0x3F, 0x45, 0x47]
         cue = threefive.Cue(cuein)
         cue.decode()
-        if cue.command.command_type == 5:
-            return cue.encode()
-        pts = None
-        duration = None
-        out = False
-        event_id = self.event_id
-        if cue.command.pts_time:
-            pts = cue.command.pts_time
-        for dscptr in cue.descriptors:
-            if dscptr.tag == 2:
-                if dscptr.segmentation_event_id:
-                    event_id = int(dscptr.segmentation_event_id, 16) & (2 ^ 31)
-                    if dscptr.segmentation_type_id in upid_starts:
-                        if dscptr.segmentation_duration_flag:
-                            duration = dscptr.segmentation_duration
-                            out = True
-                    else:
-                        if dscptr.segmentation_type_id in upid_stops:
-                            out = False
-        new_cue = threefive.encode.mk_splice_insert(event_id, pts, duration, out)
-        new_cue.descriptors = cue.descriptors
-        cue = new_cue
-        if cue.command.splice_immediate_flag:
-            print("Splice Immediate")
-        if cue.command.out_of_network_indicator:
-            if self.break_timer is None:
-                self.break_timer = 0.0
-        if cue.command.break_duration:
-            self.break_duration = cue.command.break_duration
+        if cue.command.command_type == 6:
+            pts = None
+            duration = None
+            out = False
+            event_id = self.event_id
+            if cue.command.pts_time:
+                pts = cue.command.pts_time
+            for dscptr in cue.descriptors:
+                if dscptr.tag == 2:
+                    if dscptr.segmentation_event_id:
+                        event_id = int(dscptr.segmentation_event_id, 16) & (2 ^ 31)
+                        if dscptr.segmentation_type_id in seg_starts:
+                            if dscptr.segmentation_duration_flag:
+                                duration = dscptr.segmentation_duration
+                                out = True
+                        else:
+                            if dscptr.segmentation_type_id in seg_stops:
+                                out = False
+            new_cue = threefive.encode.mk_splice_insert(event_id, pts, duration, out)
+            new_cue.descriptors = cue.descriptors
+            cue = new_cue
+            if cue.command.splice_immediate_flag:
+                print("Splice Immediate")
+            if cue.command.out_of_network_indicator:
+                if self.break_timer is None:
+                    self.break_timer = 0.0
+            if cue.command.break_duration:
+                self.break_duration = cue.command.break_duration
+        with open(self.sidecar, "a") as sidecar:
+            sidecar.write(f"{cue.command.pts_time},{cue.encode()}")
         return cue.encode()
 
     def add_cue(self, cue, line):
         """
         add_cue determines cue_state and
         calls six2five to replace time signals
         """
         cue = cue.replace("\r", "").replace("\n", "")
         if "CONT" not in line:
-            cue_stuff = f"{REV}{self.cue_state}{NORM} {cue} "
-            media_stuff = f"\n{REV}Media:{NORM} {self.media[-1]}\n"
+            cue_stuff = f"{REV}{self.cue_state}{NORM} "
+            media_stuff = f"\nMedia: {self.media[-1]}\n"
             if cue == "#EXT-X-CUE-IN":
                 self.cue_state = "IN"
-                diff_stuff = f" {REV}Diff:{NORM} {round(self.break_timer - self.break_duration,3)}"
-                print(f"{iso8601()} {cue_stuff} {diff_stuff}{media_stuff}")
+                diff_stuff = (
+                    f"\nDiff: {round(self.break_timer - self.break_duration,3)}"
+                )
+                print(f"{iso8601()} {cue_stuff}{diff_stuff}{media_stuff}")
                 self.reset_break()
                 return line
             if cue.startswith("#EXT-X-CUE-OUT"):
                 self.break_timer == 0.0
                 try:
                     self.break_duration = atoif(line.split(":")[1])
                 finally:
                     self.cue_state = "OUT"
-                print(f"{iso8601()} {cue_stuff} {REV}Duration:{NORM} {self.break_duration} {media_stuff}")
+                print(
+                    f"{iso8601()} {cue_stuff}\nDuration: {self.break_duration} {media_stuff}"
+                )
                 return line
         cue2 = self.six2five(cue)
         cue2data = Cue(cue2)
         cue2data.decode()
         line = line.replace(cue, cue2)
         return line
 
@@ -212,42 +219,41 @@
         cont_tags = tags["#EXT-X-CUE-OUT-CONT"]
         if self.cue_state in ["OUT", "CONT"]:
             self.cue_state = "CONT"
             if self.cue_state == "OUT" and self.break_timer is None:
                 if "ElapsedTime" in cont_tags:
                     self.break_timer = cont_tags["ElapsedTime"]
                     print("setting break timer to ", cont_tags["ElapsedTime"])
-
                 if "Duration" in cont_tags:
                     self.break_duration = cont_tags["Duration"]
             return line
         return "## " + line
 
     def chk_x_cue_in(self, line):
         if self.cue_state == "CONT":
             if self.break_timer is not None:
                 self.cue_state = "IN"
-                val = self.add_cue(line, line)
+                line = self.add_cue(line, line)
                 self.reset_break()
-                return val
+                return line
         return "## " + line
 
     def chk_x_cue_out(self, line):
         """
         chk_x_cue_out processes
         #EXT-X-CUE-OUT tags
         """
         if self.cue_state is None:
             self.reset_break()
             self.cue_state = "OUT"
             if self.break_timer is None:
                 self.break_timer = 0.0
             if ":" in line:
                 self.break_duration = atoif(line.split(":")[1])
-               # print("Duration:", self.break_duration)
+            # print("Duration:", self.break_duration)
             return self.add_cue(line, line)
         return "## " + line
 
     def chk_x_scte35(self, tags, line):
         if "CUE" in tags["#EXT-X-SCTE35"]:
             return self.add_cue(tags["#EXT-X-SCTE35"]["CUE"], line)
         return line
@@ -282,15 +288,15 @@
         auto_cuein handles cue.command.autoreturn
         """
         if self.cue_state == "CONT":
             if self.break_timer and self.break_duration:
                 if self.break_timer >= self.break_duration:
                     self.cue_state = "IN"
                     print(
-                        f"{iso8601()} {REV}AUTO{NORM} #EXT-X-CUE-IN{REV}Diff:{NORM}{round(self.break_timer - self.break_duration,3)} \n{REV}Media:{NORM} {self.media[-1]}\n"
+                        f"{iso8601()} {REV}AUTO CUE-IN{NORM}\nDiff: {round(self.break_timer - self.break_duration,3)}\nMedia: {self.media[-1]}\n"
                     )
                     self.reset_break()
                     return "\n#AUTO\n#EXT-X-CUE-IN\n" + line
         return line
 
     def reset_break(self):
         """
@@ -402,40 +408,40 @@
                         if not media.startswith("http"):
                             media = self.base_uri + "/" + media
                         if self.new_media(media):
                             lines = [self.parse_line(line) for line in lines]
                             pane = Pane(media, lines)
                             self.sliding_window.slide_panes(pane)
                         lines = []
-            ##            with open(self.m3u8, "w") as out:
-            ##                out.write("#EXTM3U\n")
-            ##                out.write("".join(self.headers))
-            ##                out.write(self.sliding_window.all_panes())
+                        with open(self.m3u8, "w") as out:
+                            out.write("#EXTM3U\n")
+                            out.write("".join(self.headers))
+                            out.write(self.sliding_window.all_panes())
             self.update_cue_state()
             time.sleep(self.sleep_duration)
 
 
 def cli():
-    playlists=None
+    playlists = None
     m3u8 = None
     with reader(sys.argv[1]) as arg:
         variants = [line for line in arg if b"#EXT-X-STREAM-INF" in line]
         if variants:
             fu = M3uFu()
-            reload =False
+            reload = False
             fu.m3u8 = sys.argv[1]
             fu.decode()
             playlists = [
-                segment for segment in fu.segments if "#EXT-X-STREAM-INF" in segment.tags
+                segment
+                for segment in fu.segments
+                if "#EXT-X-STREAM-INF" in segment.tags
             ]
     if playlists:
         m3u8 = playlists[0].media
     else:
         m3u8 = sys.argv[1]
     cp = CuePuller()
     cp.pull(m3u8)
 
 
-
-
 if __name__ == "__main__":
     cli()
```

