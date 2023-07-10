# Comparing `tmp/ephysio-1.0.2.tar.gz` & `tmp/ephysio-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephysio-1.0.2.tar", last modified: Mon Jul 10 00:14:06 2023, max compression
+gzip compressed data, was "ephysio-1.0.3.tar", last modified: Mon Jul 10 00:21:24 2023, max compression
```

## Comparing `ephysio-1.0.2.tar` & `ephysio-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-10 00:14:06.489058 ephysio-1.0.2/
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    35149 2023-01-11 21:50:43.000000 ephysio-1.0.2/LICENSE
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1403 2023-07-10 00:14:06.489058 ephysio-1.0.2/PKG-INFO
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1203 2023-01-11 21:50:43.000000 ephysio-1.0.2/README.md
-drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-10 00:14:06.489058 ephysio-1.0.2/ephysio/
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        3 2023-07-07 19:58:47.000000 ephysio-1.0.2/ephysio/__init__.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    12774 2023-07-09 17:40:03.000000 ephysio-1.0.2/ephysio/kilosortIO.py
--rw-------   0 wagenaar  (1000) wagenaar  (1000)    58616 2023-07-09 18:32:28.000000 ephysio-1.0.2/ephysio/openEphysIO.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     6565 2023-07-09 19:07:25.000000 ephysio-1.0.2/ephysio/spikestats.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    17733 2023-07-09 15:35:19.000000 ephysio-1.0.2/ephysio/vizio.py
-drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-10 00:14:06.489058 ephysio-1.0.2/ephysio.egg-info/
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1403 2023-07-10 00:14:06.000000 ephysio-1.0.2/ephysio.egg-info/PKG-INFO
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      290 2023-07-10 00:14:06.000000 ephysio-1.0.2/ephysio.egg-info/SOURCES.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        1 2023-07-10 00:14:06.000000 ephysio-1.0.2/ephysio.egg-info/dependency_links.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        6 2023-07-10 00:14:06.000000 ephysio-1.0.2/ephysio.egg-info/requires.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        8 2023-07-10 00:14:06.000000 ephysio-1.0.2/ephysio.egg-info/top_level.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      297 2023-07-09 15:32:05.000000 ephysio-1.0.2/pyproject.toml
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)       38 2023-07-10 00:14:06.489058 ephysio-1.0.2/setup.cfg
+drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-10 00:21:24.855644 ephysio-1.0.3/
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    35149 2023-01-11 21:50:43.000000 ephysio-1.0.3/LICENSE
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1403 2023-07-10 00:21:24.855644 ephysio-1.0.3/PKG-INFO
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1203 2023-01-11 21:50:43.000000 ephysio-1.0.3/README.md
+drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-10 00:21:24.851644 ephysio-1.0.3/ephysio/
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        3 2023-07-07 19:58:47.000000 ephysio-1.0.3/ephysio/__init__.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    12774 2023-07-09 17:40:03.000000 ephysio-1.0.3/ephysio/kilosortIO.py
+-rw-------   0 wagenaar  (1000) wagenaar  (1000)    58763 2023-07-10 00:19:49.000000 ephysio-1.0.3/ephysio/openEphysIO.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     6565 2023-07-09 19:07:25.000000 ephysio-1.0.3/ephysio/spikestats.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    17733 2023-07-09 15:35:19.000000 ephysio-1.0.3/ephysio/vizio.py
+drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-10 00:21:24.855644 ephysio-1.0.3/ephysio.egg-info/
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1403 2023-07-10 00:21:24.000000 ephysio-1.0.3/ephysio.egg-info/PKG-INFO
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      290 2023-07-10 00:21:24.000000 ephysio-1.0.3/ephysio.egg-info/SOURCES.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        1 2023-07-10 00:21:24.000000 ephysio-1.0.3/ephysio.egg-info/dependency_links.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        6 2023-07-10 00:21:24.000000 ephysio-1.0.3/ephysio.egg-info/requires.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        8 2023-07-10 00:21:24.000000 ephysio-1.0.3/ephysio.egg-info/top_level.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      297 2023-07-10 00:20:30.000000 ephysio-1.0.3/pyproject.toml
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)       38 2023-07-10 00:21:24.855644 ephysio-1.0.3/setup.cfg
```

### Comparing `ephysio-1.0.2/LICENSE` & `ephysio-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ephysio-1.0.2/PKG-INFO` & `ephysio-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysio
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tools for reading ephys data
 Author-email: Daniel Wagenaar <daw@caltech.edu>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ephysio
 Python code for reading ephys files
```

### Comparing `ephysio-1.0.2/README.md` & `ephysio-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ephysio-1.0.2/ephysio/kilosortIO.py` & `ephysio-1.0.3/ephysio/kilosortIO.py`

 * *Files identical despite different names*

### Comparing `ephysio-1.0.2/ephysio/openEphysIO.py` & `ephysio-1.0.3/ephysio/openEphysIO.py`

 * *Files 0% similar despite different names*

```diff
@@ -1140,14 +1140,18 @@
         recs.sort()
         return int(recs[0][9:])
     
     def _recfolder(self, node, expt=1, rec=1):
         fldr = self.root
         if node is not None:
             fldr += f"/{node}"
+        if expt is None:
+            expt = self._firstexpt(node)
+        if rec is None:
+            rec = self._firstrec(node, expt)
         fldr += f"/experiment{expt}"
         fldr += f"/recording{rec}"
         return fldr
 
     def contfolder(self, stream, expt=1, rec=1, node=None):
         '''CONTFOLDER - Folder name where continuous data is stored
         p = CONTFOLDER(stream) returns the full path of the "continuous" folder for the given stream.
@@ -1184,15 +1188,15 @@
 
     def nodemap(self):
         '''NODEMAP - Map of stream names per node
         NODEMAP() returns a dict mapping node names to lists of the streams
         contained in each node.'''
 
         def explorenodes(node):
-            pattern = self._recfolder(node) + "/continuous/*/timestamps.npy"
+            pattern = self._recfolder(node, None, None) + "/continuous/*/timestamps.npy"
             streams = _quickglob(pattern)
             return streams
 
         if self._nodemap is None:
             nodes = _quickglob(f"{self.root}/*")
             nodemap = {}
             if any([node.startswith("experiment") for node in nodes]):
```

### Comparing `ephysio-1.0.2/ephysio/spikestats.py` & `ephysio-1.0.3/ephysio/spikestats.py`

 * *Files identical despite different names*

### Comparing `ephysio-1.0.2/ephysio/vizio.py` & `ephysio-1.0.3/ephysio/vizio.py`

 * *Files identical despite different names*

### Comparing `ephysio-1.0.2/ephysio.egg-info/PKG-INFO` & `ephysio-1.0.3/ephysio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysio
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tools for reading ephys data
 Author-email: Daniel Wagenaar <daw@caltech.edu>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ephysio
 Python code for reading ephys files
```

