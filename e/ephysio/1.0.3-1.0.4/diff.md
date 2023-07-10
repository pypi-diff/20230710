# Comparing `tmp/ephysio-1.0.3.tar.gz` & `tmp/ephysio-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephysio-1.0.3.tar", last modified: Mon Jul 10 00:21:24 2023, max compression
+gzip compressed data, was "ephysio-1.0.4.tar", last modified: Mon Jul 10 00:28:12 2023, max compression
```

## Comparing `ephysio-1.0.3.tar` & `ephysio-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-10 00:21:24.855644 ephysio-1.0.3/
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    35149 2023-01-11 21:50:43.000000 ephysio-1.0.3/LICENSE
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1403 2023-07-10 00:21:24.855644 ephysio-1.0.3/PKG-INFO
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1203 2023-01-11 21:50:43.000000 ephysio-1.0.3/README.md
-drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-10 00:21:24.851644 ephysio-1.0.3/ephysio/
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        3 2023-07-07 19:58:47.000000 ephysio-1.0.3/ephysio/__init__.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    12774 2023-07-09 17:40:03.000000 ephysio-1.0.3/ephysio/kilosortIO.py
--rw-------   0 wagenaar  (1000) wagenaar  (1000)    58763 2023-07-10 00:19:49.000000 ephysio-1.0.3/ephysio/openEphysIO.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     6565 2023-07-09 19:07:25.000000 ephysio-1.0.3/ephysio/spikestats.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    17733 2023-07-09 15:35:19.000000 ephysio-1.0.3/ephysio/vizio.py
-drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-10 00:21:24.855644 ephysio-1.0.3/ephysio.egg-info/
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1403 2023-07-10 00:21:24.000000 ephysio-1.0.3/ephysio.egg-info/PKG-INFO
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      290 2023-07-10 00:21:24.000000 ephysio-1.0.3/ephysio.egg-info/SOURCES.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        1 2023-07-10 00:21:24.000000 ephysio-1.0.3/ephysio.egg-info/dependency_links.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        6 2023-07-10 00:21:24.000000 ephysio-1.0.3/ephysio.egg-info/requires.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        8 2023-07-10 00:21:24.000000 ephysio-1.0.3/ephysio.egg-info/top_level.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      297 2023-07-10 00:20:30.000000 ephysio-1.0.3/pyproject.toml
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)       38 2023-07-10 00:21:24.855644 ephysio-1.0.3/setup.cfg
+drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-10 00:28:12.534234 ephysio-1.0.4/
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    35149 2023-01-11 21:50:43.000000 ephysio-1.0.4/LICENSE
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1403 2023-07-10 00:28:12.534234 ephysio-1.0.4/PKG-INFO
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1203 2023-01-11 21:50:43.000000 ephysio-1.0.4/README.md
+drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-10 00:28:12.534234 ephysio-1.0.4/ephysio/
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        3 2023-07-07 19:58:47.000000 ephysio-1.0.4/ephysio/__init__.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    12774 2023-07-09 17:40:03.000000 ephysio-1.0.4/ephysio/kilosortIO.py
+-rw-------   0 wagenaar  (1000) wagenaar  (1000)    58919 2023-07-10 00:27:28.000000 ephysio-1.0.4/ephysio/openEphysIO.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     6565 2023-07-09 19:07:25.000000 ephysio-1.0.4/ephysio/spikestats.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    17733 2023-07-09 15:35:19.000000 ephysio-1.0.4/ephysio/vizio.py
+drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-10 00:28:12.534234 ephysio-1.0.4/ephysio.egg-info/
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1403 2023-07-10 00:28:12.000000 ephysio-1.0.4/ephysio.egg-info/PKG-INFO
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      290 2023-07-10 00:28:12.000000 ephysio-1.0.4/ephysio.egg-info/SOURCES.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        1 2023-07-10 00:28:12.000000 ephysio-1.0.4/ephysio.egg-info/dependency_links.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        6 2023-07-10 00:28:12.000000 ephysio-1.0.4/ephysio.egg-info/requires.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        8 2023-07-10 00:28:12.000000 ephysio-1.0.4/ephysio.egg-info/top_level.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      297 2023-07-10 00:27:47.000000 ephysio-1.0.4/pyproject.toml
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)       38 2023-07-10 00:28:12.534234 ephysio-1.0.4/setup.cfg
```

### Comparing `ephysio-1.0.3/LICENSE` & `ephysio-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ephysio-1.0.3/PKG-INFO` & `ephysio-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysio
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tools for reading ephys data
 Author-email: Daniel Wagenaar <daw@caltech.edu>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ephysio
 Python code for reading ephys files
```

### Comparing `ephysio-1.0.3/README.md` & `ephysio-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ephysio-1.0.3/ephysio/kilosortIO.py` & `ephysio-1.0.4/ephysio/kilosortIO.py`

 * *Files identical despite different names*

### Comparing `ephysio-1.0.3/ephysio/openEphysIO.py` & `ephysio-1.0.4/ephysio/openEphysIO.py`

 * *Files 1% similar despite different names*

```diff
@@ -1014,15 +1014,15 @@
         nidaqs = set(self.nidaqstreams())
         ss = []
         for node, streams in self.nodemap().items():
             fsmax = 0
             fsbystream = {}
             for s in streams:
                 if s not in nidaqs:
-                    fs = self.samplingrate(s, node=node)
+                    fs = self.samplingrate(s, node=node, expt=None, rec=None)
                     fsbystream[s] = fs
                     fsmax = max(fsmax, fs)
             for s in streams:
                 if s not in nidaqs:
                     if fsbystream[s] == fsmax:
                         ss.append(s)
         return ss
@@ -1230,14 +1230,18 @@
         '''SAMPLINGRATE - Sampling rate of a stream
         SIMPLINGRATE(stream), where STREAM is one of the items returned
         by STREAMS() or its friends, returns the sampling rate of that
         stream in Hertz. Optional experiments EXPT and REC specify the
         "experiment" and "recording", but those can usually be left out,
         as the sampling rate is generally consistent for a whole session.'''
         node = self._autonode(stream, node)
+        if expt is None:
+            expt = self._firstexpt(node)
+        if rec is None:
+            rec = self._firstrec(node, expt)
         _populate(self._sfreqs, node, expt, rec)
         if stream not in self._sfreqs[node][expt][rec]:
             info = self._oebinsection(expt, rec, stream=stream, node=node)
             self._sfreqs[node][expt][rec][stream] = info['sample_rate']
         return self._sfreqs[node][expt][rec][stream]
 
     def data(self, stream, expt=1, rec=1, node=None, stage='continuous'):
```

### Comparing `ephysio-1.0.3/ephysio/spikestats.py` & `ephysio-1.0.4/ephysio/spikestats.py`

 * *Files identical despite different names*

### Comparing `ephysio-1.0.3/ephysio/vizio.py` & `ephysio-1.0.4/ephysio/vizio.py`

 * *Files identical despite different names*

### Comparing `ephysio-1.0.3/ephysio.egg-info/PKG-INFO` & `ephysio-1.0.4/ephysio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysio
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tools for reading ephys data
 Author-email: Daniel Wagenaar <daw@caltech.edu>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ephysio
 Python code for reading ephys files
```

