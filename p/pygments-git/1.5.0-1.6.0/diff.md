# Comparing `tmp/pygments_git-1.5.0.tar.gz` & `tmp/pygments_git-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygments_git-1.5.0.tar", last modified: Fri Jun 16 14:15:23 2023, max compression
+gzip compressed data, was "pygments_git-1.6.0.tar", last modified: Mon Jul 10 14:12:05 2023, max compression
```

## Comparing `pygments_git-1.5.0.tar` & `pygments_git-1.6.0.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:15:23.525792 pygments_git-1.5.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      827 2023-06-16 14:15:21.000000 pygments_git-1.5.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2023-04-01 11:07:54.000000 pygments_git-1.5.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-04-01 11:04:32.000000 pygments_git-1.5.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4645 2023-06-16 14:15:23.525870 pygments_git-1.5.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3444 2023-06-16 14:08:48.000000 pygments_git-1.5.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-04-01 13:54:14.000000 pygments_git-1.5.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1850 2023-06-16 14:15:23.526208 pygments_git-1.5.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:15:23.515065 pygments_git-1.5.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:15:23.516216 pygments_git-1.5.0/src/pygments_git/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    13581 2023-05-31 14:19:57.000000 pygments_git-1.5.0/src/pygments_git/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-04-01 11:04:33.000000 pygments_git-1.5.0/src/pygments_git/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:15:23.525503 pygments_git-1.5.0/src/pygments_git.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4645 2023-06-16 14:15:23.000000 pygments_git-1.5.0/src/pygments_git.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      432 2023-06-16 14:15:23.000000 pygments_git-1.5.0/src/pygments_git.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 14:15:23.000000 pygments_git-1.5.0/src/pygments_git.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)      322 2023-06-16 14:15:23.000000 pygments_git-1.5.0/src/pygments_git.egg-info/entry_points.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 14:15:23.000000 pygments_git-1.5.0/src/pygments_git.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)        9 2023-06-16 14:15:23.000000 pygments_git-1.5.0/src/pygments_git.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       13 2023-06-16 14:15:23.000000 pygments_git-1.5.0/src/pygments_git.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 14:15:23.525658 pygments_git-1.5.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    10528 2023-05-31 14:19:57.000000 pygments_git-1.5.0/tests/test_pygments_git.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 14:12:05.050761 pygments_git-1.6.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      894 2023-07-10 14:12:02.000000 pygments_git-1.6.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2023-04-01 11:07:54.000000 pygments_git-1.6.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      115 2023-07-10 14:09:02.000000 pygments_git-1.6.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4595 2023-07-10 14:12:05.050840 pygments_git-1.6.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3444 2023-07-10 14:08:44.000000 pygments_git-1.6.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-07-10 14:08:44.000000 pygments_git-1.6.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1811 2023-07-10 14:12:05.051119 pygments_git-1.6.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 14:12:05.047083 pygments_git-1.6.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 14:12:05.049370 pygments_git-1.6.0/src/pygments_git/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    13581 2023-05-31 14:19:57.000000 pygments_git-1.6.0/src/pygments_git/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-04-01 11:04:33.000000 pygments_git-1.6.0/src/pygments_git/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 14:12:05.050646 pygments_git-1.6.0/src/pygments_git.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4595 2023-07-10 14:12:05.000000 pygments_git-1.6.0/src/pygments_git.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      405 2023-07-10 14:12:05.000000 pygments_git-1.6.0/src/pygments_git.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 14:12:05.000000 pygments_git-1.6.0/src/pygments_git.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      322 2023-07-10 14:12:05.000000 pygments_git-1.6.0/src/pygments_git.egg-info/entry_points.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 14:12:04.000000 pygments_git-1.6.0/src/pygments_git.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        9 2023-07-10 14:12:05.000000 pygments_git-1.6.0/src/pygments_git.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       13 2023-07-10 14:12:05.000000 pygments_git-1.6.0/src/pygments_git.egg-info/top_level.txt
```

### Comparing `pygments_git-1.5.0/CHANGELOG.rst` & `pygments_git-1.6.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+1.6.0 (2023-07-10)
+------------------
+
+* Drop Python 3.7 support.
+
 1.5.0 (2023-06-16)
 ------------------
 
 * Support Python 3.12.
 
 1.4.1 (2023-05-31)
 ------------------
```

### Comparing `pygments_git-1.5.0/LICENSE` & `pygments_git-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygments_git-1.5.0/PKG-INFO` & `pygments_git-1.6.0/src/pygments_git.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pygments_git
-Version: 1.5.0
+Name: pygments-git
+Version: 1.6.0
 Summary: Pygments lexers for Git output and files.
 Home-page: https://github.com/adamchainz/pygments-git
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/pygments-git/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -13,22 +13,21 @@
 Classifier: Development Status :: 5 - Production/Stable
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
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ============
 pygments-git
 ============
 
@@ -55,15 +54,15 @@
 
 Use **pip**:
 
 .. code-block:: sh
 
     python -m pip install pygments-git
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 ----
 
 **Working on a Django project?**
 Improve your skills with `one of my books <https://adamj.eu/books/>`__.
 
 ----
```

### Comparing `pygments_git-1.5.0/README.rst` & `pygments_git-1.6.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 Use **pip**:
 
 .. code-block:: sh
 
     python -m pip install pygments-git
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 ----
 
 **Working on a Django project?**
 Improve your skills with `one of my books <https://adamj.eu/books/>`__.
 
 ----
```

### Comparing `pygments_git-1.5.0/setup.cfg` & `pygments_git-1.6.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pygments_git
-version = 1.5.0
+version = 1.6.0
 description = Pygments lexers for Git output and files.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/pygments-git
 author = Adam Johnson
 author_email = me@adamj.eu
 license = MIT
@@ -13,15 +13,14 @@
 	Development Status :: 5 - Production/Stable
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
 	Typing :: Typed
 keywords = Pygments, Git
@@ -30,15 +29,15 @@
 	Mastodon = https://fosstodon.org/@adamchainz
 	Twitter = https://twitter.com/adamchainz
 
 [options]
 packages = find:
 install_requires = 
 	pygments
-python_requires = >=3.7
+python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 zip_safe = False
 
 [options.packages.find]
 where = src
```

### Comparing `pygments_git-1.5.0/src/pygments_git/__init__.py` & `pygments_git-1.6.0/src/pygments_git/__init__.py`

 * *Files identical despite different names*

### Comparing `pygments_git-1.5.0/src/pygments_git.egg-info/PKG-INFO` & `pygments_git-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pygments-git
-Version: 1.5.0
+Name: pygments_git
+Version: 1.6.0
 Summary: Pygments lexers for Git output and files.
 Home-page: https://github.com/adamchainz/pygments-git
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/pygments-git/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -13,22 +13,21 @@
 Classifier: Development Status :: 5 - Production/Stable
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
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ============
 pygments-git
 ============
 
@@ -55,15 +54,15 @@
 
 Use **pip**:
 
 .. code-block:: sh
 
     python -m pip install pygments-git
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 ----
 
 **Working on a Django project?**
 Improve your skills with `one of my books <https://adamj.eu/books/>`__.
 
 ----
```

