# Comparing `tmp/pytest_flake8_path-1.4.0.tar.gz` & `tmp/pytest_flake8_path-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_flake8_path-1.4.0.tar", last modified: Fri Jun 16 14:18:07 2023, max compression
+gzip compressed data, was "pytest_flake8_path-1.5.0.tar", last modified: Mon Jul 10 14:50:51 2023, max compression
```

## Comparing `pytest_flake8_path-1.4.0.tar` & `pytest_flake8_path-1.5.0.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:18:07.274574 pytest_flake8_path-1.4.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      632 2023-06-16 14:18:05.000000 pytest_flake8_path-1.4.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:53.000000 pytest_flake8_path-1.4.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-20 12:10:00.000000 pytest_flake8_path-1.4.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     7456 2023-06-16 14:18:07.274631 pytest_flake8_path-1.4.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     6201 2023-06-16 14:15:41.000000 pytest_flake8_path-1.4.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-02-28 09:05:59.000000 pytest_flake8_path-1.4.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1456 2023-06-16 14:18:07.275042 pytest_flake8_path-1.4.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:18:07.272555 pytest_flake8_path-1.4.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:18:07.273550 pytest_flake8_path-1.4.0/src/pytest_flake8_path/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1839 2022-11-04 11:16:36.000000 pytest_flake8_path-1.4.0/src/pytest_flake8_path/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:53.000000 pytest_flake8_path-1.4.0/src/pytest_flake8_path/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:18:07.274361 pytest_flake8_path-1.4.0/src/pytest_flake8_path.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     7456 2023-06-16 14:18:07.000000 pytest_flake8_path-1.4.0/src/pytest_flake8_path.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      492 2023-06-16 14:18:07.000000 pytest_flake8_path-1.4.0/src/pytest_flake8_path.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 14:18:07.000000 pytest_flake8_path-1.4.0/src/pytest_flake8_path.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       44 2023-06-16 14:18:07.000000 pytest_flake8_path-1.4.0/src/pytest_flake8_path.egg-info/entry_points.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 14:18:07.000000 pytest_flake8_path-1.4.0/src/pytest_flake8_path.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       14 2023-06-16 14:18:07.000000 pytest_flake8_path-1.4.0/src/pytest_flake8_path.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       19 2023-06-16 14:18:07.000000 pytest_flake8_path-1.4.0/src/pytest_flake8_path.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:18:07.274473 pytest_flake8_path-1.4.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3396 2022-06-03 11:59:53.000000 pytest_flake8_path-1.4.0/tests/test_pytest_flake8_path.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 14:50:51.465253 pytest_flake8_path-1.5.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      699 2023-07-10 14:50:48.000000 pytest_flake8_path-1.5.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:53.000000 pytest_flake8_path-1.5.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      115 2023-07-10 14:19:32.000000 pytest_flake8_path-1.5.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     7406 2023-07-10 14:50:51.465323 pytest_flake8_path-1.5.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     6201 2023-07-10 14:19:03.000000 pytest_flake8_path-1.5.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-07-10 14:19:03.000000 pytest_flake8_path-1.5.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1417 2023-07-10 14:50:51.465618 pytest_flake8_path-1.5.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 14:50:51.462997 pytest_flake8_path-1.5.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 14:50:51.464239 pytest_flake8_path-1.5.0/src/pytest_flake8_path/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1839 2022-11-04 11:16:36.000000 pytest_flake8_path-1.5.0/src/pytest_flake8_path/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:53.000000 pytest_flake8_path-1.5.0/src/pytest_flake8_path/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 14:50:51.465141 pytest_flake8_path-1.5.0/src/pytest_flake8_path.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     7406 2023-07-10 14:50:51.000000 pytest_flake8_path-1.5.0/src/pytest_flake8_path.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      459 2023-07-10 14:50:51.000000 pytest_flake8_path-1.5.0/src/pytest_flake8_path.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 14:50:51.000000 pytest_flake8_path-1.5.0/src/pytest_flake8_path.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       44 2023-07-10 14:50:51.000000 pytest_flake8_path-1.5.0/src/pytest_flake8_path.egg-info/entry_points.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 14:50:51.000000 pytest_flake8_path-1.5.0/src/pytest_flake8_path.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       14 2023-07-10 14:50:51.000000 pytest_flake8_path-1.5.0/src/pytest_flake8_path.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       19 2023-07-10 14:50:51.000000 pytest_flake8_path-1.5.0/src/pytest_flake8_path.egg-info/top_level.txt
```

### Comparing `pytest_flake8_path-1.4.0/CHANGELOG.rst` & `pytest_flake8_path-1.5.0/CHANGELOG.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+1.5.0 (2023-07-10)
+------------------
+
+* Drop Python 3.7 support.
+
 1.4.0 (2023-06-16)
 ------------------
 
 * Support Python 3.12.
 
 1.3.0 (2022-05-11)
 ------------------
```

### Comparing `pytest_flake8_path-1.4.0/LICENSE` & `pytest_flake8_path-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_flake8_path-1.4.0/PKG-INFO` & `pytest_flake8_path-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_flake8_path
-Version: 1.4.0
+Version: 1.5.0
 Summary: A pytest fixture for testing flake8 plugins.
 Home-page: https://github.com/adamchainz/pytest-flake8-path
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/pytest-flake8-path/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -14,22 +14,21 @@
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
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
 
 ==================
 pytest-flake8-path
 ==================
 
@@ -66,15 +65,15 @@
 
 Use **pip**:
 
 .. code-block:: sh
 
     python -m pip install pytest-flake8-path
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 ----
 
 **Working on a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of ways to write faster, more accurate tests.
 
 ----
```

### Comparing `pytest_flake8_path-1.4.0/README.rst` & `pytest_flake8_path-1.5.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 Use **pip**:
 
 .. code-block:: sh
 
     python -m pip install pytest-flake8-path
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 ----
 
 **Working on a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of ways to write faster, more accurate tests.
 
 ----
```

### Comparing `pytest_flake8_path-1.4.0/setup.cfg` & `pytest_flake8_path-1.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pytest_flake8_path
-version = 1.4.0
+version = 1.5.0
 description = A pytest fixture for testing flake8 plugins.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/pytest-flake8-path
 author = Adam Johnson
 author_email = me@adamj.eu
 license = MIT
@@ -14,15 +14,14 @@
 	Framework :: Pytest
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 	Typing :: Typed
 keywords = pytest, flake8
@@ -32,15 +31,15 @@
 	Twitter = https://twitter.com/adamchainz
 
 [options]
 packages = find:
 install_requires = 
 	flake8
 	pytest
-python_requires = >=3.7
+python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 zip_safe = False
 
 [options.packages.find]
 where = src
```

### Comparing `pytest_flake8_path-1.4.0/src/pytest_flake8_path/__init__.py` & `pytest_flake8_path-1.5.0/src/pytest_flake8_path/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_flake8_path-1.4.0/src/pytest_flake8_path.egg-info/PKG-INFO` & `pytest_flake8_path-1.5.0/src/pytest_flake8_path.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-flake8-path
-Version: 1.4.0
+Version: 1.5.0
 Summary: A pytest fixture for testing flake8 plugins.
 Home-page: https://github.com/adamchainz/pytest-flake8-path
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/pytest-flake8-path/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -14,22 +14,21 @@
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
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
 
 ==================
 pytest-flake8-path
 ==================
 
@@ -66,15 +65,15 @@
 
 Use **pip**:
 
 .. code-block:: sh
 
     python -m pip install pytest-flake8-path
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 ----
 
 **Working on a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of ways to write faster, more accurate tests.
 
 ----
```

