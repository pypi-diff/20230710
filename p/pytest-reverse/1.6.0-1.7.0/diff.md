# Comparing `tmp/pytest_reverse-1.6.0.tar.gz` & `tmp/pytest_reverse-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_reverse-1.6.0.tar", last modified: Fri Jun 16 15:00:42 2023, max compression
+gzip compressed data, was "pytest_reverse-1.7.0.tar", last modified: Mon Jul 10 15:18:11 2023, max compression
```

## Comparing `pytest_reverse-1.6.0.tar` & `pytest_reverse-1.7.0.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:00:42.199378 pytest_reverse-1.6.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      987 2023-06-16 15:00:39.000000 pytest_reverse-1.6.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:58.000000 pytest_reverse-1.6.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-20 12:10:02.000000 pytest_reverse-1.6.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3474 2023-06-16 15:00:42.199431 pytest_reverse-1.6.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2285 2023-06-16 15:00:38.000000 pytest_reverse-1.6.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-02-28 09:06:03.000000 pytest_reverse-1.6.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1385 2023-06-16 15:00:42.199678 pytest_reverse-1.6.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:00:42.197131 pytest_reverse-1.6.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:00:42.198256 pytest_reverse-1.6.0/src/pytest_reverse/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      739 2022-08-11 14:03:14.000000 pytest_reverse-1.6.0/src/pytest_reverse/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:58.000000 pytest_reverse-1.6.0/src/pytest_reverse/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:00:42.199028 pytest_reverse-1.6.0/src/pytest_reverse.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3474 2023-06-16 15:00:42.000000 pytest_reverse-1.6.0/src/pytest_reverse.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      452 2023-06-16 15:00:42.000000 pytest_reverse-1.6.0/src/pytest_reverse.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 15:00:42.000000 pytest_reverse-1.6.0/src/pytest_reverse.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       36 2023-06-16 15:00:42.000000 pytest_reverse-1.6.0/src/pytest_reverse.egg-info/entry_points.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 15:00:42.000000 pytest_reverse-1.6.0/src/pytest_reverse.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)        7 2023-06-16 15:00:42.000000 pytest_reverse-1.6.0/src/pytest_reverse.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       15 2023-06-16 15:00:42.000000 pytest_reverse-1.6.0/src/pytest_reverse.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:00:42.199139 pytest_reverse-1.6.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1801 2023-04-23 08:24:26.000000 pytest_reverse-1.6.0/tests/test_pytest_reverse.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 15:18:11.292708 pytest_reverse-1.7.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1054 2023-07-10 15:18:09.000000 pytest_reverse-1.7.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:58.000000 pytest_reverse-1.7.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      115 2023-07-10 15:11:25.000000 pytest_reverse-1.7.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3424 2023-07-10 15:18:11.292764 pytest_reverse-1.7.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2285 2023-07-10 15:11:20.000000 pytest_reverse-1.7.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-07-10 15:11:20.000000 pytest_reverse-1.7.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1346 2023-07-10 15:18:11.293031 pytest_reverse-1.7.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 15:18:11.290517 pytest_reverse-1.7.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 15:18:11.291755 pytest_reverse-1.7.0/src/pytest_reverse/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      739 2022-08-11 14:03:14.000000 pytest_reverse-1.7.0/src/pytest_reverse/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:58.000000 pytest_reverse-1.7.0/src/pytest_reverse/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 15:18:11.292605 pytest_reverse-1.7.0/src/pytest_reverse.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3424 2023-07-10 15:18:11.000000 pytest_reverse-1.7.0/src/pytest_reverse.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      423 2023-07-10 15:18:11.000000 pytest_reverse-1.7.0/src/pytest_reverse.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 15:18:11.000000 pytest_reverse-1.7.0/src/pytest_reverse.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       36 2023-07-10 15:18:11.000000 pytest_reverse-1.7.0/src/pytest_reverse.egg-info/entry_points.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 15:18:11.000000 pytest_reverse-1.7.0/src/pytest_reverse.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        7 2023-07-10 15:18:11.000000 pytest_reverse-1.7.0/src/pytest_reverse.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       15 2023-07-10 15:18:11.000000 pytest_reverse-1.7.0/src/pytest_reverse.egg-info/top_level.txt
```

### Comparing `pytest_reverse-1.6.0/CHANGELOG.rst` & `pytest_reverse-1.7.0/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+1.7.0 (2023-07-10)
+------------------
+
+* Drop Python 3.7 support.
+
 1.6.0 (2023-06-16)
 ------------------
 
 * Support Python 3.12.
 
 1.5.0 (2022-05-11)
 ------------------
```

### Comparing `pytest_reverse-1.6.0/LICENSE` & `pytest_reverse-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_reverse-1.6.0/PKG-INFO` & `pytest_reverse-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_reverse
-Version: 1.6.0
+Version: 1.7.0
 Summary: Pytest plugin to reverse test order.
 Home-page: https://github.com/adamchainz/pytest-reverse
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/pytest-reverse/blob/main/CHANGELOG.rst
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
 
 ==============
 pytest-reverse
 ==============
 
@@ -52,15 +51,15 @@
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install pytest-reverse
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 ----
 
 **Testing a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of recommendations to write faster, more accurate tests.
 I created pytest-reverse whilst working on the book!
```

### Comparing `pytest_reverse-1.6.0/README.rst` & `pytest_reverse-1.7.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install pytest-reverse
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 ----
 
 **Testing a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of recommendations to write faster, more accurate tests.
 I created pytest-reverse whilst working on the book!
```

### Comparing `pytest_reverse-1.6.0/setup.cfg` & `pytest_reverse-1.7.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pytest_reverse
-version = 1.6.0
+version = 1.7.0
 description = Pytest plugin to reverse test order.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/pytest-reverse
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
 keywords = pytest, reverse
@@ -30,15 +29,15 @@
 	Mastodon = https://fosstodon.org/@adamchainz
 	Twitter = https://twitter.com/adamchainz
 
 [options]
 packages = find:
 install_requires = 
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

### Comparing `pytest_reverse-1.6.0/src/pytest_reverse/__init__.py` & `pytest_reverse-1.7.0/src/pytest_reverse/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_reverse-1.6.0/src/pytest_reverse.egg-info/PKG-INFO` & `pytest_reverse-1.7.0/src/pytest_reverse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-reverse
-Version: 1.6.0
+Version: 1.7.0
 Summary: Pytest plugin to reverse test order.
 Home-page: https://github.com/adamchainz/pytest-reverse
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/pytest-reverse/blob/main/CHANGELOG.rst
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
 
 ==============
 pytest-reverse
 ==============
 
@@ -52,15 +51,15 @@
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install pytest-reverse
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 ----
 
 **Testing a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of recommendations to write faster, more accurate tests.
 I created pytest-reverse whilst working on the book!
```

