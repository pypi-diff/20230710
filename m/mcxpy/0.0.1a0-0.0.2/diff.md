# Comparing `tmp/mcxpy-0.0.1a0.tar.gz` & `tmp/mcxpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcxpy-0.0.1a0.tar", last modified: Mon Jul 10 18:34:39 2023, max compression
+gzip compressed data, was "mcxpy-0.0.2.tar", last modified: Mon Jul 10 18:39:45 2023, max compression
```

## Comparing `mcxpy-0.0.1a0.tar` & `mcxpy-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 18:34:39.064533 mcxpy-0.0.1a0/
--rw-rw-rw-   0        0        0     1091 2023-07-10 16:20:44.000000 mcxpy-0.0.1a0/LICENSE
--rw-rw-rw-   0        0        0     2875 2023-07-10 18:34:39.041530 mcxpy-0.0.1a0/PKG-INFO
--rw-rw-rw-   0        0        0     1230 2023-07-10 18:29:11.000000 mcxpy-0.0.1a0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 18:34:38.991517 mcxpy-0.0.1a0/mcxpy/
--rw-rw-rw-   0        0        0      405 2023-07-09 17:22:38.000000 mcxpy-0.0.1a0/mcxpy/__init__.py
--rw-rw-rw-   0        0        0      393 2023-07-09 17:22:53.000000 mcxpy-0.0.1a0/mcxpy/__init__.pyi
--rw-rw-rw-   0        0        0    13363 2023-07-09 17:33:24.000000 mcxpy-0.0.1a0/mcxpy/mcx.py
--rw-rw-rw-   0        0        0     1240 2023-07-09 17:23:32.000000 mcxpy-0.0.1a0/mcxpy/mcx.pyi
--rw-rw-rw-   0        0        0        0 2023-07-09 17:16:19.000000 mcxpy-0.0.1a0/mcxpy/py.typed
-drwxrwxrwx   0        0        0        0 2023-07-10 18:34:39.023524 mcxpy-0.0.1a0/mcxpy.egg-info/
--rw-rw-rw-   0        0        0     2875 2023-07-10 18:34:38.000000 mcxpy-0.0.1a0/mcxpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-07-10 18:34:38.000000 mcxpy-0.0.1a0/mcxpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 18:34:38.000000 mcxpy-0.0.1a0/mcxpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-10 18:34:38.000000 mcxpy-0.0.1a0/mcxpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-10 18:34:38.000000 mcxpy-0.0.1a0/mcxpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      611 2023-07-10 18:34:03.000000 mcxpy-0.0.1a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-10 18:34:39.064533 mcxpy-0.0.1a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-10 18:39:45.750632 mcxpy-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-07-10 16:20:44.000000 mcxpy-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2873 2023-07-10 18:39:45.743631 mcxpy-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1230 2023-07-10 18:29:11.000000 mcxpy-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 18:39:45.701620 mcxpy-0.0.2/mcxpy/
+-rw-rw-rw-   0        0        0      405 2023-07-09 17:22:38.000000 mcxpy-0.0.2/mcxpy/__init__.py
+-rw-rw-rw-   0        0        0      393 2023-07-09 17:22:53.000000 mcxpy-0.0.2/mcxpy/__init__.pyi
+-rw-rw-rw-   0        0        0    13363 2023-07-09 17:33:24.000000 mcxpy-0.0.2/mcxpy/mcx.py
+-rw-rw-rw-   0        0        0     1240 2023-07-09 17:23:32.000000 mcxpy-0.0.2/mcxpy/mcx.pyi
+-rw-rw-rw-   0        0        0        0 2023-07-09 17:16:19.000000 mcxpy-0.0.2/mcxpy/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-10 18:39:45.740631 mcxpy-0.0.2/mcxpy.egg-info/
+-rw-rw-rw-   0        0        0     2873 2023-07-10 18:39:45.000000 mcxpy-0.0.2/mcxpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-07-10 18:39:45.000000 mcxpy-0.0.2/mcxpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 18:39:45.000000 mcxpy-0.0.2/mcxpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-10 18:39:45.000000 mcxpy-0.0.2/mcxpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-10 18:39:45.000000 mcxpy-0.0.2/mcxpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      609 2023-07-10 18:39:08.000000 mcxpy-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-10 18:39:45.751640 mcxpy-0.0.2/setup.cfg
```

### Comparing `mcxpy-0.0.1a0/LICENSE` & `mcxpy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mcxpy-0.0.1a0/PKG-INFO` & `mcxpy-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcxpy
-Version: 0.0.1a0
+Version: 0.0.2
 Summary: For fetching mcx data
 Author: Tapan Hazarika
 License: MIT License
         
         Copyright (c)  2023 Tapan Hazarika
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mcxpy-0.0.1a0/README.md` & `mcxpy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mcxpy-0.0.1a0/mcxpy/mcx.py` & `mcxpy-0.0.2/mcxpy/mcx.py`

 * *Files identical despite different names*

### Comparing `mcxpy-0.0.1a0/mcxpy/mcx.pyi` & `mcxpy-0.0.2/mcxpy/mcx.pyi`

 * *Files identical despite different names*

### Comparing `mcxpy-0.0.1a0/mcxpy.egg-info/PKG-INFO` & `mcxpy-0.0.2/mcxpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcxpy
-Version: 0.0.1a0
+Version: 0.0.2
 Summary: For fetching mcx data
 Author: Tapan Hazarika
 License: MIT License
         
         Copyright (c)  2023 Tapan Hazarika
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mcxpy-0.0.1a0/pyproject.toml` & `mcxpy-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mcxpy"
-version = "0.0.1.a"
+version = "0.0.2"
 description = "For fetching mcx data"
 authors = [{ name = "Tapan Hazarika" }]
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = ["pandas>=2.0.0","requests"]
 classifiers = [
     "Programming Language :: Python :: 3",
```

