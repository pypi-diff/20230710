# Comparing `tmp/opensesame_plugin_media_player_mpy-0.2.1.tar.gz` & `tmp/opensesame_plugin_media_player_mpy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensesame_plugin_media_player_mpy-0.2.1.tar", max compression
+gzip compressed data, was "opensesame_plugin_media_player_mpy-0.2.2.tar", max compression
```

## Comparing `opensesame_plugin_media_player_mpy-0.2.1.tar` & `opensesame_plugin_media_player_mpy-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,65 @@
--rw-r--r--   0        0        0      199 2023-03-21 19:15:36.883107 opensesame_plugin_media_player_mpy-0.2.1/opensesame_plugins/media_player_mpy/__init__.py
--rw-r--r--   0        0        0     1869 2023-03-21 19:15:36.883107 opensesame_plugin_media_player_mpy-0.2.1/opensesame_plugins/media_player_mpy/media_player_mpy/__init__.py
--rw-r--r--   0        0        0      319 2023-03-21 19:15:36.883107 opensesame_plugin_media_player_mpy-0.2.1/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/__init__.py
--rw-r--r--   0        0        0      647 2023-03-21 19:15:36.883107 opensesame_plugin_media_player_mpy-0.2.1/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/expyriment_handler.py
--rw-r--r--   0        0        0     2896 2023-03-21 19:15:36.887107 opensesame_plugin_media_player_mpy-0.2.1/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/legacy_handler.py
--rw-r--r--   0        0        0     4652 2023-03-21 19:15:36.887107 opensesame_plugin_media_player_mpy-0.2.1/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/opengl_renderer.py
--rw-r--r--   0        0        0     6831 2023-03-21 19:15:36.887107 opensesame_plugin_media_player_mpy-0.2.1/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/psychopy_handler.py
--rw-r--r--   0        0        0     8503 2023-03-21 19:15:36.887107 opensesame_plugin_media_player_mpy-0.2.1/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/pygame_handler.py
--rw-r--r--   0        0        0     4049 2023-03-21 19:15:36.887107 opensesame_plugin_media_player_mpy-0.2.1/opensesame_plugins/media_player_mpy/media_player_mpy/media_player_mpy.md
--rw-r--r--   0        0        0    13443 2023-03-21 19:15:36.887107 opensesame_plugin_media_player_mpy-0.2.1/opensesame_plugins/media_player_mpy/media_player_mpy/media_player_mpy.py
--rw-r--r--   0        0        0      595 2023-03-21 19:15:36.887107 opensesame_plugin_media_player_mpy-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3321 2023-03-21 19:15:36.887107 opensesame_plugin_media_player_mpy-0.2.1/readme.md
--rw-r--r--   0        0        0     4331 1970-01-01 00:00:00.000000 opensesame_plugin_media_player_mpy-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      199 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/__init__.py
+-rw-r--r--   0        0        0     1869 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/__init__.py
+-rw-r--r--   0        0        0      319 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/__init__.py
+-rw-r--r--   0        0        0      647 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/expyriment_handler.py
+-rw-r--r--   0        0        0     2896 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/legacy_handler.py
+-rw-r--r--   0        0        0     4652 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/opengl_renderer.py
+-rw-r--r--   0        0        0     6831 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/psychopy_handler.py
+-rw-r--r--   0        0        0     8503 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/pygame_handler.py
+-rw-r--r--   0        0        0     4049 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/ar/media_player_mpy.md
+-rw-r--r--   0        0        0     2756 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/ar.qm
+-rw-r--r--   0        0        0     4874 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/ar.ts
+-rw-r--r--   0        0        0     4049 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/bn/media_player_mpy.md
+-rw-r--r--   0        0        0     2870 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/bn.qm
+-rw-r--r--   0        0        0     5503 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/bn.ts
+-rw-r--r--   0        0        0     4500 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/de/media_player_mpy.md
+-rw-r--r--   0        0        0     3046 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/de.qm
+-rw-r--r--   0        0        0     4613 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/de.ts
+-rw-r--r--   0        0        0     4585 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/es/media_player_mpy.md
+-rw-r--r--   0        0        0     3064 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/es.qm
+-rw-r--r--   0        0        0     4631 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/es.ts
+-rw-r--r--   0        0        0     4587 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/fr/media_player_mpy.md
+-rw-r--r--   0        0        0     3068 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/fr.qm
+-rw-r--r--   0        0        0     4644 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/fr.ts
+-rw-r--r--   0        0        0     5073 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/he/media_player_mpy.md
+-rw-r--r--   0        0        0     2654 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/he.qm
+-rw-r--r--   0        0        0     4768 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/he.ts
+-rw-r--r--   0        0        0     8573 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/hi/media_player_mpy.md
+-rw-r--r--   0        0        0     2902 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/hi.qm
+-rw-r--r--   0        0        0     5501 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/hi.ts
+-rw-r--r--   0        0        0     4122 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/id/media_player_mpy.md
+-rw-r--r--   0        0        0     2870 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/id.qm
+-rw-r--r--   0        0        0     4519 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/id.ts
+-rw-r--r--   0        0        0     4534 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/it/media_player_mpy.md
+-rw-r--r--   0        0        0     3044 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/it.qm
+-rw-r--r--   0        0        0     4606 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/it.ts
+-rw-r--r--   0        0        0     5040 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/ja/media_player_mpy.md
+-rw-r--r--   0        0        0     2300 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/ja.qm
+-rw-r--r--   0        0        0     4718 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/ja.ts
+-rw-r--r--   0        0        0     3306 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/ko/media_player_mpy.md
+-rw-r--r--   0        0        0     2314 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/ko.qm
+-rw-r--r--   0        0        0     4643 2023-07-10 12:17:58.870701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/ko.ts
+-rw-r--r--   0        0        0     4365 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/nl/media_player_mpy.md
+-rw-r--r--   0        0        0     2990 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/nl.qm
+-rw-r--r--   0        0        0     4579 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/nl.ts
+-rw-r--r--   0        0        0     4516 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/pt/media_player_mpy.md
+-rw-r--r--   0        0        0     3056 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/pt.qm
+-rw-r--r--   0        0        0     4636 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/pt.ts
+-rw-r--r--   0        0        0     7324 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/ru/media_player_mpy.md
+-rw-r--r--   0        0        0     3072 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/ru.qm
+-rw-r--r--   0        0        0     5174 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/ru.ts
+-rw-r--r--   0        0        0     4321 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/tr/media_player_mpy.md
+-rw-r--r--   0        0        0     2890 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/tr.qm
+-rw-r--r--   0        0        0     4586 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/tr.ts
+-rw-r--r--   0        0        0     4162 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/translatables.ts
+-rw-r--r--   0        0        0     3541 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/yue/media_player_mpy.md
+-rw-r--r--   0        0        0     2150 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/yue.qm
+-rw-r--r--   0        0        0     4509 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/yue.ts
+-rw-r--r--   0        0        0     3600 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/zh/media_player_mpy.md
+-rw-r--r--   0        0        0     2126 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/zh.qm
+-rw-r--r--   0        0        0     4473 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/zh.ts
+-rw-r--r--   0        0        0     4049 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/media_player_mpy.md
+-rw-r--r--   0        0        0    14651 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/media_player_mpy.py
+-rw-r--r--   0        0        0      595 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3321 2023-07-10 12:17:58.874701 opensesame_plugin_media_player_mpy-0.2.2/readme.md
+-rw-r--r--   0        0        0     4331 1970-01-01 00:00:00.000000 opensesame_plugin_media_player_mpy-0.2.2/PKG-INFO
```

### Comparing `opensesame_plugin_media_player_mpy-0.2.1/opensesame_plugins/media_player_mpy/media_player_mpy/__init__.py` & `opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/__init__.py`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_media_player_mpy-0.2.1/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/expyriment_handler.py` & `opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/expyriment_handler.py`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_media_player_mpy-0.2.1/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/legacy_handler.py` & `opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/legacy_handler.py`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_media_player_mpy-0.2.1/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/opengl_renderer.py` & `opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/opengl_renderer.py`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_media_player_mpy-0.2.1/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/psychopy_handler.py` & `opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/psychopy_handler.py`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_media_player_mpy-0.2.1/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/pygame_handler.py` & `opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/handlers/pygame_handler.py`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_media_player_mpy-0.2.1/opensesame_plugins/media_player_mpy/media_player_mpy/media_player_mpy.md` & `opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/locale/ar/media_player_mpy.md`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_media_player_mpy-0.2.1/opensesame_plugins/media_player_mpy/media_player_mpy/media_player_mpy.py` & `opensesame_plugin_media_player_mpy-0.2.2/opensesame_plugins/media_player_mpy/media_player_mpy/media_player_mpy.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,21 @@
 from libopensesame.exceptions import OSException, InvalidValue, \
     BackendNotSupported
 import os
 import time
 import mediadecoder
 
 
+class SoundRendererError(OSException):
+    """A `SoundRendererError` is raised when the `media_player_mpy` item could
+    not initialize the libraries required for sound playback. A possible 
+    workaround is to select a different sound renderer in the item controls.
+    """
+
+
 class MediaPlayerMpy(Item):
 
     @property
     def frame_no(self):
         return self.player.current_frame_no
 
     @property
@@ -82,26 +89,43 @@
                     f"Invalid path to video file: {path} (file not found)")
             # Load the video file. Returns false if this failed
             elif not self.player.load_media(path):
                 raise OSException("Video file could not be loaded")
         # Set audiorenderer
         if self.var.playaudio == u"yes" and self.player.audioformat:
             if self.var.soundrenderer == u"pygame":
-                from mediadecoder.soundrenderers import SoundrendererPygame
-                self.audio_handler = SoundrendererPygame(
-                    self.player.audioformat)
+                try:
+                    from mediadecoder.soundrenderers import SoundrendererPygame
+                    self.audio_handler = SoundrendererPygame(
+                        self.player.audioformat)
+                except Exception as e:
+                    raise SoundRendererError(
+                        'Failed to initialize pygame sound render in '
+                        'media_player_mpy. You may want to select another '
+                        'sound renderer.')
             elif self.var.soundrenderer == u"pyaudio":
-                from mediadecoder.soundrenderers import SoundrendererPyAudio
-                self.audio_handler = SoundrendererPyAudio(
-                    self.player.audioformat)
+                try:
+                    from mediadecoder.soundrenderers import SoundrendererPyAudio
+                    self.audio_handler = SoundrendererPyAudio(
+                        self.player.audioformat)
+                except Exception as e:
+                    raise SoundRendererError(
+                        'Failed to initialize pyaudio sound render in '
+                        'media_player_mpy. You may want to select another '
+                        'sound renderer.')
             elif self.var.soundrenderer == u"sounddevice":
-                from mediadecoder.soundrenderers import SoundrendererSounddevice
-                self.audio_handler = SoundrendererSounddevice(
-                    self.player.audioformat)
-
+                try:
+                    from mediadecoder.soundrenderers import SoundrendererSounddevice
+                    self.audio_handler = SoundrendererSounddevice(
+                        self.player.audioformat)
+                except Exception as e:
+                    raise SoundRendererError(
+                        'Failed to initialize sounddevice sound render in '
+                        'media_player_mpy. You may want to select another '
+                        'sound renderer.')
             self.player.set_audiorenderer(self.audio_handler)
 
         self.vid_size = self.player.clip.size
         self.windowsize = self.experiment.resolution()
 
         if self.var.resizeVideo == u"yes":
             self.dest_size = self.calculate_scaled_resolution(self.windowsize,
```

### Comparing `opensesame_plugin_media_player_mpy-0.2.1/pyproject.toml` & `opensesame_plugin_media_player_mpy-0.2.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opensesame-plugin-media_player_mpy"
-version = "0.2.1"
+version = "0.2.2"
 description = "A video playback plugin for OpenSesame, based on MoviePy"
 authors = [
     "Daniel Schreij <dschreij@gmail.com>",
     "Sebastiaan Mathôt <s.mathot@cogsci.nl>"
 ]
 readme = "readme.md"
 license = "COPYING"
```

### Comparing `opensesame_plugin_media_player_mpy-0.2.1/readme.md` & `opensesame_plugin_media_player_mpy-0.2.2/readme.md`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_media_player_mpy-0.2.1/PKG-INFO` & `opensesame_plugin_media_player_mpy-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensesame-plugin-media-player-mpy
-Version: 0.2.1
+Version: 0.2.2
 Summary: A video playback plugin for OpenSesame, based on MoviePy
 Home-page: https://osdoc.cogsci.nl
 License: COPYING
 Author: Daniel Schreij
 Author-email: dschreij@gmail.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 2
```

