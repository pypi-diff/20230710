# Comparing `tmp/docs2txt-0.1.4.tar.gz` & `tmp/docs2txt-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docs2txt-0.1.4.tar", last modified: Sun Jul  9 22:56:48 2023, max compression
+gzip compressed data, was "docs2txt-0.1.5.tar", last modified: Sun Jul  9 23:11:11 2023, max compression
```

## Comparing `docs2txt-0.1.4.tar` & `docs2txt-0.1.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:56:48.793183 docs2txt-0.1.4/
--rw-r--r--   0 er         (501) staff       (20)      155 2023-07-09 22:35:52.000000 docs2txt-0.1.4/AUTHORS.rst
--rw-r--r--   0 er         (501) staff       (20)     3543 2023-07-09 22:35:52.000000 docs2txt-0.1.4/CONTRIBUTING.rst
--rw-r--r--   0 er         (501) staff       (20)       89 2023-07-09 22:35:52.000000 docs2txt-0.1.4/HISTORY.rst
--rw-r--r--   0 er         (501) staff       (20)     1064 2023-07-09 22:35:54.000000 docs2txt-0.1.4/LICENSE
--rw-r--r--   0 er         (501) staff       (20)      262 2023-07-09 22:35:52.000000 docs2txt-0.1.4/MANIFEST.in
--rw-r--r--   0 er         (501) staff       (20)     1925 2023-07-09 22:56:48.793309 docs2txt-0.1.4/PKG-INFO
--rw-r--r--   0 er         (501) staff       (20)      934 2023-07-09 22:35:52.000000 docs2txt-0.1.4/README.rst
-drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:56:48.787848 docs2txt-0.1.4/docs/
--rw-r--r--   0 er         (501) staff       (20)      609 2023-07-09 22:35:52.000000 docs2txt-0.1.4/docs/Makefile
--rw-r--r--   0 er         (501) staff       (20)       28 2023-07-09 22:35:52.000000 docs2txt-0.1.4/docs/authors.rst
--rwxr-xr-x   0 er         (501) staff       (20)     4791 2023-07-09 22:45:01.000000 docs2txt-0.1.4/docs/conf.py
--rw-r--r--   0 er         (501) staff       (20)       33 2023-07-09 22:35:52.000000 docs2txt-0.1.4/docs/contributing.rst
--rw-r--r--   0 er         (501) staff       (20)       28 2023-07-09 22:35:52.000000 docs2txt-0.1.4/docs/history.rst
--rw-r--r--   0 er         (501) staff       (20)      310 2023-07-09 22:35:52.000000 docs2txt-0.1.4/docs/index.rst
--rw-r--r--   0 er         (501) staff       (20)     1133 2023-07-09 22:35:52.000000 docs2txt-0.1.4/docs/installation.rst
--rw-r--r--   0 er         (501) staff       (20)      770 2023-07-09 22:35:52.000000 docs2txt-0.1.4/docs/make.bat
--rw-r--r--   0 er         (501) staff       (20)       27 2023-07-09 22:35:52.000000 docs2txt-0.1.4/docs/readme.rst
--rw-r--r--   0 er         (501) staff       (20)       76 2023-07-09 22:35:52.000000 docs2txt-0.1.4/docs/usage.rst
-drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:56:48.789346 docs2txt-0.1.4/docs2txt/
--rw-r--r--   0 er         (501) staff       (20)      130 2023-07-09 22:56:40.000000 docs2txt-0.1.4/docs2txt/__init__.py
--rw-r--r--   0 er         (501) staff       (20)      888 2023-07-09 22:50:43.000000 docs2txt-0.1.4/docs2txt/__main__.py
--rw-r--r--   0 er         (501) staff       (20)     3472 2023-07-09 22:56:33.000000 docs2txt-0.1.4/docs2txt/docs_rs.py
--rw-r--r--   0 er         (501) staff       (20)      387 2023-07-09 22:56:33.000000 docs2txt-0.1.4/docs2txt/utils.py
-drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:56:48.792061 docs2txt-0.1.4/docs2txt.egg-info/
--rw-r--r--   0 er         (501) staff       (20)     1925 2023-07-09 22:56:48.000000 docs2txt-0.1.4/docs2txt.egg-info/PKG-INFO
--rw-r--r--   0 er         (501) staff       (20)      601 2023-07-09 22:56:48.000000 docs2txt-0.1.4/docs2txt.egg-info/SOURCES.txt
--rw-r--r--   0 er         (501) staff       (20)        1 2023-07-09 22:56:48.000000 docs2txt-0.1.4/docs2txt.egg-info/dependency_links.txt
--rw-r--r--   0 er         (501) staff       (20)       47 2023-07-09 22:56:48.000000 docs2txt-0.1.4/docs2txt.egg-info/entry_points.txt
--rw-r--r--   0 er         (501) staff       (20)        1 2023-07-09 21:28:14.000000 docs2txt-0.1.4/docs2txt.egg-info/not-zip-safe
--rw-r--r--   0 er         (501) staff       (20)       98 2023-07-09 22:56:48.000000 docs2txt-0.1.4/docs2txt.egg-info/requires.txt
--rw-r--r--   0 er         (501) staff       (20)        9 2023-07-09 22:56:48.000000 docs2txt-0.1.4/docs2txt.egg-info/top_level.txt
--rw-r--r--   0 er         (501) staff       (20)      380 2023-07-09 22:56:48.793883 docs2txt-0.1.4/setup.cfg
--rw-r--r--   0 er         (501) staff       (20)     2159 2023-07-09 22:54:09.000000 docs2txt-0.1.4/setup.py
-drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 22:56:48.792877 docs2txt-0.1.4/tests/
--rw-r--r--   0 er         (501) staff       (20)       38 2023-07-09 22:35:52.000000 docs2txt-0.1.4/tests/__init__.py
--rw-r--r--   0 er         (501) staff       (20)      859 2023-07-09 22:35:52.000000 docs2txt-0.1.4/tests/test_docs2txt.py
+drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 23:11:11.852726 docs2txt-0.1.5/
+-rw-r--r--   0 er         (501) staff       (20)      155 2023-07-09 22:35:52.000000 docs2txt-0.1.5/AUTHORS.rst
+-rw-r--r--   0 er         (501) staff       (20)     3543 2023-07-09 22:35:52.000000 docs2txt-0.1.5/CONTRIBUTING.rst
+-rw-r--r--   0 er         (501) staff       (20)       89 2023-07-09 22:35:52.000000 docs2txt-0.1.5/HISTORY.rst
+-rw-r--r--   0 er         (501) staff       (20)     1064 2023-07-09 22:35:54.000000 docs2txt-0.1.5/LICENSE
+-rw-r--r--   0 er         (501) staff       (20)      262 2023-07-09 22:35:52.000000 docs2txt-0.1.5/MANIFEST.in
+-rw-r--r--   0 er         (501) staff       (20)     2283 2023-07-09 23:11:11.852895 docs2txt-0.1.5/PKG-INFO
+-rw-r--r--   0 er         (501) staff       (20)     1292 2023-07-09 23:11:04.000000 docs2txt-0.1.5/README.rst
+drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 23:11:11.831633 docs2txt-0.1.5/docs/
+-rw-r--r--   0 er         (501) staff       (20)      609 2023-07-09 22:35:52.000000 docs2txt-0.1.5/docs/Makefile
+-rw-r--r--   0 er         (501) staff       (20)       28 2023-07-09 22:35:52.000000 docs2txt-0.1.5/docs/authors.rst
+-rwxr-xr-x   0 er         (501) staff       (20)     4791 2023-07-09 22:45:01.000000 docs2txt-0.1.5/docs/conf.py
+-rw-r--r--   0 er         (501) staff       (20)       33 2023-07-09 22:35:52.000000 docs2txt-0.1.5/docs/contributing.rst
+-rw-r--r--   0 er         (501) staff       (20)       28 2023-07-09 22:35:52.000000 docs2txt-0.1.5/docs/history.rst
+-rw-r--r--   0 er         (501) staff       (20)      310 2023-07-09 22:35:52.000000 docs2txt-0.1.5/docs/index.rst
+-rw-r--r--   0 er         (501) staff       (20)     1133 2023-07-09 22:35:52.000000 docs2txt-0.1.5/docs/installation.rst
+-rw-r--r--   0 er         (501) staff       (20)      770 2023-07-09 22:35:52.000000 docs2txt-0.1.5/docs/make.bat
+-rw-r--r--   0 er         (501) staff       (20)       27 2023-07-09 22:35:52.000000 docs2txt-0.1.5/docs/readme.rst
+-rw-r--r--   0 er         (501) staff       (20)       76 2023-07-09 22:35:52.000000 docs2txt-0.1.5/docs/usage.rst
+drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 23:11:11.847929 docs2txt-0.1.5/docs2txt/
+-rw-r--r--   0 er         (501) staff       (20)      130 2023-07-09 23:11:08.000000 docs2txt-0.1.5/docs2txt/__init__.py
+-rw-r--r--   0 er         (501) staff       (20)      888 2023-07-09 22:50:43.000000 docs2txt-0.1.5/docs2txt/__main__.py
+-rw-r--r--   0 er         (501) staff       (20)     3472 2023-07-09 22:56:33.000000 docs2txt-0.1.5/docs2txt/docs_rs.py
+-rw-r--r--   0 er         (501) staff       (20)      387 2023-07-09 22:56:33.000000 docs2txt-0.1.5/docs2txt/utils.py
+drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 23:11:11.851449 docs2txt-0.1.5/docs2txt.egg-info/
+-rw-r--r--   0 er         (501) staff       (20)     2283 2023-07-09 23:11:11.000000 docs2txt-0.1.5/docs2txt.egg-info/PKG-INFO
+-rw-r--r--   0 er         (501) staff       (20)      601 2023-07-09 23:11:11.000000 docs2txt-0.1.5/docs2txt.egg-info/SOURCES.txt
+-rw-r--r--   0 er         (501) staff       (20)        1 2023-07-09 23:11:11.000000 docs2txt-0.1.5/docs2txt.egg-info/dependency_links.txt
+-rw-r--r--   0 er         (501) staff       (20)       47 2023-07-09 23:11:11.000000 docs2txt-0.1.5/docs2txt.egg-info/entry_points.txt
+-rw-r--r--   0 er         (501) staff       (20)        1 2023-07-09 21:28:14.000000 docs2txt-0.1.5/docs2txt.egg-info/not-zip-safe
+-rw-r--r--   0 er         (501) staff       (20)       98 2023-07-09 23:11:11.000000 docs2txt-0.1.5/docs2txt.egg-info/requires.txt
+-rw-r--r--   0 er         (501) staff       (20)        9 2023-07-09 23:11:11.000000 docs2txt-0.1.5/docs2txt.egg-info/top_level.txt
+-rw-r--r--   0 er         (501) staff       (20)      380 2023-07-09 23:11:11.853696 docs2txt-0.1.5/setup.cfg
+-rw-r--r--   0 er         (501) staff       (20)     2159 2023-07-09 22:54:09.000000 docs2txt-0.1.5/setup.py
+drwxr-xr-x   0 er         (501) staff       (20)        0 2023-07-09 23:11:11.852362 docs2txt-0.1.5/tests/
+-rw-r--r--   0 er         (501) staff       (20)       38 2023-07-09 22:35:52.000000 docs2txt-0.1.5/tests/__init__.py
+-rw-r--r--   0 er         (501) staff       (20)      859 2023-07-09 22:35:52.000000 docs2txt-0.1.5/tests/test_docs2txt.py
```

### Comparing `docs2txt-0.1.4/CONTRIBUTING.rst` & `docs2txt-0.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.4/LICENSE` & `docs2txt-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.4/PKG-INFO` & `docs2txt-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs2txt
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple program to download documentation from docs.rs and convert it into a plaintext file.
 Home-page: https://github.com/ehutzle/docs2txt
 Author: Eric Richard
 Author-email: ehutzle@gmail.com
 License: MIT license
 Keywords: docs2txt
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =============
-rs-docs-2-txt
+docs2txt
 =============
 
 
 .. image:: https://img.shields.io/pypi/v/docs2txt.svg
         :target: https://pypi.python.org/pypi/docs2txt
 
 .. image:: https://img.shields.io/travis/ehutzle/docs2txt.svg
@@ -46,23 +46,36 @@
 * Free software: MIT license
 * Documentation: https://docs2txt.readthedocs.io.
 
 
 Features
 --------
 
-* TODO
+Rust
+^^^^
+- Download documentation from docs.rs and convert it into a plaintext file.
+
+Usage
+-----
+- Create a virtual environment and install the package ``python -m venv venv``
+- Install the package with ``pip install docs2txt``
+- Activate the virtual environment
+    - OSX / Linux: ``source venv/bin/activate``
+    - Windows: ``venv\Scripts\activate``
 
-Credits
--------
+- Run the program:
+    - ``python -m docs2txt``
 
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+Examples
+--------
+
+To download the documentation of the redb crate and save it to a folder on your desktop named "Rust Docs":
+
+- ``python -m docs2txt docs-rs --url https://docs.rs/redb/1.0.4/redb/ --output-dir '~/Desktop/Rust Docs'``
 
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
 0.1.0 (2023-07-09)
```

### Comparing `docs2txt-0.1.4/docs/Makefile` & `docs2txt-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.4/docs/conf.py` & `docs2txt-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.4/docs/installation.rst` & `docs2txt-0.1.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.4/docs/make.bat` & `docs2txt-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.4/docs2txt/__main__.py` & `docs2txt-0.1.5/docs2txt/__main__.py`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.4/docs2txt/docs_rs.py` & `docs2txt-0.1.5/docs2txt/docs_rs.py`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.4/docs2txt.egg-info/PKG-INFO` & `docs2txt-0.1.5/docs2txt.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs2txt
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple program to download documentation from docs.rs and convert it into a plaintext file.
 Home-page: https://github.com/ehutzle/docs2txt
 Author: Eric Richard
 Author-email: ehutzle@gmail.com
 License: MIT license
 Keywords: docs2txt
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =============
-rs-docs-2-txt
+docs2txt
 =============
 
 
 .. image:: https://img.shields.io/pypi/v/docs2txt.svg
         :target: https://pypi.python.org/pypi/docs2txt
 
 .. image:: https://img.shields.io/travis/ehutzle/docs2txt.svg
@@ -46,23 +46,36 @@
 * Free software: MIT license
 * Documentation: https://docs2txt.readthedocs.io.
 
 
 Features
 --------
 
-* TODO
+Rust
+^^^^
+- Download documentation from docs.rs and convert it into a plaintext file.
+
+Usage
+-----
+- Create a virtual environment and install the package ``python -m venv venv``
+- Install the package with ``pip install docs2txt``
+- Activate the virtual environment
+    - OSX / Linux: ``source venv/bin/activate``
+    - Windows: ``venv\Scripts\activate``
 
-Credits
--------
+- Run the program:
+    - ``python -m docs2txt``
 
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+Examples
+--------
+
+To download the documentation of the redb crate and save it to a folder on your desktop named "Rust Docs":
+
+- ``python -m docs2txt docs-rs --url https://docs.rs/redb/1.0.4/redb/ --output-dir '~/Desktop/Rust Docs'``
 
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
 0.1.0 (2023-07-09)
```

### Comparing `docs2txt-0.1.4/docs2txt.egg-info/SOURCES.txt` & `docs2txt-0.1.5/docs2txt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.4/setup.py` & `docs2txt-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `docs2txt-0.1.4/tests/test_docs2txt.py` & `docs2txt-0.1.5/tests/test_docs2txt.py`

 * *Files identical despite different names*

