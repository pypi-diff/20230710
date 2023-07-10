# Comparing `tmp/django-allow-cidr-0.7.0.tar.gz` & `tmp/django-allow-cidr-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-allow-cidr-0.7.0.tar", last modified: Mon Jul 10 12:28:00 2023, max compression
+gzip compressed data, was "django-allow-cidr-0.7.1.tar", last modified: Mon Jul 10 13:34:45 2023, max compression
```

## Comparing `django-allow-cidr-0.7.0.tar` & `django-allow-cidr-0.7.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:28:00.740100 django-allow-cidr-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-10 12:28:00.740100 django-allow-cidr-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:28:00.740100 django-allow-cidr-0.7.0/allow_cidr/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/allow_cidr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/allow_cidr/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/allow_cidr/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:28:00.740100 django-allow-cidr-0.7.0/django_allow_cidr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-10 12:28:00.000000 django-allow-cidr-0.7.0/django_allow_cidr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-10 12:28:00.000000 django-allow-cidr-0.7.0/django_allow_cidr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:28:00.000000 django-allow-cidr-0.7.0/django_allow_cidr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:28:00.000000 django-allow-cidr-0.7.0/django_allow_cidr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 12:28:00.000000 django-allow-cidr-0.7.0/django_allow_cidr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 12:28:00.000000 django-allow-cidr-0.7.0/django_allow_cidr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-10 12:28:00.740100 django-allow-cidr-0.7.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1936 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:28:00.740100 django-allow-cidr-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-10 12:27:47.000000 django-allow-cidr-0.7.0/tests/test_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:34:45.494689 django-allow-cidr-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-10 13:34:36.000000 django-allow-cidr-0.7.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-10 13:34:36.000000 django-allow-cidr-0.7.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-10 13:34:36.000000 django-allow-cidr-0.7.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-10 13:34:36.000000 django-allow-cidr-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-10 13:34:36.000000 django-allow-cidr-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-10 13:34:45.494689 django-allow-cidr-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-10 13:34:36.000000 django-allow-cidr-0.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:34:45.494689 django-allow-cidr-0.7.1/allow_cidr/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 13:34:36.000000 django-allow-cidr-0.7.1/allow_cidr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-10 13:34:36.000000 django-allow-cidr-0.7.1/allow_cidr/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-10 13:34:36.000000 django-allow-cidr-0.7.1/allow_cidr/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:34:45.494689 django-allow-cidr-0.7.1/django_allow_cidr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-10 13:34:45.000000 django-allow-cidr-0.7.1/django_allow_cidr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-10 13:34:45.000000 django-allow-cidr-0.7.1/django_allow_cidr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:34:45.000000 django-allow-cidr-0.7.1/django_allow_cidr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:34:45.000000 django-allow-cidr-0.7.1/django_allow_cidr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 13:34:45.000000 django-allow-cidr-0.7.1/django_allow_cidr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 13:34:45.000000 django-allow-cidr-0.7.1/django_allow_cidr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-10 13:34:45.494689 django-allow-cidr-0.7.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1936 2023-07-10 13:34:36.000000 django-allow-cidr-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:34:45.494689 django-allow-cidr-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-10 13:34:36.000000 django-allow-cidr-0.7.1/tests/test_middleware.py
```

### Comparing `django-allow-cidr-0.7.0/CONTRIBUTING.rst` & `django-allow-cidr-0.7.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-allow-cidr-0.7.0/HISTORY.rst` & `django-allow-cidr-0.7.1/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. :changelog:
 
 History
 -------
 
+0.7.1 (2023-07-10)
+++++++++++++++++++
+
+* Update setup.cfg to rename deprecated licence_file param
+
+
 0.7.0 (2023-07-10)
 ++++++++++++++++++
 
 * Add IPv6 support - thanks @rissson!
 * Add Django 4.2 to CI; freshen up CI config
```

### Comparing `django-allow-cidr-0.7.0/LICENSE` & `django-allow-cidr-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-allow-cidr-0.7.0/PKG-INFO` & `django-allow-cidr-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-allow-cidr
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Django Middleware to enable use of CIDR IP ranges in ALLOWED_HOSTS.
 Home-page: https://github.com/mozmeao/django-allow-cidr
 Author: Paul McLanahan
 Author-email: pmac@mozilla.com
 License: Apache Software License 2.0
 Keywords: django-allow-cidr
 Classifier: Development Status :: 4 - Beta
@@ -103,14 +103,20 @@
 
 
 
 
 History
 -------
 
+0.7.1 (2023-07-10)
+++++++++++++++++++
+
+* Update setup.cfg to rename deprecated licence_file param
+
+
 0.7.0 (2023-07-10)
 ++++++++++++++++++
 
 * Add IPv6 support - thanks @rissson!
 * Add Django 4.2 to CI; freshen up CI config
```

### Comparing `django-allow-cidr-0.7.0/README.rst` & `django-allow-cidr-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-allow-cidr-0.7.0/allow_cidr/middleware.py` & `django-allow-cidr-0.7.1/allow_cidr/middleware.py`

 * *Files identical despite different names*

### Comparing `django-allow-cidr-0.7.0/django_allow_cidr.egg-info/PKG-INFO` & `django-allow-cidr-0.7.1/django_allow_cidr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-allow-cidr
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Django Middleware to enable use of CIDR IP ranges in ALLOWED_HOSTS.
 Home-page: https://github.com/mozmeao/django-allow-cidr
 Author: Paul McLanahan
 Author-email: pmac@mozilla.com
 License: Apache Software License 2.0
 Keywords: django-allow-cidr
 Classifier: Development Status :: 4 - Beta
@@ -103,14 +103,20 @@
 
 
 
 
 History
 -------
 
+0.7.1 (2023-07-10)
+++++++++++++++++++
+
+* Update setup.cfg to rename deprecated licence_file param
+
+
 0.7.0 (2023-07-10)
 ++++++++++++++++++
 
 * Add IPv6 support - thanks @rissson!
 * Add Django 4.2 to CI; freshen up CI config
```

### Comparing `django-allow-cidr-0.7.0/setup.py` & `django-allow-cidr-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-allow-cidr-0.7.0/tests/test_middleware.py` & `django-allow-cidr-0.7.1/tests/test_middleware.py`

 * *Files identical despite different names*

