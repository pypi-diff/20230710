# Comparing `tmp/docs2txt-0.1.5.tar.gz` & `tmp/docs2txt-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docs2txt-0.1.5.tar", last modified: Sun Jul  9 23:11:11 2023, max compression
+gzip compressed data, was "docs2txt-0.1.6.tar", last modified: Sun Jul  9 23:15:13 2023, max compression
```

## Comparing `docs2txt-0.1.5.tar` & `docs2txt-0.1.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 23:11:11.852726 docs2txt-0.1.5/
--rw-r--r--   0 er         (501) staff       (20)      155 2023-07-09 22:35:52.000000 docs2txt-0.1.5/AUTHORS.rst
--rw-r--r--   0 er         (501) staff       (20)     3543 2023-07-09 22:35:52.000000 docs2txt-0.1.5/CONTRIBUTING.rst
--rw-r--r--   0 er         (501) staff       (20)       89 2023-07-09 22:35:52.000000 docs2txt-0.1.5/HISTORY.rst
--rw-r--r--   0 er         (501) staff       (20)     1064 2023-07-09 22:35:54.000000 docs2txt-0.1.5/LICENSE
--rw-r--r--   0 er         (501) staff       (20)      262 2023-07-09 22:35:52.000000 docs2txt-0.1.5/MANIFEST.in
--rw-r--r--   0 er         (501) staff       (20)     2283 2023-07-09 23:11:11.852895 docs2txt-0.1.5/PKG-INFO
--rw-r--r--   0 er         (501) staff       (20)     1292 2023-07-09 23:11:04.000000 docs2txt-0.1.5/README.rst
-drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 23:11:11.831633 docs2txt-0.1.5/docs/
--rw-r--r--   0 er         (501) staff       (20)      609 2023-07-09 22:35:52.000000 docs2txt-0.1.5/docs/Makefile
--rw-r--r--   0 er         (501) staff       (20)       28 2023-07-09 22:35:52.000000 docs2txt-0.1.5/docs/authors.rst
--rwxr-xr-x   0 er         (501) staff       (20)     4791 2023-07-09 22:45:01.000000 docs2txt-0.1.5/docs/conf.py
--rw-r--r--   0 er         (501) staff       (20)       33 2023-07-09 22:35:52.000000 docs2txt-0.1.5/docs/contributing.rst
--rw-r--r--   0 er         (501) staff       (20)       28 2023-07-09 22:35:52.000000 docs2txt-0.1.5/docs/history.rst
--rw-r--r--   0 er         (501) staff       (20)      310 2023-07-09 22:35:52.000000 docs2txt-0.1.5/docs/index.rst
--rw-r--r--   0 er         (501) staff       (20)     1133 2023-07-09 22:35:52.000000 docs2txt-0.1.5/docs/installation.rst
--rw-r--r--   0 er         (501) staff       (20)      770 2023-07-09 22:35:52.000000 docs2txt-0.1.5/docs/make.bat
--rw-r--r--   0 er         (501) staff       (20)       27 2023-07-09 22:35:52.000000 docs2txt-0.1.5/docs/readme.rst
--rw-r--r--   0 er         (501) staff       (20)       76 2023-07-09 22:35:52.000000 docs2txt-0.1.5/docs/usage.rst
-drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 23:11:11.847929 docs2txt-0.1.5/docs2txt/
--rw-r--r--   0 er         (501) staff       (20)      130 2023-07-09 23:11:08.000000 docs2txt-0.1.5/docs2txt/__init__.py
--rw-r--r--   0 er         (501) staff       (20)      888 2023-07-09 22:50:43.000000 docs2txt-0.1.5/docs2txt/__main__.py
--rw-r--r--   0 er         (501) staff       (20)     3472 2023-07-09 22:56:33.000000 docs2txt-0.1.5/docs2txt/docs_rs.py
--rw-r--r--   0 er         (501) staff       (20)      387 2023-07-09 22:56:33.000000 docs2txt-0.1.5/docs2txt/utils.py
-drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 23:11:11.851449 docs2txt-0.1.5/docs2txt.egg-info/
--rw-r--r--   0 er         (501) staff       (20)     2283 2023-07-09 23:11:11.000000 docs2txt-0.1.5/docs2txt.egg-info/PKG-INFO
--rw-r--r--   0 er         (501) staff       (20)      601 2023-07-09 23:11:11.000000 docs2txt-0.1.5/docs2txt.egg-info/SOURCES.txt
--rw-r--r--   0 er         (501) staff       (20)        1 2023-07-09 23:11:11.000000 docs2txt-0.1.5/docs2txt.egg-info/dependency_links.txt
--rw-r--r--   0 er         (501) staff       (20)       47 2023-07-09 23:11:11.000000 docs2txt-0.1.5/docs2txt.egg-info/entry_points.txt
--rw-r--r--   0 er         (501) staff       (20)        1 2023-07-09 21:28:14.000000 docs2txt-0.1.5/docs2txt.egg-info/not-zip-safe
--rw-r--r--   0 er         (501) staff       (20)       98 2023-07-09 23:11:11.000000 docs2txt-0.1.5/docs2txt.egg-info/requires.txt
--rw-r--r--   0 er         (501) staff       (20)        9 2023-07-09 23:11:11.000000 docs2txt-0.1.5/docs2txt.egg-info/top_level.txt
--rw-r--r--   0 er         (501) staff       (20)      380 2023-07-09 23:11:11.853696 docs2txt-0.1.5/setup.cfg
--rw-r--r--   0 er         (501) staff       (20)     2159 2023-07-09 22:54:09.000000 docs2txt-0.1.5/setup.py
-drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 23:11:11.852362 docs2txt-0.1.5/tests/
--rw-r--r--   0 er         (501) staff       (20)       38 2023-07-09 22:35:52.000000 docs2txt-0.1.5/tests/__init__.py
--rw-r--r--   0 er         (501) staff       (20)      859 2023-07-09 22:35:52.000000 docs2txt-0.1.5/tests/test_docs2txt.py
+drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 23:15:13.010503 docs2txt-0.1.6/
+-rw-r--r--   0 er         (501) staff       (20)      155 2023-07-09 22:35:52.000000 docs2txt-0.1.6/AUTHORS.rst
+-rw-r--r--   0 er         (501) staff       (20)     3543 2023-07-09 22:35:52.000000 docs2txt-0.1.6/CONTRIBUTING.rst
+-rw-r--r--   0 er         (501) staff       (20)      293 2023-07-09 23:15:03.000000 docs2txt-0.1.6/HISTORY.rst
+-rw-r--r--   0 er         (501) staff       (20)     1064 2023-07-09 22:35:54.000000 docs2txt-0.1.6/LICENSE
+-rw-r--r--   0 er         (501) staff       (20)      262 2023-07-09 22:35:52.000000 docs2txt-0.1.6/MANIFEST.in
+-rw-r--r--   0 er         (501) staff       (20)     2487 2023-07-09 23:15:13.010680 docs2txt-0.1.6/PKG-INFO
+-rw-r--r--   0 er         (501) staff       (20)     1292 2023-07-09 23:11:04.000000 docs2txt-0.1.6/README.rst
+drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 23:15:13.003514 docs2txt-0.1.6/docs/
+-rw-r--r--   0 er         (501) staff       (20)      609 2023-07-09 22:35:52.000000 docs2txt-0.1.6/docs/Makefile
+-rw-r--r--   0 er         (501) staff       (20)       28 2023-07-09 22:35:52.000000 docs2txt-0.1.6/docs/authors.rst
+-rwxr-xr-x   0 er         (501) staff       (20)     4791 2023-07-09 22:45:01.000000 docs2txt-0.1.6/docs/conf.py
+-rw-r--r--   0 er         (501) staff       (20)       33 2023-07-09 22:35:52.000000 docs2txt-0.1.6/docs/contributing.rst
+-rw-r--r--   0 er         (501) staff       (20)       28 2023-07-09 22:35:52.000000 docs2txt-0.1.6/docs/history.rst
+-rw-r--r--   0 er         (501) staff       (20)      310 2023-07-09 22:35:52.000000 docs2txt-0.1.6/docs/index.rst
+-rw-r--r--   0 er         (501) staff       (20)     1133 2023-07-09 22:35:52.000000 docs2txt-0.1.6/docs/installation.rst
+-rw-r--r--   0 er         (501) staff       (20)      770 2023-07-09 22:35:52.000000 docs2txt-0.1.6/docs/make.bat
+-rw-r--r--   0 er         (501) staff       (20)       27 2023-07-09 22:35:52.000000 docs2txt-0.1.6/docs/readme.rst
+-rw-r--r--   0 er         (501) staff       (20)       76 2023-07-09 22:35:52.000000 docs2txt-0.1.6/docs/usage.rst
+drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 23:15:13.005458 docs2txt-0.1.6/docs2txt/
+-rw-r--r--   0 er         (501) staff       (20)      130 2023-07-09 23:14:02.000000 docs2txt-0.1.6/docs2txt/__init__.py
+-rw-r--r--   0 er         (501) staff       (20)      888 2023-07-09 22:50:43.000000 docs2txt-0.1.6/docs2txt/__main__.py
+-rw-r--r--   0 er         (501) staff       (20)     3472 2023-07-09 22:56:33.000000 docs2txt-0.1.6/docs2txt/docs_rs.py
+-rw-r--r--   0 er         (501) staff       (20)      387 2023-07-09 22:56:33.000000 docs2txt-0.1.6/docs2txt/utils.py
+drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 23:15:13.008809 docs2txt-0.1.6/docs2txt.egg-info/
+-rw-r--r--   0 er         (501) staff       (20)     2487 2023-07-09 23:15:12.000000 docs2txt-0.1.6/docs2txt.egg-info/PKG-INFO
+-rw-r--r--   0 er         (501) staff       (20)      601 2023-07-09 23:15:12.000000 docs2txt-0.1.6/docs2txt.egg-info/SOURCES.txt
+-rw-r--r--   0 er         (501) staff       (20)        1 2023-07-09 23:15:12.000000 docs2txt-0.1.6/docs2txt.egg-info/dependency_links.txt
+-rw-r--r--   0 er         (501) staff       (20)       47 2023-07-09 23:15:12.000000 docs2txt-0.1.6/docs2txt.egg-info/entry_points.txt
+-rw-r--r--   0 er         (501) staff       (20)        1 2023-07-09 21:28:14.000000 docs2txt-0.1.6/docs2txt.egg-info/not-zip-safe
+-rw-r--r--   0 er         (501) staff       (20)       98 2023-07-09 23:15:12.000000 docs2txt-0.1.6/docs2txt.egg-info/requires.txt
+-rw-r--r--   0 er         (501) staff       (20)        9 2023-07-09 23:15:12.000000 docs2txt-0.1.6/docs2txt.egg-info/top_level.txt
+-rw-r--r--   0 er         (501) staff       (20)      380 2023-07-09 23:15:13.011536 docs2txt-0.1.6/setup.cfg
+-rw-r--r--   0 er         (501) staff       (20)     2159 2023-07-09 22:54:09.000000 docs2txt-0.1.6/setup.py
+drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 23:15:13.009910 docs2txt-0.1.6/tests/
+-rw-r--r--   0 er         (501) staff       (20)       38 2023-07-09 22:35:52.000000 docs2txt-0.1.6/tests/__init__.py
+-rw-r--r--   0 er         (501) staff       (20)      859 2023-07-09 22:35:52.000000 docs2txt-0.1.6/tests/test_docs2txt.py
```

### Comparing `docs2txt-0.1.5/CONTRIBUTING.rst` & `docs2txt-0.1.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.5/LICENSE` & `docs2txt-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.5/PKG-INFO` & `docs2txt-0.1.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs2txt
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple program to download documentation from docs.rs and convert it into a plaintext file.
 Home-page: https://github.com/ehutzle/docs2txt
 Author: Eric Richard
 Author-email: ehutzle@gmail.com
 License: MIT license
 Keywords: docs2txt
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -78,7 +78,22 @@
 History
 =======
 
 0.1.0 (2023-07-09)
 ------------------
 
 * First release on PyPI.
+
+0.1.1 - 0.1.4 (2023-07-09)
+--------------------------
+
+* Bug Fixes
+
+0.1.5 (2023-07-09)
+------------------
+
+* Updated Readme with usage and example
+
+0.1.6 (2023-07-09)
+------------------
+
+* Added History
```

### Comparing `docs2txt-0.1.5/README.rst` & `docs2txt-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.5/docs/Makefile` & `docs2txt-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.5/docs/conf.py` & `docs2txt-0.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.5/docs/installation.rst` & `docs2txt-0.1.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.5/docs/make.bat` & `docs2txt-0.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.5/docs2txt/__main__.py` & `docs2txt-0.1.6/docs2txt/__main__.py`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.5/docs2txt/docs_rs.py` & `docs2txt-0.1.6/docs2txt/docs_rs.py`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.5/docs2txt.egg-info/PKG-INFO` & `docs2txt-0.1.6/docs2txt.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs2txt
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple program to download documentation from docs.rs and convert it into a plaintext file.
 Home-page: https://github.com/ehutzle/docs2txt
 Author: Eric Richard
 Author-email: ehutzle@gmail.com
 License: MIT license
 Keywords: docs2txt
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -78,7 +78,22 @@
 History
 =======
 
 0.1.0 (2023-07-09)
 ------------------
 
 * First release on PyPI.
+
+0.1.1 - 0.1.4 (2023-07-09)
+--------------------------
+
+* Bug Fixes
+
+0.1.5 (2023-07-09)
+------------------
+
+* Updated Readme with usage and example
+
+0.1.6 (2023-07-09)
+------------------
+
+* Added History
```

### Comparing `docs2txt-0.1.5/docs2txt.egg-info/SOURCES.txt` & `docs2txt-0.1.6/docs2txt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.5/setup.py` & `docs2txt-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.5/tests/test_docs2txt.py` & `docs2txt-0.1.6/tests/test_docs2txt.py`

 * *Files identical despite different names*

