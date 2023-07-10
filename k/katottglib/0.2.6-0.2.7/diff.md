# Comparing `tmp/katottglib-0.2.6.tar.gz` & `tmp/katottglib-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katottglib-0.2.6.tar", last modified: Mon Jul 10 08:27:17 2023, max compression
+gzip compressed data, was "katottglib-0.2.7.tar", last modified: Mon Jul 10 13:33:15 2023, max compression
```

## Comparing `katottglib-0.2.6.tar` & `katottglib-0.2.7.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-10 08:27:17.103701 katottglib-0.2.6/
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1073 2023-06-06 21:02:05.000000 katottglib-0.2.6/LICENSE
--rw-r--r--   0 dsenchishen   (502) staff       (20)       36 2023-07-10 08:27:10.000000 katottglib-0.2.6/MANIFEST.in
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1661 2023-07-10 08:27:17.103900 katottglib-0.2.6/PKG-INFO
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1090 2023-07-10 08:27:10.000000 katottglib-0.2.6/README.rst
-drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-10 08:27:17.100355 katottglib-0.2.6/katottglib/
--rw-r--r--   0 dsenchishen   (502) staff       (20)       59 2023-07-09 22:22:03.000000 katottglib-0.2.6/katottglib/__init__.py
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1534 2023-07-01 12:09:31.000000 katottglib-0.2.6/katottglib/data.py
--rw-r--r--   0 dsenchishen   (502) staff       (20)      586 2023-06-06 21:02:05.000000 katottglib-0.2.6/katottglib/entity.py
--rw-r--r--   0 dsenchishen   (502) staff       (20)     3627 2023-07-10 08:23:06.000000 katottglib-0.2.6/katottglib/katottg.py
--rw-r--r--   0 dsenchishen   (502) staff       (20)  1476983 2023-06-04 05:40:38.000000 katottglib-0.2.6/katottglib/kodifikator.xlsx
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1845 2023-07-09 22:18:42.000000 katottglib-0.2.6/katottglib/test.py
-drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-10 08:27:17.103325 katottglib-0.2.6/katottglib.egg-info/
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1661 2023-07-10 08:27:17.000000 katottglib-0.2.6/katottglib.egg-info/PKG-INFO
--rw-r--r--   0 dsenchishen   (502) staff       (20)      365 2023-07-10 08:27:17.000000 katottglib-0.2.6/katottglib.egg-info/SOURCES.txt
--rw-r--r--   0 dsenchishen   (502) staff       (20)        1 2023-07-10 08:27:17.000000 katottglib-0.2.6/katottglib.egg-info/dependency_links.txt
--rw-r--r--   0 dsenchishen   (502) staff       (20)       30 2023-07-10 08:27:17.000000 katottglib-0.2.6/katottglib.egg-info/requires.txt
--rw-r--r--   0 dsenchishen   (502) staff       (20)       11 2023-07-10 08:27:17.000000 katottglib-0.2.6/katottglib.egg-info/top_level.txt
--rw-r--r--   0 dsenchishen   (502) staff       (20)      406 2023-06-06 21:02:05.000000 katottglib-0.2.6/pyproject.toml
--rw-r--r--   0 dsenchishen   (502) staff       (20)      639 2023-07-10 08:27:17.104821 katottglib-0.2.6/setup.cfg
--rw-r--r--   0 dsenchishen   (502) staff       (20)      427 2023-07-10 08:27:10.000000 katottglib-0.2.6/setup.py
+drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-10 13:33:15.721980 katottglib-0.2.7/
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1073 2023-06-06 21:02:05.000000 katottglib-0.2.7/LICENSE
+-rw-r--r--   0 dsenchishen   (502) staff       (20)       36 2023-07-10 08:27:10.000000 katottglib-0.2.7/MANIFEST.in
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1820 2023-07-10 13:33:15.722468 katottglib-0.2.7/PKG-INFO
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1249 2023-07-10 13:32:17.000000 katottglib-0.2.7/README.rst
+drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-10 13:33:15.716319 katottglib-0.2.7/katottglib/
+-rw-r--r--   0 dsenchishen   (502) staff       (20)       59 2023-07-09 22:22:03.000000 katottglib-0.2.7/katottglib/__init__.py
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1534 2023-07-01 12:09:31.000000 katottglib-0.2.7/katottglib/data.py
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      586 2023-06-06 21:02:05.000000 katottglib-0.2.7/katottglib/entity.py
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     3627 2023-07-10 08:23:06.000000 katottglib-0.2.7/katottglib/katottg.py
+-rw-r--r--   0 dsenchishen   (502) staff       (20)  1476983 2023-06-04 05:40:38.000000 katottglib-0.2.7/katottglib/kodifikator.xlsx
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1845 2023-07-09 22:18:42.000000 katottglib-0.2.7/katottglib/test.py
+drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-10 13:33:15.720795 katottglib-0.2.7/katottglib.egg-info/
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1820 2023-07-10 13:33:15.000000 katottglib-0.2.7/katottglib.egg-info/PKG-INFO
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      332 2023-07-10 13:33:15.000000 katottglib-0.2.7/katottglib.egg-info/SOURCES.txt
+-rw-r--r--   0 dsenchishen   (502) staff       (20)        1 2023-07-10 13:33:15.000000 katottglib-0.2.7/katottglib.egg-info/dependency_links.txt
+-rw-r--r--   0 dsenchishen   (502) staff       (20)       11 2023-07-10 13:33:15.000000 katottglib-0.2.7/katottglib.egg-info/top_level.txt
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      406 2023-06-06 21:02:05.000000 katottglib-0.2.7/pyproject.toml
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      639 2023-07-10 13:33:15.724363 katottglib-0.2.7/setup.cfg
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      431 2023-07-10 13:32:16.000000 katottglib-0.2.7/setup.py
```

### Comparing `katottglib-0.2.6/LICENSE` & `katottglib-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `katottglib-0.2.6/PKG-INFO` & `katottglib-0.2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katottglib
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Python lib to operate KATOTTG addresses (classified administrative division of Ukraine).
 Home-page: https://github.com/sen-den/katottglib
 Author: Denis Senchishen
 Author-email: dsenchishen@icloud.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,21 +17,27 @@
 ===========
 KATOTTG lib
 ===========
 
 Quick start
 -----------
 
-- Install with `pip install katottglib`
-- Import `import katottglib`
-- Search for entities with `find_by_name` `katottglib.find_by_name(name="Lviv")`
+- Install pandas ``pip install pandas`` (temporary not pinned)
+- Install with ``pip install katottglib``
+- Import ``import katottglib``
+- Search for entities with ``find_by_name`` ``katottglib.find_by_name(name="Lviv")``
 
 Release notes
 -------------
 
+v0.2.7 (2023-07-10)
+...................
+
+Temporary unpin pandas and openpyxl versions.
+
 v0.2.6 (2023-07-10)
 ...................
 
 Try to fix continuation import errors on some installations.
 
 v0.2.5 (2023-07-10)
 ...................
```

### Comparing `katottglib-0.2.6/README.rst` & `katottglib-0.2.7/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 ===========
 KATOTTG lib
 ===========
 
 Quick start
 -----------
 
-- Install with `pip install katottglib`
-- Import `import katottglib`
-- Search for entities with `find_by_name` `katottglib.find_by_name(name="Lviv")`
+- Install pandas ``pip install pandas`` (temporary not pinned)
+- Install with ``pip install katottglib``
+- Import ``import katottglib``
+- Search for entities with ``find_by_name`` ``katottglib.find_by_name(name="Lviv")``
 
 Release notes
 -------------
 
+v0.2.7 (2023-07-10)
+...................
+
+Temporary unpin pandas and openpyxl versions.
+
 v0.2.6 (2023-07-10)
 ...................
 
 Try to fix continuation import errors on some installations.
 
 v0.2.5 (2023-07-10)
 ...................
```

### Comparing `katottglib-0.2.6/katottglib/data.py` & `katottglib-0.2.7/katottglib/data.py`

 * *Files identical despite different names*

### Comparing `katottglib-0.2.6/katottglib/entity.py` & `katottglib-0.2.7/katottglib/entity.py`

 * *Files identical despite different names*

### Comparing `katottglib-0.2.6/katottglib/katottg.py` & `katottglib-0.2.7/katottglib/katottg.py`

 * *Files identical despite different names*

### Comparing `katottglib-0.2.6/katottglib/kodifikator.xlsx` & `katottglib-0.2.7/katottglib/kodifikator.xlsx`

 * *Files identical despite different names*

### Comparing `katottglib-0.2.6/katottglib/test.py` & `katottglib-0.2.7/katottglib/test.py`

 * *Files identical despite different names*

### Comparing `katottglib-0.2.6/katottglib.egg-info/PKG-INFO` & `katottglib-0.2.7/katottglib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katottglib
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Python lib to operate KATOTTG addresses (classified administrative division of Ukraine).
 Home-page: https://github.com/sen-den/katottglib
 Author: Denis Senchishen
 Author-email: dsenchishen@icloud.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,21 +17,27 @@
 ===========
 KATOTTG lib
 ===========
 
 Quick start
 -----------
 
-- Install with `pip install katottglib`
-- Import `import katottglib`
-- Search for entities with `find_by_name` `katottglib.find_by_name(name="Lviv")`
+- Install pandas ``pip install pandas`` (temporary not pinned)
+- Install with ``pip install katottglib``
+- Import ``import katottglib``
+- Search for entities with ``find_by_name`` ``katottglib.find_by_name(name="Lviv")``
 
 Release notes
 -------------
 
+v0.2.7 (2023-07-10)
+...................
+
+Temporary unpin pandas and openpyxl versions.
+
 v0.2.6 (2023-07-10)
 ...................
 
 Try to fix continuation import errors on some installations.
 
 v0.2.5 (2023-07-10)
 ...................
```

### Comparing `katottglib-0.2.6/setup.cfg` & `katottglib-0.2.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = katottglib
-version = 0.2.6
+version = 0.2.7
 description = A Python lib to operate KATOTTG addresses (classified administrative division of Ukraine).
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/sen-den/katottglib
 author = Denis Senchishen
 author_email = dsenchishen@icloud.com
 license = MIT
```

