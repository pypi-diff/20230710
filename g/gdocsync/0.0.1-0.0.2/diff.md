# Comparing `tmp/gdocsync-0.0.1.tar.gz` & `tmp/gdocsync-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdocsync-0.0.1.tar", last modified: Mon Jul 10 05:23:18 2023, max compression
+gzip compressed data, was "gdocsync-0.0.2.tar", last modified: Mon Jul 10 05:25:21 2023, max compression
```

## Comparing `gdocsync-0.0.1.tar` & `gdocsync-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-10 05:23:18.971127 gdocsync-0.0.1/
--rw-r--r--   0 peterdemin   (503) staff       (20)     1050 2023-07-10 04:49:41.000000 gdocsync-0.0.1/LICENSE
--rw-r--r--   0 peterdemin   (503) staff       (20)     1184 2023-07-10 05:23:18.971187 gdocsync-0.0.1/PKG-INFO
--rw-r--r--   0 peterdemin   (503) staff       (20)      739 2023-07-10 04:49:41.000000 gdocsync-0.0.1/README.rst
--rw-r--r--   0 peterdemin   (503) staff       (20)    21045 2023-07-10 04:49:41.000000 gdocsync-0.0.1/pyproject.toml
--rw-r--r--   0 peterdemin   (503) staff       (20)      654 2023-07-10 05:23:18.971447 gdocsync-0.0.1/setup.cfg
-drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-10 05:23:18.968010 gdocsync-0.0.1/src/
-drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-10 05:23:18.970394 gdocsync-0.0.1/src/gdocsync/
--rw-r--r--   0 peterdemin   (503) staff       (20)        0 2023-07-10 04:55:01.000000 gdocsync-0.0.1/src/gdocsync/__init__.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      327 2023-07-10 05:21:38.000000 gdocsync-0.0.1/src/gdocsync/cli.py
--rw-r--r--   0 peterdemin   (503) staff       (20)       69 2023-07-10 05:17:11.000000 gdocsync-0.0.1/src/gdocsync/constants.py
--rw-r--r--   0 peterdemin   (503) staff       (20)     2575 2023-07-10 05:12:07.000000 gdocsync-0.0.1/src/gdocsync/google_drive_client.py
--rw-r--r--   0 peterdemin   (503) staff       (20)     1311 2023-07-10 05:19:49.000000 gdocsync-0.0.1/src/gdocsync/johnny_decimal.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      549 2023-07-10 05:03:46.000000 gdocsync-0.0.1/src/gdocsync/pandoc_client.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      151 2023-07-10 05:01:50.000000 gdocsync-0.0.1/src/gdocsync/regexes.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      823 2023-07-10 05:09:34.000000 gdocsync-0.0.1/src/gdocsync/shelve_cache.py
--rw-r--r--   0 peterdemin   (503) staff       (20)     1115 2023-07-10 05:20:36.000000 gdocsync-0.0.1/src/gdocsync/sync.py
--rw-r--r--   0 peterdemin   (503) staff       (20)      517 2023-07-10 05:02:15.000000 gdocsync-0.0.1/src/gdocsync/test_regexes.py
-drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-10 05:23:18.971029 gdocsync-0.0.1/src/gdocsync.egg-info/
--rw-r--r--   0 peterdemin   (503) staff       (20)     1184 2023-07-10 05:23:18.000000 gdocsync-0.0.1/src/gdocsync.egg-info/PKG-INFO
--rw-r--r--   0 peterdemin   (503) staff       (20)      497 2023-07-10 05:23:18.000000 gdocsync-0.0.1/src/gdocsync.egg-info/SOURCES.txt
--rw-r--r--   0 peterdemin   (503) staff       (20)        1 2023-07-10 05:23:18.000000 gdocsync-0.0.1/src/gdocsync.egg-info/dependency_links.txt
--rw-r--r--   0 peterdemin   (503) staff       (20)       46 2023-07-10 05:23:18.000000 gdocsync-0.0.1/src/gdocsync.egg-info/entry_points.txt
--rw-r--r--   0 peterdemin   (503) staff       (20)        9 2023-07-10 05:23:18.000000 gdocsync-0.0.1/src/gdocsync.egg-info/top_level.txt
+drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-10 05:25:21.517006 gdocsync-0.0.2/
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1050 2023-07-10 04:49:41.000000 gdocsync-0.0.2/LICENSE
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1184 2023-07-10 05:25:21.517095 gdocsync-0.0.2/PKG-INFO
+-rw-r--r--   0 peterdemin   (503) staff       (20)      739 2023-07-10 04:49:41.000000 gdocsync-0.0.2/README.rst
+-rw-r--r--   0 peterdemin   (503) staff       (20)    21045 2023-07-10 04:49:41.000000 gdocsync-0.0.2/pyproject.toml
+-rw-r--r--   0 peterdemin   (503) staff       (20)      751 2023-07-10 05:25:21.517434 gdocsync-0.0.2/setup.cfg
+drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-10 05:25:21.512878 gdocsync-0.0.2/src/
+drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-10 05:25:21.515897 gdocsync-0.0.2/src/gdocsync/
+-rw-r--r--   0 peterdemin   (503) staff       (20)        0 2023-07-10 04:55:01.000000 gdocsync-0.0.2/src/gdocsync/__init__.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      327 2023-07-10 05:21:38.000000 gdocsync-0.0.2/src/gdocsync/cli.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)       69 2023-07-10 05:17:11.000000 gdocsync-0.0.2/src/gdocsync/constants.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)     2575 2023-07-10 05:12:07.000000 gdocsync-0.0.2/src/gdocsync/google_drive_client.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1311 2023-07-10 05:19:49.000000 gdocsync-0.0.2/src/gdocsync/johnny_decimal.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      549 2023-07-10 05:03:46.000000 gdocsync-0.0.2/src/gdocsync/pandoc_client.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      151 2023-07-10 05:01:50.000000 gdocsync-0.0.2/src/gdocsync/regexes.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      823 2023-07-10 05:09:34.000000 gdocsync-0.0.2/src/gdocsync/shelve_cache.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1115 2023-07-10 05:20:36.000000 gdocsync-0.0.2/src/gdocsync/sync.py
+-rw-r--r--   0 peterdemin   (503) staff       (20)      517 2023-07-10 05:02:15.000000 gdocsync-0.0.2/src/gdocsync/test_regexes.py
+drwxr-xr-x   0 peterdemin   (503) staff       (20)        0 2023-07-10 05:25:21.516890 gdocsync-0.0.2/src/gdocsync.egg-info/
+-rw-r--r--   0 peterdemin   (503) staff       (20)     1184 2023-07-10 05:25:21.000000 gdocsync-0.0.2/src/gdocsync.egg-info/PKG-INFO
+-rw-r--r--   0 peterdemin   (503) staff       (20)      532 2023-07-10 05:25:21.000000 gdocsync-0.0.2/src/gdocsync.egg-info/SOURCES.txt
+-rw-r--r--   0 peterdemin   (503) staff       (20)        1 2023-07-10 05:25:21.000000 gdocsync-0.0.2/src/gdocsync.egg-info/dependency_links.txt
+-rw-r--r--   0 peterdemin   (503) staff       (20)       46 2023-07-10 05:25:21.000000 gdocsync-0.0.2/src/gdocsync.egg-info/entry_points.txt
+-rw-r--r--   0 peterdemin   (503) staff       (20)       73 2023-07-10 05:25:21.000000 gdocsync-0.0.2/src/gdocsync.egg-info/requires.txt
+-rw-r--r--   0 peterdemin   (503) staff       (20)        9 2023-07-10 05:25:21.000000 gdocsync-0.0.2/src/gdocsync.egg-info/top_level.txt
```

### Comparing `gdocsync-0.0.1/LICENSE` & `gdocsync-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.1/PKG-INFO` & `gdocsync-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdocsync
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://github.com/peterdemin/gdocsync
 Author: Peter Demin
 Author-email: peterdemin@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gdocsync-0.0.1/README.rst` & `gdocsync-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.1/pyproject.toml` & `gdocsync-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.1/src/gdocsync/google_drive_client.py` & `gdocsync-0.0.2/src/gdocsync/google_drive_client.py`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.1/src/gdocsync/johnny_decimal.py` & `gdocsync-0.0.2/src/gdocsync/johnny_decimal.py`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.1/src/gdocsync/pandoc_client.py` & `gdocsync-0.0.2/src/gdocsync/pandoc_client.py`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.1/src/gdocsync/shelve_cache.py` & `gdocsync-0.0.2/src/gdocsync/shelve_cache.py`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.1/src/gdocsync/sync.py` & `gdocsync-0.0.2/src/gdocsync/sync.py`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.1/src/gdocsync/test_regexes.py` & `gdocsync-0.0.2/src/gdocsync/test_regexes.py`

 * *Files identical despite different names*

### Comparing `gdocsync-0.0.1/src/gdocsync.egg-info/PKG-INFO` & `gdocsync-0.0.2/src/gdocsync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdocsync
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://github.com/peterdemin/gdocsync
 Author: Peter Demin
 Author-email: peterdemin@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

