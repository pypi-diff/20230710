# Comparing `tmp/delphi_epidata-4.1.4.tar.gz` & `tmp/delphi_epidata-4.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delphi_epidata-4.1.4.tar", last modified: Tue Jun 27 18:28:15 2023, max compression
+gzip compressed data, was "delphi_epidata-4.1.5.tar", last modified: Mon Jul 10 21:37:04 2023, max compression
```

## Comparing `delphi_epidata-4.1.4.tar` & `delphi_epidata-4.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:28:15.222568 delphi_epidata-4.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-27 18:28:02.000000 delphi_epidata-4.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-27 18:28:15.222568 delphi_epidata-4.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-27 18:28:02.000000 delphi_epidata-4.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:28:15.218568 delphi_epidata-4.1.4/delphi_epidata/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-27 18:28:02.000000 delphi_epidata-4.1.4/delphi_epidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23169 2023-06-27 18:28:14.000000 delphi_epidata-4.1.4/delphi_epidata/delphi_epidata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:28:15.222568 delphi_epidata-4.1.4/delphi_epidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-27 18:28:15.000000 delphi_epidata-4.1.4/delphi_epidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-27 18:28:15.000000 delphi_epidata-4.1.4/delphi_epidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:28:15.000000 delphi_epidata-4.1.4/delphi_epidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 18:28:15.000000 delphi_epidata-4.1.4/delphi_epidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 18:28:15.000000 delphi_epidata-4.1.4/delphi_epidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:28:15.222568 delphi_epidata-4.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-27 18:28:02.000000 delphi_epidata-4.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:37:04.296933 delphi_epidata-4.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-10 21:36:54.000000 delphi_epidata-4.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-10 21:37:04.296933 delphi_epidata-4.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-10 21:36:54.000000 delphi_epidata-4.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:37:04.292932 delphi_epidata-4.1.5/delphi_epidata/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-10 21:36:54.000000 delphi_epidata-4.1.5/delphi_epidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23169 2023-07-10 21:37:03.000000 delphi_epidata-4.1.5/delphi_epidata/delphi_epidata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:37:04.296933 delphi_epidata-4.1.5/delphi_epidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-10 21:37:04.000000 delphi_epidata-4.1.5/delphi_epidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-10 21:37:04.000000 delphi_epidata-4.1.5/delphi_epidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 21:37:04.000000 delphi_epidata-4.1.5/delphi_epidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 21:37:04.000000 delphi_epidata-4.1.5/delphi_epidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 21:37:04.000000 delphi_epidata-4.1.5/delphi_epidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 21:37:04.296933 delphi_epidata-4.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-10 21:36:54.000000 delphi_epidata-4.1.5/setup.py
```

### Comparing `delphi_epidata-4.1.4/LICENSE` & `delphi_epidata-4.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `delphi_epidata-4.1.4/PKG-INFO` & `delphi_epidata-4.1.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delphi_epidata
-Version: 4.1.4
+Version: 4.1.5
 Summary: A programmatic interface to Delphi's Epidata API.
 Home-page: https://github.com/cmu-delphi/delphi-epidata
 Author: David Farrow
 Author-email: dfarrow0@gmail.com
 License: UNKNOWN
 Description: # Delphi Epidata API Client
```

### Comparing `delphi_epidata-4.1.4/delphi_epidata/delphi_epidata.py` & `delphi_epidata-4.1.5/delphi_epidata/delphi_epidata.py`

 * *Files identical despite different names*

### Comparing `delphi_epidata-4.1.4/delphi_epidata.egg-info/PKG-INFO` & `delphi_epidata-4.1.5/delphi_epidata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delphi-epidata
-Version: 4.1.4
+Version: 4.1.5
 Summary: A programmatic interface to Delphi's Epidata API.
 Home-page: https://github.com/cmu-delphi/delphi-epidata
 Author: David Farrow
 Author-email: dfarrow0@gmail.com
 License: UNKNOWN
 Description: # Delphi Epidata API Client
```

### Comparing `delphi_epidata-4.1.4/setup.py` & `delphi_epidata-4.1.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="delphi_epidata",
-    version="4.1.4",
+    version="4.1.5",
     author="David Farrow",
     author_email="dfarrow0@gmail.com",
     description="A programmatic interface to Delphi's Epidata API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cmu-delphi/delphi-epidata",
     packages=setuptools.find_packages(),
```

