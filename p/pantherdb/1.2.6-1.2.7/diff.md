# Comparing `tmp/pantherdb-1.2.6.tar.gz` & `tmp/pantherdb-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pantherdb-1.2.6.tar", last modified: Fri Jul  7 10:19:02 2023, max compression
+gzip compressed data, was "pantherdb-1.2.7.tar", last modified: Mon Jul 10 10:21:30 2023, max compression
```

## Comparing `pantherdb-1.2.6.tar` & `pantherdb-1.2.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:19:02.541128 pantherdb-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-07 10:19:02.541128 pantherdb-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-07 10:18:46.000000 pantherdb-1.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:19:02.541128 pantherdb-1.2.6/pantherdb/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-07 10:18:46.000000 pantherdb-1.2.6/pantherdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11153 2023-07-07 10:18:46.000000 pantherdb-1.2.6/pantherdb/pantherdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:19:02.541128 pantherdb-1.2.6/pantherdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-07 10:19:02.000000 pantherdb-1.2.6/pantherdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-07 10:19:02.000000 pantherdb-1.2.6/pantherdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:19:02.000000 pantherdb-1.2.6/pantherdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-07 10:19:02.000000 pantherdb-1.2.6/pantherdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 10:19:02.000000 pantherdb-1.2.6/pantherdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 10:19:02.541128 pantherdb-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-07 10:18:46.000000 pantherdb-1.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:19:02.541128 pantherdb-1.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    16870 2023-07-07 10:18:46.000000 pantherdb-1.2.6/tests/test_normal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:21:30.657537 pantherdb-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-10 10:21:30.657537 pantherdb-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-10 10:21:16.000000 pantherdb-1.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:21:30.653537 pantherdb-1.2.7/pantherdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-10 10:21:16.000000 pantherdb-1.2.7/pantherdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11153 2023-07-10 10:21:16.000000 pantherdb-1.2.7/pantherdb/pantherdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:21:30.657537 pantherdb-1.2.7/pantherdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-10 10:21:30.000000 pantherdb-1.2.7/pantherdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-10 10:21:30.000000 pantherdb-1.2.7/pantherdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:21:30.000000 pantherdb-1.2.7/pantherdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 10:21:30.000000 pantherdb-1.2.7/pantherdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 10:21:30.000000 pantherdb-1.2.7/pantherdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 10:21:30.657537 pantherdb-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-10 10:21:16.000000 pantherdb-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:21:30.657537 pantherdb-1.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    16870 2023-07-10 10:21:16.000000 pantherdb-1.2.7/tests/test_normal.py
```

### Comparing `pantherdb-1.2.6/PKG-INFO` & `pantherdb-1.2.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: pantherdb
-Version: 1.2.6
-Summary: is a Simple, FileBase and Document Oriented database
-Home-page: https://github.com/alirn76/pantherdb
-Author: Ali RajabNezhad
-Author-email: alirn76@yahoo.com
-License: MIT
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 ## Introduction
 
 PantherDB is a <b>Simple</b>, <b>FileBase</b> and <b>Document Oriented</b> database that you can use in your projects.
 
 ### Features:
 - Document Oriented
 - Easy to use
```

### Comparing `pantherdb-1.2.6/README.md` & `pantherdb-1.2.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: pantherdb
+Version: 1.2.7
+Summary: is a Simple, FileBase and Document Oriented database
+Home-page: https://github.com/alirn76/pantherdb
+Author: Ali RajabNezhad
+Author-email: alirn76@yahoo.com
+License: MIT
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 ## Introduction
 
 PantherDB is a <b>Simple</b>, <b>FileBase</b> and <b>Document Oriented</b> database that you can use in your projects.
 
 ### Features:
 - Document Oriented
 - Easy to use
```

### Comparing `pantherdb-1.2.6/pantherdb/pantherdb.py` & `pantherdb-1.2.7/pantherdb/pantherdb.py`

 * *Files identical despite different names*

### Comparing `pantherdb-1.2.6/pantherdb.egg-info/PKG-INFO` & `pantherdb-1.2.7/pantherdb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pantherdb
-Version: 1.2.6
+Version: 1.2.7
 Summary: is a Simple, FileBase and Document Oriented database
 Home-page: https://github.com/alirn76/pantherdb
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Introduction
 
 PantherDB is a <b>Simple</b>, <b>FileBase</b> and <b>Document Oriented</b> database that you can use in your projects.
```

### Comparing `pantherdb-1.2.6/setup.py` & `pantherdb-1.2.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,13 +27,14 @@
     classifiers=[
         'Operating System :: OS Independent',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
     install_requires=[
-        'orjson~=3.9',
+        'orjson~=3.9.2',
         'cryptography~=39.0',
     ],
 )
```

### Comparing `pantherdb-1.2.6/tests/test_normal.py` & `pantherdb-1.2.7/tests/test_normal.py`

 * *Files identical despite different names*

