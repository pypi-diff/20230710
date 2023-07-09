# Comparing `tmp/katottglib-0.2.2.tar.gz` & `tmp/katottglib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katottglib-0.2.2.tar", last modified: Sun Jul  9 22:02:38 2023, max compression
+gzip compressed data, was "katottglib-0.2.3.tar", last modified: Sun Jul  9 22:25:49 2023, max compression
```

## Comparing `katottglib-0.2.2.tar` & `katottglib-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-09 22:02:38.263825 katottglib-0.2.2/
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1073 2023-06-06 21:02:05.000000 katottglib-0.2.2/LICENSE
--rw-r--r--   0 dsenchishen   (502) staff       (20)       30 2023-07-09 19:43:57.000000 katottglib-0.2.2/MANIFEST.in
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1294 2023-07-09 22:02:38.264187 katottglib-0.2.2/PKG-INFO
--rw-r--r--   0 dsenchishen   (502) staff       (20)      723 2023-07-09 21:57:06.000000 katottglib-0.2.2/README.rst
-drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-09 22:02:38.250880 katottglib-0.2.2/data/
--rw-r--r--   0 dsenchishen   (502) staff       (20)       53 2023-06-06 21:02:05.000000 katottglib-0.2.2/data/__init__.py
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1534 2023-07-01 12:09:31.000000 katottglib-0.2.2/data/data.py
--rw-r--r--   0 dsenchishen   (502) staff       (20)      586 2023-06-06 21:02:05.000000 katottglib-0.2.2/data/entity.py
--rw-r--r--   0 dsenchishen   (502) staff       (20)  1476983 2023-06-04 05:40:38.000000 katottglib-0.2.2/data/kodifikator.xlsx
-drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-09 22:02:38.261993 katottglib-0.2.2/katottglib.egg-info/
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1294 2023-07-09 22:02:38.000000 katottglib-0.2.2/katottglib.egg-info/PKG-INFO
--rw-r--r--   0 dsenchishen   (502) staff       (20)      284 2023-07-09 22:02:38.000000 katottglib-0.2.2/katottglib.egg-info/SOURCES.txt
--rw-r--r--   0 dsenchishen   (502) staff       (20)        1 2023-07-09 22:02:38.000000 katottglib-0.2.2/katottglib.egg-info/dependency_links.txt
--rw-r--r--   0 dsenchishen   (502) staff       (20)       10 2023-07-09 22:02:38.000000 katottglib-0.2.2/katottglib.egg-info/top_level.txt
--rw-r--r--   0 dsenchishen   (502) staff       (20)      406 2023-06-06 21:02:05.000000 katottglib-0.2.2/pyproject.toml
--rw-r--r--   0 dsenchishen   (502) staff       (20)      639 2023-07-09 22:02:38.265085 katottglib-0.2.2/setup.cfg
--rw-r--r--   0 dsenchishen   (502) staff       (20)      346 2023-07-09 22:02:35.000000 katottglib-0.2.2/setup.py
-drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-09 22:02:38.262798 katottglib-0.2.2/test/
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1878 2023-06-09 20:22:51.000000 katottglib-0.2.2/test/__init__.py
+drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-09 22:25:49.519563 katottglib-0.2.3/
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1073 2023-06-06 21:02:05.000000 katottglib-0.2.3/LICENSE
+-rw-r--r--   0 dsenchishen   (502) staff       (20)       30 2023-07-09 19:43:57.000000 katottglib-0.2.3/MANIFEST.in
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1379 2023-07-09 22:25:49.519805 katottglib-0.2.3/PKG-INFO
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      808 2023-07-09 22:25:33.000000 katottglib-0.2.3/README.rst
+drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-09 22:25:49.516991 katottglib-0.2.3/katottglib/
+-rw-r--r--   0 dsenchishen   (502) staff       (20)       59 2023-07-09 22:22:03.000000 katottglib-0.2.3/katottglib/__init__.py
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     3612 2023-07-09 22:19:51.000000 katottglib-0.2.3/katottglib/katottg.py
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1845 2023-07-09 22:18:42.000000 katottglib-0.2.3/katottglib/test.py
+drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-09 22:25:49.519194 katottglib-0.2.3/katottglib.egg-info/
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1379 2023-07-09 22:25:49.000000 katottglib-0.2.3/katottglib.egg-info/PKG-INFO
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      264 2023-07-09 22:25:49.000000 katottglib-0.2.3/katottglib.egg-info/SOURCES.txt
+-rw-r--r--   0 dsenchishen   (502) staff       (20)        1 2023-07-09 22:25:49.000000 katottglib-0.2.3/katottglib.egg-info/dependency_links.txt
+-rw-r--r--   0 dsenchishen   (502) staff       (20)       11 2023-07-09 22:25:49.000000 katottglib-0.2.3/katottglib.egg-info/top_level.txt
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      406 2023-06-06 21:02:05.000000 katottglib-0.2.3/pyproject.toml
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      639 2023-07-09 22:25:49.520571 katottglib-0.2.3/setup.cfg
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      375 2023-07-09 22:25:33.000000 katottglib-0.2.3/setup.py
```

### Comparing `katottglib-0.2.2/LICENSE` & `katottglib-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `katottglib-0.2.2/PKG-INFO` & `katottglib-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katottglib
-Version: 0.2.2
+Version: 0.2.3
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
 
+v0.2.3 (2023-07-10)
+...................
+
+Fix installation by refining the structure
+
 v0.2.2 (2023-07-10)
 ...................
 
 Updated setup.py config
 
 
 v0.2.1 (2023-07-09)
```

### Comparing `katottglib-0.2.2/README.rst` & `katottglib-0.2.3/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 - Install with `pip install katottglib`
 - Import `import katottglib`
 - Search for entities with `find_by_name` `katottglib.find_by_name(name="Lviv")`
 
 Release notes
 -------------
 
+v0.2.3 (2023-07-10)
+...................
+
+Fix installation by refining the structure
+
 v0.2.2 (2023-07-10)
 ...................
 
 Updated setup.py config
 
 
 v0.2.1 (2023-07-09)
```

### Comparing `katottglib-0.2.2/katottglib.egg-info/PKG-INFO` & `katottglib-0.2.3/katottglib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katottglib
-Version: 0.2.2
+Version: 0.2.3
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
 
+v0.2.3 (2023-07-10)
+...................
+
+Fix installation by refining the structure
+
 v0.2.2 (2023-07-10)
 ...................
 
 Updated setup.py config
 
 
 v0.2.1 (2023-07-09)
```

### Comparing `katottglib-0.2.2/setup.cfg` & `katottglib-0.2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = katottglib
-version = 0.2.2
+version = 0.2.3
 description = A Python lib to operate KATOTTG addresses (classified administrative division of Ukraine).
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/sen-den/katottglib
 author = Denis Senchishen
 author_email = dsenchishen@icloud.com
 license = MIT
```

