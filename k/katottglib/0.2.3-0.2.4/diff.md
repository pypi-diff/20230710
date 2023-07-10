# Comparing `tmp/katottglib-0.2.3.tar.gz` & `tmp/katottglib-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katottglib-0.2.3.tar", last modified: Sun Jul  9 22:25:49 2023, max compression
+gzip compressed data, was "katottglib-0.2.4.tar", last modified: Sun Jul  9 22:29:02 2023, max compression
```

## Comparing `katottglib-0.2.3.tar` & `katottglib-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-09 22:25:49.519563 katottglib-0.2.3/
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1073 2023-06-06 21:02:05.000000 katottglib-0.2.3/LICENSE
--rw-r--r--   0 dsenchishen   (502) staff       (20)       30 2023-07-09 19:43:57.000000 katottglib-0.2.3/MANIFEST.in
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1379 2023-07-09 22:25:49.519805 katottglib-0.2.3/PKG-INFO
--rw-r--r--   0 dsenchishen   (502) staff       (20)      808 2023-07-09 22:25:33.000000 katottglib-0.2.3/README.rst
-drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-09 22:25:49.516991 katottglib-0.2.3/katottglib/
--rw-r--r--   0 dsenchishen   (502) staff       (20)       59 2023-07-09 22:22:03.000000 katottglib-0.2.3/katottglib/__init__.py
--rw-r--r--   0 dsenchishen   (502) staff       (20)     3612 2023-07-09 22:19:51.000000 katottglib-0.2.3/katottglib/katottg.py
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1845 2023-07-09 22:18:42.000000 katottglib-0.2.3/katottglib/test.py
-drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-09 22:25:49.519194 katottglib-0.2.3/katottglib.egg-info/
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1379 2023-07-09 22:25:49.000000 katottglib-0.2.3/katottglib.egg-info/PKG-INFO
--rw-r--r--   0 dsenchishen   (502) staff       (20)      264 2023-07-09 22:25:49.000000 katottglib-0.2.3/katottglib.egg-info/SOURCES.txt
--rw-r--r--   0 dsenchishen   (502) staff       (20)        1 2023-07-09 22:25:49.000000 katottglib-0.2.3/katottglib.egg-info/dependency_links.txt
--rw-r--r--   0 dsenchishen   (502) staff       (20)       11 2023-07-09 22:25:49.000000 katottglib-0.2.3/katottglib.egg-info/top_level.txt
--rw-r--r--   0 dsenchishen   (502) staff       (20)      406 2023-06-06 21:02:05.000000 katottglib-0.2.3/pyproject.toml
--rw-r--r--   0 dsenchishen   (502) staff       (20)      639 2023-07-09 22:25:49.520571 katottglib-0.2.3/setup.cfg
--rw-r--r--   0 dsenchishen   (502) staff       (20)      375 2023-07-09 22:25:33.000000 katottglib-0.2.3/setup.py
+drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-09 22:29:02.596779 katottglib-0.2.4/
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1073 2023-06-06 21:02:05.000000 katottglib-0.2.4/LICENSE
+-rw-r--r--   0 dsenchishen   (502) staff       (20)       30 2023-07-09 19:43:57.000000 katottglib-0.2.4/MANIFEST.in
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1475 2023-07-09 22:29:02.597027 katottglib-0.2.4/PKG-INFO
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      904 2023-07-09 22:29:00.000000 katottglib-0.2.4/README.rst
+drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-09 22:29:02.593742 katottglib-0.2.4/katottglib/
+-rw-r--r--   0 dsenchishen   (502) staff       (20)       59 2023-07-09 22:22:03.000000 katottglib-0.2.4/katottglib/__init__.py
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     3612 2023-07-09 22:19:51.000000 katottglib-0.2.4/katottglib/katottg.py
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1845 2023-07-09 22:18:42.000000 katottglib-0.2.4/katottglib/test.py
+drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-09 22:29:02.596423 katottglib-0.2.4/katottglib.egg-info/
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1475 2023-07-09 22:29:02.000000 katottglib-0.2.4/katottglib.egg-info/PKG-INFO
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      297 2023-07-09 22:29:02.000000 katottglib-0.2.4/katottglib.egg-info/SOURCES.txt
+-rw-r--r--   0 dsenchishen   (502) staff       (20)        1 2023-07-09 22:29:02.000000 katottglib-0.2.4/katottglib.egg-info/dependency_links.txt
+-rw-r--r--   0 dsenchishen   (502) staff       (20)       30 2023-07-09 22:29:02.000000 katottglib-0.2.4/katottglib.egg-info/requires.txt
+-rw-r--r--   0 dsenchishen   (502) staff       (20)       11 2023-07-09 22:29:02.000000 katottglib-0.2.4/katottglib.egg-info/top_level.txt
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      406 2023-06-06 21:02:05.000000 katottglib-0.2.4/pyproject.toml
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      639 2023-07-09 22:29:02.597486 katottglib-0.2.4/setup.cfg
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      427 2023-07-09 22:29:00.000000 katottglib-0.2.4/setup.py
```

### Comparing `katottglib-0.2.3/LICENSE` & `katottglib-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `katottglib-0.2.3/PKG-INFO` & `katottglib-0.2.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katottglib
-Version: 0.2.3
+Version: 0.2.4
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
 
+v0.2.4 (2023-07-10)
+...................
+
+Fix installation by adding setup.py install_requires
+
+
 v0.2.3 (2023-07-10)
 ...................
 
 Fix installation by refining the structure
 
 v0.2.2 (2023-07-10)
 ...................
```

### Comparing `katottglib-0.2.3/README.rst` & `katottglib-0.2.4/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 - Install with `pip install katottglib`
 - Import `import katottglib`
 - Search for entities with `find_by_name` `katottglib.find_by_name(name="Lviv")`
 
 Release notes
 -------------
 
+v0.2.4 (2023-07-10)
+...................
+
+Fix installation by adding setup.py install_requires
+
+
 v0.2.3 (2023-07-10)
 ...................
 
 Fix installation by refining the structure
 
 v0.2.2 (2023-07-10)
 ...................
```

### Comparing `katottglib-0.2.3/katottglib/katottg.py` & `katottglib-0.2.4/katottglib/katottg.py`

 * *Files identical despite different names*

### Comparing `katottglib-0.2.3/katottglib/test.py` & `katottglib-0.2.4/katottglib/test.py`

 * *Files identical despite different names*

### Comparing `katottglib-0.2.3/katottglib.egg-info/PKG-INFO` & `katottglib-0.2.4/katottglib.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katottglib
-Version: 0.2.3
+Version: 0.2.4
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
 
+v0.2.4 (2023-07-10)
+...................
+
+Fix installation by adding setup.py install_requires
+
+
 v0.2.3 (2023-07-10)
 ...................
 
 Fix installation by refining the structure
 
 v0.2.2 (2023-07-10)
 ...................
```

### Comparing `katottglib-0.2.3/setup.cfg` & `katottglib-0.2.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = katottglib
-version = 0.2.3
+version = 0.2.4
 description = A Python lib to operate KATOTTG addresses (classified administrative division of Ukraine).
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/sen-den/katottglib
 author = Denis Senchishen
 author_email = dsenchishen@icloud.com
 license = MIT
```

