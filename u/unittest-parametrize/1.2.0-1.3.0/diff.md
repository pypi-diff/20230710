# Comparing `tmp/unittest_parametrize-1.2.0.tar.gz` & `tmp/unittest_parametrize-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unittest_parametrize-1.2.0.tar", last modified: Fri Jun 16 14:01:40 2023, max compression
+gzip compressed data, was "unittest_parametrize-1.3.0.tar", last modified: Mon Jul 10 12:25:46 2023, max compression
```

## Comparing `unittest_parametrize-1.2.0.tar` & `unittest_parametrize-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:01:40.778684 unittest_parametrize-1.2.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      322 2023-06-16 14:01:37.000000 unittest_parametrize-1.2.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2023-03-28 10:40:12.000000 unittest_parametrize-1.2.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-03-28 10:36:40.000000 unittest_parametrize-1.2.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)    15260 2023-06-16 14:01:40.778807 unittest_parametrize-1.2.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)    14083 2023-06-16 13:38:54.000000 unittest_parametrize-1.2.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-03-28 10:36:40.000000 unittest_parametrize-1.2.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1536 2023-06-16 14:01:40.779220 unittest_parametrize-1.2.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:01:40.768764 unittest_parametrize-1.2.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:01:40.770119 unittest_parametrize-1.2.0/src/unittest_parametrize/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4797 2023-06-16 13:38:54.000000 unittest_parametrize-1.2.0/src/unittest_parametrize/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-03-28 10:44:29.000000 unittest_parametrize-1.2.0/src/unittest_parametrize/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:01:40.778105 unittest_parametrize-1.2.0/src/unittest_parametrize.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    15260 2023-06-16 14:01:40.000000 unittest_parametrize-1.2.0/src/unittest_parametrize.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      461 2023-06-16 14:01:40.000000 unittest_parametrize-1.2.0/src/unittest_parametrize.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 14:01:40.000000 unittest_parametrize-1.2.0/src/unittest_parametrize.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 14:01:40.000000 unittest_parametrize-1.2.0/src/unittest_parametrize.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       46 2023-06-16 14:01:40.000000 unittest_parametrize-1.2.0/src/unittest_parametrize.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       21 2023-06-16 14:01:40.000000 unittest_parametrize-1.2.0/src/unittest_parametrize.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:01:40.778256 unittest_parametrize-1.2.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     9420 2023-06-16 13:38:54.000000 unittest_parametrize-1.2.0/tests/test_unittest_parametrize.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 12:25:46.673828 unittest_parametrize-1.3.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      389 2023-07-10 12:25:44.000000 unittest_parametrize-1.3.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2023-03-28 10:40:12.000000 unittest_parametrize-1.3.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      115 2023-07-10 12:23:09.000000 unittest_parametrize-1.3.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    15210 2023-07-10 12:25:46.673903 unittest_parametrize-1.3.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    14083 2023-07-10 12:23:06.000000 unittest_parametrize-1.3.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-07-10 12:23:06.000000 unittest_parametrize-1.3.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1497 2023-07-10 12:25:46.674216 unittest_parametrize-1.3.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 12:25:46.671961 unittest_parametrize-1.3.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 12:25:46.672878 unittest_parametrize-1.3.0/src/unittest_parametrize/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4797 2023-06-16 13:38:54.000000 unittest_parametrize-1.3.0/src/unittest_parametrize/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-03-28 10:44:29.000000 unittest_parametrize-1.3.0/src/unittest_parametrize/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 12:25:46.673716 unittest_parametrize-1.3.0/src/unittest_parametrize.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    15210 2023-07-10 12:25:46.000000 unittest_parametrize-1.3.0/src/unittest_parametrize.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      426 2023-07-10 12:25:46.000000 unittest_parametrize-1.3.0/src/unittest_parametrize.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 12:25:46.000000 unittest_parametrize-1.3.0/src/unittest_parametrize.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 12:25:46.000000 unittest_parametrize-1.3.0/src/unittest_parametrize.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       46 2023-07-10 12:25:46.000000 unittest_parametrize-1.3.0/src/unittest_parametrize.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       21 2023-07-10 12:25:46.000000 unittest_parametrize-1.3.0/src/unittest_parametrize.egg-info/top_level.txt
```

### Comparing `unittest_parametrize-1.2.0/LICENSE` & `unittest_parametrize-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unittest_parametrize-1.2.0/PKG-INFO` & `unittest_parametrize-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unittest_parametrize
-Version: 1.2.0
+Version: 1.3.0
 Summary: Parametrize tests within unittest TestCases.
 Home-page: https://github.com/adamchainz/unittest-parametrize
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/unittest-parametrize/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -12,22 +12,21 @@
 Keywords: unittest
 Classifier: Development Status :: 5 - Production/Stable
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
 
 ====================
 unittest-parametrize
 ====================
 
@@ -51,15 +50,15 @@
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install unittest-parametrize
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 ----
 
 **Testing a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of recommendations to write faster, more accurate tests.
 
 ----
```

### Comparing `unittest_parametrize-1.2.0/README.rst` & `unittest_parametrize-1.3.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install unittest-parametrize
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 ----
 
 **Testing a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of recommendations to write faster, more accurate tests.
 
 ----
```

### Comparing `unittest_parametrize-1.2.0/setup.cfg` & `unittest_parametrize-1.3.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = unittest_parametrize
-version = 1.2.0
+version = 1.3.0
 description = Parametrize tests within unittest TestCases.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/unittest-parametrize
 author = Adam Johnson
 author_email = me@adamj.eu
 license = MIT
@@ -12,15 +12,14 @@
 classifiers = 
 	Development Status :: 5 - Production/Stable
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
 keywords = unittest
@@ -29,15 +28,15 @@
 	Mastodon = https://fosstodon.org/@adamchainz
 	Twitter = https://twitter.com/adamchainz
 
 [options]
 packages = find:
 install_requires = 
 	typing-extensions;python_version < "3.10"
-python_requires = >=3.7
+python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 zip_safe = False
 
 [options.packages.find]
 where = src
```

### Comparing `unittest_parametrize-1.2.0/src/unittest_parametrize/__init__.py` & `unittest_parametrize-1.3.0/src/unittest_parametrize/__init__.py`

 * *Files identical despite different names*

### Comparing `unittest_parametrize-1.2.0/src/unittest_parametrize.egg-info/PKG-INFO` & `unittest_parametrize-1.3.0/src/unittest_parametrize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unittest-parametrize
-Version: 1.2.0
+Version: 1.3.0
 Summary: Parametrize tests within unittest TestCases.
 Home-page: https://github.com/adamchainz/unittest-parametrize
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/unittest-parametrize/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -12,22 +12,21 @@
 Keywords: unittest
 Classifier: Development Status :: 5 - Production/Stable
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
 
 ====================
 unittest-parametrize
 ====================
 
@@ -51,15 +50,15 @@
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install unittest-parametrize
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 ----
 
 **Testing a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of recommendations to write faster, more accurate tests.
 
 ----
```

