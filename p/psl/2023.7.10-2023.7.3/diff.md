# Comparing `tmp/psl-2023.7.10.tar.gz` & `tmp/psl-2023.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psl-2023.7.10.tar", last modified: Mon Jul 10 13:09:12 2023, max compression
+gzip compressed data, was "psl-2023.7.3.tar", last modified: Mon Jul  3 13:09:44 2023, max compression
```

## Comparing `psl-2023.7.10.tar` & `psl-2023.7.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:09:12.692476 psl-2023.7.10/
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-07-10 13:08:37.000000 psl-2023.7.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 13:08:37.000000 psl-2023.7.10/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-10 13:09:12.692476 psl-2023.7.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-10 13:08:37.000000 psl-2023.7.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:09:12.692476 psl-2023.7.10/psl/
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-07-10 13:08:47.000000 psl-2023.7.10/psl/__init__.py
--rw-------   0 runner    (1001) docker     (123)   110999 2023-07-10 13:08:47.000000 psl-2023.7.10/psl/psl.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:08:37.000000 psl-2023.7.10/psl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:09:12.692476 psl-2023.7.10/psl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-10 13:09:12.000000 psl-2023.7.10/psl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-10 13:09:12.000000 psl-2023.7.10/psl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:09:12.000000 psl-2023.7.10/psl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:09:00.000000 psl-2023.7.10/psl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:09:12.000000 psl-2023.7.10/psl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 13:09:12.692476 psl-2023.7.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-10 13:08:37.000000 psl-2023.7.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:09:44.307404 psl-2023.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-07-03 13:09:02.000000 psl-2023.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-03 13:09:02.000000 psl-2023.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-03 13:09:44.307404 psl-2023.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-03 13:09:02.000000 psl-2023.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:09:44.303404 psl-2023.7.3/psl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-03 13:09:14.000000 psl-2023.7.3/psl/__init__.py
+-rw-------   0 runner    (1001) docker     (123)   111024 2023-07-03 13:09:14.000000 psl-2023.7.3/psl/psl.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:09:02.000000 psl-2023.7.3/psl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:09:44.307404 psl-2023.7.3/psl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-03 13:09:44.000000 psl-2023.7.3/psl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-03 13:09:44.000000 psl-2023.7.3/psl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:09:44.000000 psl-2023.7.3/psl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:09:30.000000 psl-2023.7.3/psl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-03 13:09:44.000000 psl-2023.7.3/psl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 13:09:44.307404 psl-2023.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-03 13:09:02.000000 psl-2023.7.3/setup.py
```

### Comparing `psl-2023.7.10/LICENSE` & `psl-2023.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `psl-2023.7.10/PKG-INFO` & `psl-2023.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2023.7.10
+Version: 2023.7.3
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2023.7.10/README.md` & `psl-2023.7.3/README.md`

 * *Files identical despite different names*

### Comparing `psl-2023.7.10/psl/__init__.py` & `psl-2023.7.3/psl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 import pathlib
 import typing
 
-__version__ = "2023.7.10"
-__checksum__ = "ab450582328e0bb81d22d0eef67a70e4536b8dd9"
+__version__ = "2023.7.3"
+__checksum__ = "c6a23cf216230ba3c1b9863f7a89d9529ea6f702"
 __all__ = ["PUBLIC_SUFFIX_URL", "domain_suffixes", "Suffixes", "domain_can_set_cookie"]
 
 
 PUBLIC_SUFFIX_URL = "https://publicsuffix.org/list/public_suffix_list.dat"
 _PUBLIC_SUFFIX_PATH = pathlib.Path(__file__).parent / "psl.txt"
```

### Comparing `psl-2023.7.10/psl/psl.txt` & `psl-2023.7.3/psl/psl.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6209,14 +6209,15 @@
 homesense
 honda
 horse
 hospital
 host
 hosting
 hot
+hoteles
 hotels
 hotmail
 house
 how
 hsbc
 hughes
 hyatt
@@ -6456,14 +6457,15 @@
 page
 panasonic
 paris
 pars
 partners
 parts
 party
+passagens
 pay
 pccw
 pet
 pfizer
 pharmacy
 phd
 philips
@@ -6745,14 +6747,15 @@
 vodka
 volkswagen
 volvo
 vote
 voting
 voto
 voyage
+vuelos
 wales
 walmart
 walter
 wang
 wanggou
 watch
 watches
```

### Comparing `psl-2023.7.10/psl.egg-info/PKG-INFO` & `psl-2023.7.3/psl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2023.7.10
+Version: 2023.7.3
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2023.7.10/setup.py` & `psl-2023.7.3/setup.py`

 * *Files identical despite different names*

