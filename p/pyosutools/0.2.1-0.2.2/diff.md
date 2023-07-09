# Comparing `tmp/pyosutools-0.2.1.tar.gz` & `tmp/pyosutools-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyosutools-0.2.1.tar", last modified: Sun Jul  9 13:26:57 2023, max compression
+gzip compressed data, was "pyosutools-0.2.2.tar", last modified: Sun Jul  9 22:08:31 2023, max compression
```

## Comparing `pyosutools-0.2.1.tar` & `pyosutools-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:26:57.829534 pyosutools-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-09 13:26:46.000000 pyosutools-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-09 13:26:57.829534 pyosutools-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:26:46.000000 pyosutools-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:26:57.825534 pyosutools-0.2.1/pyosutools/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:26:57.829534 pyosutools-0.2.1/pyosutools/beatmaps/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/beatmaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9191 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/beatmaps/beatmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/beatmaps/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:26:57.829534 pyosutools-0.2.1/pyosutools/db/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/db/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/db/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/db/osu.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/db/presence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/db/scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:26:57.829534 pyosutools-0.2.1/pyosutools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-09 13:26:57.000000 pyosutools-0.2.1/pyosutools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-09 13:26:57.000000 pyosutools-0.2.1/pyosutools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:26:57.000000 pyosutools-0.2.1/pyosutools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-09 13:26:57.000000 pyosutools-0.2.1/pyosutools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 13:26:57.000000 pyosutools-0.2.1/pyosutools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:26:57.829534 pyosutools-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:08:31.790630 pyosutools-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-09 22:08:16.000000 pyosutools-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-09 22:08:31.790630 pyosutools-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 22:08:16.000000 pyosutools-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:08:31.790630 pyosutools-0.2.2/pyosutools/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:08:31.790630 pyosutools-0.2.2/pyosutools/beatmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/beatmaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/beatmaps/beatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/beatmaps/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:08:31.790630 pyosutools-0.2.2/pyosutools/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/db/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/db/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/db/osu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/db/presence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/db/scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:08:31.790630 pyosutools-0.2.2/pyosutools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-09 22:08:31.000000 pyosutools-0.2.2/pyosutools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-09 22:08:31.000000 pyosutools-0.2.2/pyosutools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 22:08:31.000000 pyosutools-0.2.2/pyosutools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-09 22:08:31.000000 pyosutools-0.2.2/pyosutools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 22:08:31.000000 pyosutools-0.2.2/pyosutools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 22:08:31.790630 pyosutools-0.2.2/setup.cfg
```

### Comparing `pyosutools-0.2.1/LICENSE` & `pyosutools-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.1/PKG-INFO` & `pyosutools-0.2.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyosutools
-Version: 0.2.1
+Version: 0.2.2
 Summary: Parsing osu! files for easier usage
 Author-email: OlegSuperBro <olegrakovic323@gmail.com>
 Project-URL: Homepage, https://github.com/OlegSuperBro/pyosutools
 Project-URL: Bug Tracker, https://github.com/OlegSuperBro/pyosutools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyosutools-0.2.1/pyosutools/beatmaps/beatmap.py` & `pyosutools-0.2.2/pyosutools/beatmaps/beatmap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from __future__ import annotations
 import re
 from dataclasses import dataclass
 from io import TextIOWrapper
 from os import PathLike
-from typing import List, Tuple, Self, Union
+from typing import List, Tuple, Union
 
 from pyosutools.beatmaps.datatypes import (GeneralSettings, EditorSettings, Metadata, Difficulty,
                                            BaseEvent, TimingPoint, ComboColors, BaseHitObject, HitObjectType,
                                            EventType, BackgroundEvent, BreakEvent, VideoEvent,
                                            CircleObject, ManiaHoldObject, SliderObject, SpinnerObject,
                                            SliderType, CurvePoint, HitSound, HitSample)
 from pyosutools.utils import is_int
@@ -17,28 +18,28 @@
     version: int
     general_settings: GeneralSettings
     editor_settings: EditorSettings
     metadata: Metadata
     difficulty: Difficulty
     events: List[BaseEvent]
     timing_points: List[TimingPoint]
-    colours: list[ComboColors]
-    hit_objects: list[BaseHitObject]
+    colours: List[ComboColors]
+    hit_objects: List[BaseHitObject]
 
     @staticmethod
-    def from_path(path: Union[str, PathLike]) -> Self:
+    def from_path(path: Union[str, PathLike]) -> Beatmap:
         with open(path, "r") as f:
             return Beatmap.from_file(f)
 
     @staticmethod
-    def from_file(file: TextIOWrapper) -> Self:
+    def from_file(file: TextIOWrapper) -> Beatmap:
         return Beatmap.from_data(file.readlines())
 
     @staticmethod
-    def from_data(data: List[str]) -> Self:
+    def from_data(data: List[str]) -> Beatmap:
         return _Parser.parse(data)
 
 
 SECTIONS = [
     "General",
     "Editor",
     "Metadata",
@@ -79,36 +80,35 @@
         y = int(values[1])
         time = int(values[2])
         hit_object_type = HitObjectType(int(values[3]))
         hit_sound = HitSound(int(values[4]))
 
         hit_sample_data = _Parser.parse_hit_sample_data(values[-1:][0])
         hit_sample = HitSample(**hit_sample_data) if hit_sample_data is not None else None
-
-        hit_object = BaseHitObject(x, y, time, hit_sound, hit_sample)
-
-        if hit_object_type == HitObjectType["CIRCLE"]:
+        if HitObjectType["CIRCLE"] in hit_object_type:
             hit_object = CircleObject(x, y, time, hit_sound, hit_sample)
-        elif hit_object_type == HitObjectType["SLIDER"]:
-            hit_object = SliderObject(x, y, time, hit_sound, hit_sample, **_Parser.parse_slider_object_data(values[5:-1]))
-        elif hit_object_type == HitObjectType["SPINNER"]:
-            hit_object = SpinnerObject(x, y, time, hit_sound, hit_sample, **_Parser.parse_spinner_object_data(values[5:-1]))
-        elif hit_object_type == HitObjectType["MANIA_HOLD"]:
-            hit_object = ManiaHoldObject(x, y, time, hit_sound, hit_sample, **_Parser.parse_mania_hold_object_data(values[5:-1]))
+        elif HitObjectType["SLIDER"] in hit_object_type:
+            hit_object = SliderObject(x, y, time, hit_sound, hit_sample, **_Parser.parse_slider_object_data(values[5:]))
+        elif HitObjectType["SPINNER"] in hit_object_type:
+            hit_object = SpinnerObject(x, y, time, hit_sound, hit_sample, **_Parser.parse_spinner_object_data(values[5:]))
+        elif HitObjectType["MANIA_HOLD"] in hit_object_type:
+            hit_object = ManiaHoldObject(x, y, time, hit_sound, hit_sample, **_Parser.parse_mania_hold_object_data(values[5:]))
+        else:
+            hit_object = BaseHitObject(x, y, time, hit_sound, hit_sample)
 
         return hit_object
 
     @staticmethod
     def parse_slider_object_data(values: List[str]) -> dict:
         values = list(map(lambda x: x.split("|"), values))
         return {
             "curve_type": SliderType(values[0][0]),
-            "curve_points": [CurvePoint(value[0], value[1]) for value in values[0][1:]],
+            "curve_points": [CurvePoint(int(value.split(":")[0]), int(value.split(":")[1])) for value in values[0][1:]],
             "slides": int(values[1][0]),
-            "length": float(values[2][0]) if len(values) > 2 else None,
+            "length": float(values[2][0]),
             "edge_sounds": (values[3][0]) if len(values) > 3 else None,
             "edge_sets": (values[4][0]) if len(values) > 4 else None
         }
 
     @staticmethod
     def parse_spinner_object_data(values: List[str]) -> dict:
         return {
```

### Comparing `pyosutools-0.2.1/pyosutools/beatmaps/datatypes.py` & `pyosutools-0.2.2/pyosutools/beatmaps/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.1/pyosutools/datatypes.py` & `pyosutools-0.2.2/pyosutools/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.1/pyosutools/db/collection.py` & `pyosutools-0.2.2/pyosutools/db/collection.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.1/pyosutools/db/datatypes.py` & `pyosutools-0.2.2/pyosutools/db/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.1/pyosutools/db/osu.py` & `pyosutools-0.2.2/pyosutools/db/osu.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         Returns
         ----
         Beatmap
             instance of Beatmap
         """
         cursor = self.sql_beatmaps_db.cursor()
-        return Beatmap.from_sql(*cursor.execute(f"SELECT * FROM 'beatmaps' WHERE md5_hash='{hash}'").fetchone())
+        return _Parser.beatmap_from_sql(*cursor.execute(f"SELECT * FROM 'beatmaps' WHERE md5_hash='{hash}'").fetchone())
 
     def beatmaps_execute_sql(self, command) -> Any:
         """
         Executes sql command in table with beatmaps
         """
         cursor = self.sql_beatmaps_db.cursor()
         return cursor.execute(command).fetchall()
@@ -313,16 +313,40 @@
 
         return Beatmap(artist, artist_unicode, title, title_unicode, creator, difficulty, audio_file, md5_hash, osu_file, ranked_status, count_hitcircles, count_sliders,
                        count_spiners, last_modification, ar, cs, hp, od, slider_velocity, std_pairs, taiko_pairs, ctb_pairs, mania_pairs, drain_time, total_time, preview_time,
                        timing_points, difficulty_id, beatmap_id, thread_id, std_grade, taiko_grade, ctb_grade, mania_grade, local_offset, stack_laniency, gameplay_mode, song_source,
                        song_tags, online_offset, title_font, unplayed, last_played, is_osz2, folder_name, last_checked, ignore_sound, ignore_skin, disable_storyboard, disable_video,
                        visual_override, mania_scroll_speed)
 
+    @staticmethod
+    def beatmap_from_sql(*args):
+        # TODO: rewrite func cuz this one is kinda unsave
+        """
+        Get beatmap from sql row
+
+        Returns
+        ----
+        Beatmap
+            osu! beatmap
+        """
+        new_args = []
+        for arg in args:
+            if arg is None:
+                new_args.append(arg)
+                continue
+
+            if type(arg) == str and (arg[:2] == "b\'" or arg[:2] == "b\""):
+                new_args.append(pickle.loads(bytearray(eval(arg))))
+                continue
+            new_args.append(arg)
+
+        return Beatmap(*new_args)
+
 
-def parse_osudb(osudb_file: Union[str, os.PathLike, io.BytesIO], beatmaps_db: Union[str, os.PathLike] = None, skip_beatmaps: bool = False) -> Osudb:
+def parse_osudb(osudb_file: Union[str, os.PathLike, io.BytesIO], beatmaps_db: Union[str, os.PathLike] = None, skip_beatmaps: bool = False, sql_check_same_thread: bool = True) -> Osudb:
     """
     Parse osu!.db file
 
     Args
     ----
     osudb_file: str | os.PathLike | io.BytesIO
         Path or opened file
@@ -345,12 +369,12 @@
     """
     if not isinstance(osudb_file, io.BytesIO):
         osudb_file = open(osudb_file, "rb")
 
     db_connection = None
 
     if beatmaps_db is None:
-        db_connection = sqlite3.connect(tempfile.gettempdir() + "pyosudb_tmp.sql")
+        db_connection = sqlite3.connect(tempfile.gettempdir() + "pyosudb_tmp.sql", check_same_thread=sql_check_same_thread)
     else:
-        db_connection = sqlite3.connect(beatmaps_db)
+        db_connection = sqlite3.connect(beatmaps_db, check_same_thread=sql_check_same_thread)
 
     return _Parser(osudb_file).parse(db_connection, skip_beatmaps)
```

### Comparing `pyosutools-0.2.1/pyosutools/db/presence.py` & `pyosutools-0.2.2/pyosutools/db/presence.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.1/pyosutools/db/scores.py` & `pyosutools-0.2.2/pyosutools/db/scores.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.1/pyosutools/utils.py` & `pyosutools-0.2.2/pyosutools/utils.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.1/pyosutools.egg-info/PKG-INFO` & `pyosutools-0.2.2/pyosutools.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyosutools
-Version: 0.2.1
+Version: 0.2.2
 Summary: Parsing osu! files for easier usage
 Author-email: OlegSuperBro <olegrakovic323@gmail.com>
 Project-URL: Homepage, https://github.com/OlegSuperBro/pyosutools
 Project-URL: Bug Tracker, https://github.com/OlegSuperBro/pyosutools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyosutools-0.2.1/pyosutools.egg-info/SOURCES.txt` & `pyosutools-0.2.2/pyosutools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.1/pyproject.toml` & `pyosutools-0.2.2/pyproject.toml`

 * *Files identical despite different names*

