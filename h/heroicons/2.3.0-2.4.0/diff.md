# Comparing `tmp/heroicons-2.3.0.tar.gz` & `tmp/heroicons-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heroicons-2.3.0.tar", last modified: Fri Jun 16 14:45:37 2023, max compression
+gzip compressed data, was "heroicons-2.4.0.tar", last modified: Mon Jul 10 14:04:32 2023, max compression
```

## Comparing `heroicons-2.3.0.tar` & `heroicons-2.4.0.tar`

### file list

```diff
@@ -1,32 +1,27 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:45:37.825495 heroicons-2.3.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3962 2023-06-16 14:45:35.000000 heroicons-2.3.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2202 2022-06-03 11:59:28.000000 heroicons-2.3.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      139 2023-01-20 12:10:00.000000 heroicons-2.3.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     9524 2023-06-16 14:45:37.825578 heroicons-2.3.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     8051 2023-06-16 14:25:05.000000 heroicons-2.3.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-02-28 09:05:58.000000 heroicons-2.3.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1718 2023-06-16 14:45:37.825921 heroicons-2.3.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:45:37.814854 heroicons-2.3.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:45:37.818177 heroicons-2.3.0/src/heroicons/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2014 2022-11-04 11:16:34.000000 heroicons-2.3.0/src/heroicons/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      144 2022-10-05 11:03:02.000000 heroicons-2.3.0/src/heroicons/__main__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      595 2022-06-03 11:59:31.000000 heroicons-2.3.0/src/heroicons/_compat.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     6936 2022-10-05 15:25:33.000000 heroicons-2.3.0/src/heroicons/cli.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)   370575 2023-04-14 10:39:21.000000 heroicons-2.3.0/src/heroicons/heroicons.zip
--rw-r--r--   0 adamjohnson   (501) staff       (20)      660 2022-10-07 15:01:47.000000 heroicons-2.3.0/src/heroicons/jinja.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:31.000000 heroicons-2.3.0/src/heroicons/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:45:37.824886 heroicons-2.3.0/src/heroicons/templatetags/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:31.000000 heroicons-2.3.0/src/heroicons/templatetags/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1180 2022-11-04 11:16:34.000000 heroicons-2.3.0/src/heroicons/templatetags/heroicons.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:45:37.824617 heroicons-2.3.0/src/heroicons.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     9524 2023-06-16 14:45:37.000000 heroicons-2.3.0/src/heroicons.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      623 2023-06-16 14:45:37.000000 heroicons-2.3.0/src/heroicons.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 14:45:37.000000 heroicons-2.3.0/src/heroicons.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 14:45:37.000000 heroicons-2.3.0/src/heroicons.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       43 2023-06-16 14:45:37.000000 heroicons-2.3.0/src/heroicons.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       10 2023-06-16 14:45:37.000000 heroicons-2.3.0/src/heroicons.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:45:37.825384 heroicons-2.3.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     7460 2022-10-05 15:25:33.000000 heroicons-2.3.0/tests/test_cli.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)    13878 2022-11-04 11:16:34.000000 heroicons-2.3.0/tests/test_django.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      924 2022-10-05 09:36:11.000000 heroicons-2.3.0/tests/test_heroicons.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)    13950 2022-11-04 11:16:34.000000 heroicons-2.3.0/tests/test_jinja.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 14:04:32.085624 heroicons-2.4.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4029 2023-07-10 14:04:29.000000 heroicons-2.4.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2202 2022-06-03 11:59:28.000000 heroicons-2.4.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      151 2023-07-10 13:58:32.000000 heroicons-2.4.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     9474 2023-07-10 14:04:32.085692 heroicons-2.4.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     8051 2023-07-10 14:03:14.000000 heroicons-2.4.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-07-10 14:03:14.000000 heroicons-2.4.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1679 2023-07-10 14:04:32.085983 heroicons-2.4.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 14:04:32.080431 heroicons-2.4.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 14:04:32.084562 heroicons-2.4.0/src/heroicons/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2014 2022-11-04 11:16:34.000000 heroicons-2.4.0/src/heroicons/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      144 2022-10-05 11:03:02.000000 heroicons-2.4.0/src/heroicons/__main__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      595 2022-06-03 11:59:31.000000 heroicons-2.4.0/src/heroicons/_compat.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     6936 2022-10-05 15:25:33.000000 heroicons-2.4.0/src/heroicons/cli.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)   370575 2023-04-14 10:39:21.000000 heroicons-2.4.0/src/heroicons/heroicons.zip
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      660 2022-10-07 15:01:47.000000 heroicons-2.4.0/src/heroicons/jinja.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:31.000000 heroicons-2.4.0/src/heroicons/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 14:04:32.085405 heroicons-2.4.0/src/heroicons/templatetags/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:31.000000 heroicons-2.4.0/src/heroicons/templatetags/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1180 2022-11-04 11:16:34.000000 heroicons-2.4.0/src/heroicons/templatetags/heroicons.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 14:04:32.085196 heroicons-2.4.0/src/heroicons.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     9474 2023-07-10 14:04:32.000000 heroicons-2.4.0/src/heroicons.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      540 2023-07-10 14:04:32.000000 heroicons-2.4.0/src/heroicons.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 14:04:32.000000 heroicons-2.4.0/src/heroicons.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 14:04:31.000000 heroicons-2.4.0/src/heroicons.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       43 2023-07-10 14:04:32.000000 heroicons-2.4.0/src/heroicons.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       10 2023-07-10 14:04:32.000000 heroicons-2.4.0/src/heroicons.egg-info/top_level.txt
```

### Comparing `heroicons-2.3.0/CHANGELOG.rst` & `heroicons-2.4.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+2.4.0 (2023-07-10)
+------------------
+
+* Drop Python 3.7 support.
+
 2.3.0 (2023-06-16)
 ------------------
 
 * Support Python 3.12.
 
 2.2.0 (2023-02-25)
 ------------------
```

### Comparing `heroicons-2.3.0/LICENSE` & `heroicons-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heroicons-2.3.0/PKG-INFO` & `heroicons-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heroicons
-Version: 2.3.0
+Version: 2.4.0
 Summary: Use heroicons in your Django and Jinja templates.
 Home-page: https://github.com/adamchainz/heroicons
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/heroicons/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -17,23 +17,22 @@
 Classifier: Framework :: Django :: 4.2
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
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: django
 Provides-Extra: jinja
 License-File: LICENSE
 
 =========
 heroicons
@@ -56,15 +55,15 @@
    :alt: pre-commit
 
 Use `heroicons <https://heroicons.com/>`__ in your Django and Jinja templates.
 
 Requirements
 ------------
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 ----
 
 **Working on a Django project?**
 Improve your skills with `one of my books <https://adamj.eu/books/>`__.
```

### Comparing `heroicons-2.3.0/README.rst` & `heroicons-2.4.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
    :alt: pre-commit
 
 Use `heroicons <https://heroicons.com/>`__ in your Django and Jinja templates.
 
 Requirements
 ------------
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 ----
 
 **Working on a Django project?**
 Improve your skills with `one of my books <https://adamj.eu/books/>`__.
```

### Comparing `heroicons-2.3.0/setup.cfg` & `heroicons-2.4.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = heroicons
-version = 2.3.0
+version = 2.4.0
 description = Use heroicons in your Django and Jinja templates.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/heroicons
 author = Adam Johnson
 author_email = me@adamj.eu
 license = MIT
@@ -17,15 +17,14 @@
 	Framework :: Django :: 4.2
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
 	Programming Language :: Python :: Implementation :: CPython
 	Typing :: Typed
@@ -33,15 +32,15 @@
 project_urls = 
 	Changelog = https://github.com/adamchainz/heroicons/blob/main/CHANGELOG.rst
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

### Comparing `heroicons-2.3.0/src/heroicons/__init__.py` & `heroicons-2.4.0/src/heroicons/__init__.py`

 * *Files identical despite different names*

### Comparing `heroicons-2.3.0/src/heroicons/_compat.py` & `heroicons-2.4.0/src/heroicons/_compat.py`

 * *Files identical despite different names*

### Comparing `heroicons-2.3.0/src/heroicons/cli.py` & `heroicons-2.4.0/src/heroicons/cli.py`

 * *Files identical despite different names*

### Comparing `heroicons-2.3.0/src/heroicons/heroicons.zip` & `heroicons-2.4.0/src/heroicons/heroicons.zip`

 * *Files identical despite different names*

### Comparing `heroicons-2.3.0/src/heroicons/jinja.py` & `heroicons-2.4.0/src/heroicons/jinja.py`

 * *Files identical despite different names*

### Comparing `heroicons-2.3.0/src/heroicons/templatetags/heroicons.py` & `heroicons-2.4.0/src/heroicons/templatetags/heroicons.py`

 * *Files identical despite different names*

### Comparing `heroicons-2.3.0/src/heroicons.egg-info/PKG-INFO` & `heroicons-2.4.0/src/heroicons.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heroicons
-Version: 2.3.0
+Version: 2.4.0
 Summary: Use heroicons in your Django and Jinja templates.
 Home-page: https://github.com/adamchainz/heroicons
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/heroicons/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -17,23 +17,22 @@
 Classifier: Framework :: Django :: 4.2
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
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: django
 Provides-Extra: jinja
 License-File: LICENSE
 
 =========
 heroicons
@@ -56,15 +55,15 @@
    :alt: pre-commit
 
 Use `heroicons <https://heroicons.com/>`__ in your Django and Jinja templates.
 
 Requirements
 ------------
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 ----
 
 **Working on a Django project?**
 Improve your skills with `one of my books <https://adamj.eu/books/>`__.
```

### Comparing `heroicons-2.3.0/src/heroicons.egg-info/SOURCES.txt` & `heroicons-2.4.0/src/heroicons.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -14,12 +14,8 @@
 src/heroicons.egg-info/PKG-INFO
 src/heroicons.egg-info/SOURCES.txt
 src/heroicons.egg-info/dependency_links.txt
 src/heroicons.egg-info/not-zip-safe
 src/heroicons.egg-info/requires.txt
 src/heroicons.egg-info/top_level.txt
 src/heroicons/templatetags/__init__.py
-src/heroicons/templatetags/heroicons.py
-tests/test_cli.py
-tests/test_django.py
-tests/test_heroicons.py
-tests/test_jinja.py
+src/heroicons/templatetags/heroicons.py
```

