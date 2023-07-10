# Comparing `tmp/wagtail_csp-1.1.tar.gz` & `tmp/wagtail_csp-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_csp-1.1.tar", last modified: Sun Jul  9 18:39:11 2023, max compression
+gzip compressed data, was "wagtail_csp-1.2.tar", last modified: Mon Jul 10 00:29:54 2023, max compression
```

## Comparing `wagtail_csp-1.1.tar` & `wagtail_csp-1.2.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxr-x   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-09 18:39:11.811230 wagtail_csp-1.1/
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     1526 2023-07-09 18:21:56.000000 wagtail_csp-1.1/LICENSE
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)       35 2023-07-09 18:21:56.000000 wagtail_csp-1.1/MANIFEST.in
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     2161 2023-07-09 18:39:11.811230 wagtail_csp-1.1/PKG-INFO
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      687 2023-07-09 18:21:56.000000 wagtail_csp-1.1/README.rst
-drwxrwxr-x   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-09 18:39:11.799229 wagtail_csp-1.1/csp/
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/__init__.py
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      138 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/context_processors.py
-drwxrwxr-x   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-09 18:39:11.803229 wagtail_csp-1.1/csp/contrib/
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/contrib/__init__.py
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      908 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/contrib/rate_limiting.py
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     1166 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/decorators.py
-drwxrwxr-x   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-09 18:39:11.803229 wagtail_csp-1.1/csp/extensions/
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     1775 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/extensions/__init__.py
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     2724 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/middleware.py
-drwxrwxr-x   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-09 18:39:11.803229 wagtail_csp-1.1/csp/migrations/
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/migrations/__init__.py
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     2067 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/models.py
-drwxrwxr-x   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-09 18:39:11.803229 wagtail_csp-1.1/csp/templatetags/
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/templatetags/__init__.py
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     1315 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/templatetags/csp.py
-drwxrwxr-x   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-09 18:39:11.807229 wagtail_csp-1.1/csp/tests/
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)       50 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/tests/__init__.py
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      109 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/tests/environment.py
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      982 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/tests/settings.py
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      661 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/tests/test_context_processors.py
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      707 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/tests/test_contrib.py
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     4306 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/tests/test_decorators.py
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     3149 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/tests/test_jinja_extension.py
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     3954 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/tests/test_middleware.py
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     3232 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/tests/test_templatetags.py
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     8636 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/tests/test_utils.py
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     1430 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/tests/utils.py
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      745 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/urls.py
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     9113 2023-07-09 18:21:56.000000 wagtail_csp-1.1/csp/utils.py
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      201 2023-07-09 18:39:11.811230 wagtail_csp-1.1/setup.cfg
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     2643 2023-07-09 18:38:34.000000 wagtail_csp-1.1/setup.py
-drwxrwxr-x   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-09 18:39:11.807229 wagtail_csp-1.1/wagtail_csp.egg-info/
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     2161 2023-07-09 18:39:11.000000 wagtail_csp-1.1/wagtail_csp.egg-info/PKG-INFO
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      832 2023-07-09 18:39:11.000000 wagtail_csp-1.1/wagtail_csp.egg-info/SOURCES.txt
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)        1 2023-07-09 18:39:11.000000 wagtail_csp-1.1/wagtail_csp.egg-info/dependency_links.txt
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)        1 2023-07-09 18:39:11.000000 wagtail_csp-1.1/wagtail_csp.egg-info/not-zip-safe
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      208 2023-07-09 18:39:11.000000 wagtail_csp-1.1/wagtail_csp.egg-info/requires.txt
--rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)        4 2023-07-09 18:39:11.000000 wagtail_csp-1.1/wagtail_csp.egg-info/top_level.txt
+drwxrwxr-x   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-10 00:29:54.361818 wagtail_csp-1.2/
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     1526 2023-07-10 00:19:04.000000 wagtail_csp-1.2/LICENSE
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)       35 2023-07-10 00:19:04.000000 wagtail_csp-1.2/MANIFEST.in
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     2126 2023-07-10 00:29:54.361818 wagtail_csp-1.2/PKG-INFO
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      687 2023-07-10 00:19:04.000000 wagtail_csp-1.2/README.rst
+drwxrwxr-x   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-10 00:29:54.357816 wagtail_csp-1.2/csp/
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/__init__.py
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      138 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/context_processors.py
+drwxrwxr-x   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-10 00:29:54.357816 wagtail_csp-1.2/csp/contrib/
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/contrib/__init__.py
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      908 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/contrib/rate_limiting.py
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     1166 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/decorators.py
+drwxrwxr-x   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-10 00:29:54.357816 wagtail_csp-1.2/csp/extensions/
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     1775 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/extensions/__init__.py
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     2724 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/middleware.py
+drwxrwxr-x   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-10 00:29:54.357816 wagtail_csp-1.2/csp/migrations/
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     2520 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/migrations/0001_initial.py
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/migrations/__init__.py
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     2067 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/models.py
+drwxrwxr-x   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-10 00:29:54.357816 wagtail_csp-1.2/csp/templatetags/
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/templatetags/__init__.py
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     1315 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/templatetags/csp.py
+drwxrwxr-x   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-10 00:29:54.361818 wagtail_csp-1.2/csp/tests/
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)       50 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/tests/__init__.py
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      109 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/tests/environment.py
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      982 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/tests/settings.py
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      661 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/tests/test_context_processors.py
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      707 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/tests/test_contrib.py
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     4306 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/tests/test_decorators.py
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     3149 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/tests/test_jinja_extension.py
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     3954 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/tests/test_middleware.py
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     3232 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/tests/test_templatetags.py
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     8636 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/tests/test_utils.py
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     1430 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/tests/utils.py
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      745 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/urls.py
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     9113 2023-07-10 00:19:04.000000 wagtail_csp-1.2/csp/utils.py
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      201 2023-07-10 00:29:54.361818 wagtail_csp-1.2/setup.cfg
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     2608 2023-07-10 00:26:16.000000 wagtail_csp-1.2/setup.py
+drwxrwxr-x   0 ehuffman  (1000) ehuffman  (1000)        0 2023-07-10 00:29:54.361818 wagtail_csp-1.2/wagtail_csp.egg-info/
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)     2126 2023-07-10 00:29:54.000000 wagtail_csp-1.2/wagtail_csp.egg-info/PKG-INFO
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      863 2023-07-10 00:29:54.000000 wagtail_csp-1.2/wagtail_csp.egg-info/SOURCES.txt
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)        1 2023-07-10 00:29:54.000000 wagtail_csp-1.2/wagtail_csp.egg-info/dependency_links.txt
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)        1 2023-07-10 00:29:54.000000 wagtail_csp-1.2/wagtail_csp.egg-info/not-zip-safe
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)      208 2023-07-10 00:29:54.000000 wagtail_csp-1.2/wagtail_csp.egg-info/requires.txt
+-rw-rw-r--   0 ehuffman  (1000) ehuffman  (1000)        4 2023-07-10 00:29:54.000000 wagtail_csp-1.2/wagtail_csp.egg-info/top_level.txt
```

### Comparing `wagtail_csp-1.1/LICENSE` & `wagtail_csp-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_csp-1.1/PKG-INFO` & `wagtail_csp-1.2/wagtail_csp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: wagtail_csp
-Version: 1.1
+Name: wagtail-csp
+Version: 1.2
 Summary: Wagtail Content Security Policy support.
 Home-page: https://gitlab.com/womens-declaration/wagtail-csp
 Author: anti_commute
 Author-email: anti_commute@protonmail.com
 License: BSD
-Project-URL: Changelog, https://gitlab.com/womens-declaration/wagtail-csp/-/blob/wagtail-settings/CHANGES
+Project-URL: Changelog, https://gitlab.com/womens-declaration/wagtail-csp/-/blob/main/CHANGES
 Project-URL: Bug Tracker, https://gitlab.com/womens-declaration/wagtail-csp/-/issues
-Project-URL: Source Code, https://gitlab.com/womens-declaration/wagtail-csp/-/tree/wagtail-settings
+Project-URL: Source Code, https://gitlab.com/womens-declaration/wagtail-csp/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Environment :: Web Environment :: Mozilla
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `wagtail_csp-1.1/README.rst` & `wagtail_csp-1.2/README.rst`

 * *Files identical despite different names*

### Comparing `wagtail_csp-1.1/csp/contrib/rate_limiting.py` & `wagtail_csp-1.2/csp/contrib/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `wagtail_csp-1.1/csp/decorators.py` & `wagtail_csp-1.2/csp/decorators.py`

 * *Files identical despite different names*

### Comparing `wagtail_csp-1.1/csp/extensions/__init__.py` & `wagtail_csp-1.2/csp/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_csp-1.1/csp/middleware.py` & `wagtail_csp-1.2/csp/middleware.py`

 * *Files identical despite different names*

### Comparing `wagtail_csp-1.1/csp/models.py` & `wagtail_csp-1.2/csp/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_csp-1.1/csp/templatetags/csp.py` & `wagtail_csp-1.2/csp/templatetags/csp.py`

 * *Files identical despite different names*

### Comparing `wagtail_csp-1.1/csp/tests/settings.py` & `wagtail_csp-1.2/csp/tests/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_csp-1.1/csp/tests/test_context_processors.py` & `wagtail_csp-1.2/csp/tests/test_context_processors.py`

 * *Files identical despite different names*

### Comparing `wagtail_csp-1.1/csp/tests/test_contrib.py` & `wagtail_csp-1.2/csp/tests/test_contrib.py`

 * *Files identical despite different names*

### Comparing `wagtail_csp-1.1/csp/tests/test_decorators.py` & `wagtail_csp-1.2/csp/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `wagtail_csp-1.1/csp/tests/test_jinja_extension.py` & `wagtail_csp-1.2/csp/tests/test_jinja_extension.py`

 * *Files identical despite different names*

### Comparing `wagtail_csp-1.1/csp/tests/test_middleware.py` & `wagtail_csp-1.2/csp/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `wagtail_csp-1.1/csp/tests/test_templatetags.py` & `wagtail_csp-1.2/csp/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `wagtail_csp-1.1/csp/tests/test_utils.py` & `wagtail_csp-1.2/csp/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_csp-1.1/csp/tests/utils.py` & `wagtail_csp-1.2/csp/tests/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_csp-1.1/csp/urls.py` & `wagtail_csp-1.2/csp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_csp-1.1/csp/utils.py` & `wagtail_csp-1.2/csp/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_csp-1.1/setup.py` & `wagtail_csp-1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import os
 import codecs
 from setuptools import setup, find_packages
 
 
-version = '1.1'
+version = '1.2'
 
 
 if sys.argv[-1] == 'publish':
     os.system('python setup.py sdist upload')
     os.system('python setup.py bdist_wheel upload')
     print('You probably want to also tag the version now:')
     print('  git tag -a %s -m "version %s"' % (version, version))
@@ -52,17 +52,17 @@
     long_description=read('README.rst'),
     author='anti_commute',
     author_email='anti_commute@protonmail.com',
     url='https://gitlab.com/womens-declaration/wagtail-csp',
     license='BSD',
     packages=find_packages(),
     project_urls={
-        "Changelog": "https://gitlab.com/womens-declaration/wagtail-csp/-/blob/wagtail-settings/CHANGES",
+        "Changelog": "https://gitlab.com/womens-declaration/wagtail-csp/-/blob/main/CHANGES",
         "Bug Tracker": "https://gitlab.com/womens-declaration/wagtail-csp/-/issues",
-        "Source Code": "https://gitlab.com/womens-declaration/wagtail-csp/-/tree/wagtail-settings",
+        "Source Code": "https://gitlab.com/womens-declaration/wagtail-csp/",
     },
     install_requires=install_requires,
     extras_require={
         'tests': test_requires,
         'jinja2': jinja2_requires,
     },
     include_package_data=True,
```

### Comparing `wagtail_csp-1.1/wagtail_csp.egg-info/PKG-INFO` & `wagtail_csp-1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: wagtail-csp
-Version: 1.1
+Name: wagtail_csp
+Version: 1.2
 Summary: Wagtail Content Security Policy support.
 Home-page: https://gitlab.com/womens-declaration/wagtail-csp
 Author: anti_commute
 Author-email: anti_commute@protonmail.com
 License: BSD
-Project-URL: Changelog, https://gitlab.com/womens-declaration/wagtail-csp/-/blob/wagtail-settings/CHANGES
+Project-URL: Changelog, https://gitlab.com/womens-declaration/wagtail-csp/-/blob/main/CHANGES
 Project-URL: Bug Tracker, https://gitlab.com/womens-declaration/wagtail-csp/-/issues
-Project-URL: Source Code, https://gitlab.com/womens-declaration/wagtail-csp/-/tree/wagtail-settings
+Project-URL: Source Code, https://gitlab.com/womens-declaration/wagtail-csp/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Environment :: Web Environment :: Mozilla
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `wagtail_csp-1.1/wagtail_csp.egg-info/SOURCES.txt` & `wagtail_csp-1.2/wagtail_csp.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 csp/middleware.py
 csp/models.py
 csp/urls.py
 csp/utils.py
 csp/contrib/__init__.py
 csp/contrib/rate_limiting.py
 csp/extensions/__init__.py
+csp/migrations/0001_initial.py
 csp/migrations/__init__.py
 csp/templatetags/__init__.py
 csp/templatetags/csp.py
 csp/tests/__init__.py
 csp/tests/environment.py
 csp/tests/settings.py
 csp/tests/test_context_processors.py
```

