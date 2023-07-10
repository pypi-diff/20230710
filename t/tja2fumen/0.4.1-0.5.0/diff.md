# Comparing `tmp/tja2fumen-0.4.1.tar.gz` & `tmp/tja2fumen-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tja2fumen-0.4.1.tar", last modified: Fri Jul  7 03:41:38 2023, max compression
+gzip compressed data, was "tja2fumen-0.5.0.tar", last modified: Mon Jul 10 00:07:13 2023, max compression
```

## Comparing `tja2fumen-0.4.1.tar` & `tja2fumen-0.5.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 03:41:38.663354 tja2fumen-0.4.1/
--rw-rw-rw-   0        0        0     1083 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/LICENSE.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4388 2023-07-07 03:41:38.663354 tja2fumen-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     2669 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/README.md
--rw-rw-rw-   0        0        0      897 2023-07-07 03:41:26.000000 tja2fumen-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-07 03:41:38.678982 tja2fumen-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0       98 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 03:41:38.647740 tja2fumen-0.4.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 03:41:38.663354 tja2fumen-0.4.1/src/tja2fumen/
--rw-rw-rw-   0        0        0     1825 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/__init__.py
--rw-rw-rw-   0        0        0     3856 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/constants.py
--rw-rw-rw-   0        0        0    15506 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/converters.py
--rw-rw-rw-   0        0        0    19907 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/parsers.py
-drwxrwxrwx   0        0        0        0 2023-07-07 03:41:38.663354 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/
--rw-rw-rw-   0        0        0    23889 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Easy-1.csv
--rw-rw-rw-   0        0        0    23889 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv
--rw-rw-rw-   0        0        0    23890 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv
--rw-rw-rw-   0        0        0    23886 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv
--rw-rw-rw-   0        0        0    23884 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Hard-3.csv
--rw-rw-rw-   0        0        0    23884 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Hard-4.csv
--rw-rw-rw-   0        0        0    23883 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv
--rw-rw-rw-   0        0        0    23889 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv
--rw-rw-rw-   0        0        0    23889 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Normal-3.csv
--rw-rw-rw-   0        0        0    23887 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Normal-4.csv
--rw-rw-rw-   0        0        0    23886 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv
--rw-rw-rw-   0        0        0    23880 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv
--rw-rw-rw-   0        0        0    23872 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Oni-8.csv
--rw-rw-rw-   0        0        0    23869 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv
--rw-rw-rw-   0        0        0     3308 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/utils.py
--rw-rw-rw-   0        0        0     2905 2023-07-07 03:40:39.000000 tja2fumen-0.4.1/src/tja2fumen/writers.py
-drwxrwxrwx   0        0        0        0 2023-07-07 03:41:38.663354 tja2fumen-0.4.1/src/tja2fumen.egg-info/
--rw-rw-rw-   0        0        0     4388 2023-07-07 03:41:38.000000 tja2fumen-0.4.1/src/tja2fumen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-07-07 03:41:38.000000 tja2fumen-0.4.1/src/tja2fumen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 03:41:38.000000 tja2fumen-0.4.1/src/tja2fumen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-07 03:41:38.000000 tja2fumen-0.4.1/src/tja2fumen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-07-07 03:41:38.000000 tja2fumen-0.4.1/src/tja2fumen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-07 03:41:38.000000 tja2fumen-0.4.1/src/tja2fumen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 00:07:13.200594 tja2fumen-0.5.0/
+-rw-rw-rw-   0        0        0     1083 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4388 2023-07-10 00:07:13.200594 tja2fumen-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2669 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/README.md
+-rw-rw-rw-   0        0        0      897 2023-07-10 00:07:01.000000 tja2fumen-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-10 00:07:13.200594 tja2fumen-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0       98 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 00:07:13.184971 tja2fumen-0.5.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-10 00:07:13.184971 tja2fumen-0.5.0/src/tja2fumen/
+-rw-rw-rw-   0        0        0     1825 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/__init__.py
+-rw-rw-rw-   0        0        0     3856 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/constants.py
+-rw-rw-rw-   0        0        0    17917 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/converters.py
+-rw-rw-rw-   0        0        0    19863 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/parsers.py
+drwxrwxrwx   0        0        0        0 2023-07-10 00:07:13.200594 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/
+-rw-rw-rw-   0        0        0    23889 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Easy-1.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv
+-rw-rw-rw-   0        0        0    23890 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv
+-rw-rw-rw-   0        0        0    23886 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv
+-rw-rw-rw-   0        0        0    23884 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Hard-3.csv
+-rw-rw-rw-   0        0        0    23884 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Hard-4.csv
+-rw-rw-rw-   0        0        0    23883 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Normal-3.csv
+-rw-rw-rw-   0        0        0    23887 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Normal-4.csv
+-rw-rw-rw-   0        0        0    23886 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv
+-rw-rw-rw-   0        0        0    23880 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv
+-rw-rw-rw-   0        0        0    23872 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Oni-8.csv
+-rw-rw-rw-   0        0        0    23869 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv
+-rw-rw-rw-   0        0        0     3308 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/utils.py
+-rw-rw-rw-   0        0        0     2910 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/writers.py
+drwxrwxrwx   0        0        0        0 2023-07-10 00:07:13.184971 tja2fumen-0.5.0/src/tja2fumen.egg-info/
+-rw-rw-rw-   0        0        0     4388 2023-07-10 00:07:13.000000 tja2fumen-0.5.0/src/tja2fumen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-07-10 00:07:13.000000 tja2fumen-0.5.0/src/tja2fumen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 00:07:13.000000 tja2fumen-0.5.0/src/tja2fumen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-10 00:07:13.000000 tja2fumen-0.5.0/src/tja2fumen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-07-10 00:07:13.000000 tja2fumen-0.5.0/src/tja2fumen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-10 00:07:13.000000 tja2fumen-0.5.0/src/tja2fumen.egg-info/top_level.txt
```

### Comparing `tja2fumen-0.4.1/LICENSE.txt` & `tja2fumen-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.1/PKG-INFO` & `tja2fumen-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.4.1
+Version: 0.5.0
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `tja2fumen-0.4.1/README.md` & `tja2fumen-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.1/pyproject.toml` & `tja2fumen-0.5.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tja2fumen"
-version = "0.4.1"
+version = "0.5.0"
 description = "Convert TJA chart files into fumen (.bin) chart files"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["taiko", "tatsujin", "fumen", "TJA"]
 
 [project.urls]  # Optional
```

### Comparing `tja2fumen-0.4.1/src/tja2fumen/__init__.py` & `tja2fumen-0.5.0/src/tja2fumen/__init__.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.1/src/tja2fumen/constants.py` & `tja2fumen-0.5.0/src/tja2fumen/constants.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.1/src/tja2fumen/converters.py` & `tja2fumen-0.5.0/src/tja2fumen/converters.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 # Filler metadata that the `writeFumen` function expects
 # TODO: Determine how to properly set the item byte (https://github.com/vivaria/tja2fumen/issues/17)
 default_note = {'type': '', 'pos': 0.0, 'item': 0, 'padding': 0.0,
                 'scoreInit': 0, 'scoreDiff': 0, 'duration': 0.0}
 default_branch = {'length': 0, 'padding': 0, 'speed': 1.0}
 default_measure = {
     'bpm': 0.0,
-    'fumenOffset': 0.0,
+    'fumenOffsetStart': 0.0,
+    'fumenOffsetEnd': 0.0,
+    'duration': 0.0,
     'gogo': False,
     'barline': True,
     'padding1': 0,
     'branchStart': None,
     'branchInfo': [-1, -1, -1, -1, -1, -1],
     'padding2': 0,
     'normal': deepcopy(default_branch),
@@ -119,85 +121,118 @@
 
     return branchesCorrected
 
 
 def convertTJAToFumen(tja):
     # Preprocess commands
     tja['branches'] = processTJACommands(tja)
-    # Parse TJA measures to create converted TJA -> Fumen file
+
+    # Pre-allocate the measures for the converted TJA
     tjaConverted = {'measures': [deepcopy(default_measure) for _ in range(len(tja['branches']['normal']))]}
+
+    # Iterate through the different branches in the TJA
     for currentBranch, branch in tja['branches'].items():
         if not len(branch):
             continue
         total_notes = 0
         total_notes_branch = 0
         note_counter_branch = 0
-        measureDurationPrev = 0
         currentDrumroll = None
         courseBalloons = tja['metadata']['balloon'].copy()
+
+        # Iterate through the measures within the branch
         for idx_m, measureTJA in enumerate(branch):
+            # Fetch a pair of measures
+            measureFumenPrev = tjaConverted['measures'][idx_m-1] if idx_m != 0 else None
             measureFumen = tjaConverted['measures'][idx_m]
 
-            # Check to see if the measure contains a branching condition
-            if measureTJA['branchStart']:
-                if measureTJA['branchStart'][0] == 'p':
-                    if currentBranch == 'normal':
-                        idx_b1, idx_b2 = 0, 1
-                    elif currentBranch == 'advanced':
-                        idx_b1, idx_b2 = 2, 3
-                    elif currentBranch == 'master':
-                        idx_b1, idx_b2 = 4, 5
-                    measureFumen['branchInfo'][idx_b1] = int(total_notes_branch * measureTJA['branchStart'][1] * 20)
-                    measureFumen['branchInfo'][idx_b2] = int(total_notes_branch * measureTJA['branchStart'][2] * 20)
-                elif measureTJA['branchStart'][0] == 'r':
-                    measureFumen['branchInfo'] = measureTJA['branchStart'][1:] * 3
-                total_notes_branch = 0
-            total_notes_branch += note_counter_branch
+            # Copy over basic measure properties from the TJA (that don't depend on notes or commands)
+            measureFumen[currentBranch]['speed'] = measureTJA['scroll']
+            measureFumen['gogo'] = measureTJA['gogo']
+            measureFumen['bpm'] = measureTJA['bpm']
 
             # Compute the duration of the measure
+            # First, we compute the duration for a full 4/4 measure
+            measureDurationFullMeasure = 4 * 60_000 / measureTJA['bpm']
+            # Next, we adjust this duration based on both:
+            #   1. The *actual* measure size (e.g. #MEASURE 1/8, #MEASURE 5/4, etc.)
             measureSize = measureTJA['time_sig'][0] / measureTJA['time_sig'][1]
+            #   2. Whether this is a "submeasure" (i.e. it contains mid-measure commands, which split up the measure)
+            #      - If this is a submeasure, then `measureLength` will be less than the total number of subdivisions.
             measureLength = measureTJA['pos_end'] - measureTJA['pos_start']
-            measureRatio = 1.0 if measureTJA['subdivisions'] == 0.0 else (measureLength / measureTJA['subdivisions'])
-            # - measureDurationBase: The "base" measure duration, computed using a single BPM value.
-            # - measureDuration: The actual measure duration, which may be adjusted if there is a mid-measure BPM change.
-            measureDurationFullMeasure = 4 * 60_000 / measureTJA['bpm']
-            measureDurationBase = measureDuration = (measureDurationFullMeasure * measureSize * measureRatio)
-            # The following adjustment accounts for BPM changes. (!!! Discovered by tana :3 !!!)
-            if idx_m != len(branch)-1:
-                measureTJANext = branch[idx_m + 1]
-                if measureTJA['bpm'] != measureTJANext['bpm']:
-                    measureDuration -= (4 * 60_000 * ((1 / measureTJANext['bpm']) - (1 / measureTJA['bpm'])))
-
-            # Compute the millisecond offset for each measure
+            #      - In other words, `measureRatio` will be less than 1.0:
+            measureRatio = (1.0 if measureTJA['subdivisions'] == 0.0  # Avoid division by 0 for empty measures
+                            else (measureLength / measureTJA['subdivisions']))
+            # Apply the 2 adjustments to the measure duration
+            measureFumen['duration'] = measureDuration = measureDurationFullMeasure * measureSize * measureRatio
+
+            # Compute the millisecond offsets for the start and end of each measure
+            #  - Start: When the notes first appear on screen (to the right)
+            #  - End:   When the notes arrive at the judgment line, and the note gets hit.
             if idx_m == 0:
                 tjaOffset = float(tja['metadata']['offset']) * 1000 * -1
-                tjaConverted['measures'][idx_m]['fumenOffset'] = tjaOffset - measureDurationFullMeasure
+                measureFumen['fumenOffsetStart'] = tjaOffset - measureDurationFullMeasure
             else:
-                # Use the previous measure's offset plus the previous duration to compute the current measure's offset
-                measureOffsetPrev = tjaConverted['measures'][idx_m-1]['fumenOffset']
-                measureFumen['fumenOffset'] = measureOffsetPrev + measureDurationPrev + measureTJA['delay']
-            measureDurationPrev = measureDuration
+                # First, start the measure using the end timing of the previous measure (plus any #DELAY commands)
+                measureFumen['fumenOffsetStart'] = measureFumenPrev['fumenOffsetEnd'] + measureTJA['delay']
+                # Next, adjust the start timing to account for #BPMCHANGE commands (!!! Discovered by tana :3 !!!)
+                # To understand what's going on here, imagine the following simple example:
+                #   * You have a very slow-moving note (i.e. low BPM), like the big DON in Donkama 2000.
+                #   * All the other notes move fast (i.e. high BPM), moving past the big slow note.
+                #   * To get this overlapping to work, you need the big slow note to START EARLY, but also END LATE:
+                #      - An early start means you need to subtract a LOT of time from the starting fumenOffset.
+                #      - Thankfully, the low BPM of the slow note will create a HUGE `measureOffsetAdjustment`,
+                #        since we are dividing by the BPMs, and dividing by a small number will result in a big number.
+                measureOffsetAdjustment = (4 * 60_000 / measureTJA['bpm']) - (4 * 60_000 / measureFumenPrev['bpm'])
+                #      - When we subtract this adjustment from the fumenOffsetStart, we get the "START EARLY" part:
+                measureFumen['fumenOffsetStart'] -= measureOffsetAdjustment
+                #      - The low BPM of the slow note will also create a HUGE measure duration.
+                #      - When we add this long duration to the EARLY START, we end up with the "END LATE" part:
+            measureFumen['fumenOffsetEnd'] = measureFumen['fumenOffsetStart'] + measureFumen['duration']
 
             # Best guess at what 'barline' status means for each measure:
             # - 'True' means the measure lands on a barline (i.e. most measures), and thus barline should be shown
             # - 'False' means that the measure doesn't land on a barline, and thus barline should be hidden.
             #   For example:
             #     1. Measures where #BARLINEOFF has been set
             #     2. Sub-measures that don't fall on the barline
             if measureTJA['barline'] is False or (measureRatio != 1.0 and measureTJA['pos_start'] != 0):
                 measureFumen['barline'] = False
 
+            # Check to see if the measure contains a branching condition
+            if measureTJA['branchStart']:
+                # Determine which values to assign based on the type of branching condition
+                if measureTJA['branchStart'][0] == 'p':
+                    vals = [int(total_notes_branch * v * 20) if 0 <= v <= 1  # Ensure value is actually a percentage
+                            else int(v * 100)                                # If it's not, pass the value as-is
+                            for v in measureTJA['branchStart'][1:]]
+                elif measureTJA['branchStart'][0] == 'r':
+                    vals = measureTJA['branchStart'][1:]
+                # Determine which bytes to assign the values to
+                if currentBranch == 'normal':
+                    idx_b1, idx_b2 = 0, 1
+                elif currentBranch == 'advanced':
+                    idx_b1, idx_b2 = 2, 3
+                elif currentBranch == 'master':
+                    idx_b1, idx_b2 = 4, 5
+                # Assign the values to their intended bytes
+                measureFumen['branchInfo'][idx_b1] = vals[0]
+                measureFumen['branchInfo'][idx_b2] = vals[1]
+                # Reset the note counter corresponding to this branch
+                total_notes_branch = 0
+            total_notes_branch += note_counter_branch
+
             # Create note dictionaries based on TJA measure data (containing 0's plus 1/2/3/4/etc. for notes)
             note_counter_branch = 0
             note_counter = 0
             for idx_d, data in enumerate(measureTJA['data']):
                 if data['type'] == 'note':
                     # Note positions must be calculated using the base measure duration (that uses a single BPM value)
                     # (In other words, note positions do not take into account any mid-measure BPM change adjustments.)
-                    note_pos = measureDurationBase * (data['pos'] - measureTJA['pos_start']) / measureLength
+                    note_pos = measureDuration * (data['pos'] - measureTJA['pos_start']) / measureLength
                     # Handle the note that represents the end of a drumroll/balloon
                     if data['value'] == "EndDRB":
                         # If a drumroll spans a single measure, then add the difference between start/end position
                         if 'multimeasure' not in currentDrumroll.keys():
                             currentDrumroll['duration'] += (note_pos - currentDrumroll['pos'])
                         # Otherwise, if a drumroll spans multiple measures, then we want to add the duration between
                         # the start of the measure (i.e. pos=0.0) and the drumroll's end position.
@@ -231,27 +266,24 @@
                     # Count dons, kas, and balloons for the purpose of tracking branching accuracy
                     if note['type'].lower() in ['don', 'ka']:
                         note_counter_branch += 1
                     elif note['type'].lower() in ['balloon', 'kusudama']:
                         note_counter_branch += 1.5
                     measureFumen[currentBranch][note_counter] = note
                     note_counter += 1
-            measureFumen[currentBranch]['length'] = note_counter
-            measureFumen[currentBranch]['speed'] = measureTJA['scroll']
-            measureFumen['gogo'] = measureTJA['gogo']
-            measureFumen['bpm'] = measureTJA['bpm']
 
             # If drumroll hasn't ended by the end of this measure, increase duration by measure timing
             if currentDrumroll:
                 if currentDrumroll['duration'] == 0.0:
-                    currentDrumroll['duration'] += (measureDurationBase - currentDrumroll['pos'])
+                    currentDrumroll['duration'] += (measureDuration - currentDrumroll['pos'])
                     currentDrumroll['multimeasure'] = True
                 else:
-                    currentDrumroll['duration'] += measureDurationBase
+                    currentDrumroll['duration'] += measureDuration
 
+            measureFumen[currentBranch]['length'] = note_counter
             total_notes += note_counter
 
     # Take a stock header metadata sample and add song-specific metadata
     headerMetadata = sampleHeaderMetadata.copy()
     headerMetadata[8] = DIFFICULTY_BYTES[tja['metadata']['course']][0]
     headerMetadata[9] = DIFFICULTY_BYTES[tja['metadata']['course']][1]
     headerMetadata[20], headerMetadata[21] = computeSoulGaugeBytes(
```

### Comparing `tja2fumen-0.4.1/src/tja2fumen/parsers.py` & `tja2fumen-0.5.0/src/tja2fumen/parsers.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,19 +77,22 @@
             match_command = re.match(r"^#([A-Z]+)(?:\s+(.+))?", line)
             match_notes = re.match(r"^(([0-9]|A|B|C|F|G)*,?).*$", line)
             if match_command:
                 nameUpper = match_command.group(1).upper()
                 value = match_command.group(2).strip() if match_command.group(2) else ''
                 # For STYLE:Double, #START P1/P2 indicates the start of a new chart
                 # But, we want multiplayer charts to inherit the metadata from the course as a whole, so we deepcopy
-                if nameUpper == "START" and value in ["P1", "P2"]:                   
-                    currentCourse = currentCourseCached + value
-                    courses[currentCourse] = deepcopy(courses[currentCourseCached])
-                    courses[currentCourse]['data'] = list()  # Keep the metadata, but reset the note data
-                    value = ''  # Once we've made the new course, we can reset this to a normal #START command
+                if nameUpper == "START":
+                    if value in ["P1", "P2"]:
+                        currentCourse = currentCourseCached + value
+                        courses[currentCourse] = deepcopy(courses[currentCourseCached])
+                        courses[currentCourse]['data'] = list()  # Keep the metadata, but reset the note data
+                        value = ''  # Once we've made the new course, we can reset this to a normal #START command
+                    elif value:
+                        raise ValueError(f"Invalid value '{value}' for #START command.")
             elif match_notes:
                 nameUpper = 'NOTES'
                 value = match_notes.group(1)
             courses[currentCourse]['data'].append({"name": nameUpper, "value": value})
             
     # If a course has no song data, then this is likely because the course has "STYLE: Double" but no "STYLE: Single".
     # To fix this, we copy over the P1 chart from "STYLE: Double" to fill the "STYLE: Single" role.
@@ -164,14 +167,18 @@
                     values[2] = float(values[2]) / 100  # %
                 currentEvent = {"name": 'branchStart', "position": pos, "value": values}
                 idx_m_branchstart = idx_m  # Preserve the index of the BRANCHSTART command to re-use for each branch
 
             # Append event to the current measure's events
             for branch in branches.keys() if currentBranch == 'all' else [currentBranch]:
                 branches[branch][idx_m]['events'].append(currentEvent)
+        elif line['name'] == 'SECTION':
+            # Simply repeat the same #BRANCHSTART condition that happened previously
+            # The purpose of #SECTION is to "Reset accuracy values for notes and drumrolls on the next measure."
+            branches[branch][idx_m]['events'].append({"name": 'branchStart', "position": pos, "value": values})
 
         # 3. Parse commands that don't create an event (e.g. simply changing the current branch)
         else:
             if line["name"] == 'START' or line['name'] == 'END':
                 currentBranch = 'all' if hasBranches else 'normal'
                 flagLevelhold = False
             elif line['name'] == 'LEVELHOLD':
@@ -191,16 +198,14 @@
             # Ignored commands
             elif line['name'] == 'LYRIC':
                 pass
             elif line['name'] == 'NEXTSONG':
                 pass
 
             # Not implemented commands
-            elif line['name'] == 'SECTION':
-                pass  # This seems to be inconsequential, but I'm not 100% sure. Need to test more branching fumens.
             else:
                 raise NotImplementedError
 
     # Delete the last measure in the branch if no notes or events were added to it (due to preallocating empty measures)
     for branch in branches.values():
         if not branch[-1]['data'] and not branch[-1]['events']:
             del branch[-1]
@@ -296,21 +301,15 @@
         #     - 'iiiiii': branchInfo  (represented by six integers (24 bytes))
         #     - 'i': <padding>        (represented by one integer (4 bytes)
         measureStruct = readStruct(file, order, format_string="ffBBHiiiiiii")
 
         # Create the measure dictionary using the newly-parsed measure data
         measure = {}
         measure["bpm"] = measureStruct[0]
-        measure["fumenOffset"] = measureStruct[1]
-        # if measureNumber == 0:
-        #     measure["offset"] = measure["fumenOffset"] + 240000 / measure["bpm"]
-        # else:
-        #     prev = song['measures'][measureNumber - 1]
-        #     measure["offset"] = ((prev["offset"] + measure["fumenOffset"] + 240000) /
-        #                          (measure["bpm"] - prev["fumenOffset"] - 240000 / prev["bpm"]))
+        measure["fumenOffsetStart"] = measureStruct[1]
         measure["gogo"] = getBool(measureStruct[2])
         measure["barline"] = getBool(measureStruct[3])
         measure["padding1"] = measureStruct[4]
         measure["branchInfo"] = list(measureStruct[5:11])
         measure["padding2"] = measureStruct[11]
 
         # Iterate through the three branch types
```

### Comparing `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Easy-1.csv` & `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Easy-1.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv` & `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv` & `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv` & `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Hard-3.csv` & `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Hard-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Hard-4.csv` & `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Hard-4.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv` & `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv` & `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Normal-3.csv` & `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Normal-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Normal-4.csv` & `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Normal-4.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv` & `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv` & `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Oni-8.csv` & `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Oni-8.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.1/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv` & `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.1/src/tja2fumen/utils.py` & `tja2fumen-0.5.0/src/tja2fumen/utils.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.4.1/src/tja2fumen/writers.py` & `tja2fumen-0.5.0/src/tja2fumen/writers.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     writeStruct(file, order, format_string="I", value_list=[len(song['measures'])], seek=0x200)
     writeStruct(file, order, format_string="I", value_list=[song['unknownMetadata']], seek=0x204)
 
     # Write measure data
     file.seek(0x208)
     for measureNumber in range(len(song['measures'])):
         measure = song['measures'][measureNumber]
-        measureStruct = [measure['bpm'], measure['fumenOffset'], int(measure['gogo']), int(measure['barline'])]
+        measureStruct = [measure['bpm'], measure['fumenOffsetStart'], int(measure['gogo']), int(measure['barline'])]
         measureStruct.extend([measure['padding1']] + measure['branchInfo'] + [measure['padding2']])
         writeStruct(file, order, format_string="ffBBHiiiiiii", value_list=measureStruct)
 
         for branchNumber in range(len(branchNames)):
             branch = measure[branchNames[branchNumber]]
             branchStruct = [branch['length'], branch['padding'], branch['speed']]
             writeStruct(file, order, format_string="HHf", value_list=branchStruct)
```

### Comparing `tja2fumen-0.4.1/src/tja2fumen.egg-info/PKG-INFO` & `tja2fumen-0.5.0/src/tja2fumen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.4.1
+Version: 0.5.0
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `tja2fumen-0.4.1/src/tja2fumen.egg-info/SOURCES.txt` & `tja2fumen-0.5.0/src/tja2fumen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

