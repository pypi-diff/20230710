# Comparing `tmp/django_rich-1.6.0.tar.gz` & `tmp/django_rich-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_rich-1.6.0.tar", last modified: Wed Jun 14 14:56:41 2023, max compression
+gzip compressed data, was "django_rich-1.7.0.tar", last modified: Mon Jul 10 12:34:48 2023, max compression
```

## Comparing `django_rich-1.6.0.tar` & `django_rich-1.7.0.tar`

### file list

```diff
@@ -1,26 +1,23 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 14:56:41.812113 django_rich-1.6.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      683 2023-06-14 14:56:39.000000 django_rich-1.6.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:58:55.000000 django_rich-1.6.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      121 2023-01-20 12:09:58.000000 django_rich-1.6.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     6747 2023-06-14 14:56:41.812180 django_rich-1.6.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     5330 2023-06-14 14:50:29.000000 django_rich-1.6.0/README.rst
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 14:56:41.808486 django_rich-1.6.0/img/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    51489 2022-06-03 11:58:59.000000 django_rich-1.6.0/img/RichRunner.png
--rw-r--r--   0 adamjohnson   (501) staff       (20)      500 2023-02-28 09:05:55.000000 django_rich-1.6.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1685 2023-06-14 14:56:41.812486 django_rich-1.6.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 14:56:41.807617 django_rich-1.6.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 14:56:41.809971 django_rich-1.6.0/src/django_rich/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:59.000000 django_rich-1.6.0/src/django_rich/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1609 2023-02-02 16:02:04.000000 django_rich-1.6.0/src/django_rich/management.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:59.000000 django_rich-1.6.0/src/django_rich/py.typed
--rw-r--r--   0 adamjohnson   (501) staff       (20)     6240 2022-11-08 22:22:18.000000 django_rich-1.6.0/src/django_rich/test.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 14:56:41.811201 django_rich-1.6.0/src/django_rich.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     6747 2023-06-14 14:56:41.000000 django_rich-1.6.0/src/django_rich.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      471 2023-06-14 14:56:41.000000 django_rich-1.6.0/src/django_rich.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-14 14:56:41.000000 django_rich-1.6.0/src/django_rich.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-14 14:56:41.000000 django_rich-1.6.0/src/django_rich.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       25 2023-06-14 14:56:41.000000 django_rich-1.6.0/src/django_rich.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2023-06-14 14:56:41.000000 django_rich-1.6.0/src/django_rich.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 14:56:41.811694 django_rich-1.6.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2947 2023-02-02 15:54:25.000000 django_rich-1.6.0/tests/test_management.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)    17316 2023-02-02 15:54:25.000000 django_rich-1.6.0/tests/test_test.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 12:34:48.059162 django_rich-1.7.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      750 2023-07-10 12:34:45.000000 django_rich-1.7.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:58:55.000000 django_rich-1.7.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      133 2023-07-10 09:17:51.000000 django_rich-1.7.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     6697 2023-07-10 12:34:48.059241 django_rich-1.7.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     5330 2023-07-10 12:31:19.000000 django_rich-1.7.0/README.rst
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 12:34:48.054251 django_rich-1.7.0/img/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    51489 2022-06-03 11:58:59.000000 django_rich-1.7.0/img/RichRunner.png
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      500 2023-07-10 12:31:19.000000 django_rich-1.7.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1646 2023-07-10 12:34:48.059579 django_rich-1.7.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 12:34:48.053331 django_rich-1.7.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 12:34:48.055938 django_rich-1.7.0/src/django_rich/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:59.000000 django_rich-1.7.0/src/django_rich/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1609 2023-02-02 16:02:04.000000 django_rich-1.7.0/src/django_rich/management.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:59.000000 django_rich-1.7.0/src/django_rich/py.typed
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     6240 2022-11-08 22:22:18.000000 django_rich-1.7.0/src/django_rich/test.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 12:34:48.059055 django_rich-1.7.0/src/django_rich.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     6697 2023-07-10 12:34:48.000000 django_rich-1.7.0/src/django_rich.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      427 2023-07-10 12:34:48.000000 django_rich-1.7.0/src/django_rich.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 12:34:48.000000 django_rich-1.7.0/src/django_rich.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 12:34:47.000000 django_rich-1.7.0/src/django_rich.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       25 2023-07-10 12:34:48.000000 django_rich-1.7.0/src/django_rich.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2023-07-10 12:34:48.000000 django_rich-1.7.0/src/django_rich.egg-info/top_level.txt
```

### Comparing `django_rich-1.6.0/CHANGELOG.rst` & `django_rich-1.7.0/CHANGELOG.rst`

 * *Files 15% similar despite different names*

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
 1.6.0 (2023-06-14)
 ------------------
 
 * Support Python 3.12.
 
 1.5.0 (2023-02-25)
 ------------------
```

### Comparing `django_rich-1.6.0/LICENSE` & `django_rich-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_rich-1.6.0/PKG-INFO` & `django_rich-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_rich
-Version: 1.6.0
+Version: 1.7.0
 Summary: Extensions for using Rich with Django.
 Home-page: https://github.com/adamchainz/django-rich
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-rich/blob/main/CHANGELOG.rst
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
 License-File: LICENSE
 
 ===========
 django-rich
 ===========
 
@@ -54,15 +53,15 @@
    :alt: pre-commit
 
 Extensions for using `Rich <https://rich.readthedocs.io/>`__ with Django.
 
 Requirements
 ------------
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 ----
 
 **Want to work smarter and faster?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
```

### Comparing `django_rich-1.6.0/README.rst` & `django_rich-1.7.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
    :alt: pre-commit
 
 Extensions for using `Rich <https://rich.readthedocs.io/>`__ with Django.
 
 Requirements
 ------------
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 ----
 
 **Want to work smarter and faster?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
```

### Comparing `django_rich-1.6.0/img/RichRunner.png` & `django_rich-1.7.0/img/RichRunner.png`

 * *Files identical despite different names*

### Comparing `django_rich-1.6.0/setup.cfg` & `django_rich-1.7.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_rich
-version = 1.6.0
+version = 1.7.0
 description = Extensions for using Rich with Django.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/django-rich
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
@@ -36,15 +35,15 @@
 	Twitter = https://twitter.com/adamchainz
 
 [options]
 packages = find:
 install_requires = 
 	Django>=3.2
 	rich>=10.0.0
-python_requires = >=3.7
+python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 zip_safe = False
 
 [options.packages.find]
 where = src
```

### Comparing `django_rich-1.6.0/src/django_rich/management.py` & `django_rich-1.7.0/src/django_rich/management.py`

 * *Files identical despite different names*

### Comparing `django_rich-1.6.0/src/django_rich/test.py` & `django_rich-1.7.0/src/django_rich/test.py`

 * *Files identical despite different names*

### Comparing `django_rich-1.6.0/src/django_rich.egg-info/PKG-INFO` & `django_rich-1.7.0/src/django_rich.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rich
-Version: 1.6.0
+Version: 1.7.0
 Summary: Extensions for using Rich with Django.
 Home-page: https://github.com/adamchainz/django-rich
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-rich/blob/main/CHANGELOG.rst
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
 License-File: LICENSE
 
 ===========
 django-rich
 ===========
 
@@ -54,15 +53,15 @@
    :alt: pre-commit
 
 Extensions for using `Rich <https://rich.readthedocs.io/>`__ with Django.
 
 Requirements
 ------------
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 ----
 
 **Want to work smarter and faster?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
```

