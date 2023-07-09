# Comparing `tmp/katottglib-0.2.1.tar.gz` & `tmp/katottglib-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katottglib-0.2.1.tar", last modified: Sun Jul  9 19:46:58 2023, max compression
+gzip compressed data, was "katottglib-0.2.2.tar", last modified: Sun Jul  9 22:02:38 2023, max compression
```

## Comparing `katottglib-0.2.1.tar` & `katottglib-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-09 19:46:58.365025 katottglib-0.2.1/
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1073 2023-06-06 21:02:05.000000 katottglib-0.2.1/LICENSE
--rw-r--r--   0 dsenchishen   (502) staff       (20)       30 2023-07-09 19:43:57.000000 katottglib-0.2.1/MANIFEST.in
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1227 2023-07-09 19:46:58.365273 katottglib-0.2.1/PKG-INFO
--rw-r--r--   0 dsenchishen   (502) staff       (20)      656 2023-07-09 19:45:57.000000 katottglib-0.2.1/README.rst
-drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-09 19:46:58.358248 katottglib-0.2.1/data/
--rw-r--r--   0 dsenchishen   (502) staff       (20)       53 2023-06-06 21:02:05.000000 katottglib-0.2.1/data/__init__.py
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1534 2023-07-01 12:09:31.000000 katottglib-0.2.1/data/data.py
--rw-r--r--   0 dsenchishen   (502) staff       (20)      586 2023-06-06 21:02:05.000000 katottglib-0.2.1/data/entity.py
--rw-r--r--   0 dsenchishen   (502) staff       (20)  1476983 2023-06-04 05:40:38.000000 katottglib-0.2.1/data/kodifikator.xlsx
-drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-09 19:46:58.364051 katottglib-0.2.1/katottglib.egg-info/
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1227 2023-07-09 19:46:58.000000 katottglib-0.2.1/katottglib.egg-info/PKG-INFO
--rw-r--r--   0 dsenchishen   (502) staff       (20)      284 2023-07-09 19:46:58.000000 katottglib-0.2.1/katottglib.egg-info/SOURCES.txt
--rw-r--r--   0 dsenchishen   (502) staff       (20)        1 2023-07-09 19:46:58.000000 katottglib-0.2.1/katottglib.egg-info/dependency_links.txt
--rw-r--r--   0 dsenchishen   (502) staff       (20)       10 2023-07-09 19:46:58.000000 katottglib-0.2.1/katottglib.egg-info/top_level.txt
--rw-r--r--   0 dsenchishen   (502) staff       (20)      406 2023-06-06 21:02:05.000000 katottglib-0.2.1/pyproject.toml
--rw-r--r--   0 dsenchishen   (502) staff       (20)      639 2023-07-09 19:46:58.365784 katottglib-0.2.1/setup.cfg
--rw-r--r--   0 dsenchishen   (502) staff       (20)       38 2021-03-15 19:22:38.000000 katottglib-0.2.1/setup.py
-drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-09 19:46:58.364456 katottglib-0.2.1/test/
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1878 2023-06-09 20:22:51.000000 katottglib-0.2.1/test/__init__.py
+drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-09 22:02:38.263825 katottglib-0.2.2/
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1073 2023-06-06 21:02:05.000000 katottglib-0.2.2/LICENSE
+-rw-r--r--   0 dsenchishen   (502) staff       (20)       30 2023-07-09 19:43:57.000000 katottglib-0.2.2/MANIFEST.in
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1294 2023-07-09 22:02:38.264187 katottglib-0.2.2/PKG-INFO
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      723 2023-07-09 21:57:06.000000 katottglib-0.2.2/README.rst
+drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-09 22:02:38.250880 katottglib-0.2.2/data/
+-rw-r--r--   0 dsenchishen   (502) staff       (20)       53 2023-06-06 21:02:05.000000 katottglib-0.2.2/data/__init__.py
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1534 2023-07-01 12:09:31.000000 katottglib-0.2.2/data/data.py
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      586 2023-06-06 21:02:05.000000 katottglib-0.2.2/data/entity.py
+-rw-r--r--   0 dsenchishen   (502) staff       (20)  1476983 2023-06-04 05:40:38.000000 katottglib-0.2.2/data/kodifikator.xlsx
+drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-09 22:02:38.261993 katottglib-0.2.2/katottglib.egg-info/
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1294 2023-07-09 22:02:38.000000 katottglib-0.2.2/katottglib.egg-info/PKG-INFO
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      284 2023-07-09 22:02:38.000000 katottglib-0.2.2/katottglib.egg-info/SOURCES.txt
+-rw-r--r--   0 dsenchishen   (502) staff       (20)        1 2023-07-09 22:02:38.000000 katottglib-0.2.2/katottglib.egg-info/dependency_links.txt
+-rw-r--r--   0 dsenchishen   (502) staff       (20)       10 2023-07-09 22:02:38.000000 katottglib-0.2.2/katottglib.egg-info/top_level.txt
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      406 2023-06-06 21:02:05.000000 katottglib-0.2.2/pyproject.toml
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      639 2023-07-09 22:02:38.265085 katottglib-0.2.2/setup.cfg
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      346 2023-07-09 22:02:35.000000 katottglib-0.2.2/setup.py
+drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-09 22:02:38.262798 katottglib-0.2.2/test/
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1878 2023-06-09 20:22:51.000000 katottglib-0.2.2/test/__init__.py
```

### Comparing `katottglib-0.2.1/LICENSE` & `katottglib-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `katottglib-0.2.1/PKG-INFO` & `katottglib-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katottglib
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python lib to operate KATOTTG addresses (classified administrative division of Ukraine).
 Home-page: https://github.com/sen-den/katottglib
 Author: Denis Senchishen
 Author-email: dsenchishen@icloud.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -24,14 +24,20 @@
 - Install with `pip install katottglib`
 - Import `import katottglib`
 - Search for entities with `find_by_name` `katottglib.find_by_name(name="Lviv")`
 
 Release notes
 -------------
 
+v0.2.2 (2023-07-10)
+...................
+
+Updated setup.py config
+
+
 v0.2.1 (2023-07-09)
 ...................
 
 Fixes and improvements to performance.
 
 - data/kodifikator.xlsx is included into the dist.
```

### Comparing `katottglib-0.2.1/README.rst` & `katottglib-0.2.2/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 - Install with `pip install katottglib`
 - Import `import katottglib`
 - Search for entities with `find_by_name` `katottglib.find_by_name(name="Lviv")`
 
 Release notes
 -------------
 
+v0.2.2 (2023-07-10)
+...................
+
+Updated setup.py config
+
+
 v0.2.1 (2023-07-09)
 ...................
 
 Fixes and improvements to performance.
 
 - data/kodifikator.xlsx is included into the dist.
```

### Comparing `katottglib-0.2.1/data/data.py` & `katottglib-0.2.2/data/data.py`

 * *Files identical despite different names*

### Comparing `katottglib-0.2.1/data/entity.py` & `katottglib-0.2.2/data/entity.py`

 * *Files identical despite different names*

### Comparing `katottglib-0.2.1/data/kodifikator.xlsx` & `katottglib-0.2.2/data/kodifikator.xlsx`

 * *Files identical despite different names*

### Comparing `katottglib-0.2.1/katottglib.egg-info/PKG-INFO` & `katottglib-0.2.2/katottglib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katottglib
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python lib to operate KATOTTG addresses (classified administrative division of Ukraine).
 Home-page: https://github.com/sen-den/katottglib
 Author: Denis Senchishen
 Author-email: dsenchishen@icloud.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -24,14 +24,20 @@
 - Install with `pip install katottglib`
 - Import `import katottglib`
 - Search for entities with `find_by_name` `katottglib.find_by_name(name="Lviv")`
 
 Release notes
 -------------
 
+v0.2.2 (2023-07-10)
+...................
+
+Updated setup.py config
+
+
 v0.2.1 (2023-07-09)
 ...................
 
 Fixes and improvements to performance.
 
 - data/kodifikator.xlsx is included into the dist.
```

### Comparing `katottglib-0.2.1/setup.cfg` & `katottglib-0.2.2/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = katottglib
-version = 0.2.1
+version = 0.2.2
 description = A Python lib to operate KATOTTG addresses (classified administrative division of Ukraine).
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/sen-den/katottglib
 author = Denis Senchishen
 author_email = dsenchishen@icloud.com
 license = MIT
```

### Comparing `katottglib-0.2.1/test/__init__.py` & `katottglib-0.2.2/test/__init__.py`

 * *Files identical despite different names*

