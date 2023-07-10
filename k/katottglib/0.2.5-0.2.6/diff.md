# Comparing `tmp/katottglib-0.2.5.tar.gz` & `tmp/katottglib-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katottglib-0.2.5.tar", last modified: Mon Jul 10 07:36:25 2023, max compression
+gzip compressed data, was "katottglib-0.2.6.tar", last modified: Mon Jul 10 08:27:17 2023, max compression
```

## Comparing `katottglib-0.2.5.tar` & `katottglib-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-10 07:36:25.359605 katottglib-0.2.5/
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1073 2023-06-06 21:02:05.000000 katottglib-0.2.5/LICENSE
--rw-r--r--   0 dsenchishen   (502) staff       (20)       30 2023-07-09 19:43:57.000000 katottglib-0.2.5/MANIFEST.in
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1558 2023-07-10 07:36:25.359730 katottglib-0.2.5/PKG-INFO
--rw-r--r--   0 dsenchishen   (502) staff       (20)      987 2023-07-10 07:36:01.000000 katottglib-0.2.5/README.rst
-drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-10 07:36:25.357452 katottglib-0.2.5/katottglib/
--rw-r--r--   0 dsenchishen   (502) staff       (20)       59 2023-07-09 22:22:03.000000 katottglib-0.2.5/katottglib/__init__.py
--rw-r--r--   0 dsenchishen   (502) staff       (20)     3632 2023-07-10 07:33:20.000000 katottglib-0.2.5/katottglib/katottg.py
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1845 2023-07-09 22:18:42.000000 katottglib-0.2.5/katottglib/test.py
-drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-10 07:36:25.359377 katottglib-0.2.5/katottglib.egg-info/
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1558 2023-07-10 07:36:25.000000 katottglib-0.2.5/katottglib.egg-info/PKG-INFO
--rw-r--r--   0 dsenchishen   (502) staff       (20)      297 2023-07-10 07:36:25.000000 katottglib-0.2.5/katottglib.egg-info/SOURCES.txt
--rw-r--r--   0 dsenchishen   (502) staff       (20)        1 2023-07-10 07:36:25.000000 katottglib-0.2.5/katottglib.egg-info/dependency_links.txt
--rw-r--r--   0 dsenchishen   (502) staff       (20)       30 2023-07-10 07:36:25.000000 katottglib-0.2.5/katottglib.egg-info/requires.txt
--rw-r--r--   0 dsenchishen   (502) staff       (20)       11 2023-07-10 07:36:25.000000 katottglib-0.2.5/katottglib.egg-info/top_level.txt
--rw-r--r--   0 dsenchishen   (502) staff       (20)      406 2023-06-06 21:02:05.000000 katottglib-0.2.5/pyproject.toml
--rw-r--r--   0 dsenchishen   (502) staff       (20)      639 2023-07-10 07:36:25.360145 katottglib-0.2.5/setup.cfg
--rw-r--r--   0 dsenchishen   (502) staff       (20)      427 2023-07-10 07:36:01.000000 katottglib-0.2.5/setup.py
+drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-10 08:27:17.103701 katottglib-0.2.6/
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1073 2023-06-06 21:02:05.000000 katottglib-0.2.6/LICENSE
+-rw-r--r--   0 dsenchishen   (502) staff       (20)       36 2023-07-10 08:27:10.000000 katottglib-0.2.6/MANIFEST.in
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1661 2023-07-10 08:27:17.103900 katottglib-0.2.6/PKG-INFO
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1090 2023-07-10 08:27:10.000000 katottglib-0.2.6/README.rst
+drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-10 08:27:17.100355 katottglib-0.2.6/katottglib/
+-rw-r--r--   0 dsenchishen   (502) staff       (20)       59 2023-07-09 22:22:03.000000 katottglib-0.2.6/katottglib/__init__.py
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1534 2023-07-01 12:09:31.000000 katottglib-0.2.6/katottglib/data.py
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      586 2023-06-06 21:02:05.000000 katottglib-0.2.6/katottglib/entity.py
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     3627 2023-07-10 08:23:06.000000 katottglib-0.2.6/katottglib/katottg.py
+-rw-r--r--   0 dsenchishen   (502) staff       (20)  1476983 2023-06-04 05:40:38.000000 katottglib-0.2.6/katottglib/kodifikator.xlsx
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1845 2023-07-09 22:18:42.000000 katottglib-0.2.6/katottglib/test.py
+drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-10 08:27:17.103325 katottglib-0.2.6/katottglib.egg-info/
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1661 2023-07-10 08:27:17.000000 katottglib-0.2.6/katottglib.egg-info/PKG-INFO
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      365 2023-07-10 08:27:17.000000 katottglib-0.2.6/katottglib.egg-info/SOURCES.txt
+-rw-r--r--   0 dsenchishen   (502) staff       (20)        1 2023-07-10 08:27:17.000000 katottglib-0.2.6/katottglib.egg-info/dependency_links.txt
+-rw-r--r--   0 dsenchishen   (502) staff       (20)       30 2023-07-10 08:27:17.000000 katottglib-0.2.6/katottglib.egg-info/requires.txt
+-rw-r--r--   0 dsenchishen   (502) staff       (20)       11 2023-07-10 08:27:17.000000 katottglib-0.2.6/katottglib.egg-info/top_level.txt
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      406 2023-06-06 21:02:05.000000 katottglib-0.2.6/pyproject.toml
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      639 2023-07-10 08:27:17.104821 katottglib-0.2.6/setup.cfg
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      427 2023-07-10 08:27:10.000000 katottglib-0.2.6/setup.py
```

### Comparing `katottglib-0.2.5/LICENSE` & `katottglib-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `katottglib-0.2.5/PKG-INFO` & `katottglib-0.2.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katottglib
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Python lib to operate KATOTTG addresses (classified administrative division of Ukraine).
 Home-page: https://github.com/sen-den/katottglib
 Author: Denis Senchishen
 Author-email: dsenchishen@icloud.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -24,14 +24,19 @@
 - Install with `pip install katottglib`
 - Import `import katottglib`
 - Search for entities with `find_by_name` `katottglib.find_by_name(name="Lviv")`
 
 Release notes
 -------------
 
+v0.2.6 (2023-07-10)
+...................
+
+Try to fix continuation import errors on some installations.
+
 v0.2.5 (2023-07-10)
 ...................
 
 Fix import statements to be consistent.
 
 
 v0.2.4 (2023-07-10)
```

### Comparing `katottglib-0.2.5/README.rst` & `katottglib-0.2.6/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 - Install with `pip install katottglib`
 - Import `import katottglib`
 - Search for entities with `find_by_name` `katottglib.find_by_name(name="Lviv")`
 
 Release notes
 -------------
 
+v0.2.6 (2023-07-10)
+...................
+
+Try to fix continuation import errors on some installations.
+
 v0.2.5 (2023-07-10)
 ...................
 
 Fix import statements to be consistent.
 
 
 v0.2.4 (2023-07-10)
```

### Comparing `katottglib-0.2.5/katottglib/katottg.py` & `katottglib-0.2.6/katottglib/katottg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from difflib import SequenceMatcher
 
 import pandas as pd
 
 from katottglib.data import load_data
-from katottglib.data.entity import KatottgEntity
+from katottglib.entity import KatottgEntity
 
 
 __all__ = [
     "find_by_name",
     "find_by_id",
 ]
```

### Comparing `katottglib-0.2.5/katottglib/test.py` & `katottglib-0.2.6/katottglib/test.py`

 * *Files identical despite different names*

### Comparing `katottglib-0.2.5/katottglib.egg-info/PKG-INFO` & `katottglib-0.2.6/katottglib.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katottglib
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Python lib to operate KATOTTG addresses (classified administrative division of Ukraine).
 Home-page: https://github.com/sen-den/katottglib
 Author: Denis Senchishen
 Author-email: dsenchishen@icloud.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -24,14 +24,19 @@
 - Install with `pip install katottglib`
 - Import `import katottglib`
 - Search for entities with `find_by_name` `katottglib.find_by_name(name="Lviv")`
 
 Release notes
 -------------
 
+v0.2.6 (2023-07-10)
+...................
+
+Try to fix continuation import errors on some installations.
+
 v0.2.5 (2023-07-10)
 ...................
 
 Fix import statements to be consistent.
 
 
 v0.2.4 (2023-07-10)
```

### Comparing `katottglib-0.2.5/setup.cfg` & `katottglib-0.2.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = katottglib
-version = 0.2.5
+version = 0.2.6
 description = A Python lib to operate KATOTTG addresses (classified administrative division of Ukraine).
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/sen-den/katottglib
 author = Denis Senchishen
 author_email = dsenchishen@icloud.com
 license = MIT
```

