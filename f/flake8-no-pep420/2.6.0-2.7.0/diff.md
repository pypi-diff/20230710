# Comparing `tmp/flake8_no_pep420-2.6.0.tar.gz` & `tmp/flake8_no_pep420-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_no_pep420-2.6.0.tar", last modified: Thu Jun 15 14:24:34 2023, max compression
+gzip compressed data, was "flake8_no_pep420-2.7.0.tar", last modified: Mon Jul 10 13:46:35 2023, max compression
```

## Comparing `flake8_no_pep420-2.6.0.tar` & `flake8_no_pep420-2.7.0.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-15 14:24:34.914785 flake8_no_pep420-2.6.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1340 2023-06-15 14:24:31.000000 flake8_no_pep420-2.6.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:25.000000 flake8_no_pep420-2.6.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-20 12:10:00.000000 flake8_no_pep420-2.6.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4524 2023-06-15 14:24:34.914882 flake8_no_pep420-2.6.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3314 2023-06-15 14:23:25.000000 flake8_no_pep420-2.6.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-02-28 09:05:59.000000 flake8_no_pep420-2.6.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1483 2023-06-15 14:24:34.915226 flake8_no_pep420-2.6.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-15 14:24:34.905600 flake8_no_pep420-2.6.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-15 14:24:34.906893 flake8_no_pep420-2.6.0/src/flake8_no_pep420/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1062 2023-04-27 15:37:02.000000 flake8_no_pep420-2.6.0/src/flake8_no_pep420/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:25.000000 flake8_no_pep420-2.6.0/src/flake8_no_pep420/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-15 14:24:34.914081 flake8_no_pep420-2.6.0/src/flake8_no_pep420.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4524 2023-06-15 14:24:34.000000 flake8_no_pep420-2.6.0/src/flake8_no_pep420.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      472 2023-06-15 14:24:34.000000 flake8_no_pep420-2.6.0/src/flake8_no_pep420.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-15 14:24:34.000000 flake8_no_pep420-2.6.0/src/flake8_no_pep420.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       58 2023-06-15 14:24:34.000000 flake8_no_pep420-2.6.0/src/flake8_no_pep420.egg-info/entry_points.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-15 14:24:34.000000 flake8_no_pep420-2.6.0/src/flake8_no_pep420.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       66 2023-06-15 14:24:34.000000 flake8_no_pep420-2.6.0/src/flake8_no_pep420.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       17 2023-06-15 14:24:34.000000 flake8_no_pep420-2.6.0/src/flake8_no_pep420.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-15 14:24:34.914423 flake8_no_pep420-2.6.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2580 2023-04-27 15:37:02.000000 flake8_no_pep420-2.6.0/tests/test_flake8_no_pep420.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 13:46:35.246993 flake8_no_pep420-2.7.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1407 2023-07-10 13:46:31.000000 flake8_no_pep420-2.7.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:25.000000 flake8_no_pep420-2.7.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      115 2023-07-10 13:42:36.000000 flake8_no_pep420-2.7.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4474 2023-07-10 13:46:35.247044 flake8_no_pep420-2.7.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3314 2023-07-10 13:42:36.000000 flake8_no_pep420-2.7.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-07-10 13:42:36.000000 flake8_no_pep420-2.7.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1401 2023-07-10 13:46:35.247283 flake8_no_pep420-2.7.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 13:46:35.245268 flake8_no_pep420-2.7.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 13:46:35.246130 flake8_no_pep420-2.7.0/src/flake8_no_pep420/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      966 2023-07-10 13:42:36.000000 flake8_no_pep420-2.7.0/src/flake8_no_pep420/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:25.000000 flake8_no_pep420-2.7.0/src/flake8_no_pep420/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 13:46:35.246896 flake8_no_pep420-2.7.0/src/flake8_no_pep420.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4474 2023-07-10 13:46:35.000000 flake8_no_pep420-2.7.0/src/flake8_no_pep420.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      441 2023-07-10 13:46:35.000000 flake8_no_pep420-2.7.0/src/flake8_no_pep420.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 13:46:35.000000 flake8_no_pep420-2.7.0/src/flake8_no_pep420.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       58 2023-07-10 13:46:35.000000 flake8_no_pep420-2.7.0/src/flake8_no_pep420.egg-info/entry_points.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 13:46:35.000000 flake8_no_pep420-2.7.0/src/flake8_no_pep420.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       20 2023-07-10 13:46:35.000000 flake8_no_pep420-2.7.0/src/flake8_no_pep420.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       17 2023-07-10 13:46:35.000000 flake8_no_pep420-2.7.0/src/flake8_no_pep420.egg-info/top_level.txt
```

### Comparing `flake8_no_pep420-2.6.0/CHANGELOG.rst` & `flake8_no_pep420-2.7.0/CHANGELOG.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+2.7.0 (2023-07-10)
+------------------
+
+* Drop Python 3.7 support.
+
 2.6.0 (2023-06-15)
 ------------------
 
 * Support Python 3.12.
 
 2.5.0 (2023-06-15)
 ------------------
```

### Comparing `flake8_no_pep420-2.6.0/LICENSE` & `flake8_no_pep420-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_no_pep420-2.6.0/PKG-INFO` & `flake8_no_pep420-2.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8_no_pep420
-Version: 2.6.0
+Version: 2.7.0
 Summary: A flake8 plugin to ban PEP-420 implicit namespace packages.
 Home-page: https://github.com/adamchainz/flake8-no-pep420
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/flake8-no-pep420/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -13,22 +13,21 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ================
 flake8-no-pep420
 ================
 
@@ -46,15 +45,15 @@
    :alt: pre-commit
 
 A `flake8 <https://flake8.readthedocs.io/en/latest/index.html>`_ plugin to ban `PEP-420 <https://www.python.org/dev/peps/pep-0420/>`__ implicit namespace packages.
 
 Requirements
 ============
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 Installation
 ============
 
 First, install with ``pip``:
 
 .. code-block:: sh
```

### Comparing `flake8_no_pep420-2.6.0/README.rst` & `flake8_no_pep420-2.7.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
    :alt: pre-commit
 
 A `flake8 <https://flake8.readthedocs.io/en/latest/index.html>`_ plugin to ban `PEP-420 <https://www.python.org/dev/peps/pep-0420/>`__ implicit namespace packages.
 
 Requirements
 ============
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 Installation
 ============
 
 First, install with ``pip``:
 
 .. code-block:: sh
```

### Comparing `flake8_no_pep420-2.6.0/setup.cfg` & `flake8_no_pep420-2.7.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flake8_no_pep420
-version = 2.6.0
+version = 2.7.0
 description = A flake8 plugin to ban PEP-420 implicit namespace packages.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/flake8-no-pep420
 author = Adam Johnson
 author_email = me@adamj.eu
 license = MIT
@@ -13,15 +13,14 @@
 	Development Status :: 5 - Production/Stable
 	Framework :: Flake8
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 	Typing :: Typed
 keywords = flake8
@@ -30,16 +29,15 @@
 	Mastodon = https://fosstodon.org/@adamchainz
 	Twitter = https://twitter.com/adamchainz
 
 [options]
 packages = find:
 install_requires = 
 	flake8!=3.2.0,>=3.0
-	importlib-metadata;python_version < "3.8"
-python_requires = >=3.7
+python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 zip_safe = False
 
 [options.packages.find]
 where = src
```

### Comparing `flake8_no_pep420-2.6.0/src/flake8_no_pep420/__init__.py` & `flake8_no_pep420-2.7.0/src/flake8_no_pep420/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 from __future__ import annotations
 
 import ast
 import os
-import sys
+from importlib.metadata import version
 from typing import Any
 from typing import Generator
 
-if sys.version_info >= (3, 8):
-    from importlib.metadata import version
-else:
-    from importlib_metadata import version
-
 
 class NoPep420Checker:
     name = "flake8-no-pep420"
     version = version("flake8-no-pep420")
 
     def __init__(self, tree: ast.AST, filename: str) -> None:
         self._filename = filename
```

### Comparing `flake8_no_pep420-2.6.0/src/flake8_no_pep420.egg-info/PKG-INFO` & `flake8_no_pep420-2.7.0/src/flake8_no_pep420.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-no-pep420
-Version: 2.6.0
+Version: 2.7.0
 Summary: A flake8 plugin to ban PEP-420 implicit namespace packages.
 Home-page: https://github.com/adamchainz/flake8-no-pep420
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/flake8-no-pep420/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -13,22 +13,21 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ================
 flake8-no-pep420
 ================
 
@@ -46,15 +45,15 @@
    :alt: pre-commit
 
 A `flake8 <https://flake8.readthedocs.io/en/latest/index.html>`_ plugin to ban `PEP-420 <https://www.python.org/dev/peps/pep-0420/>`__ implicit namespace packages.
 
 Requirements
 ============
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 Installation
 ============
 
 First, install with ``pip``:
 
 .. code-block:: sh
```

