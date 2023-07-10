# Comparing `tmp/patchy-2.7.0.tar.gz` & `tmp/patchy-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patchy-2.7.0.tar", last modified: Fri Jun 16 15:01:49 2023, max compression
+gzip compressed data, was "patchy-2.8.0.tar", last modified: Mon Jul 10 14:05:11 2023, max compression
```

## Comparing `patchy-2.7.0.tar` & `patchy-2.8.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:01:49.607440 patchy-2.7.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3163 2023-06-16 15:01:47.000000 patchy-2.7.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:50.000000 patchy-2.7.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      122 2023-01-20 12:10:00.000000 patchy-2.7.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)    10451 2023-06-16 15:01:49.607506 patchy-2.7.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     9261 2023-06-16 14:55:31.000000 patchy-2.7.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)    29870 2022-06-03 11:59:50.000000 patchy-2.7.0/pirate.png
--rw-r--r--   0 adamjohnson   (501) staff       (20)      468 2023-02-28 09:05:59.000000 patchy-2.7.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1526 2023-06-16 15:01:49.607811 patchy-2.7.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:01:49.603919 patchy-2.7.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:01:49.605835 patchy-2.7.0/src/patchy/
--rw-r--r--   0 adamjohnson   (501) staff       (20)       63 2022-06-03 11:59:50.000000 patchy-2.7.0/src/patchy/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)    10653 2023-01-16 13:52:56.000000 patchy-2.7.0/src/patchy/api.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1044 2022-06-03 11:59:50.000000 patchy-2.7.0/src/patchy/cache.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:50.000000 patchy-2.7.0/src/patchy/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:01:49.606593 patchy-2.7.0/src/patchy.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    10451 2023-06-16 15:01:49.000000 patchy-2.7.0/src/patchy.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      505 2023-06-16 15:01:49.000000 patchy-2.7.0/src/patchy.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 15:01:49.000000 patchy-2.7.0/src/patchy.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-16 15:01:49.000000 patchy-2.7.0/src/patchy.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       48 2023-06-16 15:01:49.000000 patchy-2.7.0/src/patchy.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        7 2023-06-16 15:01:49.000000 patchy-2.7.0/src/patchy.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-16 15:01:49.607331 patchy-2.7.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      897 2022-06-03 11:59:50.000000 patchy-2.7.0/tests/test_cache.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)    20480 2023-01-16 15:18:18.000000 patchy-2.7.0/tests/test_patch.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1187 2022-11-04 11:16:35.000000 patchy-2.7.0/tests/test_patch_then_unpatch.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3098 2022-11-04 11:16:35.000000 patchy-2.7.0/tests/test_replace.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1540 2023-01-16 15:18:18.000000 patchy-2.7.0/tests/test_temp_patch.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1545 2023-01-16 13:50:50.000000 patchy-2.7.0/tests/test_unpatch.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 14:05:11.048174 patchy-2.8.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3230 2023-07-10 14:05:08.000000 patchy-2.8.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:50.000000 patchy-2.8.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      122 2023-01-20 12:10:00.000000 patchy-2.8.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    10401 2023-07-10 14:05:11.048254 patchy-2.8.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     9261 2023-07-10 14:04:51.000000 patchy-2.8.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    29870 2022-06-03 11:59:50.000000 patchy-2.8.0/pirate.png
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      468 2023-07-10 14:04:51.000000 patchy-2.8.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1487 2023-07-10 14:05:11.048564 patchy-2.8.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 14:05:11.043567 patchy-2.8.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 14:05:11.045773 patchy-2.8.0/src/patchy/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       63 2022-06-03 11:59:50.000000 patchy-2.8.0/src/patchy/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    10653 2023-01-16 13:52:56.000000 patchy-2.8.0/src/patchy/api.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1044 2022-06-03 11:59:50.000000 patchy-2.8.0/src/patchy/cache.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:50.000000 patchy-2.8.0/src/patchy/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 14:05:11.046628 patchy-2.8.0/src/patchy.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    10401 2023-07-10 14:05:11.000000 patchy-2.8.0/src/patchy.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      505 2023-07-10 14:05:11.000000 patchy-2.8.0/src/patchy.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 14:05:11.000000 patchy-2.8.0/src/patchy.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-07-10 14:05:10.000000 patchy-2.8.0/src/patchy.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       48 2023-07-10 14:05:11.000000 patchy-2.8.0/src/patchy.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        7 2023-07-10 14:05:11.000000 patchy-2.8.0/src/patchy.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-07-10 14:05:11.047956 patchy-2.8.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      897 2022-06-03 11:59:50.000000 patchy-2.8.0/tests/test_cache.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    20480 2023-01-16 15:18:18.000000 patchy-2.8.0/tests/test_patch.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1187 2022-11-04 11:16:35.000000 patchy-2.8.0/tests/test_patch_then_unpatch.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3098 2022-11-04 11:16:35.000000 patchy-2.8.0/tests/test_replace.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1540 2023-01-16 15:18:18.000000 patchy-2.8.0/tests/test_temp_patch.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1545 2023-01-16 13:50:50.000000 patchy-2.8.0/tests/test_unpatch.py
```

### Comparing `patchy-2.7.0/CHANGELOG.rst` & `patchy-2.8.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+2.8.0 (2023-07-10)
+------------------
+
+* Drop Python 3.7 support.
+
 2.7.0 (2023-06-16)
 ------------------
 
 * Support Python 3.12.
 
 2.6.1 (2023-01-16)
 ------------------
```

### Comparing `patchy-2.7.0/LICENSE` & `patchy-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `patchy-2.7.0/PKG-INFO` & `patchy-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchy
-Version: 2.7.0
+Version: 2.8.0
 Summary: Patch the inner source of python functions at runtime.
 Home-page: https://github.com/adamchainz/patchy
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/patchy/blob/main/CHANGELOG.rst
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
 
 ======
 Patchy
 ======
 
@@ -85,15 +84,15 @@
 
 Use **pip**:
 
 .. code-block:: bash
 
     python -m pip install patchy
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 ----
 
 **Hacking on a Django project?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
 
 ----
```

### Comparing `patchy-2.7.0/README.rst` & `patchy-2.8.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 Use **pip**:
 
 .. code-block:: bash
 
     python -m pip install patchy
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 ----
 
 **Hacking on a Django project?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
 
 ----
```

### Comparing `patchy-2.7.0/pirate.png` & `patchy-2.8.0/pirate.png`

 * *Files identical despite different names*

### Comparing `patchy-2.7.0/setup.cfg` & `patchy-2.8.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = patchy
-version = 2.7.0
+version = 2.8.0
 description = Patch the inner source of python functions at runtime.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/patchy
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
 keywords = patchy
@@ -30,15 +29,15 @@
 	Mastodon = https://fosstodon.org/@adamchainz
 	Twitter = https://twitter.com/adamchainz
 
 [options]
 packages = find:
 install_requires = 
 	pkgutil-resolve-name;python_version < "3.9"
-python_requires = >=3.7
+python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 zip_safe = False
 
 [options.packages.find]
 where = src
```

### Comparing `patchy-2.7.0/src/patchy/api.py` & `patchy-2.8.0/src/patchy/api.py`

 * *Files identical despite different names*

### Comparing `patchy-2.7.0/src/patchy/cache.py` & `patchy-2.8.0/src/patchy/cache.py`

 * *Files identical despite different names*

### Comparing `patchy-2.7.0/src/patchy.egg-info/PKG-INFO` & `patchy-2.8.0/src/patchy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchy
-Version: 2.7.0
+Version: 2.8.0
 Summary: Patch the inner source of python functions at runtime.
 Home-page: https://github.com/adamchainz/patchy
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/patchy/blob/main/CHANGELOG.rst
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
 
 ======
 Patchy
 ======
 
@@ -85,15 +84,15 @@
 
 Use **pip**:
 
 .. code-block:: bash
 
     python -m pip install patchy
 
-Python 3.7 to 3.12 supported.
+Python 3.8 to 3.12 supported.
 
 ----
 
 **Hacking on a Django project?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
 
 ----
```

### Comparing `patchy-2.7.0/tests/test_cache.py` & `patchy-2.8.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `patchy-2.7.0/tests/test_patch.py` & `patchy-2.8.0/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `patchy-2.7.0/tests/test_patch_then_unpatch.py` & `patchy-2.8.0/tests/test_patch_then_unpatch.py`

 * *Files identical despite different names*

### Comparing `patchy-2.7.0/tests/test_replace.py` & `patchy-2.8.0/tests/test_replace.py`

 * *Files identical despite different names*

### Comparing `patchy-2.7.0/tests/test_temp_patch.py` & `patchy-2.8.0/tests/test_temp_patch.py`

 * *Files identical despite different names*

### Comparing `patchy-2.7.0/tests/test_unpatch.py` & `patchy-2.8.0/tests/test_unpatch.py`

 * *Files identical despite different names*

