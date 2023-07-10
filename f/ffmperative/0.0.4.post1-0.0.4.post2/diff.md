# Comparing `tmp/ffmperative-0.0.4.post1-py3-none-any.whl.zip` & `tmp/ffmperative-0.0.4.post2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 12851 bytes, number of entries: 11
+Zip file size: 13980 bytes, number of entries: 11
 -rw-r--r--  2.0 unx     1532 b- defN 23-Jul-06 23:04 ffmperative/__init__.py
 -rw-r--r--  2.0 unx      824 b- defN 23-Jul-06 00:34 ffmperative/cli.py
--rw-r--r--  2.0 unx    12911 b- defN 23-Jul-10 05:17 ffmperative/extras.py
--rw-r--r--  2.0 unx    15005 b- defN 23-Jul-06 23:04 ffmperative/tools.py
+-rw-r--r--  2.0 unx    17288 b- defN 23-Jul-10 14:59 ffmperative/extras.py
+-rw-r--r--  2.0 unx    15123 b- defN 23-Jul-10 14:59 ffmperative/tools.py
 -rw-r--r--  2.0 unx      871 b- defN 23-Jul-06 23:04 ffmperative/utils.py
--rw-rw-r--  2.0 unx     1065 b- defN 23-Jul-10 05:18 ffmperative-0.0.4.post1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4253 b- defN 23-Jul-10 05:18 ffmperative-0.0.4.post1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 05:18 ffmperative-0.0.4.post1.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Jul-10 05:18 ffmperative-0.0.4.post1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Jul-10 05:18 ffmperative-0.0.4.post1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      928 b- defN 23-Jul-10 05:18 ffmperative-0.0.4.post1.dist-info/RECORD
-11 files, 37539 bytes uncompressed, 11271 bytes compressed:  70.0%
+-rw-rw-r--  2.0 unx     1065 b- defN 23-Jul-10 15:03 ffmperative-0.0.4.post2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4253 b- defN 23-Jul-10 15:03 ffmperative-0.0.4.post2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 15:03 ffmperative-0.0.4.post2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Jul-10 15:03 ffmperative-0.0.4.post2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-10 15:03 ffmperative-0.0.4.post2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      928 b- defN 23-Jul-10 15:03 ffmperative-0.0.4.post2.dist-info/RECORD
+11 files, 42034 bytes uncompressed, 12400 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: ffmperative/tools.py
 Comment: 
 
 Filename: ffmperative/utils.py
 Comment: 
 
-Filename: ffmperative-0.0.4.post1.dist-info/LICENSE
+Filename: ffmperative-0.0.4.post2.dist-info/LICENSE
 Comment: 
 
-Filename: ffmperative-0.0.4.post1.dist-info/METADATA
+Filename: ffmperative-0.0.4.post2.dist-info/METADATA
 Comment: 
 
-Filename: ffmperative-0.0.4.post1.dist-info/WHEEL
+Filename: ffmperative-0.0.4.post2.dist-info/WHEEL
 Comment: 
 
-Filename: ffmperative-0.0.4.post1.dist-info/entry_points.txt
+Filename: ffmperative-0.0.4.post2.dist-info/entry_points.txt
 Comment: 
 
-Filename: ffmperative-0.0.4.post1.dist-info/top_level.txt
+Filename: ffmperative-0.0.4.post2.dist-info/top_level.txt
 Comment: 
 
-Filename: ffmperative-0.0.4.post1.dist-info/RECORD
+Filename: ffmperative-0.0.4.post2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ffmperative/extras.py

```diff
@@ -71,28 +71,146 @@
         self.model_a, self.metadata = whisperx.load_align_model(
             language_code=language, device=self.device
         )
 
     def convert_to_srt_time(self, time: float) -> str:
         hh, rem = divmod(time, 3600)
         mm, ss = divmod(rem, 60)
-        ms = str(time).split(".")[1]
+        ms = str(time).split(".")[1][:3].ljust(3, "0")
         return "{:02d}:{:02d}:{:02d},{}".format(int(hh), int(mm), int(ss), ms)
 
-    def create_srt_content(self, result: dict) -> str:
+    def format_timestamp(
+        self,
+        seconds: float,
+        always_include_hours: bool = True,
+        decimal_marker: str = ",",
+    ):
+        assert seconds >= 0, "non-negative timestamp expected"
+        milliseconds = round(seconds * 1000.0)
+
+        hours = milliseconds // 3_600_000
+        milliseconds -= hours * 3_600_000
+
+        minutes = milliseconds // 60_000
+        milliseconds -= minutes * 60_000
+
+        seconds = milliseconds // 1_000
+        milliseconds -= seconds * 1_000
+
+        hours_marker = f"{hours:02d}:" if always_include_hours or hours > 0 else ""
+        return f"{hours_marker}{minutes:02d}:{seconds:02d}{decimal_marker}{milliseconds:03d}"
+
+    def iterate_result(self, result: dict, options: dict):
+        raw_max_line_width: Optional[int] = options["max_line_width"]
+        max_line_count: Optional[int] = options["max_line_count"]
+        highlight_words: bool = options["highlight_words"]
+        max_line_width = 1000 if raw_max_line_width is None else raw_max_line_width
+        preserve_segments = max_line_count is None or raw_max_line_width is None
+
+        def iterate_subtitles():
+            line_len = 0
+            line_count = 1
+            # the next subtitle to yield (a list of word timings with whitespace)
+            subtitle: list[dict] = []
+            times = []
+            last = result["segments"][0]["start"]
+            for segment in result["segments"]:
+                for i, original_timing in enumerate(segment["words"]):
+                    timing = original_timing.copy()
+                    long_pause = not preserve_segments
+                    if "start" in timing:
+                        long_pause = long_pause and timing["start"] - last > 3.0
+                    else:
+                        long_pause = False
+                    has_room = line_len + len(timing["word"]) <= max_line_width
+                    seg_break = i == 0 and len(subtitle) > 0 and preserve_segments
+                    if line_len > 0 and has_room and not long_pause and not seg_break:
+                        # line continuation
+                        line_len += len(timing["word"])
+                    else:
+                        # new line
+                        timing["word"] = timing["word"].strip()
+                        if (
+                            len(subtitle) > 0
+                            and max_line_count is not None
+                            and (long_pause or line_count >= max_line_count)
+                            or seg_break
+                        ):
+                            # subtitle break
+                            yield subtitle, times
+                            subtitle = []
+                            times = []
+                            line_count = 1
+                        elif line_len > 0:
+                            # line break
+                            line_count += 1
+                            timing["word"] = "\n" + timing["word"]
+                        line_len = len(timing["word"].strip())
+                    subtitle.append(timing)
+                    times.append(
+                        (segment["start"], segment["end"], segment.get("speaker"))
+                    )
+                    if "start" in timing:
+                        last = timing["start"]
+            if len(subtitle) > 0:
+                yield subtitle, times
+
+        if "words" in result["segments"][0]:
+            for subtitle, _ in iterate_subtitles():
+                sstart, ssend, speaker = _[0]
+                subtitle_start = self.format_timestamp(sstart)
+                subtitle_end = self.format_timestamp(ssend)
+                subtitle_text = " ".join([word["word"] for word in subtitle])
+                has_timing = any(["start" in word for word in subtitle])
+
+                # add [$SPEAKER_ID]: to each subtitle if speaker is available
+                prefix = ""
+                if speaker is not None:
+                    prefix = f"[{speaker}]: "
+
+                if highlight_words and has_timing:
+                    last = subtitle_start
+                    all_words = [timing["word"] for timing in subtitle]
+                    for i, this_word in enumerate(subtitle):
+                        if "start" in this_word:
+                            start = self.format_timestamp(this_word["start"])
+                            end = self.format_timestamp(this_word["end"])
+                            if last != start:
+                                yield last, start, subtitle_text
+
+                            yield start, end, prefix + " ".join(
+                                [
+                                    re.sub(r"^(\s*)(.*)$", r"\1<u>\2</u>", word)
+                                    if j == i
+                                    else word
+                                    for j, word in enumerate(all_words)
+                                ]
+                            )
+                            last = end
+                else:
+                    yield subtitle_start, subtitle_end, prefix + subtitle_text
+        else:
+            for segment in result["segments"]:
+                segment_start = self.format_timestamp(segment["start"])
+                segment_end = self.format_timestamp(segment["end"])
+                segment_text = segment["text"].strip().replace("-->", "->")
+                if "speaker" in segment:
+                    segment_text = f"[{segment['speaker']}]: {segment_text}"
+                yield segment_start, segment_end, segment_text
+
+    def create_srt_content(self, result: dict, highlight_words: bool) -> str:
         srt_content = []
-        for idx, js in enumerate(result["segments"]):
-            start_time, end_time = (
-                self.convert_to_srt_time(js["start"]),
-                self.convert_to_srt_time(js["end"]),
-            )
+        options = {
+            "max_line_width": None,
+            "max_line_count": None,
+            "highlight_words": highlight_words,
+        }
+        for idx, (start, end, text) in enumerate(self.iterate_result(result, options)):
             srt_content.append(
-                "{}\n{} --> {}\n{}\n\n".format(
-                    idx + 1, start_time, end_time, js["text"]
-                )
+                "{}\n{} --> {}\n{}\n\n".format(idx + 1, start, end, text)
             )
         return "".join(srt_content)
 
     def write_to_srt(self, srt_path: str, srt_content: str):
         with open(srt_path, "w") as outfile:
             outfile.write(srt_content)
 
@@ -107,62 +225,36 @@
             self.model_a,
             self.metadata,
             audio,
             self.device,
             return_char_alignments=False,
         )
 
-    def generate_srt(self, input_path: str, srt_path: str, batch_size: int = 16):
+    def generate_srt(
+        self,
+        input_path: str,
+        srt_path: str,
+        highlight_words: bool = True,
+        batch_size: int = 16,
+    ):
         transcribed_result = self.transcribe_audio(input_path, batch_size)
         aligned_result = self.align_audio(
             transcribed_result["segments"], audio=whisperx.load_audio(input_path)
         )
-        srt_content = self.create_srt_content(aligned_result)
+        srt_content = self.create_srt_content(aligned_result, highlight_words)
         self.write_to_srt(srt_path, srt_content)
 
     def __call__(
         self,
         input_path,
         output_path,
         highlight_words: bool = True,
         batch_size: int = 16,
     ):
-        if not highlight_words:
-            self.generate_srt(input_path, output_path, batch_size)
-        else:
-            audio = whisperx.load_audio(input_path)
-            result = self.model.transcribe(audio, batch_size=batch_size)
-            result = whisperx.align(
-                result["segments"],
-                self.model_a,
-                self.metadata,
-                audio,
-                self.device,
-                return_char_alignments=False,
-            )
-
-            with open(output_path, "w") as outfile:
-                for idx, segment in enumerate(result["segments"]):
-                    start_time_srt = self.convert_to_srt_time(segment["start"])
-                    end_time_srt = self.convert_to_srt_time(segment["end"])
-
-                    words = []
-                    for word_timing in segment["words"]:
-                        words.append(word_timing["word"])
-
-                    highlighted_text = " ".join(
-                        ["<u>" + word + "</u>" if j == idx else word for j, word in enumerate(words)]
-                    )
-
-                    # Write to SRT file
-                    outfile.write(
-                        "{}\n{} --> {}\n{}\n\n".format(
-                            idx + 1, start_time_srt, end_time_srt, highlighted_text
-                        )
-                    )
+        self.generate_srt(input_path, output_path, highlight_words, batch_size)
 
 
 class VideoAutoCropTool(Tool):
     name = "auto_crop_tool"
     description = """
     This tool automatically crops a video.
     Inputs are input_path as a string and output_path as a string.
```

## ffmperative/tools.py

```diff
@@ -39,21 +39,20 @@
     inputs = ["text", "text", "text"]
     outputs = ["None"]
 
     def __call__(self, input_path: str, audio_path: str, output_path: str):
         input_video = ffmpeg.input(input_path)
         added_audio = ffmpeg.input(audio_path)
 
-        merged_audio = ffmpeg.filter([input_video.audio, added_audio], "amix")
-
-        (
-            ffmpeg.concat(input_video, merged_audio, v=1, a=1)
-            .output(output_path)
-            .run(overwrite_output=True)
-        )
+        if has_audio(input_path):
+            merged_audio = ffmpeg.filter([input_video.audio, added_audio], "amix")
+            output_video = ffmpeg.concat(input_video, merged_audio, v=1, a=1)
+        else:
+            output_video = ffmpeg.concat(input_video, added_audio, v=1, a=1)
+        output_video.output(output_path).run(overwrite_output=True)
 
 
 class FFProbeTool(Tool):
     name = "ffprobe_tool"
     description = """
     This tool extracts metadata from input video using ffmpeg/ffprobe
     Input is input_path and output is video metadata as JSON.
```

## Comparing `ffmperative-0.0.4.post1.dist-info/LICENSE` & `ffmperative-0.0.4.post2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ffmperative-0.0.4.post1.dist-info/METADATA` & `ffmperative-0.0.4.post2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmperative
-Version: 0.0.4.post1
+Version: 0.0.4.post2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pillow
 Requires-Dist: opencv-python
 Requires-Dist: ffprobe-python
 Requires-Dist: ffmpeg-python
```

