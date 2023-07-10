# Comparing `tmp/pytest_restrict-4.5.0.tar.gz` & `tmp/pytest_restrict-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_restrict-4.5.0.tar", last modified: Fri Jun 16 15:00:58 2023, max compression
+gzip compressed data, was "pytest_restrict-4.6.0.tar", last modified: Mon Jul 10 15:06:03 2023, max compression
```

## Comparing `pytest_restrict-4.5.0.tar` & `pytest_restrict-4.6.0.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:00:58.009623 pytest_restrict-4.5.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2051 2023-06-16 15:00:55.000000 pytest_restrict-4.5.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:57.000000 pytest_restrict-4.5.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-20 12:10:02.000000 pytest_restrict-4.5.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4252 2023-06-16 15:00:58.009684 pytest_restrict-4.5.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3041 2023-06-16 15:00:53.000000 pytest_restrict-4.5.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-02-28 09:06:03.000000 pytest_restrict-4.5.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1432 2023-06-16 15:00:58.009943 pytest_restrict-4.5.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:00:58.007228 pytest_restrict-4.5.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:00:58.008465 pytest_restrict-4.5.0/src/pytest_restrict/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1831 2022-06-03 11:59:58.000000 pytest_restrict-4.5.0/src/pytest_restrict/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:58.000000 pytest_restrict-4.5.0/src/pytest_restrict/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:00:58.009292 pytest_restrict-4.5.0/src/pytest_restrict.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4252 2023-06-16 15:00:58.000000 pytest_restrict-4.5.0/src/pytest_restrict.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      462 2023-06-16 15:00:58.000000 pytest_restrict-4.5.0/src/pytest_restrict.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 15:00:58.000000 pytest_restrict-4.5.0/src/pytest_restrict.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       38 2023-06-16 15:00:58.000000 pytest_restrict-4.5.0/src/pytest_restrict.egg-info/entry_points.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 15:00:57.000000 pytest_restrict-4.5.0/src/pytest_restrict.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       28 2023-06-16 15:00:58.000000 pytest_restrict-4.5.0/src/pytest_restrict.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       16 2023-06-16 15:00:58.000000 pytest_restrict-4.5.0/src/pytest_restrict.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:00:58.009419 pytest_restrict-4.5.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3182 2022-06-03 11:59:58.000000 pytest_restrict-4.5.0/tests/test_pytest_restrict.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 15:06:03.077491 pytest_restrict-4.6.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2118 2023-07-10 15:06:00.000000 pytest_restrict-4.6.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:57.000000 pytest_restrict-4.6.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      115 2023-07-10 14:57:50.000000 pytest_restrict-4.6.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4202 2023-07-10 15:06:03.077552 pytest_restrict-4.6.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3041 2023-07-10 14:55:35.000000 pytest_restrict-4.6.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-07-10 14:55:35.000000 pytest_restrict-4.6.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1393 2023-07-10 15:06:03.077798 pytest_restrict-4.6.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 15:06:03.075438 pytest_restrict-4.6.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 15:06:03.076584 pytest_restrict-4.6.0/src/pytest_restrict/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1831 2022-06-03 11:59:58.000000 pytest_restrict-4.6.0/src/pytest_restrict/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:58.000000 pytest_restrict-4.6.0/src/pytest_restrict/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 15:06:03.077387 pytest_restrict-4.6.0/src/pytest_restrict.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4202 2023-07-10 15:06:03.000000 pytest_restrict-4.6.0/src/pytest_restrict.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      432 2023-07-10 15:06:03.000000 pytest_restrict-4.6.0/src/pytest_restrict.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 15:06:03.000000 pytest_restrict-4.6.0/src/pytest_restrict.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       38 2023-07-10 15:06:03.000000 pytest_restrict-4.6.0/src/pytest_restrict.egg-info/entry_points.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 15:06:02.000000 pytest_restrict-4.6.0/src/pytest_restrict.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       28 2023-07-10 15:06:03.000000 pytest_restrict-4.6.0/src/pytest_restrict.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       16 2023-07-10 15:06:03.000000 pytest_restrict-4.6.0/src/pytest_restrict.egg-info/top_level.txt
```

### Comparing `pytest_restrict-4.5.0/CHANGELOG.rst` & `pytest_restrict-4.6.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+4.6.0 (2023-07-10)
+------------------
+
+* Drop Python 3.7 support.
+
 4.5.0 (2023-06-16)
 ------------------
 
 * Support Python 3.12.
 
 4.4.0 (2022-05-11)
 ------------------
```

### Comparing `pytest_restrict-4.5.0/LICENSE` & `pytest_restrict-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_restrict-4.5.0/PKG-INFO` & `pytest_restrict-4.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_restrict
-Version: 4.5.0
+Version: 4.6.0
 Summary: Pytest plugin to restrict the test types allowed
 Home-page: https://github.com/adamchainz/pytest-restrict
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/pytest-restrict/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -13,22 +13,21 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
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
 
 ===============
 pytest-restrict
 ===============
 
@@ -58,15 +57,15 @@
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install pytest-restrict
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 ----
 
 **Testing a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of ways to write faster, more accurate tests.
 
 ----
```

### Comparing `pytest_restrict-4.5.0/README.rst` & `pytest_restrict-4.6.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install pytest-restrict
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 ----
 
 **Testing a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of ways to write faster, more accurate tests.
 
 ----
```

### Comparing `pytest_restrict-4.5.0/setup.cfg` & `pytest_restrict-4.6.0/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pytest_restrict
-version = 4.5.0
+version = 4.6.0
 description = Pytest plugin to restrict the test types allowed
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/pytest-restrict
 author = Adam Johnson
 author_email = me@adamj.eu
 license = MIT
@@ -13,15 +13,14 @@
 	Development Status :: 5 - Production/Stable
 	Framework :: Pytest
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
 keywords = pytest, restrict, class
@@ -31,15 +30,15 @@
 	Twitter = https://twitter.com/adamchainz
 
 [options]
 packages = find:
 install_requires = 
 	pkgutil-resolve-name
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

### Comparing `pytest_restrict-4.5.0/src/pytest_restrict/__init__.py` & `pytest_restrict-4.6.0/src/pytest_restrict/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_restrict-4.5.0/src/pytest_restrict.egg-info/PKG-INFO` & `pytest_restrict-4.6.0/src/pytest_restrict.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-restrict
-Version: 4.5.0
+Version: 4.6.0
 Summary: Pytest plugin to restrict the test types allowed
 Home-page: https://github.com/adamchainz/pytest-restrict
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/pytest-restrict/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -13,22 +13,21 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
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
 
 ===============
 pytest-restrict
 ===============
 
@@ -58,15 +57,15 @@
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install pytest-restrict
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 ----
 
 **Testing a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of ways to write faster, more accurate tests.
 
 ----
```

