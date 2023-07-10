# Comparing `tmp/kthbuild-3.3.0.tar.gz` & `tmp/kthbuild-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kthbuild-3.3.0.tar", last modified: Mon Jul 10 10:14:00 2023, max compression
+gzip compressed data, was "kthbuild-3.4.0.tar", last modified: Mon Jul 10 10:18:53 2023, max compression
```

## Comparing `kthbuild-3.3.0.tar` & `kthbuild-3.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 10:14:00.058287 kthbuild-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-10 10:13:31.000000 kthbuild-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-07-10 10:14:00.058287 kthbuild-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-07-10 10:13:31.000000 kthbuild-3.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 10:14:00.058287 kthbuild-3.3.0/kthbuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-07-10 10:14:00.000000 kthbuild-3.3.0/kthbuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-10 10:14:00.000000 kthbuild-3.3.0/kthbuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-10 10:14:00.000000 kthbuild-3.3.0/kthbuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-10 10:14:00.000000 kthbuild-3.3.0/kthbuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-10 10:14:00.000000 kthbuild-3.3.0/kthbuild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    42295 2023-07-10 10:13:31.000000 kthbuild-3.3.0/kthbuild.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-10 10:14:00.058287 kthbuild-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-07-10 10:13:31.000000 kthbuild-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 10:18:53.960210 kthbuild-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-10 10:18:25.000000 kthbuild-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-07-10 10:18:53.956210 kthbuild-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-07-10 10:18:25.000000 kthbuild-3.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 10:18:53.956210 kthbuild-3.4.0/kthbuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-07-10 10:18:53.000000 kthbuild-3.4.0/kthbuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-10 10:18:53.000000 kthbuild-3.4.0/kthbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-10 10:18:53.000000 kthbuild-3.4.0/kthbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-10 10:18:53.000000 kthbuild-3.4.0/kthbuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-10 10:18:53.000000 kthbuild-3.4.0/kthbuild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    42295 2023-07-10 10:18:25.000000 kthbuild-3.4.0/kthbuild.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-10 10:18:53.960210 kthbuild-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-07-10 10:18:25.000000 kthbuild-3.4.0/setup.py
```

### Comparing `kthbuild-3.3.0/LICENSE` & `kthbuild-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kthbuild-3.3.0/PKG-INFO` & `kthbuild-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kthbuild
-Version: 3.3.0
+Version: 3.4.0
 Summary: Knuth node build tools
 Home-page: https://github.com/k-nuth/kthbuild
 Author: Fernando Pelliccioni
 Author-email: fpelliccioni@gmail.com
 License: MIT
 Keywords: knuth kth crypto bitcoin btc bch cash build tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kthbuild-3.3.0/kthbuild.egg-info/PKG-INFO` & `kthbuild-3.4.0/kthbuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kthbuild
-Version: 3.3.0
+Version: 3.4.0
 Summary: Knuth node build tools
 Home-page: https://github.com/k-nuth/kthbuild
 Author: Fernando Pelliccioni
 Author-email: fpelliccioni@gmail.com
 License: MIT
 Keywords: knuth kth crypto bitcoin btc bch cash build tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kthbuild-3.3.0/kthbuild.py` & `kthbuild-3.4.0/kthbuild.py`

 * *Files identical despite different names*

### Comparing `kthbuild-3.3.0/setup.py` & `kthbuild-3.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import subprocess
 import os
 import platform
 
 __title__ = "kthbuild"
 __summary__ = "Knuth node build tools"
 __uri__ = "https://github.com/k-nuth/kthbuild"
-__version__ = "3.3.0"
+__version__ = "3.4.0"
 __author__ = "Fernando Pelliccioni"
 __email__ = "fpelliccioni@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) 2019-2023 Knuth Project"
 
 
 install_requires = [
```

