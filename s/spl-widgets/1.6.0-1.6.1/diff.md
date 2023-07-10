# Comparing `tmp/spl_widgets-1.6.0.tar.gz` & `tmp/spl_widgets-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spl_widgets-1.6.0.tar", last modified: Mon Jul 10 21:02:31 2023, max compression
+gzip compressed data, was "spl_widgets-1.6.1.tar", last modified: Mon Jul 10 21:05:00 2023, max compression
```

## Comparing `spl_widgets-1.6.0.tar` & `spl_widgets-1.6.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:02:31.986881 spl_widgets-1.6.0/
--rw-r--r--   0 colin      (501) staff       (20)     1073 2021-11-03 16:44:37.000000 spl_widgets-1.6.0/LICENSE
--rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-10 21:02:31.986560 spl_widgets-1.6.0/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)     2101 2022-06-26 15:02:40.000000 spl_widgets-1.6.0/README.md
--rw-r--r--   0 colin      (501) staff       (20)      103 2021-11-03 16:36:22.000000 spl_widgets-1.6.0/pyproject.toml
--rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-10 21:02:31.987007 spl_widgets-1.6.0/setup.cfg
--rw-r--r--   0 colin      (501) staff       (20)     1232 2023-07-10 21:02:14.000000 spl_widgets-1.6.0/setup.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:02:31.950394 spl_widgets-1.6.0/src/
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:02:31.957962 spl_widgets-1.6.0/src/spl_widgets/
--rw-r--r--   0 colin      (501) staff       (20)      279 2022-06-26 16:32:08.000000 spl_widgets-1.6.0/src/spl_widgets/__init__.py
--rw-r--r--   0 colin      (501) staff       (20)        0 2022-06-26 14:59:05.000000 spl_widgets-1.6.0/src/spl_widgets/__main__.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:02:31.963612 spl_widgets-1.6.0/src/spl_widgets/autoscorer/
--rw-r--r--   0 colin      (501) staff       (20)    13846 2023-07-10 17:51:43.000000 spl_widgets-1.6.0/src/spl_widgets/autoscorer/autoscore.py
--rw-r--r--   0 colin      (501) staff       (20)    16323 2023-07-10 17:51:43.000000 spl_widgets-1.6.0/src/spl_widgets/autoscorer/autoscorer_gui.py
--rw-r--r--   0 colin      (501) staff       (20)     5387 2023-07-02 19:26:17.000000 spl_widgets-1.6.0/src/spl_widgets/autoscorer/tokenize_to_ipa.py
--rw-r--r--   0 colin      (501) staff       (20)     3722 2023-05-26 16:24:48.000000 spl_widgets-1.6.0/src/spl_widgets/batch_tune.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:02:31.981820 spl_widgets-1.6.0/src/spl_widgets/data/
--rw-r--r--   0 colin      (501) staff       (20)  9670656 2023-05-26 16:25:12.000000 spl_widgets-1.6.0/src/spl_widgets/data/cmudict.sqlite
--rw-r--r--   0 colin      (501) staff       (20)       73 2023-07-09 17:07:05.000000 spl_widgets-1.6.0/src/spl_widgets/data/help_text.json
--rwxr-xr-x   0 colin      (501) staff       (20)     5378 2022-10-21 13:14:40.000000 spl_widgets-1.6.0/src/spl_widgets/gorilla_clean.py
--rw-r--r--   0 colin      (501) staff       (20)     2483 2022-12-17 21:45:28.000000 spl_widgets-1.6.0/src/spl_widgets/jukemake.py
--rw-r--r--   0 colin      (501) staff       (20)     4166 2023-05-25 22:28:36.000000 spl_widgets-1.6.0/src/spl_widgets/misc_util.py
--rwxr-xr-x   0 colin      (501) staff       (20)     3598 2023-04-14 19:27:21.000000 spl_widgets-1.6.0/src/spl_widgets/stk_swx.py
--rw-r--r--   0 colin      (501) staff       (20)     3614 2023-04-23 14:58:27.000000 spl_widgets-1.6.0/src/spl_widgets/tune_freq.py
--rw-r--r--   0 colin      (501) staff       (20)    17694 2023-05-26 16:20:21.000000 spl_widgets-1.6.0/src/spl_widgets/tuner.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:02:31.986074 spl_widgets-1.6.0/src/spl_widgets/util/
--rw-r--r--   0 colin      (501) staff       (20)     1169 2023-07-10 17:51:43.000000 spl_widgets-1.6.0/src/spl_widgets/util/color_util.py
--rw-r--r--   0 colin      (501) staff       (20)     3923 2023-05-26 16:25:12.000000 spl_widgets-1.6.0/src/spl_widgets/util/gui_util.py
--rw-r--r--   0 colin      (501) staff       (20)     3642 2023-05-26 16:25:13.000000 spl_widgets-1.6.0/src/spl_widgets/util/sqlite_db.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:02:31.961066 spl_widgets-1.6.0/src/spl_widgets.egg-info/
--rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-10 21:02:31.000000 spl_widgets-1.6.0/src/spl_widgets.egg-info/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)      839 2023-07-10 21:02:31.000000 spl_widgets-1.6.0/src/spl_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 colin      (501) staff       (20)        1 2023-07-10 21:02:31.000000 spl_widgets-1.6.0/src/spl_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 colin      (501) staff       (20)      265 2023-07-10 21:02:31.000000 spl_widgets-1.6.0/src/spl_widgets.egg-info/entry_points.txt
--rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-10 21:02:31.000000 spl_widgets-1.6.0/src/spl_widgets.egg-info/requires.txt
--rw-r--r--   0 colin      (501) staff       (20)       12 2023-07-10 21:02:31.000000 spl_widgets-1.6.0/src/spl_widgets.egg-info/top_level.txt
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:05:00.441568 spl_widgets-1.6.1/
+-rw-r--r--   0 colin      (501) staff       (20)     1073 2021-11-03 16:44:37.000000 spl_widgets-1.6.1/LICENSE
+-rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-10 21:05:00.441100 spl_widgets-1.6.1/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)     2101 2022-06-26 15:02:40.000000 spl_widgets-1.6.1/README.md
+-rw-r--r--   0 colin      (501) staff       (20)      103 2021-11-03 16:36:22.000000 spl_widgets-1.6.1/pyproject.toml
+-rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-10 21:05:00.441705 spl_widgets-1.6.1/setup.cfg
+-rw-r--r--   0 colin      (501) staff       (20)     1232 2023-07-10 21:04:49.000000 spl_widgets-1.6.1/setup.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:05:00.396727 spl_widgets-1.6.1/src/
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:05:00.407590 spl_widgets-1.6.1/src/spl_widgets/
+-rw-r--r--   0 colin      (501) staff       (20)      279 2022-06-26 16:32:08.000000 spl_widgets-1.6.1/src/spl_widgets/__init__.py
+-rw-r--r--   0 colin      (501) staff       (20)        0 2022-06-26 14:59:05.000000 spl_widgets-1.6.1/src/spl_widgets/__main__.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:05:00.413266 spl_widgets-1.6.1/src/spl_widgets/autoscorer/
+-rw-r--r--   0 colin      (501) staff       (20)    13846 2023-07-10 17:51:43.000000 spl_widgets-1.6.1/src/spl_widgets/autoscorer/autoscore.py
+-rw-r--r--   0 colin      (501) staff       (20)    16304 2023-07-10 21:04:34.000000 spl_widgets-1.6.1/src/spl_widgets/autoscorer/autoscorer_gui.py
+-rw-r--r--   0 colin      (501) staff       (20)     5387 2023-07-02 19:26:17.000000 spl_widgets-1.6.1/src/spl_widgets/autoscorer/tokenize_to_ipa.py
+-rw-r--r--   0 colin      (501) staff       (20)     3722 2023-05-26 16:24:48.000000 spl_widgets-1.6.1/src/spl_widgets/batch_tune.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:05:00.433890 spl_widgets-1.6.1/src/spl_widgets/data/
+-rw-r--r--   0 colin      (501) staff       (20)  9670656 2023-05-26 16:25:12.000000 spl_widgets-1.6.1/src/spl_widgets/data/cmudict.sqlite
+-rw-r--r--   0 colin      (501) staff       (20)       73 2023-07-09 17:07:05.000000 spl_widgets-1.6.1/src/spl_widgets/data/help_text.json
+-rwxr-xr-x   0 colin      (501) staff       (20)     5378 2022-10-21 13:14:40.000000 spl_widgets-1.6.1/src/spl_widgets/gorilla_clean.py
+-rw-r--r--   0 colin      (501) staff       (20)     2483 2022-12-17 21:45:28.000000 spl_widgets-1.6.1/src/spl_widgets/jukemake.py
+-rw-r--r--   0 colin      (501) staff       (20)     4166 2023-05-25 22:28:36.000000 spl_widgets-1.6.1/src/spl_widgets/misc_util.py
+-rwxr-xr-x   0 colin      (501) staff       (20)     3598 2023-04-14 19:27:21.000000 spl_widgets-1.6.1/src/spl_widgets/stk_swx.py
+-rw-r--r--   0 colin      (501) staff       (20)     3614 2023-04-23 14:58:27.000000 spl_widgets-1.6.1/src/spl_widgets/tune_freq.py
+-rw-r--r--   0 colin      (501) staff       (20)    17694 2023-05-26 16:20:21.000000 spl_widgets-1.6.1/src/spl_widgets/tuner.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:05:00.439969 spl_widgets-1.6.1/src/spl_widgets/util/
+-rw-r--r--   0 colin      (501) staff       (20)     1169 2023-07-10 17:51:43.000000 spl_widgets-1.6.1/src/spl_widgets/util/color_util.py
+-rw-r--r--   0 colin      (501) staff       (20)     3923 2023-05-26 16:25:12.000000 spl_widgets-1.6.1/src/spl_widgets/util/gui_util.py
+-rw-r--r--   0 colin      (501) staff       (20)     3642 2023-05-26 16:25:13.000000 spl_widgets-1.6.1/src/spl_widgets/util/sqlite_db.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-10 21:05:00.410950 spl_widgets-1.6.1/src/spl_widgets.egg-info/
+-rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-10 21:05:00.000000 spl_widgets-1.6.1/src/spl_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)      839 2023-07-10 21:05:00.000000 spl_widgets-1.6.1/src/spl_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 colin      (501) staff       (20)        1 2023-07-10 21:05:00.000000 spl_widgets-1.6.1/src/spl_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 colin      (501) staff       (20)      265 2023-07-10 21:05:00.000000 spl_widgets-1.6.1/src/spl_widgets.egg-info/entry_points.txt
+-rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-10 21:05:00.000000 spl_widgets-1.6.1/src/spl_widgets.egg-info/requires.txt
+-rw-r--r--   0 colin      (501) staff       (20)       12 2023-07-10 21:05:00.000000 spl_widgets-1.6.1/src/spl_widgets.egg-info/top_level.txt
```

### Comparing `spl_widgets-1.6.0/LICENSE` & `spl_widgets-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.0/README.md` & `spl_widgets-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.0/setup.py` & `spl_widgets-1.6.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 # with open("README.md", "r", encoding="utf-8") as fh:
 #     long_description = fh.read()
 
 setuptools.setup(
     name="spl_widgets",
-    version="1.6.0",
+    version="1.6.1",
     author="Colin Simon-Fellowes",
     author_email="colin.tsf@gmail.com",
     description="Widgets for the Barnard Speech Perception Laboratory",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="https://github.com/clntsf/spl_widgets",
     classifiers=[
```

### Comparing `spl_widgets-1.6.0/src/spl_widgets/autoscorer/autoscore.py` & `spl_widgets-1.6.1/src/spl_widgets/autoscorer/autoscore.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.0/src/spl_widgets/autoscorer/autoscorer_gui.py` & `spl_widgets-1.6.1/src/spl_widgets/autoscorer/autoscorer_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 
 from pathlib import Path
 from subprocess import run
 import re
 import pandas as pd
 
 from spl_widgets.util.gui_util import RadioFrame, MarginListBox, HelpLinkLabel
-# from spl_widgets.autoscorer import autoscore
-import autoscore
+from spl_widgets.autoscorer import autoscore
 
 HL = "*"*29
 
 class AutoscorerGUI:
     scoring_mode_radios: RadioFrame
     input_data_listbox: MarginListBox
     ideal_ipa_listbox: MarginListBox
```

### Comparing `spl_widgets-1.6.0/src/spl_widgets/autoscorer/tokenize_to_ipa.py` & `spl_widgets-1.6.1/src/spl_widgets/autoscorer/tokenize_to_ipa.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.0/src/spl_widgets/batch_tune.py` & `spl_widgets-1.6.1/src/spl_widgets/batch_tune.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.0/src/spl_widgets/data/cmudict.sqlite` & `spl_widgets-1.6.1/src/spl_widgets/data/cmudict.sqlite`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.0/src/spl_widgets/gorilla_clean.py` & `spl_widgets-1.6.1/src/spl_widgets/gorilla_clean.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.0/src/spl_widgets/jukemake.py` & `spl_widgets-1.6.1/src/spl_widgets/jukemake.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.0/src/spl_widgets/misc_util.py` & `spl_widgets-1.6.1/src/spl_widgets/misc_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.0/src/spl_widgets/stk_swx.py` & `spl_widgets-1.6.1/src/spl_widgets/stk_swx.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.0/src/spl_widgets/tune_freq.py` & `spl_widgets-1.6.1/src/spl_widgets/tune_freq.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.0/src/spl_widgets/tuner.py` & `spl_widgets-1.6.1/src/spl_widgets/tuner.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.0/src/spl_widgets/util/color_util.py` & `spl_widgets-1.6.1/src/spl_widgets/util/color_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.0/src/spl_widgets/util/gui_util.py` & `spl_widgets-1.6.1/src/spl_widgets/util/gui_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.0/src/spl_widgets/util/sqlite_db.py` & `spl_widgets-1.6.1/src/spl_widgets/util/sqlite_db.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.6.0/src/spl_widgets.egg-info/SOURCES.txt` & `spl_widgets-1.6.1/src/spl_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

