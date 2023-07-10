# Comparing `tmp/ufomerge-1.2.0.tar.gz` & `tmp/ufomerge-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufomerge-1.2.0.tar", last modified: Wed Jun 21 09:58:43 2023, max compression
+gzip compressed data, was "ufomerge-1.3.0.tar", last modified: Mon Jul 10 11:28:26 2023, max compression
```

## Comparing `ufomerge-1.2.0.tar` & `ufomerge-1.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-21 09:58:43.276602 ufomerge-1.2.0/
--rw-r--r--   0 simon      (501) staff       (20)      302 2023-05-04 21:34:42.000000 ufomerge-1.2.0/AUTHORS.txt
--rw-r--r--   0 simon      (501) staff       (20)     1060 2023-05-04 21:34:45.000000 ufomerge-1.2.0/CONTRIBUTORS.txt
--rw-r--r--   0 simon      (501) staff       (20)    11358 2023-05-04 21:33:18.000000 ufomerge-1.2.0/LICENSE
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-21 09:58:43.272517 ufomerge-1.2.0/Lib/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-21 09:58:43.274703 ufomerge-1.2.0/Lib/ufomerge/
--rw-r--r--   0 simon      (501) staff       (20)    30294 2023-06-21 09:41:06.000000 ufomerge-1.2.0/Lib/ufomerge/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)       87 2023-05-04 20:25:37.000000 ufomerge-1.2.0/Lib/ufomerge/__main__.py
--rw-r--r--   0 simon      (501) staff       (20)      160 2023-06-21 09:58:43.000000 ufomerge-1.2.0/Lib/ufomerge/_version.py
--rw-r--r--   0 simon      (501) staff       (20)     4261 2023-05-04 21:10:17.000000 ufomerge-1.2.0/Lib/ufomerge/cli.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-21 09:58:43.275535 ufomerge-1.2.0/Lib/ufomerge.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)     2402 2023-06-21 09:58:43.000000 ufomerge-1.2.0/Lib/ufomerge.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)      433 2023-06-21 09:58:43.000000 ufomerge-1.2.0/Lib/ufomerge.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2023-06-21 09:58:43.000000 ufomerge-1.2.0/Lib/ufomerge.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)       47 2023-06-21 09:58:43.000000 ufomerge-1.2.0/Lib/ufomerge.egg-info/entry_points.txt
--rw-r--r--   0 simon      (501) staff       (20)       18 2023-06-21 09:58:43.000000 ufomerge-1.2.0/Lib/ufomerge.egg-info/requires.txt
--rw-r--r--   0 simon      (501) staff       (20)        9 2023-06-21 09:58:43.000000 ufomerge-1.2.0/Lib/ufomerge.egg-info/top_level.txt
--rw-r--r--   0 simon      (501) staff       (20)     2402 2023-06-21 09:58:43.276459 ufomerge-1.2.0/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)     2073 2023-05-04 21:34:01.000000 ufomerge-1.2.0/README.md
--rw-r--r--   0 simon      (501) staff       (20)      616 2023-06-21 09:02:36.000000 ufomerge-1.2.0/pyproject.toml
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-21 09:58:43.276635 ufomerge-1.2.0/setup.cfg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-21 09:58:43.276174 ufomerge-1.2.0/tests/
--rw-r--r--   0 simon      (501) staff       (20)     1357 2023-05-04 13:39:59.000000 ufomerge-1.2.0/tests/conftest.py
--rw-r--r--   0 simon      (501) staff       (20)     1315 2023-05-04 13:16:44.000000 ufomerge-1.2.0/tests/test_basic.py
--rw-r--r--   0 simon      (501) staff       (20)     2969 2023-05-04 17:05:29.000000 ufomerge-1.2.0/tests/test_layout.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-10 11:28:26.533823 ufomerge-1.3.0/
+-rw-r--r--   0 simon      (501) staff       (20)      302 2023-05-04 21:34:42.000000 ufomerge-1.3.0/AUTHORS.txt
+-rw-r--r--   0 simon      (501) staff       (20)     1060 2023-05-04 21:34:45.000000 ufomerge-1.3.0/CONTRIBUTORS.txt
+-rw-r--r--   0 simon      (501) staff       (20)    11358 2023-05-04 21:33:18.000000 ufomerge-1.3.0/LICENSE
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-10 11:28:26.529764 ufomerge-1.3.0/Lib/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-10 11:28:26.531685 ufomerge-1.3.0/Lib/ufomerge/
+-rw-r--r--   0 simon      (501) staff       (20)    32172 2023-07-10 11:26:04.000000 ufomerge-1.3.0/Lib/ufomerge/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)       87 2023-05-04 20:25:37.000000 ufomerge-1.3.0/Lib/ufomerge/__main__.py
+-rw-r--r--   0 simon      (501) staff       (20)      160 2023-07-10 11:28:26.000000 ufomerge-1.3.0/Lib/ufomerge/_version.py
+-rw-r--r--   0 simon      (501) staff       (20)     4261 2023-05-04 21:10:17.000000 ufomerge-1.3.0/Lib/ufomerge/cli.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-10 11:28:26.532528 ufomerge-1.3.0/Lib/ufomerge.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     2402 2023-07-10 11:28:26.000000 ufomerge-1.3.0/Lib/ufomerge.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)      433 2023-07-10 11:28:26.000000 ufomerge-1.3.0/Lib/ufomerge.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2023-07-10 11:28:26.000000 ufomerge-1.3.0/Lib/ufomerge.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)       47 2023-07-10 11:28:26.000000 ufomerge-1.3.0/Lib/ufomerge.egg-info/entry_points.txt
+-rw-r--r--   0 simon      (501) staff       (20)       18 2023-07-10 11:28:26.000000 ufomerge-1.3.0/Lib/ufomerge.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)        9 2023-07-10 11:28:26.000000 ufomerge-1.3.0/Lib/ufomerge.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)     2402 2023-07-10 11:28:26.533636 ufomerge-1.3.0/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)     2073 2023-05-04 21:34:01.000000 ufomerge-1.3.0/README.md
+-rw-r--r--   0 simon      (501) staff       (20)      616 2023-06-21 09:02:36.000000 ufomerge-1.3.0/pyproject.toml
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-07-10 11:28:26.533876 ufomerge-1.3.0/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-10 11:28:26.533214 ufomerge-1.3.0/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     1357 2023-05-04 13:39:59.000000 ufomerge-1.3.0/tests/conftest.py
+-rw-r--r--   0 simon      (501) staff       (20)     1315 2023-05-04 13:16:44.000000 ufomerge-1.3.0/tests/test_basic.py
+-rw-r--r--   0 simon      (501) staff       (20)     2969 2023-05-04 17:05:29.000000 ufomerge-1.3.0/tests/test_layout.py
```

### Comparing `ufomerge-1.2.0/CONTRIBUTORS.txt` & `ufomerge-1.3.0/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `ufomerge-1.2.0/LICENSE` & `ufomerge-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ufomerge-1.2.0/Lib/ufomerge/__init__.py` & `ufomerge-1.3.0/Lib/ufomerge/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import defaultdict
 import copy
 from io import StringIO
 import logging
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Iterable, OrderedDict, Set, Tuple
 
@@ -45,18 +46,54 @@
         # Set up the glyphset
 
         if not self.glyphs and not self.codepoints:
             self.glyphs = self.ufo2.keys()
 
         self.incoming_glyphset = dict.fromkeys(self.glyphs, True)
 
-        for glyph in self.ufo2:
-            if any(cp in self.codepoints for cp in glyph.unicodes):
-                if glyph.name is not None:
-                    self.incoming_glyphset[glyph.name] = True
+        # Now add codepoints
+        if self.codepoints:
+            existing_map = {}
+            to_delete = defaultdict(list)
+            for glyph in self.ufo1:
+                for cp in glyph.unicodes:
+                    existing_map[cp] = glyph.name
+
+            for glyph in self.ufo2:
+                for cp in glyph.unicodes:
+                    if cp in self.codepoints:
+                        # But see if we have a corresponding glyph already
+                        if cp in existing_map:
+                            if self.existing_handling == "skip":
+                                logger.info(
+                                    "Skipping codepoint U+%04X already present as '%s' in target file"
+                                    % (cp, glyph.name)
+                                )
+                                # Blacklist this glyph
+                                if glyph.name in self.incoming_glyphset:
+                                    del self.incoming_glyphset[glyph.name]
+                                break
+                            elif self.existing_handling == "replace":
+                                to_delete[existing_map[cp]].append(cp)
+                        if glyph.name is not None:
+                            self.incoming_glyphset[glyph.name] = True
+
+            # Clear up any glyphs for UFO1 we don't want any more
+            for glyphname, codepoints in to_delete.items():
+                self.ufo1[glyphname].unicodes = list(
+                    set(self.ufo1[glyphname].unicodes) - set(codepoints)
+                )
+                codepoints_string = ", ".join("U+%04X" % cp for cp in codepoints)
+                logger.info(
+                    "Removing mappings %s from glyph '%s' due to incoming codepoints"
+                    % (codepoints_string, glyphname)
+                )
+                # We *could* delete it from the target glyphset, but there
+                # is a problem here - what if it's actually mentioned in the
+                # feature file?! So we don't.
 
         for glyph in self.exclude_glyphs:
             del self.incoming_glyphset[glyph]
 
         # Check those glyphs actually are in UFO 2
         not_there = set(self.incoming_glyphset) - set(self.ufo2.keys())
         if len(not_there):
```

### Comparing `ufomerge-1.2.0/Lib/ufomerge/cli.py` & `ufomerge-1.3.0/Lib/ufomerge/cli.py`

 * *Files identical despite different names*

### Comparing `ufomerge-1.2.0/Lib/ufomerge.egg-info/PKG-INFO` & `ufomerge-1.3.0/Lib/ufomerge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufomerge
-Version: 1.2.0
+Version: 1.3.0
 Summary: Merge together two source fonts in UFO format
 Author-email: Simon Cozens <simon@simon-cozens.org>
 Classifier: Environment :: Console
 Classifier: Topic :: Text Processing :: Fonts
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.txt
```

### Comparing `ufomerge-1.2.0/PKG-INFO` & `ufomerge-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufomerge
-Version: 1.2.0
+Version: 1.3.0
 Summary: Merge together two source fonts in UFO format
 Author-email: Simon Cozens <simon@simon-cozens.org>
 Classifier: Environment :: Console
 Classifier: Topic :: Text Processing :: Fonts
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.txt
```

### Comparing `ufomerge-1.2.0/README.md` & `ufomerge-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ufomerge-1.2.0/pyproject.toml` & `ufomerge-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ufomerge-1.2.0/tests/conftest.py` & `ufomerge-1.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ufomerge-1.2.0/tests/test_basic.py` & `ufomerge-1.3.0/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `ufomerge-1.2.0/tests/test_layout.py` & `ufomerge-1.3.0/tests/test_layout.py`

 * *Files identical despite different names*

