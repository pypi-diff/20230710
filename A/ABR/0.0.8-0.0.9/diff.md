# Comparing `tmp/ABR-0.0.8.tar.gz` & `tmp/ABR-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ABR-0.0.8.tar", last modified: Wed Jun 28 20:26:02 2023, max compression
+gzip compressed data, was "ABR-0.0.9.tar", last modified: Thu Jun 29 22:13:05 2023, max compression
```

## Comparing `ABR-0.0.8.tar` & `ABR-0.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:26:02.887104 ABR-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:26:02.879104 ABR-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:26:02.883104 ABR-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-28 20:25:53.000000 ABR-0.0.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-28 20:25:53.000000 ABR-0.0.8/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:26:02.883104 ABR-0.0.8/ABR.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-06-28 20:26:02.000000 ABR-0.0.8/ABR.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-28 20:26:02.000000 ABR-0.0.8/ABR.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 20:26:02.000000 ABR-0.0.8/ABR.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-28 20:26:02.000000 ABR-0.0.8/ABR.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-28 20:26:02.000000 ABR-0.0.8/ABR.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-28 20:26:02.000000 ABR-0.0.8/ABR.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-28 20:25:53.000000 ABR-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-06-28 20:26:02.887104 ABR-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-06-28 20:25:53.000000 ABR-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:26:02.883104 ABR-0.0.8/abr/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-28 20:25:53.000000 ABR-0.0.8/abr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-28 20:25:53.000000 ABR-0.0.8/abr/abr-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-06-28 20:25:53.000000 ABR-0.0.8/abr/abrpanel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-28 20:25:53.000000 ABR-0.0.8/abr/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:26:02.883104 ABR-0.0.8/abr/data/
--rw-r--r--   0 runner    (1001) docker     (123)   226332 2023-06-28 20:25:53.000000 ABR-0.0.8/abr/data/ABR-52-3
--rw-r--r--   0 runner    (1001) docker     (123)   245030 2023-06-28 20:25:53.000000 ABR-0.0.8/abr/data/CAP-139-5
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-28 20:25:53.000000 ABR-0.0.8/abr/data/CAP-139-5-16.0kHz-Brad-analyzed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-28 20:25:53.000000 ABR-0.0.8/abr/data/CAP-139-5-16.0kHz-analyzed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-06-28 20:25:53.000000 ABR-0.0.8/abr/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-28 20:25:53.000000 ABR-0.0.8/abr/launch_window.enaml
--rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-06-28 20:25:53.000000 ABR-0.0.8/abr/main_window.enaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:26:02.887104 ABR-0.0.8/abr/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-28 20:25:53.000000 ABR-0.0.8/abr/parsers/EPL.py
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-28 20:25:53.000000 ABR-0.0.8/abr/parsers/NCRAR.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-06-28 20:25:53.000000 ABR-0.0.8/abr/parsers/PSI.py
--rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-06-28 20:25:53.000000 ABR-0.0.8/abr/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-28 20:25:53.000000 ABR-0.0.8/abr/parsers/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-28 20:25:53.000000 ABR-0.0.8/abr/peakdetect.py
--rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-06-28 20:25:53.000000 ABR-0.0.8/abr/presenter.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-28 20:26:02.000000 ABR-0.0.8/abr/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-28 20:25:53.000000 ABR-0.0.8/packaging.md
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-28 20:25:53.000000 ABR-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 20:26:02.887104 ABR-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:13:05.229523 ABR-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:13:05.225523 ABR-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:13:05.225523 ABR-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-29 22:12:53.000000 ABR-0.0.9/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-29 22:12:53.000000 ABR-0.0.9/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:13:05.225523 ABR-0.0.9/ABR.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-29 22:13:05.000000 ABR-0.0.9/ABR.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-29 22:13:05.000000 ABR-0.0.9/ABR.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 22:13:05.000000 ABR-0.0.9/ABR.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-29 22:13:05.000000 ABR-0.0.9/ABR.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 22:13:05.000000 ABR-0.0.9/ABR.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 22:13:05.000000 ABR-0.0.9/ABR.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-29 22:12:53.000000 ABR-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-29 22:13:05.229523 ABR-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-06-29 22:12:53.000000 ABR-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:13:05.225523 ABR-0.0.9/abr/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-29 22:12:53.000000 ABR-0.0.9/abr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-29 22:12:53.000000 ABR-0.0.9/abr/abr-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-06-29 22:12:53.000000 ABR-0.0.9/abr/abrpanel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-29 22:12:53.000000 ABR-0.0.9/abr/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:13:05.229523 ABR-0.0.9/abr/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   226332 2023-06-29 22:12:53.000000 ABR-0.0.9/abr/data/ABR-52-3
+-rw-r--r--   0 runner    (1001) docker     (123)   245030 2023-06-29 22:12:53.000000 ABR-0.0.9/abr/data/CAP-139-5
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-29 22:12:53.000000 ABR-0.0.9/abr/data/CAP-139-5-16.0kHz-Brad-analyzed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-29 22:12:53.000000 ABR-0.0.9/abr/data/CAP-139-5-16.0kHz-analyzed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-06-29 22:12:53.000000 ABR-0.0.9/abr/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-29 22:12:53.000000 ABR-0.0.9/abr/launch_window.enaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-06-29 22:12:53.000000 ABR-0.0.9/abr/main_window.enaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:13:05.229523 ABR-0.0.9/abr/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-29 22:12:53.000000 ABR-0.0.9/abr/parsers/EPL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-29 22:12:53.000000 ABR-0.0.9/abr/parsers/NCRAR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-06-29 22:12:53.000000 ABR-0.0.9/abr/parsers/PSI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-06-29 22:12:53.000000 ABR-0.0.9/abr/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-29 22:12:53.000000 ABR-0.0.9/abr/parsers/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-29 22:12:53.000000 ABR-0.0.9/abr/peakdetect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-06-29 22:12:53.000000 ABR-0.0.9/abr/presenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 22:13:05.000000 ABR-0.0.9/abr/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-29 22:12:53.000000 ABR-0.0.9/packaging.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-29 22:12:53.000000 ABR-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 22:13:05.229523 ABR-0.0.9/setup.cfg
```

### Comparing `ABR-0.0.8/.github/workflows/publish-to-pypi.yml` & `ABR-0.0.9/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `ABR-0.0.8/.gitignore` & `ABR-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ABR-0.0.8/ABR.egg-info/PKG-INFO` & `ABR-0.0.9/ABR.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ABR
-Version: 0.0.8
+Version: 0.0.9
 Summary: Evoked potential analysis software
 Author-email: Brad Buran <bburan@alum.mit.edu>, Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <bburan@alum.mit.edu>, Brad Buran <buran@ohsu.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, Brad Buran
         All rights reserved.
@@ -53,17 +53,19 @@
 * ABR data generated by [psiexperiment](https://github.com/psiexperiment/psiexperiment).
 * ABR data generated by the Intelligent Hearing Systems (IHS) text export.
 
 Individal research groups have also adapted the program to work with their own file formats.
 
 ## Installing
 
-The simplest way to get started is to download the [Anaconda Python Distribution](https://www.anaconda.com/distribution/). Once installed, you will have new programs available in your start menu. Open `Anaconda Prompt` and type `conda install -c bburan abr`. On windows, this will download the software and add a new shortcut to your start menu called `ABR analysis` which can be used to launch the program.
+The simplest way to get started is to download the [Anaconda Python Distribution](https://www.anaconda.com/distribution/). Once installed, you will have new programs available in your start menu. One of these is called `Anaconda Prompt`. Open this program and type `pip install abr`.
 
-This program also works on Mac OS and Linux, but I do not have specific instructions for getting started on these platforms yet. Please give me a nudge if you need help with this and I can help you get started.
+## Running the program
+
+Open the `Anaconda Prompt` and type `abr`.
 
 ## Programs available
 
 There are two main interfaces to the ABR analysis program. The first is the basic interface where you manually drag files from your file browser and drop them on the window. You can drag one file or multiple files. Each file will be opened in a separate tab. The second interface is an automatic one that will loop through all unprocessed ABR files found in a folder and present each file to you individually for analysis. Once you save the analysis, it will immediately move to the next file.
 
 Both interfaces are accessed via the launcher. When you first open the launcher, you will specify:
 
@@ -82,42 +84,12 @@
 
 The amplitude and latency of each point are saved along with the threshold of the series. If the point is part of a subthreshold waveform, the additive inverse of the latency is saved (i.e. when parsing the file, subthreshold data can be recognized by negative latencies).  Amplitudes from subthreshold points can be used to estimate the noise floor if desired.
 
 ## Interface
 
 The current waveform is displayed as a thick, black line.  Once a threshold is specified, subthreshold waveforms are indicated by a dashed line.  The selected point is indicated by a white square.  Negativities are indicated by triangles, positivities as squares.  Red is P1/N1, yellow is P2/N2, green is P3/N3, light blue is P4/N4, and dark blue is P5/N5.
 
-The following keys can be used when analyzing a waveform:
-
-    Up/Down arrows
-        Select previous/next waveform in the series
-    Right/Left arrows
-        Move a toggled peak left or right along the waveform.  Movement of the
-        peak will "snap" to estimated peaks in the waveform.  To adjust the peak
-        in fine increments, hold down the alt key simultaneously.
-    Number keys 1-5
-        Select the corresponding peak on the current waveform.  To select N1-5,
-        hold down alt while pressing the corresponding number.
-    I
-        Estimates P1-5 for all waveforms on the first press. N1-5 for all
-        waveforms on the second press. After that, nothing happens.
-    U
-        Updates guess for corresponding P or N of successive waveforms based on
-        position of currently toggled P or N.
-    N
-        Toggles normalized view of waveform.
-    +/- keys
-        Increases/decreases scaling factor of waveform.
-    S
-        Saves amplitude and latency of peaks.
-    T
-        Set threshold to current waveform.
-    Alt+Up
-        Indicate that all waveforms are below threshold.
-    Alt+Down
-        Indicate that all waveforms are above threshold.
-
-Some keys will repeat if you hold down the key, which may be useful when navigating through the waveforms or adjusting the location of a peak.
+Instructions for using the program are included in the user interface.
 
 # Attributions
 
-Code relating to marking points unscoreable and/or shifting waveforms up/down to ensure they don't run off the plot are adapted from work performed for the United States government and, therefore, are in the public domain. All other part of the code remain licensed under the BSD.
+Code relating to marking points unscoreable and/or shifting waveforms up/down to ensure they don't run off the plot are adapted from work performed for the United States government and, therefore, are in the public domain. All other part of the code remain licensed under the BSD 3-clause.
```

### Comparing `ABR-0.0.8/ABR.egg-info/SOURCES.txt` & `ABR-0.0.9/ABR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ABR-0.0.8/LICENSE.txt` & `ABR-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ABR-0.0.8/PKG-INFO` & `ABR-0.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ABR
-Version: 0.0.8
+Version: 0.0.9
 Summary: Evoked potential analysis software
 Author-email: Brad Buran <bburan@alum.mit.edu>, Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <bburan@alum.mit.edu>, Brad Buran <buran@ohsu.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, Brad Buran
         All rights reserved.
@@ -53,17 +53,19 @@
 * ABR data generated by [psiexperiment](https://github.com/psiexperiment/psiexperiment).
 * ABR data generated by the Intelligent Hearing Systems (IHS) text export.
 
 Individal research groups have also adapted the program to work with their own file formats.
 
 ## Installing
 
-The simplest way to get started is to download the [Anaconda Python Distribution](https://www.anaconda.com/distribution/). Once installed, you will have new programs available in your start menu. Open `Anaconda Prompt` and type `conda install -c bburan abr`. On windows, this will download the software and add a new shortcut to your start menu called `ABR analysis` which can be used to launch the program.
+The simplest way to get started is to download the [Anaconda Python Distribution](https://www.anaconda.com/distribution/). Once installed, you will have new programs available in your start menu. One of these is called `Anaconda Prompt`. Open this program and type `pip install abr`.
 
-This program also works on Mac OS and Linux, but I do not have specific instructions for getting started on these platforms yet. Please give me a nudge if you need help with this and I can help you get started.
+## Running the program
+
+Open the `Anaconda Prompt` and type `abr`.
 
 ## Programs available
 
 There are two main interfaces to the ABR analysis program. The first is the basic interface where you manually drag files from your file browser and drop them on the window. You can drag one file or multiple files. Each file will be opened in a separate tab. The second interface is an automatic one that will loop through all unprocessed ABR files found in a folder and present each file to you individually for analysis. Once you save the analysis, it will immediately move to the next file.
 
 Both interfaces are accessed via the launcher. When you first open the launcher, you will specify:
 
@@ -82,42 +84,12 @@
 
 The amplitude and latency of each point are saved along with the threshold of the series. If the point is part of a subthreshold waveform, the additive inverse of the latency is saved (i.e. when parsing the file, subthreshold data can be recognized by negative latencies).  Amplitudes from subthreshold points can be used to estimate the noise floor if desired.
 
 ## Interface
 
 The current waveform is displayed as a thick, black line.  Once a threshold is specified, subthreshold waveforms are indicated by a dashed line.  The selected point is indicated by a white square.  Negativities are indicated by triangles, positivities as squares.  Red is P1/N1, yellow is P2/N2, green is P3/N3, light blue is P4/N4, and dark blue is P5/N5.
 
-The following keys can be used when analyzing a waveform:
-
-    Up/Down arrows
-        Select previous/next waveform in the series
-    Right/Left arrows
-        Move a toggled peak left or right along the waveform.  Movement of the
-        peak will "snap" to estimated peaks in the waveform.  To adjust the peak
-        in fine increments, hold down the alt key simultaneously.
-    Number keys 1-5
-        Select the corresponding peak on the current waveform.  To select N1-5,
-        hold down alt while pressing the corresponding number.
-    I
-        Estimates P1-5 for all waveforms on the first press. N1-5 for all
-        waveforms on the second press. After that, nothing happens.
-    U
-        Updates guess for corresponding P or N of successive waveforms based on
-        position of currently toggled P or N.
-    N
-        Toggles normalized view of waveform.
-    +/- keys
-        Increases/decreases scaling factor of waveform.
-    S
-        Saves amplitude and latency of peaks.
-    T
-        Set threshold to current waveform.
-    Alt+Up
-        Indicate that all waveforms are below threshold.
-    Alt+Down
-        Indicate that all waveforms are above threshold.
-
-Some keys will repeat if you hold down the key, which may be useful when navigating through the waveforms or adjusting the location of a peak.
+Instructions for using the program are included in the user interface.
 
 # Attributions
 
-Code relating to marking points unscoreable and/or shifting waveforms up/down to ensure they don't run off the plot are adapted from work performed for the United States government and, therefore, are in the public domain. All other part of the code remain licensed under the BSD.
+Code relating to marking points unscoreable and/or shifting waveforms up/down to ensure they don't run off the plot are adapted from work performed for the United States government and, therefore, are in the public domain. All other part of the code remain licensed under the BSD 3-clause.
```

### Comparing `ABR-0.0.8/README.md` & `ABR-0.0.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 * ABR data generated by [psiexperiment](https://github.com/psiexperiment/psiexperiment).
 * ABR data generated by the Intelligent Hearing Systems (IHS) text export.
 
 Individal research groups have also adapted the program to work with their own file formats.
 
 ## Installing
 
-The simplest way to get started is to download the [Anaconda Python Distribution](https://www.anaconda.com/distribution/). Once installed, you will have new programs available in your start menu. Open `Anaconda Prompt` and type `conda install -c bburan abr`. On windows, this will download the software and add a new shortcut to your start menu called `ABR analysis` which can be used to launch the program.
+The simplest way to get started is to download the [Anaconda Python Distribution](https://www.anaconda.com/distribution/). Once installed, you will have new programs available in your start menu. One of these is called `Anaconda Prompt`. Open this program and type `pip install abr`.
 
-This program also works on Mac OS and Linux, but I do not have specific instructions for getting started on these platforms yet. Please give me a nudge if you need help with this and I can help you get started.
+## Running the program
+
+Open the `Anaconda Prompt` and type `abr`.
 
 ## Programs available
 
 There are two main interfaces to the ABR analysis program. The first is the basic interface where you manually drag files from your file browser and drop them on the window. You can drag one file or multiple files. Each file will be opened in a separate tab. The second interface is an automatic one that will loop through all unprocessed ABR files found in a folder and present each file to you individually for analysis. Once you save the analysis, it will immediately move to the next file.
 
 Both interfaces are accessed via the launcher. When you first open the launcher, you will specify:
 
@@ -36,42 +38,12 @@
 
 The amplitude and latency of each point are saved along with the threshold of the series. If the point is part of a subthreshold waveform, the additive inverse of the latency is saved (i.e. when parsing the file, subthreshold data can be recognized by negative latencies).  Amplitudes from subthreshold points can be used to estimate the noise floor if desired.
 
 ## Interface
 
 The current waveform is displayed as a thick, black line.  Once a threshold is specified, subthreshold waveforms are indicated by a dashed line.  The selected point is indicated by a white square.  Negativities are indicated by triangles, positivities as squares.  Red is P1/N1, yellow is P2/N2, green is P3/N3, light blue is P4/N4, and dark blue is P5/N5.
 
-The following keys can be used when analyzing a waveform:
-
-    Up/Down arrows
-        Select previous/next waveform in the series
-    Right/Left arrows
-        Move a toggled peak left or right along the waveform.  Movement of the
-        peak will "snap" to estimated peaks in the waveform.  To adjust the peak
-        in fine increments, hold down the alt key simultaneously.
-    Number keys 1-5
-        Select the corresponding peak on the current waveform.  To select N1-5,
-        hold down alt while pressing the corresponding number.
-    I
-        Estimates P1-5 for all waveforms on the first press. N1-5 for all
-        waveforms on the second press. After that, nothing happens.
-    U
-        Updates guess for corresponding P or N of successive waveforms based on
-        position of currently toggled P or N.
-    N
-        Toggles normalized view of waveform.
-    +/- keys
-        Increases/decreases scaling factor of waveform.
-    S
-        Saves amplitude and latency of peaks.
-    T
-        Set threshold to current waveform.
-    Alt+Up
-        Indicate that all waveforms are below threshold.
-    Alt+Down
-        Indicate that all waveforms are above threshold.
-
-Some keys will repeat if you hold down the key, which may be useful when navigating through the waveforms or adjusting the location of a peak.
+Instructions for using the program are included in the user interface.
 
 # Attributions
 
-Code relating to marking points unscoreable and/or shifting waveforms up/down to ensure they don't run off the plot are adapted from work performed for the United States government and, therefore, are in the public domain. All other part of the code remain licensed under the BSD.
+Code relating to marking points unscoreable and/or shifting waveforms up/down to ensure they don't run off the plot are adapted from work performed for the United States government and, therefore, are in the public domain. All other part of the code remain licensed under the BSD 3-clause.
```

### Comparing `ABR-0.0.8/abr/abr-icon.png` & `ABR-0.0.9/abr/abr-icon.png`

 * *Files identical despite different names*

### Comparing `ABR-0.0.8/abr/abrpanel.py` & `ABR-0.0.9/abr/abrpanel.py`

 * *Files identical despite different names*

### Comparing `ABR-0.0.8/abr/app.py` & `ABR-0.0.9/abr/app.py`

 * *Files identical despite different names*

### Comparing `ABR-0.0.8/abr/data/ABR-52-3` & `ABR-0.0.9/abr/data/ABR-52-3`

 * *Files identical despite different names*

### Comparing `ABR-0.0.8/abr/data/CAP-139-5` & `ABR-0.0.9/abr/data/CAP-139-5`

 * *Files identical despite different names*

### Comparing `ABR-0.0.8/abr/data/CAP-139-5-16.0kHz-Brad-analyzed.txt` & `ABR-0.0.9/abr/data/CAP-139-5-16.0kHz-Brad-analyzed.txt`

 * *Files identical despite different names*

### Comparing `ABR-0.0.8/abr/data/CAP-139-5-16.0kHz-analyzed.txt` & `ABR-0.0.9/abr/data/CAP-139-5-16.0kHz-analyzed.txt`

 * *Files identical despite different names*

### Comparing `ABR-0.0.8/abr/datatype.py` & `ABR-0.0.9/abr/datatype.py`

 * *Files identical despite different names*

### Comparing `ABR-0.0.8/abr/launch_window.enaml` & `ABR-0.0.9/abr/launch_window.enaml`

 * *Files identical despite different names*

### Comparing `ABR-0.0.8/abr/main_window.enaml` & `ABR-0.0.9/abr/main_window.enaml`

 * *Files identical despite different names*

### Comparing `ABR-0.0.8/abr/parsers/EPL.py` & `ABR-0.0.9/abr/parsers/EPL.py`

 * *Files identical despite different names*

### Comparing `ABR-0.0.8/abr/parsers/NCRAR.py` & `ABR-0.0.9/abr/parsers/NCRAR.py`

 * *Files identical despite different names*

### Comparing `ABR-0.0.8/abr/parsers/PSI.py` & `ABR-0.0.9/abr/parsers/PSI.py`

 * *Files identical despite different names*

### Comparing `ABR-0.0.8/abr/parsers/__init__.py` & `ABR-0.0.9/abr/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `ABR-0.0.8/abr/parsers/dataset.py` & `ABR-0.0.9/abr/parsers/dataset.py`

 * *Files identical despite different names*

### Comparing `ABR-0.0.8/abr/peakdetect.py` & `ABR-0.0.9/abr/peakdetect.py`

 * *Files identical despite different names*

### Comparing `ABR-0.0.8/abr/presenter.py` & `ABR-0.0.9/abr/presenter.py`

 * *Files identical despite different names*

### Comparing `ABR-0.0.8/pyproject.toml` & `ABR-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ]
 maintainers = [
     {name = "Brad Buran", email="bburan@alum.mit.edu"},
     {name = "Brad Buran", email="buran@ohsu.edu"},
 ]
 dependencies = [
 	"atom",
-	"enaml[qt5-pyqt]",
+	"enaml[qt5-pyside]",
 	"numpy",
 	"scipy",
 	"pandas",
 	"matplotlib",
 ]
 dynamic = ["version"]
 classifiers = [
```

