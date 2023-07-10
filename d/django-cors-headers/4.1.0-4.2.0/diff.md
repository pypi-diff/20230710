# Comparing `tmp/django_cors_headers-4.1.0.tar.gz` & `tmp/django_cors_headers-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cors_headers-4.1.0.tar", last modified: Wed Jun 14 10:56:57 2023, max compression
+gzip compressed data, was "django_cors_headers-4.2.0.tar", last modified: Mon Jul 10 09:09:25 2023, max compression
```

## Comparing `django_cors_headers-4.1.0.tar` & `django_cors_headers-4.2.0.tar`

### file list

```diff
@@ -1,29 +1,25 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 10:56:57.580370 django_cors_headers-4.1.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    12227 2023-06-14 10:56:54.000000 django_cors_headers-4.1.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1111 2023-04-27 20:44:48.000000 django_cors_headers-4.1.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-04-27 20:44:48.000000 django_cors_headers-4.1.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)    16622 2023-06-14 10:56:57.580444 django_cors_headers-4.1.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)    14941 2023-06-14 10:56:26.000000 django_cors_headers-4.1.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      500 2023-05-12 08:45:23.000000 django_cors_headers-4.1.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1921 2023-06-14 10:56:57.580767 django_cors_headers-4.1.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 10:56:57.576686 django_cors_headers-4.1.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 10:56:57.579028 django_cors_headers-4.1.0/src/corsheaders/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-04-27 20:44:48.000000 django_cors_headers-4.1.0/src/corsheaders/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      378 2023-04-27 20:44:48.000000 django_cors_headers-4.1.0/src/corsheaders/apps.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     5920 2023-05-12 09:12:46.000000 django_cors_headers-4.1.0/src/corsheaders/checks.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2146 2023-05-12 09:12:46.000000 django_cors_headers-4.1.0/src/corsheaders/conf.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      273 2023-05-12 08:45:23.000000 django_cors_headers-4.1.0/src/corsheaders/defaults.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     6122 2023-05-12 09:12:46.000000 django_cors_headers-4.1.0/src/corsheaders/middleware.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-04-27 20:44:48.000000 django_cors_headers-4.1.0/src/corsheaders/py.typed
--rw-r--r--   0 adamjohnson   (501) staff       (20)      291 2023-04-27 20:44:48.000000 django_cors_headers-4.1.0/src/corsheaders/signals.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 10:56:57.579801 django_cors_headers-4.1.0/src/django_cors_headers.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    16622 2023-06-14 10:56:57.000000 django_cors_headers-4.1.0/src/django_cors_headers.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      626 2023-06-14 10:56:57.000000 django_cors_headers-4.1.0/src/django_cors_headers.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-14 10:56:57.000000 django_cors_headers-4.1.0/src/django_cors_headers.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-14 10:56:57.000000 django_cors_headers-4.1.0/src/django_cors_headers.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2023-06-14 10:56:57.000000 django_cors_headers-4.1.0/src/django_cors_headers.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2023-06-14 10:56:57.000000 django_cors_headers-4.1.0/src/django_cors_headers.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 10:56:57.580192 django_cors_headers-4.1.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     6000 2023-05-12 09:12:46.000000 django_cors_headers-4.1.0/tests/test_checks.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1553 2023-04-27 20:44:48.000000 django_cors_headers-4.1.0/tests/test_conf.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)    17280 2023-05-12 09:12:46.000000 django_cors_headers-4.1.0/tests/test_middleware.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 09:09:25.585176 django_cors_headers-4.2.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    12294 2023-07-10 09:09:17.000000 django_cors_headers-4.2.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1111 2023-04-27 20:44:48.000000 django_cors_headers-4.2.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      115 2023-07-10 09:07:15.000000 django_cors_headers-4.2.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    16572 2023-07-10 09:09:25.585276 django_cors_headers-4.2.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    14941 2023-07-09 06:45:18.000000 django_cors_headers-4.2.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      500 2023-07-09 06:45:18.000000 django_cors_headers-4.2.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1882 2023-07-10 09:09:25.585593 django_cors_headers-4.2.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 09:09:25.582805 django_cors_headers-4.2.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 09:09:25.584354 django_cors_headers-4.2.0/src/corsheaders/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-04-27 20:44:48.000000 django_cors_headers-4.2.0/src/corsheaders/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      378 2023-04-27 20:44:48.000000 django_cors_headers-4.2.0/src/corsheaders/apps.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     5920 2023-05-12 09:12:46.000000 django_cors_headers-4.2.0/src/corsheaders/checks.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2146 2023-05-12 09:12:46.000000 django_cors_headers-4.2.0/src/corsheaders/conf.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      273 2023-05-12 08:45:23.000000 django_cors_headers-4.2.0/src/corsheaders/defaults.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     6122 2023-05-12 09:12:46.000000 django_cors_headers-4.2.0/src/corsheaders/middleware.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-04-27 20:44:48.000000 django_cors_headers-4.2.0/src/corsheaders/py.typed
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      291 2023-04-27 20:44:48.000000 django_cors_headers-4.2.0/src/corsheaders/signals.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 09:09:25.585075 django_cors_headers-4.2.0/src/django_cors_headers.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    16572 2023-07-10 09:09:25.000000 django_cors_headers-4.2.0/src/django_cors_headers.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      561 2023-07-10 09:09:25.000000 django_cors_headers-4.2.0/src/django_cors_headers.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 09:09:25.000000 django_cors_headers-4.2.0/src/django_cors_headers.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 09:09:25.000000 django_cors_headers-4.2.0/src/django_cors_headers.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2023-07-10 09:09:25.000000 django_cors_headers-4.2.0/src/django_cors_headers.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2023-07-10 09:09:25.000000 django_cors_headers-4.2.0/src/django_cors_headers.egg-info/top_level.txt
```

### Comparing `django_cors_headers-4.1.0/CHANGELOG.rst` & `django_cors_headers-4.2.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+4.2.0 (2023-07-10)
+------------------
+
+* Drop Python 3.7 support.
+
 4.1.0 (2023-06-14)
 ------------------
 
 * Support Python 3.12.
 
 4.0.0 (2023-05-12)
 ------------------
```

### Comparing `django_cors_headers-4.1.0/LICENSE` & `django_cors_headers-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cors_headers-4.1.0/PKG-INFO` & `django_cors_headers-4.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_cors_headers
-Version: 4.1.0
+Version: 4.2.0
 Summary: django-cors-headers is a Django application for handling the server headers required for Cross-Origin Resource Sharing (CORS).
 Home-page: https://github.com/adamchainz/django-cors-headers
 Author: Otto Yiu
 Author-email: otto@live.ca
 Maintainer: Adam Johnson
 Maintainer-email: me@adamj.eu
 License: MIT
@@ -21,23 +21,22 @@
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
 
 ===================
 django-cors-headers
 ===================
 
@@ -76,15 +75,15 @@
 * The `MDN Article <https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS>`_
 * The `HTML5 Rocks Tutorial <https://www.html5rocks.com/en/tutorials/cors/>`_
 * The `Wikipedia Page <https://en.wikipedia.org/wiki/Cross-origin_resource_sharing>`_
 
 Requirements
 ------------
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 ----
 
 **Want to work smarter and faster?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
```

### Comparing `django_cors_headers-4.1.0/README.rst` & `django_cors_headers-4.2.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 * The `MDN Article <https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS>`_
 * The `HTML5 Rocks Tutorial <https://www.html5rocks.com/en/tutorials/cors/>`_
 * The `Wikipedia Page <https://en.wikipedia.org/wiki/Cross-origin_resource_sharing>`_
 
 Requirements
 ------------
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 ----
 
 **Want to work smarter and faster?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
```

### Comparing `django_cors_headers-4.1.0/setup.cfg` & `django_cors_headers-4.2.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_cors_headers
-version = 4.1.0
+version = 4.2.0
 description = django-cors-headers is a Django application for handling the server headers required for Cross-Origin Resource Sharing (CORS).
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/django-cors-headers
 author = Otto Yiu
 author_email = otto@live.ca
 maintainer = Adam Johnson
@@ -21,15 +21,14 @@
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
@@ -44,15 +43,15 @@
 	Mastodon = https://fosstodon.org/@adamchainz
 	Twitter = https://twitter.com/adamchainz
 
 [options]
 packages = find:
 install_requires = 
 	Django>=3.2
-python_requires = >=3.7
+python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 zip_safe = False
 
 [options.packages.find]
 where = src
```

### Comparing `django_cors_headers-4.1.0/src/corsheaders/checks.py` & `django_cors_headers-4.2.0/src/corsheaders/checks.py`

 * *Files identical despite different names*

### Comparing `django_cors_headers-4.1.0/src/corsheaders/conf.py` & `django_cors_headers-4.2.0/src/corsheaders/conf.py`

 * *Files identical despite different names*

### Comparing `django_cors_headers-4.1.0/src/corsheaders/middleware.py` & `django_cors_headers-4.2.0/src/corsheaders/middleware.py`

 * *Files identical despite different names*

### Comparing `django_cors_headers-4.1.0/src/django_cors_headers.egg-info/PKG-INFO` & `django_cors_headers-4.2.0/src/django_cors_headers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cors-headers
-Version: 4.1.0
+Version: 4.2.0
 Summary: django-cors-headers is a Django application for handling the server headers required for Cross-Origin Resource Sharing (CORS).
 Home-page: https://github.com/adamchainz/django-cors-headers
 Author: Otto Yiu
 Author-email: otto@live.ca
 Maintainer: Adam Johnson
 Maintainer-email: me@adamj.eu
 License: MIT
@@ -21,23 +21,22 @@
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
 
 ===================
 django-cors-headers
 ===================
 
@@ -76,15 +75,15 @@
 * The `MDN Article <https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS>`_
 * The `HTML5 Rocks Tutorial <https://www.html5rocks.com/en/tutorials/cors/>`_
 * The `Wikipedia Page <https://en.wikipedia.org/wiki/Cross-origin_resource_sharing>`_
 
 Requirements
 ------------
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 ----
 
 **Want to work smarter and faster?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
```

### Comparing `django_cors_headers-4.1.0/src/django_cors_headers.egg-info/SOURCES.txt` & `django_cors_headers-4.2.0/src/django_cors_headers.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -13,11 +13,8 @@
 src/corsheaders/py.typed
 src/corsheaders/signals.py
 src/django_cors_headers.egg-info/PKG-INFO
 src/django_cors_headers.egg-info/SOURCES.txt
 src/django_cors_headers.egg-info/dependency_links.txt
 src/django_cors_headers.egg-info/not-zip-safe
 src/django_cors_headers.egg-info/requires.txt
-src/django_cors_headers.egg-info/top_level.txt
-tests/test_checks.py
-tests/test_conf.py
-tests/test_middleware.py
+src/django_cors_headers.egg-info/top_level.txt
```

