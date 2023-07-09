# Comparing `tmp/docs2txt-0.1.3.tar.gz` & `tmp/docs2txt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docs2txt-0.1.3.tar", last modified: Sun Jul  9 22:54:32 2023, max compression
+gzip compressed data, was "docs2txt-0.1.4.tar", last modified: Sun Jul  9 22:56:48 2023, max compression
```

## Comparing `docs2txt-0.1.3.tar` & `docs2txt-0.1.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:54:32.801303 docs2txt-0.1.3/
--rw-r--r--   0 er         (501) staff       (20)      155 2023-07-09 22:35:52.000000 docs2txt-0.1.3/AUTHORS.rst
--rw-r--r--   0 er         (501) staff       (20)     3543 2023-07-09 22:35:52.000000 docs2txt-0.1.3/CONTRIBUTING.rst
--rw-r--r--   0 er         (501) staff       (20)       89 2023-07-09 22:35:52.000000 docs2txt-0.1.3/HISTORY.rst
--rw-r--r--   0 er         (501) staff       (20)     1064 2023-07-09 22:35:54.000000 docs2txt-0.1.3/LICENSE
--rw-r--r--   0 er         (501) staff       (20)      262 2023-07-09 22:35:52.000000 docs2txt-0.1.3/MANIFEST.in
--rw-r--r--   0 er         (501) staff       (20)     1925 2023-07-09 22:54:32.801434 docs2txt-0.1.3/PKG-INFO
--rw-r--r--   0 er         (501) staff       (20)      934 2023-07-09 22:35:52.000000 docs2txt-0.1.3/README.rst
-drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:54:32.796442 docs2txt-0.1.3/docs/
--rw-r--r--   0 er         (501) staff       (20)      609 2023-07-09 22:35:52.000000 docs2txt-0.1.3/docs/Makefile
--rw-r--r--   0 er         (501) staff       (20)       28 2023-07-09 22:35:52.000000 docs2txt-0.1.3/docs/authors.rst
--rwxr-xr-x   0 er         (501) staff       (20)     4791 2023-07-09 22:45:01.000000 docs2txt-0.1.3/docs/conf.py
--rw-r--r--   0 er         (501) staff       (20)       33 2023-07-09 22:35:52.000000 docs2txt-0.1.3/docs/contributing.rst
--rw-r--r--   0 er         (501) staff       (20)       28 2023-07-09 22:35:52.000000 docs2txt-0.1.3/docs/history.rst
--rw-r--r--   0 er         (501) staff       (20)      310 2023-07-09 22:35:52.000000 docs2txt-0.1.3/docs/index.rst
--rw-r--r--   0 er         (501) staff       (20)     1133 2023-07-09 22:35:52.000000 docs2txt-0.1.3/docs/installation.rst
--rw-r--r--   0 er         (501) staff       (20)      770 2023-07-09 22:35:52.000000 docs2txt-0.1.3/docs/make.bat
--rw-r--r--   0 er         (501) staff       (20)       27 2023-07-09 22:35:52.000000 docs2txt-0.1.3/docs/readme.rst
--rw-r--r--   0 er         (501) staff       (20)       76 2023-07-09 22:35:52.000000 docs2txt-0.1.3/docs/usage.rst
-drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:54:32.797860 docs2txt-0.1.3/docs2txt/
--rw-r--r--   0 er         (501) staff       (20)      130 2023-07-09 22:54:31.000000 docs2txt-0.1.3/docs2txt/__init__.py
--rw-r--r--   0 er         (501) staff       (20)      888 2023-07-09 22:50:43.000000 docs2txt-0.1.3/docs2txt/__main__.py
--rw-r--r--   0 er         (501) staff       (20)     3471 2023-07-09 22:35:52.000000 docs2txt-0.1.3/docs2txt/docs_rs.py
--rw-r--r--   0 er         (501) staff       (20)      415 2023-07-09 22:35:52.000000 docs2txt-0.1.3/docs2txt/utils.py
-drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:54:32.800313 docs2txt-0.1.3/docs2txt.egg-info/
--rw-r--r--   0 er         (501) staff       (20)     1925 2023-07-09 22:54:32.000000 docs2txt-0.1.3/docs2txt.egg-info/PKG-INFO
--rw-r--r--   0 er         (501) staff       (20)      601 2023-07-09 22:54:32.000000 docs2txt-0.1.3/docs2txt.egg-info/SOURCES.txt
--rw-r--r--   0 er         (501) staff       (20)        1 2023-07-09 22:54:32.000000 docs2txt-0.1.3/docs2txt.egg-info/dependency_links.txt
--rw-r--r--   0 er         (501) staff       (20)       47 2023-07-09 22:54:32.000000 docs2txt-0.1.3/docs2txt.egg-info/entry_points.txt
--rw-r--r--   0 er         (501) staff       (20)        1 2023-07-09 21:28:14.000000 docs2txt-0.1.3/docs2txt.egg-info/not-zip-safe
--rw-r--r--   0 er         (501) staff       (20)       85 2023-07-09 22:54:32.000000 docs2txt-0.1.3/docs2txt.egg-info/requires.txt
--rw-r--r--   0 er         (501) staff       (20)        9 2023-07-09 22:54:32.000000 docs2txt-0.1.3/docs2txt.egg-info/top_level.txt
--rw-r--r--   0 er         (501) staff       (20)      380 2023-07-09 22:54:32.802034 docs2txt-0.1.3/setup.cfg
--rw-r--r--   0 er         (501) staff       (20)     2159 2023-07-09 22:54:09.000000 docs2txt-0.1.3/setup.py
-drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:54:32.801018 docs2txt-0.1.3/tests/
--rw-r--r--   0 er         (501) staff       (20)       38 2023-07-09 22:35:52.000000 docs2txt-0.1.3/tests/__init__.py
--rw-r--r--   0 er         (501) staff       (20)      859 2023-07-09 22:35:52.000000 docs2txt-0.1.3/tests/test_docs2txt.py
+drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:56:48.793183 docs2txt-0.1.4/
+-rw-r--r--   0 er         (501) staff       (20)      155 2023-07-09 22:35:52.000000 docs2txt-0.1.4/AUTHORS.rst
+-rw-r--r--   0 er         (501) staff       (20)     3543 2023-07-09 22:35:52.000000 docs2txt-0.1.4/CONTRIBUTING.rst
+-rw-r--r--   0 er         (501) staff       (20)       89 2023-07-09 22:35:52.000000 docs2txt-0.1.4/HISTORY.rst
+-rw-r--r--   0 er         (501) staff       (20)     1064 2023-07-09 22:35:54.000000 docs2txt-0.1.4/LICENSE
+-rw-r--r--   0 er         (501) staff       (20)      262 2023-07-09 22:35:52.000000 docs2txt-0.1.4/MANIFEST.in
+-rw-r--r--   0 er         (501) staff       (20)     1925 2023-07-09 22:56:48.793309 docs2txt-0.1.4/PKG-INFO
+-rw-r--r--   0 er         (501) staff       (20)      934 2023-07-09 22:35:52.000000 docs2txt-0.1.4/README.rst
+drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:56:48.787848 docs2txt-0.1.4/docs/
+-rw-r--r--   0 er         (501) staff       (20)      609 2023-07-09 22:35:52.000000 docs2txt-0.1.4/docs/Makefile
+-rw-r--r--   0 er         (501) staff       (20)       28 2023-07-09 22:35:52.000000 docs2txt-0.1.4/docs/authors.rst
+-rwxr-xr-x   0 er         (501) staff       (20)     4791 2023-07-09 22:45:01.000000 docs2txt-0.1.4/docs/conf.py
+-rw-r--r--   0 er         (501) staff       (20)       33 2023-07-09 22:35:52.000000 docs2txt-0.1.4/docs/contributing.rst
+-rw-r--r--   0 er         (501) staff       (20)       28 2023-07-09 22:35:52.000000 docs2txt-0.1.4/docs/history.rst
+-rw-r--r--   0 er         (501) staff       (20)      310 2023-07-09 22:35:52.000000 docs2txt-0.1.4/docs/index.rst
+-rw-r--r--   0 er         (501) staff       (20)     1133 2023-07-09 22:35:52.000000 docs2txt-0.1.4/docs/installation.rst
+-rw-r--r--   0 er         (501) staff       (20)      770 2023-07-09 22:35:52.000000 docs2txt-0.1.4/docs/make.bat
+-rw-r--r--   0 er         (501) staff       (20)       27 2023-07-09 22:35:52.000000 docs2txt-0.1.4/docs/readme.rst
+-rw-r--r--   0 er         (501) staff       (20)       76 2023-07-09 22:35:52.000000 docs2txt-0.1.4/docs/usage.rst
+drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:56:48.789346 docs2txt-0.1.4/docs2txt/
+-rw-r--r--   0 er         (501) staff       (20)      130 2023-07-09 22:56:40.000000 docs2txt-0.1.4/docs2txt/__init__.py
+-rw-r--r--   0 er         (501) staff       (20)      888 2023-07-09 22:50:43.000000 docs2txt-0.1.4/docs2txt/__main__.py
+-rw-r--r--   0 er         (501) staff       (20)     3472 2023-07-09 22:56:33.000000 docs2txt-0.1.4/docs2txt/docs_rs.py
+-rw-r--r--   0 er         (501) staff       (20)      387 2023-07-09 22:56:33.000000 docs2txt-0.1.4/docs2txt/utils.py
+drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:56:48.792061 docs2txt-0.1.4/docs2txt.egg-info/
+-rw-r--r--   0 er         (501) staff       (20)     1925 2023-07-09 22:56:48.000000 docs2txt-0.1.4/docs2txt.egg-info/PKG-INFO
+-rw-r--r--   0 er         (501) staff       (20)      601 2023-07-09 22:56:48.000000 docs2txt-0.1.4/docs2txt.egg-info/SOURCES.txt
+-rw-r--r--   0 er         (501) staff       (20)        1 2023-07-09 22:56:48.000000 docs2txt-0.1.4/docs2txt.egg-info/dependency_links.txt
+-rw-r--r--   0 er         (501) staff       (20)       47 2023-07-09 22:56:48.000000 docs2txt-0.1.4/docs2txt.egg-info/entry_points.txt
+-rw-r--r--   0 er         (501) staff       (20)        1 2023-07-09 21:28:14.000000 docs2txt-0.1.4/docs2txt.egg-info/not-zip-safe
+-rw-r--r--   0 er         (501) staff       (20)       98 2023-07-09 22:56:48.000000 docs2txt-0.1.4/docs2txt.egg-info/requires.txt
+-rw-r--r--   0 er         (501) staff       (20)        9 2023-07-09 22:56:48.000000 docs2txt-0.1.4/docs2txt.egg-info/top_level.txt
+-rw-r--r--   0 er         (501) staff       (20)      380 2023-07-09 22:56:48.793883 docs2txt-0.1.4/setup.cfg
+-rw-r--r--   0 er         (501) staff       (20)     2159 2023-07-09 22:54:09.000000 docs2txt-0.1.4/setup.py
+drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:56:48.792877 docs2txt-0.1.4/tests/
+-rw-r--r--   0 er         (501) staff       (20)       38 2023-07-09 22:35:52.000000 docs2txt-0.1.4/tests/__init__.py
+-rw-r--r--   0 er         (501) staff       (20)      859 2023-07-09 22:35:52.000000 docs2txt-0.1.4/tests/test_docs2txt.py
```

### Comparing `docs2txt-0.1.3/CONTRIBUTING.rst` & `docs2txt-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.3/LICENSE` & `docs2txt-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.3/PKG-INFO` & `docs2txt-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs2txt
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple program to download documentation from docs.rs and convert it into a plaintext file.
 Home-page: https://github.com/ehutzle/docs2txt
 Author: Eric Richard
 Author-email: ehutzle@gmail.com
 License: MIT license
 Keywords: docs2txt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `docs2txt-0.1.3/README.rst` & `docs2txt-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.3/docs/Makefile` & `docs2txt-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.3/docs/conf.py` & `docs2txt-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.3/docs/installation.rst` & `docs2txt-0.1.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.3/docs/make.bat` & `docs2txt-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.3/docs2txt/__main__.py` & `docs2txt-0.1.4/docs2txt/__main__.py`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.3/docs2txt/docs_rs.py` & `docs2txt-0.1.4/docs2txt/docs_rs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Main module."""
+
 from pathlib import Path
 
 import requests
 from bs4 import BeautifulSoup
 from rich.console import Console
 from tqdm import tqdm
```

### Comparing `docs2txt-0.1.3/docs2txt.egg-info/PKG-INFO` & `docs2txt-0.1.4/docs2txt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs2txt
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple program to download documentation from docs.rs and convert it into a plaintext file.
 Home-page: https://github.com/ehutzle/docs2txt
 Author: Eric Richard
 Author-email: ehutzle@gmail.com
 License: MIT license
 Keywords: docs2txt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `docs2txt-0.1.3/docs2txt.egg-info/SOURCES.txt` & `docs2txt-0.1.4/docs2txt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.3/setup.py` & `docs2txt-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.3/tests/test_docs2txt.py` & `docs2txt-0.1.4/tests/test_docs2txt.py`

 * *Files identical despite different names*

