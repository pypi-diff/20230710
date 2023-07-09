# Comparing `tmp/bb_dirtree-0.2.1.tar.gz` & `tmp/bb_dirtree-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bb_dirtree-0.2.1.tar", max compression
+gzip compressed data, was "bb_dirtree-0.2.2.tar", max compression
```

## Comparing `bb_dirtree-0.2.1.tar` & `bb_dirtree-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2022-05-30 20:03:10.000000 bb_dirtree-0.2.1/LICENSE
--rw-r--r--   0        0        0     3713 2022-07-19 03:55:14.000000 bb_dirtree-0.2.1/README.md
--rw-r--r--   0        0        0     3804 2022-08-14 02:50:32.000000 bb_dirtree-0.2.1/bbdirtree/COLORS.py
--rw-r--r--   0        0        0     3419 2023-07-09 18:22:47.243423 bb_dirtree-0.2.1/bbdirtree/__init__.py
--rw-r--r--   0        0        0    15995 2023-07-09 19:30:42.350166 bb_dirtree-0.2.1/bbdirtree/__main__.py
--rw-r--r--   0        0        0      554 2023-07-09 19:31:47.003501 bb_dirtree-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4238 1970-01-01 00:00:00.000000 bb_dirtree-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-05-30 20:03:10.000000 bb_dirtree-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3828 2023-07-09 22:45:35.687053 bb_dirtree-0.2.2/README.md
+-rw-r--r--   0        0        0     3804 2022-08-14 02:50:32.000000 bb_dirtree-0.2.2/bbdirtree/COLORS.py
+-rw-r--r--   0        0        0     3419 2023-07-09 18:22:47.243423 bb_dirtree-0.2.2/bbdirtree/__init__.py
+-rw-r--r--   0        0        0    15995 2023-07-09 19:30:42.350166 bb_dirtree-0.2.2/bbdirtree/__main__.py
+-rw-r--r--   0        0        0      554 2023-07-09 22:45:48.697053 bb_dirtree-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4353 1970-01-01 00:00:00.000000 bb_dirtree-0.2.2/PKG-INFO
```

### Comparing `bb_dirtree-0.2.1/LICENSE` & `bb_dirtree-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bb_dirtree-0.2.1/README.md` & `bb_dirtree-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -128,11 +128,17 @@
 
 - added support for windows hidden files
 
 #### v0.1.5 - 5-31-2022
 
 - made corrections to help message
 
-#### v0.5.7 - 6-7-2022
+#### v0.1.7 - 6-7-2022
 
 - changed color of files in html output
 - small changes to output format
+
+#### v0.2.2 - 7-9-2023
+
+- added script to run from $PATH
+- cleaned up code
+- changed header text at top of output
```

### Comparing `bb_dirtree-0.2.1/bbdirtree/COLORS.py` & `bb_dirtree-0.2.2/bbdirtree/COLORS.py`

 * *Files identical despite different names*

### Comparing `bb_dirtree-0.2.1/bbdirtree/__init__.py` & `bb_dirtree-0.2.2/bbdirtree/__init__.py`

 * *Files identical despite different names*

### Comparing `bb_dirtree-0.2.1/bbdirtree/__main__.py` & `bb_dirtree-0.2.2/bbdirtree/__main__.py`

 * *Files identical despite different names*

### Comparing `bb_dirtree-0.2.1/pyproject.toml` & `bb_dirtree-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "BB-DirTree"
-version = "0.2.1"
+version = "0.2.2"
 description = "Create a nice looking directory tree with options"
 authors = ["Erik Beebe <beebeapps_feedback@tuta.io>"]
 license = "MIT"
 packages = [ { include = 'bbdirtree' } ]
 readme = "README.md"
 
 keywords = [ "script", "qt", "files" ]
```

### Comparing `bb_dirtree-0.2.1/PKG-INFO` & `bb_dirtree-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bb-dirtree
-Version: 0.2.1
+Version: 0.2.2
 Summary: Create a nice looking directory tree with options
 License: MIT
 Keywords: script,qt,files
 Author: Erik Beebe
 Author-email: beebeapps_feedback@tuta.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -144,12 +144,18 @@
 
 - added support for windows hidden files
 
 #### v0.1.5 - 5-31-2022
 
 - made corrections to help message
 
-#### v0.5.7 - 6-7-2022
+#### v0.1.7 - 6-7-2022
 
 - changed color of files in html output
 - small changes to output format
 
+#### v0.2.2 - 7-9-2023
+
+- added script to run from $PATH
+- cleaned up code
+- changed header text at top of output
+
```

