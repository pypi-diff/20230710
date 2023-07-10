# Comparing `tmp/Perfole-0.0.2.tar.gz` & `tmp/Perfole-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Perfole-0.0.2.tar", last modified: Mon Jul 10 12:01:57 2023, max compression
+gzip compressed data, was "Perfole-0.0.3.tar", last modified: Mon Jul 10 12:43:42 2023, max compression
```

## Comparing `Perfole-0.0.2.tar` & `Perfole-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-10 12:01:57.797309 Perfole-0.0.2/
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1374 2023-07-10 12:01:57.797170 Perfole-0.0.2/PKG-INFO
-drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-10 12:01:57.796251 Perfole-0.0.2/Perfole/
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)    12927 2023-07-10 11:40:47.000000 Perfole-0.0.2/Perfole/Perfole.py
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-07 16:50:05.000000 Perfole-0.0.2/Perfole/__init__.py
-drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-10 12:01:57.796977 Perfole-0.0.2/Perfole.egg-info/
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1374 2023-07-10 12:01:57.000000 Perfole-0.0.2/Perfole.egg-info/PKG-INFO
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)      223 2023-07-10 12:01:57.000000 Perfole-0.0.2/Perfole.egg-info/SOURCES.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        1 2023-07-10 12:01:57.000000 Perfole-0.0.2/Perfole.egg-info/dependency_links.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        9 2023-07-10 12:01:57.000000 Perfole-0.0.2/Perfole.egg-info/requires.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        8 2023-07-10 12:01:57.000000 Perfole-0.0.2/Perfole.egg-info/top_level.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1183 2023-07-10 11:07:54.000000 Perfole-0.0.2/README.md
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     4528 2023-07-10 08:04:58.000000 Perfole-0.0.2/license.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)       38 2023-07-10 12:01:57.797355 Perfole-0.0.2/setup.cfg
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)      469 2023-07-10 11:30:25.000000 Perfole-0.0.2/setup.py
+drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-10 12:43:42.263121 Perfole-0.0.3/
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1374 2023-07-10 12:43:42.262989 Perfole-0.0.3/PKG-INFO
+drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-10 12:43:42.261525 Perfole-0.0.3/Perfole/
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)    12927 2023-07-10 11:40:47.000000 Perfole-0.0.3/Perfole/Perfole.py
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-07 16:50:05.000000 Perfole-0.0.3/Perfole/__init__.py
+drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-10 12:43:42.262432 Perfole-0.0.3/Perfole.egg-info/
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1374 2023-07-10 12:43:42.000000 Perfole-0.0.3/Perfole.egg-info/PKG-INFO
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)      223 2023-07-10 12:43:42.000000 Perfole-0.0.3/Perfole.egg-info/SOURCES.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        1 2023-07-10 12:43:42.000000 Perfole-0.0.3/Perfole.egg-info/dependency_links.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        9 2023-07-10 12:43:42.000000 Perfole-0.0.3/Perfole.egg-info/requires.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        8 2023-07-10 12:43:42.000000 Perfole-0.0.3/Perfole.egg-info/top_level.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1183 2023-07-10 11:07:54.000000 Perfole-0.0.3/README.md
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     4528 2023-07-10 08:04:58.000000 Perfole-0.0.3/license.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)       38 2023-07-10 12:43:42.263184 Perfole-0.0.3/setup.cfg
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)      501 2023-07-10 12:43:16.000000 Perfole-0.0.3/setup.py
```

### Comparing `Perfole-0.0.2/PKG-INFO` & `Perfole-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Perfole
-Version: 0.0.2
+Version: 0.0.3
 Summary: Measure performance
 Author: breeze-testing
 License: license.txt
 Description-Content-Type: text/markdown
 License-File: license.txt
```

### Comparing `Perfole-0.0.2/Perfole/Perfole.py` & `Perfole-0.0.3/Perfole/Perfole.py`

 * *Files identical despite different names*

### Comparing `Perfole-0.0.2/Perfole.egg-info/PKG-INFO` & `Perfole-0.0.3/Perfole.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Perfole
-Version: 0.0.2
+Version: 0.0.3
 Summary: Measure performance
 Author: breeze-testing
 License: license.txt
 Description-Content-Type: text/markdown
 License-File: license.txt
```

### Comparing `Perfole-0.0.2/README.md` & `Perfole-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `Perfole-0.0.2/license.txt` & `Perfole-0.0.3/license.txt`

 * *Files identical despite different names*

