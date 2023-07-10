# Comparing `tmp/pytest_is_running-1.4.0.tar.gz` & `tmp/pytest_is_running-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_is_running-1.4.0.tar", last modified: Fri Jun 16 15:01:14 2023, max compression
+gzip compressed data, was "pytest_is_running-1.5.0.tar", last modified: Mon Jul 10 15:02:03 2023, max compression
```

## Comparing `pytest_is_running-1.4.0.tar` & `pytest_is_running-1.5.0.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:01:14.586911 pytest_is_running-1.4.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      470 2023-06-16 15:01:12.000000 pytest_is_running-1.4.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:54.000000 pytest_is_running-1.4.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-20 12:10:00.000000 pytest_is_running-1.4.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3971 2023-06-16 15:01:14.586988 pytest_is_running-1.4.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2752 2023-06-16 15:01:10.000000 pytest_is_running-1.4.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-02-28 09:05:59.000000 pytest_is_running-1.4.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1647 2023-06-16 15:01:14.587290 pytest_is_running-1.4.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:01:14.584056 pytest_is_running-1.4.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:01:14.585823 pytest_is_running-1.4.0/src/pytest_is_running/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      107 2022-06-03 11:59:54.000000 pytest_is_running-1.4.0/src/pytest_is_running/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      339 2022-08-11 14:02:01.000000 pytest_is_running-1.4.0/src/pytest_is_running/plugin.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:54.000000 pytest_is_running-1.4.0/src/pytest_is_running/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:01:14.586571 pytest_is_running-1.4.0/src/pytest_is_running.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3971 2023-06-16 15:01:14.000000 pytest_is_running-1.4.0/src/pytest_is_running.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      470 2023-06-16 15:01:14.000000 pytest_is_running-1.4.0/src/pytest_is_running.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 15:01:14.000000 pytest_is_running-1.4.0/src/pytest_is_running.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       49 2023-06-16 15:01:14.000000 pytest_is_running-1.4.0/src/pytest_is_running.egg-info/entry_points.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 15:01:14.000000 pytest_is_running-1.4.0/src/pytest_is_running.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       18 2023-06-16 15:01:14.000000 pytest_is_running-1.4.0/src/pytest_is_running.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:01:14.586686 pytest_is_running-1.4.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2735 2022-11-04 11:16:37.000000 pytest_is_running-1.4.0/tests/test_pytest_is_running.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 15:02:03.288912 pytest_is_running-1.5.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      537 2023-07-10 15:02:01.000000 pytest_is_running-1.5.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:54.000000 pytest_is_running-1.5.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      115 2023-07-10 15:00:08.000000 pytest_is_running-1.5.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3921 2023-07-10 15:02:03.288976 pytest_is_running-1.5.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2752 2023-07-10 15:00:01.000000 pytest_is_running-1.5.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-07-10 15:00:01.000000 pytest_is_running-1.5.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1608 2023-07-10 15:02:03.289276 pytest_is_running-1.5.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 15:02:03.286399 pytest_is_running-1.5.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 15:02:03.287956 pytest_is_running-1.5.0/src/pytest_is_running/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      107 2022-06-03 11:59:54.000000 pytest_is_running-1.5.0/src/pytest_is_running/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      339 2022-08-11 14:02:01.000000 pytest_is_running-1.5.0/src/pytest_is_running/plugin.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:54.000000 pytest_is_running-1.5.0/src/pytest_is_running/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 15:02:03.288794 pytest_is_running-1.5.0/src/pytest_is_running.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3921 2023-07-10 15:02:03.000000 pytest_is_running-1.5.0/src/pytest_is_running.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      438 2023-07-10 15:02:03.000000 pytest_is_running-1.5.0/src/pytest_is_running.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 15:02:03.000000 pytest_is_running-1.5.0/src/pytest_is_running.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       49 2023-07-10 15:02:03.000000 pytest_is_running-1.5.0/src/pytest_is_running.egg-info/entry_points.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 15:02:03.000000 pytest_is_running-1.5.0/src/pytest_is_running.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       18 2023-07-10 15:02:03.000000 pytest_is_running-1.5.0/src/pytest_is_running.egg-info/top_level.txt
```

### Comparing `pytest_is_running-1.4.0/LICENSE` & `pytest_is_running-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_is_running-1.4.0/PKG-INFO` & `pytest_is_running-1.5.0/src/pytest_is_running.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pytest_is_running
-Version: 1.4.0
+Name: pytest-is-running
+Version: 1.5.0
 Summary: pytest plugin providing a function to check if pytest is running.
 Home-page: https://github.com/adamchainz/pytest-is-running
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/pytest-is-running/blob/main/CHANGELOG.rst
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
 
 =================
 pytest-is-running
 =================
 
@@ -55,15 +54,15 @@
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install pytest-is-running
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 ----
 
 **Working on a Django project?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
 I created pytest-is-running whilst working on the book!
```

### Comparing `pytest_is_running-1.4.0/README.rst` & `pytest_is_running-1.5.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install pytest-is-running
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 ----
 
 **Working on a Django project?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
 I created pytest-is-running whilst working on the book!
```

### Comparing `pytest_is_running-1.4.0/setup.cfg` & `pytest_is_running-1.5.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pytest_is_running
-version = 1.4.0
+version = 1.5.0
 description = pytest plugin providing a function to check if pytest is running.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/pytest-is-running
 author = Adam Johnson
 author_email = me@adamj.eu
 license = MIT
@@ -13,30 +13,29 @@
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
 keywords = pytest
 project_urls = 
 	Changelog = https://github.com/adamchainz/pytest-is-running/blob/main/CHANGELOG.rst
 	Mastodon = https://fosstodon.org/@adamchainz
 	Twitter = https://twitter.com/adamchainz
 
 [options]
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 zip_safe = False
 
 [options.packages.find]
 where = src
```

### Comparing `pytest_is_running-1.4.0/src/pytest_is_running.egg-info/PKG-INFO` & `pytest_is_running-1.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pytest-is-running
-Version: 1.4.0
+Name: pytest_is_running
+Version: 1.5.0
 Summary: pytest plugin providing a function to check if pytest is running.
 Home-page: https://github.com/adamchainz/pytest-is-running
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/pytest-is-running/blob/main/CHANGELOG.rst
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
 
 =================
 pytest-is-running
 =================
 
@@ -55,15 +54,15 @@
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install pytest-is-running
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 ----
 
 **Working on a Django project?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
 I created pytest-is-running whilst working on the book!
```

