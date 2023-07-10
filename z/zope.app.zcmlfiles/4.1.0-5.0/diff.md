# Comparing `tmp/zope.app.zcmlfiles-4.1.0.tar.gz` & `tmp/zope.app.zcmlfiles-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.app.zcmlfiles-4.1.0.tar", last modified: Tue Aug 23 11:18:14 2022, max compression
+gzip compressed data, was "zope.app.zcmlfiles-5.0.tar", last modified: Mon Jul 10 06:15:45 2023, max compression
```

## Comparing `zope.app.zcmlfiles-4.1.0.tar` & `zope.app.zcmlfiles-5.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-23 11:18:14.707408 zope.app.zcmlfiles-4.1.0/
--rw-r--r--   0 mac        (513) staff       (20)     2871 2022-08-23 11:18:12.000000 zope.app.zcmlfiles-4.1.0/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2022-08-23 11:18:12.000000 zope.app.zcmlfiles-4.1.0/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-08-23 11:18:12.000000 zope.app.zcmlfiles-4.1.0/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2022-08-23 11:18:12.000000 zope.app.zcmlfiles-4.1.0/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      225 2022-08-23 11:18:12.000000 zope.app.zcmlfiles-4.1.0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     4290 2022-08-23 11:18:14.707536 zope.app.zcmlfiles-4.1.0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)       86 2022-08-23 11:18:12.000000 zope.app.zcmlfiles-4.1.0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      417 2022-08-23 11:18:14.708162 zope.app.zcmlfiles-4.1.0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     4294 2022-08-23 11:18:12.000000 zope.app.zcmlfiles-4.1.0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-23 11:18:14.698077 zope.app.zcmlfiles-4.1.0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-23 11:18:14.701917 zope.app.zcmlfiles-4.1.0/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       76 2022-08-23 11:18:12.000000 zope.app.zcmlfiles-4.1.0/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-23 11:18:14.704756 zope.app.zcmlfiles-4.1.0/src/zope/app/
--rw-r--r--   0 mac        (513) staff       (20)       76 2022-08-23 11:18:12.000000 zope.app.zcmlfiles-4.1.0/src/zope/app/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-23 11:18:14.707170 zope.app.zcmlfiles-4.1.0/src/zope/app/zcmlfiles/
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-08-23 11:18:12.000000 zope.app.zcmlfiles-4.1.0/src/zope/app/zcmlfiles/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      830 2022-08-23 11:18:12.000000 zope.app.zcmlfiles-4.1.0/src/zope/app/zcmlfiles/browser.zcml
--rw-r--r--   0 mac        (513) staff       (20)     2220 2022-08-23 11:18:12.000000 zope.app.zcmlfiles-4.1.0/src/zope/app/zcmlfiles/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)      363 2022-08-23 11:18:12.000000 zope.app.zcmlfiles-4.1.0/src/zope/app/zcmlfiles/ftesting.zcml
--rw-r--r--   0 mac        (513) staff       (20)      871 2022-08-23 11:18:12.000000 zope.app.zcmlfiles-4.1.0/src/zope/app/zcmlfiles/menus.zcml
--rw-r--r--   0 mac        (513) staff       (20)      521 2022-08-23 11:18:12.000000 zope.app.zcmlfiles-4.1.0/src/zope/app/zcmlfiles/meta.zcml
--rw-r--r--   0 mac        (513) staff       (20)     1488 2022-08-23 11:18:12.000000 zope.app.zcmlfiles-4.1.0/src/zope/app/zcmlfiles/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-23 11:18:14.704399 zope.app.zcmlfiles-4.1.0/src/zope.app.zcmlfiles.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     4290 2022-08-23 11:18:14.000000 zope.app.zcmlfiles-4.1.0/src/zope.app.zcmlfiles.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      723 2022-08-23 11:18:14.000000 zope.app.zcmlfiles-4.1.0/src/zope.app.zcmlfiles.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-08-23 11:18:14.000000 zope.app.zcmlfiles-4.1.0/src/zope.app.zcmlfiles.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)       14 2022-08-23 11:18:14.000000 zope.app.zcmlfiles-4.1.0/src/zope.app.zcmlfiles.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-08-23 11:18:14.000000 zope.app.zcmlfiles-4.1.0/src/zope.app.zcmlfiles.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      914 2022-08-23 11:18:14.000000 zope.app.zcmlfiles-4.1.0/src/zope.app.zcmlfiles.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-08-23 11:18:14.000000 zope.app.zcmlfiles-4.1.0/src/zope.app.zcmlfiles.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1422 2022-08-23 11:18:12.000000 zope.app.zcmlfiles-4.1.0/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-10 06:15:45.315639 zope.app.zcmlfiles-5.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2981 2023-07-10 06:15:44.000000 zope.app.zcmlfiles-5.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-10 06:15:44.000000 zope.app.zcmlfiles-5.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-10 06:15:44.000000 zope.app.zcmlfiles-5.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-10 06:15:44.000000 zope.app.zcmlfiles-5.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      225 2023-07-10 06:15:44.000000 zope.app.zcmlfiles-5.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4254 2023-07-10 06:15:45.315705 zope.app.zcmlfiles-5.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)       86 2023-07-10 06:15:44.000000 zope.app.zcmlfiles-5.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      418 2023-07-10 06:15:45.315934 zope.app.zcmlfiles-5.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4177 2023-07-10 06:15:44.000000 zope.app.zcmlfiles-5.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-10 06:15:45.311782 zope.app.zcmlfiles-5.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-10 06:15:45.313350 zope.app.zcmlfiles-5.0/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-07-10 06:15:44.000000 zope.app.zcmlfiles-5.0/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-10 06:15:45.314513 zope.app.zcmlfiles-5.0/src/zope/app/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-07-10 06:15:44.000000 zope.app.zcmlfiles-5.0/src/zope/app/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-10 06:15:45.315514 zope.app.zcmlfiles-5.0/src/zope/app/zcmlfiles/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-10 06:15:44.000000 zope.app.zcmlfiles-5.0/src/zope/app/zcmlfiles/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      830 2023-07-10 06:15:44.000000 zope.app.zcmlfiles-5.0/src/zope/app/zcmlfiles/browser.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2220 2023-07-10 06:15:44.000000 zope.app.zcmlfiles-5.0/src/zope/app/zcmlfiles/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      363 2023-07-10 06:15:44.000000 zope.app.zcmlfiles-5.0/src/zope/app/zcmlfiles/ftesting.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      871 2023-07-10 06:15:44.000000 zope.app.zcmlfiles-5.0/src/zope/app/zcmlfiles/menus.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      521 2023-07-10 06:15:44.000000 zope.app.zcmlfiles-5.0/src/zope/app/zcmlfiles/meta.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1487 2023-07-10 06:15:44.000000 zope.app.zcmlfiles-5.0/src/zope/app/zcmlfiles/tests.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-10 06:15:45.314381 zope.app.zcmlfiles-5.0/src/zope.app.zcmlfiles.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4254 2023-07-10 06:15:45.000000 zope.app.zcmlfiles-5.0/src/zope.app.zcmlfiles.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      723 2023-07-10 06:15:45.000000 zope.app.zcmlfiles-5.0/src/zope.app.zcmlfiles.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-10 06:15:45.000000 zope.app.zcmlfiles-5.0/src/zope.app.zcmlfiles.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       14 2023-07-10 06:15:45.000000 zope.app.zcmlfiles-5.0/src/zope.app.zcmlfiles.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-10 06:15:45.000000 zope.app.zcmlfiles-5.0/src/zope.app.zcmlfiles.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      914 2023-07-10 06:15:45.000000 zope.app.zcmlfiles-5.0/src/zope.app.zcmlfiles.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-07-10 06:15:45.000000 zope.app.zcmlfiles-5.0/src/zope.app.zcmlfiles.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1398 2023-07-10 06:15:44.000000 zope.app.zcmlfiles-5.0/tox.ini
```

### Comparing `zope.app.zcmlfiles-4.1.0/CHANGES.rst` & `zope.app.zcmlfiles-5.0/CHANGES.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Change History
 ==============
 
+5.0 (2023-07-10)
+----------------
+
+- Add support for Python 3.11.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 4.1.0 (2022-08-23)
 ------------------
 
 - Add support for Python 3.7, 3.8, 3.9, 3.10.
 
 - Drop support for Python 3.4.
```

### Comparing `zope.app.zcmlfiles-4.1.0/CONTRIBUTING.md` & `zope.app.zcmlfiles-5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.app.zcmlfiles-4.1.0/LICENSE.txt` & `zope.app.zcmlfiles-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.app.zcmlfiles-4.1.0/PKG-INFO` & `zope.app.zcmlfiles-5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 Metadata-Version: 2.1
 Name: zope.app.zcmlfiles
-Version: 4.1.0
+Version: 5.0
 Summary: Zope application server ZCML files
 Home-page: http://github.com/zopefoundation/zope.app.zcmlfiles
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: zope setup configuration standard menu
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
 Classifier: Framework :: Zope :: 3
+Requires-Python: >=3.7
 Provides-Extra: test
 License-File: LICENSE.txt
 
 Zope application server ZCML files
 **********************************
 
 .. contents::
 
 
 Change History
 ==============
 
+5.0 (2023-07-10)
+----------------
+
+- Add support for Python 3.11.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 4.1.0 (2022-08-23)
 ------------------
 
 - Add support for Python 3.7, 3.8, 3.9, 3.10.
 
 - Drop support for Python 3.4.
 
@@ -151,9 +156,7 @@
 
 - Added missing dependency.
 
 3.4.0 (2007-10-03)
 ------------------
 
 - Initial public release as an individual package.
-
-
```

### Comparing `zope.app.zcmlfiles-4.1.0/setup.py` & `zope.app.zcmlfiles-5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,47 +34,45 @@
     read('README.rst')
     + '\n' +
     read('CHANGES.rst')
 )
 
 setup(
     name='zope.app.zcmlfiles',
-    version='4.1.0',
+    version='5.0',
     url='http://github.com/zopefoundation/zope.app.zcmlfiles',
     author='Zope Foundation and Contributors',
     author_email='zope-dev@zope.org',
     license='ZPL 2.1',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Zope Public License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Operating System :: OS Independent',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Software Development',
         'Framework :: Zope :: 3',
     ],
     description='Zope application server ZCML files',
     long_description=long_description,
     keywords="zope setup configuration standard menu",
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['zope', 'zope.app'],
     include_package_data=True,
+    python_requires='>=3.7',
     extras_require={
         'test': [
             'webtest',
             'zope.testing',
             'zope.testrunner',
         ],
     },
```

### Comparing `zope.app.zcmlfiles-4.1.0/src/zope/app/zcmlfiles/browser.zcml` & `zope.app.zcmlfiles-5.0/src/zope/app/zcmlfiles/browser.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.zcmlfiles-4.1.0/src/zope/app/zcmlfiles/configure.zcml` & `zope.app.zcmlfiles-5.0/src/zope/app/zcmlfiles/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.zcmlfiles-4.1.0/src/zope/app/zcmlfiles/menus.zcml` & `zope.app.zcmlfiles-5.0/src/zope/app/zcmlfiles/menus.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.zcmlfiles-4.1.0/src/zope/app/zcmlfiles/meta.zcml` & `zope.app.zcmlfiles-5.0/src/zope/app/zcmlfiles/meta.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.zcmlfiles-4.1.0/src/zope/app/zcmlfiles/tests.py` & `zope.app.zcmlfiles-5.0/src/zope/app/zcmlfiles/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import unittest
 import warnings
 
 from zope.component.testing import PlacelessSetup
 from zope.configuration import xmlconfig
 
 import zope.app.zcmlfiles
```

### Comparing `zope.app.zcmlfiles-4.1.0/src/zope.app.zcmlfiles.egg-info/PKG-INFO` & `zope.app.zcmlfiles-5.0/src/zope.app.zcmlfiles.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 Metadata-Version: 2.1
 Name: zope.app.zcmlfiles
-Version: 4.1.0
+Version: 5.0
 Summary: Zope application server ZCML files
 Home-page: http://github.com/zopefoundation/zope.app.zcmlfiles
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: zope setup configuration standard menu
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
 Classifier: Framework :: Zope :: 3
+Requires-Python: >=3.7
 Provides-Extra: test
 License-File: LICENSE.txt
 
 Zope application server ZCML files
 **********************************
 
 .. contents::
 
 
 Change History
 ==============
 
+5.0 (2023-07-10)
+----------------
+
+- Add support for Python 3.11.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 4.1.0 (2022-08-23)
 ------------------
 
 - Add support for Python 3.7, 3.8, 3.9, 3.10.
 
 - Drop support for Python 3.4.
 
@@ -151,9 +156,7 @@
 
 - Added missing dependency.
 
 3.4.0 (2007-10-03)
 ------------------
 
 - Initial public release as an individual package.
-
-
```

### Comparing `zope.app.zcmlfiles-4.1.0/src/zope.app.zcmlfiles.egg-info/SOURCES.txt` & `zope.app.zcmlfiles-5.0/src/zope.app.zcmlfiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zope.app.zcmlfiles-4.1.0/src/zope.app.zcmlfiles.egg-info/requires.txt` & `zope.app.zcmlfiles-5.0/src/zope.app.zcmlfiles.egg-info/requires.txt`

 * *Files identical despite different names*

