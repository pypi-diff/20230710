# Comparing `tmp/pyMapVBVD-0.5.3.tar.gz` & `tmp/pyMapVBVD-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyMapVBVD-0.5.3.tar", last modified: Fri Jul  7 12:53:52 2023, max compression
+gzip compressed data, was "pyMapVBVD-0.5.4.tar", last modified: Mon Jul 10 07:42:46 2023, max compression
```

## Comparing `pyMapVBVD-0.5.3.tar` & `pyMapVBVD-0.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:53:52.881327 pyMapVBVD-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-07 12:53:52.881327 pyMapVBVD-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:53:52.881327 pyMapVBVD-0.5.3/mapvbvd/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/mapvbvd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17996 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/mapvbvd/_attrdict.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 12:53:52.881327 pyMapVBVD-0.5.3/mapvbvd/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    23055 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/mapvbvd/mapVBVD.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/mapvbvd/read_twix_hdr.py
--rw-r--r--   0 runner    (1001) docker     (123)    38649 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/mapvbvd/twix_map_obj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:53:52.877327 pyMapVBVD-0.5.3/pyMapVBVD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-07 12:53:52.000000 pyMapVBVD-0.5.3/pyMapVBVD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-07 12:53:52.000000 pyMapVBVD-0.5.3/pyMapVBVD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:53:52.000000 pyMapVBVD-0.5.3/pyMapVBVD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-07 12:53:52.000000 pyMapVBVD-0.5.3/pyMapVBVD.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-07 12:53:52.000000 pyMapVBVD-0.5.3/pyMapVBVD.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-07 12:53:52.881327 pyMapVBVD-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:53:52.881327 pyMapVBVD-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-07 12:53:36.000000 pyMapVBVD-0.5.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-07 12:53:38.000000 pyMapVBVD-0.5.3/tests/test_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-07 12:53:38.000000 pyMapVBVD-0.5.3/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-07 12:53:38.000000 pyMapVBVD-0.5.3/tests/test_slicing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-07 12:53:38.000000 pyMapVBVD-0.5.3/tests/test_svs.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-07-07 12:53:38.000000 pyMapVBVD-0.5.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:42:46.105472 pyMapVBVD-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-10 07:42:34.000000 pyMapVBVD-0.5.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-10 07:42:34.000000 pyMapVBVD-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-10 07:42:34.000000 pyMapVBVD-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-10 07:42:46.105472 pyMapVBVD-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-10 07:42:34.000000 pyMapVBVD-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:42:46.105472 pyMapVBVD-0.5.4/mapvbvd/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-10 07:42:34.000000 pyMapVBVD-0.5.4/mapvbvd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17996 2023-07-10 07:42:34.000000 pyMapVBVD-0.5.4/mapvbvd/_attrdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-10 07:42:46.105472 pyMapVBVD-0.5.4/mapvbvd/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23055 2023-07-10 07:42:34.000000 pyMapVBVD-0.5.4/mapvbvd/mapVBVD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-07-10 07:42:34.000000 pyMapVBVD-0.5.4/mapvbvd/read_twix_hdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38649 2023-07-10 07:42:34.000000 pyMapVBVD-0.5.4/mapvbvd/twix_map_obj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:42:46.105472 pyMapVBVD-0.5.4/pyMapVBVD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-10 07:42:46.000000 pyMapVBVD-0.5.4/pyMapVBVD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-10 07:42:46.000000 pyMapVBVD-0.5.4/pyMapVBVD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 07:42:46.000000 pyMapVBVD-0.5.4/pyMapVBVD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 07:42:46.000000 pyMapVBVD-0.5.4/pyMapVBVD.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 07:42:46.000000 pyMapVBVD-0.5.4/pyMapVBVD.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-10 07:42:34.000000 pyMapVBVD-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 07:42:34.000000 pyMapVBVD-0.5.4/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-10 07:42:46.105472 pyMapVBVD-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-10 07:42:34.000000 pyMapVBVD-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:42:46.105472 pyMapVBVD-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-10 07:42:35.000000 pyMapVBVD-0.5.4/tests/test_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-10 07:42:35.000000 pyMapVBVD-0.5.4/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-10 07:42:35.000000 pyMapVBVD-0.5.4/tests/test_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-10 07:42:35.000000 pyMapVBVD-0.5.4/tests/test_svs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-07-10 07:42:35.000000 pyMapVBVD-0.5.4/versioneer.py
```

### Comparing `pyMapVBVD-0.5.3/LICENSE` & `pyMapVBVD-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyMapVBVD-0.5.3/PKG-INFO` & `pyMapVBVD-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyMapVBVD
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python twix file reader
 Home-page: https://github.com/wtclarke/pymapvbvd
 Author: Will Clarke
 Author-email: william.clarke@ndcn.ox.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyMapVBVD-0.5.3/README.md` & `pyMapVBVD-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pyMapVBVD-0.5.3/mapvbvd/_attrdict.py` & `pyMapVBVD-0.5.4/mapvbvd/_attrdict.py`

 * *Files identical despite different names*

### Comparing `pyMapVBVD-0.5.3/mapvbvd/mapVBVD.py` & `pyMapVBVD-0.5.4/mapvbvd/mapVBVD.py`

 * *Files identical despite different names*

### Comparing `pyMapVBVD-0.5.3/mapvbvd/read_twix_hdr.py` & `pyMapVBVD-0.5.4/mapvbvd/read_twix_hdr.py`

 * *Files identical despite different names*

### Comparing `pyMapVBVD-0.5.3/mapvbvd/twix_map_obj.py` & `pyMapVBVD-0.5.4/mapvbvd/twix_map_obj.py`

 * *Files identical despite different names*

### Comparing `pyMapVBVD-0.5.3/pyMapVBVD.egg-info/PKG-INFO` & `pyMapVBVD-0.5.4/pyMapVBVD.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyMapVBVD
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python twix file reader
 Home-page: https://github.com/wtclarke/pymapvbvd
 Author: Will Clarke
 Author-email: william.clarke@ndcn.ox.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyMapVBVD-0.5.3/setup.py` & `pyMapVBVD-0.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     cmdclass=versioneer.get_cmdclass(),
     description='Python twix file reader',
     author='Will Clarke',
     author_email='william.clarke@ndcn.ox.ac.uk',
     url='https://github.com/wtclarke/pymapvbvd',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_packages(exclude=["tests*"]),
     install_requires=install_requires,
     extras_require={"tests": ['pytest', ]},
     license_file='LICENSE',
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

### Comparing `pyMapVBVD-0.5.3/tests/test_flags.py` & `pyMapVBVD-0.5.4/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `pyMapVBVD-0.5.3/tests/test_read.py` & `pyMapVBVD-0.5.4/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `pyMapVBVD-0.5.3/tests/test_slicing.py` & `pyMapVBVD-0.5.4/tests/test_slicing.py`

 * *Files identical despite different names*

### Comparing `pyMapVBVD-0.5.3/tests/test_svs.py` & `pyMapVBVD-0.5.4/tests/test_svs.py`

 * *Files identical despite different names*

### Comparing `pyMapVBVD-0.5.3/versioneer.py` & `pyMapVBVD-0.5.4/versioneer.py`

 * *Files identical despite different names*

