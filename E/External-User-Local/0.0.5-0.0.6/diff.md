# Comparing `tmp/External-User-Local-0.0.5.tar.gz` & `tmp/External-User-Local-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "External-User-Local-0.0.5.tar", last modified: Mon Jul 10 07:33:26 2023, max compression
+gzip compressed data, was "External-User-Local-0.0.6.tar", last modified: Mon Jul 10 07:35:54 2023, max compression
```

## Comparing `External-User-Local-0.0.5.tar` & `External-User-Local-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:33:26.666838 External-User-Local-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:33:26.662838 External-User-Local-0.0.5/External_User_Local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-10 07:33:26.000000 External-User-Local-0.0.5/External_User_Local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-10 07:33:26.000000 External-User-Local-0.0.5/External_User_Local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 07:33:26.000000 External-User-Local-0.0.5/External_User_Local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 07:33:26.000000 External-User-Local-0.0.5/External_User_Local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-10 07:33:26.666838 External-User-Local-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-10 07:33:09.000000 External-User-Local-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:33:26.662838 External-User-Local-0.0.5/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 07:33:09.000000 External-User-Local-0.0.5/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-10 07:33:09.000000 External-User-Local-0.0.5/db/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-07-10 07:33:09.000000 External-User-Local-0.0.5/db/library_DB.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 07:33:26.666838 External-User-Local-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-10 07:33:09.000000 External-User-Local-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:33:26.666838 External-User-Local-0.0.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 07:33:09.000000 External-User-Local-0.0.5/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-10 07:33:09.000000 External-User-Local-0.0.5/src/library.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:33:26.666838 External-User-Local-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-10 07:33:09.000000 External-User-Local-0.0.5/tests/test_insertExternal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:35:54.844751 External-User-Local-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:35:54.840751 External-User-Local-0.0.6/External_User_Local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-10 07:35:54.000000 External-User-Local-0.0.6/External_User_Local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-10 07:35:54.000000 External-User-Local-0.0.6/External_User_Local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 07:35:54.000000 External-User-Local-0.0.6/External_User_Local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 07:35:54.000000 External-User-Local-0.0.6/External_User_Local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-10 07:35:54.844751 External-User-Local-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-10 07:35:40.000000 External-User-Local-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:35:54.844751 External-User-Local-0.0.6/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 07:35:40.000000 External-User-Local-0.0.6/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-10 07:35:40.000000 External-User-Local-0.0.6/db/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-07-10 07:35:40.000000 External-User-Local-0.0.6/db/library_DB.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 07:35:54.844751 External-User-Local-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-10 07:35:40.000000 External-User-Local-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:35:54.844751 External-User-Local-0.0.6/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 07:35:40.000000 External-User-Local-0.0.6/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-10 07:35:40.000000 External-User-Local-0.0.6/src/library.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:35:54.844751 External-User-Local-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-10 07:35:40.000000 External-User-Local-0.0.6/tests/test_insertExternal.py
```

### Comparing `External-User-Local-0.0.5/README.md` & `External-User-Local-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `External-User-Local-0.0.5/db/library_DB.py` & `External-User-Local-0.0.6/db/library_DB.py`

 * *Files identical despite different names*

### Comparing `External-User-Local-0.0.5/setup.py` & `External-User-Local-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      # TODO: Please update the name and delete this line i.e. XXX-local or XXX-remote (without the -python-package suffix)
      name='External-User-Local',  
-     version='0.0.5',
+     version='0.0.6',
      author="Circles",
      author_email="info@circles.life",
      # TODO: Please update the description and delete this line
      description="PyPI Package for Circles access token library Local/Remote Python",
      # TODO: Please update the long description and delete this line    
      long_description="This is a package for sharing common access tokens function used in different repositories",
      long_description_content_type="text/markdown",
```

### Comparing `External-User-Local-0.0.5/src/library.py` & `External-User-Local-0.0.6/src/library.py`

 * *Files identical despite different names*

### Comparing `External-User-Local-0.0.5/tests/test_insertExternal.py` & `External-User-Local-0.0.6/tests/test_insertExternal.py`

 * *Files identical despite different names*

