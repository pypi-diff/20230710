# Comparing `tmp/bayes_mapvar-0.0.1.tar.gz` & `tmp/bayes_mapvar-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayes_mapvar-0.0.1.tar", last modified: Mon Jul 10 03:42:11 2023, max compression
+gzip compressed data, was "bayes_mapvar-0.0.2.tar", last modified: Mon Jul 10 03:15:42 2023, max compression
```

## Comparing `bayes_mapvar-0.0.1.tar` & `bayes_mapvar-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 charles.lindsey   (501) staff       (20)        0 2023-07-10 03:42:11.635211 bayes_mapvar-0.0.1/
--rw-r--r--   0 charles.lindsey   (501) staff       (20)     1072 2023-07-09 23:43:24.000000 bayes_mapvar-0.0.1/LICENSE.txt
--rw-r--r--   0 charles.lindsey   (501) staff       (20)      696 2023-07-10 03:42:11.634931 bayes_mapvar-0.0.1/PKG-INFO
--rw-r--r--   0 charles.lindsey   (501) staff       (20)      397 2023-07-10 02:48:05.000000 bayes_mapvar-0.0.1/README.md
--rw-r--r--   0 charles.lindsey   (501) staff       (20)       87 2023-07-10 01:49:44.000000 bayes_mapvar-0.0.1/pyproject.toml
--rw-r--r--   0 charles.lindsey   (501) staff       (20)       38 2023-07-10 03:42:11.635308 bayes_mapvar-0.0.1/setup.cfg
--rw-r--r--   0 charles.lindsey   (501) staff       (20)      766 2023-07-10 03:39:34.000000 bayes_mapvar-0.0.1/setup.py
-drwxr-xr-x   0 charles.lindsey   (501) staff       (20)        0 2023-07-10 03:42:11.625446 bayes_mapvar-0.0.1/src/
-drwxr-xr-x   0 charles.lindsey   (501) staff       (20)        0 2023-07-10 03:42:11.631365 bayes_mapvar-0.0.1/src/bayes_mapvar/
--rw-r--r--   0 charles.lindsey   (501) staff       (20)      235 2023-07-10 01:25:37.000000 bayes_mapvar-0.0.1/src/bayes_mapvar/__init__.py
--rw-r--r--   0 charles.lindsey   (501) staff       (20)      137 2023-07-08 00:53:57.000000 bayes_mapvar-0.0.1/src/bayes_mapvar/exceptions.py
--rw-r--r--   0 charles.lindsey   (501) staff       (20)     9664 2023-07-10 01:24:51.000000 bayes_mapvar-0.0.1/src/bayes_mapvar/map_utils.py
--rw-r--r--   0 charles.lindsey   (501) staff       (20)     6191 2023-07-08 21:02:44.000000 bayes_mapvar-0.0.1/src/bayes_mapvar/mapvar.py
--rw-r--r--   0 charles.lindsey   (501) staff       (20)     4751 2023-07-07 22:42:06.000000 bayes_mapvar-0.0.1/src/bayes_mapvar/var_utils.py
-drwxr-xr-x   0 charles.lindsey   (501) staff       (20)        0 2023-07-10 03:42:11.633486 bayes_mapvar-0.0.1/src/bayes_mapvar.egg-info/
--rw-r--r--   0 charles.lindsey   (501) staff       (20)      696 2023-07-10 03:42:11.000000 bayes_mapvar-0.0.1/src/bayes_mapvar.egg-info/PKG-INFO
--rw-r--r--   0 charles.lindsey   (501) staff       (20)      411 2023-07-10 03:42:11.000000 bayes_mapvar-0.0.1/src/bayes_mapvar.egg-info/SOURCES.txt
--rw-r--r--   0 charles.lindsey   (501) staff       (20)        1 2023-07-10 03:42:11.000000 bayes_mapvar-0.0.1/src/bayes_mapvar.egg-info/dependency_links.txt
--rw-r--r--   0 charles.lindsey   (501) staff       (20)      192 2023-07-10 03:42:11.000000 bayes_mapvar-0.0.1/src/bayes_mapvar.egg-info/requires.txt
--rw-r--r--   0 charles.lindsey   (501) staff       (20)       13 2023-07-10 03:42:11.000000 bayes_mapvar-0.0.1/src/bayes_mapvar.egg-info/top_level.txt
-drwxr-xr-x   0 charles.lindsey   (501) staff       (20)        0 2023-07-10 03:42:11.633794 bayes_mapvar-0.0.1/tests/
--rw-r--r--   0 charles.lindsey   (501) staff       (20)      842 2023-07-07 22:14:23.000000 bayes_mapvar-0.0.1/tests/test_utils.py
+drwxr-xr-x   0 charles.lindsey   (501) staff       (20)        0 2023-07-10 03:15:42.201526 bayes_mapvar-0.0.2/
+-rw-r--r--   0 charles.lindsey   (501) staff       (20)     1072 2023-07-09 23:43:24.000000 bayes_mapvar-0.0.2/LICENSE.txt
+-rw-r--r--   0 charles.lindsey   (501) staff       (20)      696 2023-07-10 03:15:42.201276 bayes_mapvar-0.0.2/PKG-INFO
+-rw-r--r--   0 charles.lindsey   (501) staff       (20)      397 2023-07-10 02:48:05.000000 bayes_mapvar-0.0.2/README.md
+-rw-r--r--   0 charles.lindsey   (501) staff       (20)       87 2023-07-10 01:49:44.000000 bayes_mapvar-0.0.2/pyproject.toml
+-rw-r--r--   0 charles.lindsey   (501) staff       (20)       38 2023-07-10 03:15:42.201614 bayes_mapvar-0.0.2/setup.cfg
+-rw-r--r--   0 charles.lindsey   (501) staff       (20)      766 2023-07-10 03:04:54.000000 bayes_mapvar-0.0.2/setup.py
+drwxr-xr-x   0 charles.lindsey   (501) staff       (20)        0 2023-07-10 03:15:42.192680 bayes_mapvar-0.0.2/src/
+drwxr-xr-x   0 charles.lindsey   (501) staff       (20)        0 2023-07-10 03:15:42.198096 bayes_mapvar-0.0.2/src/bayes_mapvar/
+-rw-r--r--   0 charles.lindsey   (501) staff       (20)      235 2023-07-10 01:25:37.000000 bayes_mapvar-0.0.2/src/bayes_mapvar/__init__.py
+-rw-r--r--   0 charles.lindsey   (501) staff       (20)      137 2023-07-08 00:53:57.000000 bayes_mapvar-0.0.2/src/bayes_mapvar/exceptions.py
+-rw-r--r--   0 charles.lindsey   (501) staff       (20)     9664 2023-07-10 01:24:51.000000 bayes_mapvar-0.0.2/src/bayes_mapvar/map_utils.py
+-rw-r--r--   0 charles.lindsey   (501) staff       (20)     6191 2023-07-08 21:02:44.000000 bayes_mapvar-0.0.2/src/bayes_mapvar/mapvar.py
+-rw-r--r--   0 charles.lindsey   (501) staff       (20)     4751 2023-07-07 22:42:06.000000 bayes_mapvar-0.0.2/src/bayes_mapvar/var_utils.py
+drwxr-xr-x   0 charles.lindsey   (501) staff       (20)        0 2023-07-10 03:15:42.200139 bayes_mapvar-0.0.2/src/bayes_mapvar.egg-info/
+-rw-r--r--   0 charles.lindsey   (501) staff       (20)      696 2023-07-10 03:15:42.000000 bayes_mapvar-0.0.2/src/bayes_mapvar.egg-info/PKG-INFO
+-rw-r--r--   0 charles.lindsey   (501) staff       (20)      411 2023-07-10 03:15:42.000000 bayes_mapvar-0.0.2/src/bayes_mapvar.egg-info/SOURCES.txt
+-rw-r--r--   0 charles.lindsey   (501) staff       (20)        1 2023-07-10 03:15:42.000000 bayes_mapvar-0.0.2/src/bayes_mapvar.egg-info/dependency_links.txt
+-rw-r--r--   0 charles.lindsey   (501) staff       (20)      192 2023-07-10 03:15:42.000000 bayes_mapvar-0.0.2/src/bayes_mapvar.egg-info/requires.txt
+-rw-r--r--   0 charles.lindsey   (501) staff       (20)       13 2023-07-10 03:15:42.000000 bayes_mapvar-0.0.2/src/bayes_mapvar.egg-info/top_level.txt
+drwxr-xr-x   0 charles.lindsey   (501) staff       (20)        0 2023-07-10 03:15:42.200421 bayes_mapvar-0.0.2/tests/
+-rw-r--r--   0 charles.lindsey   (501) staff       (20)      842 2023-07-07 22:14:23.000000 bayes_mapvar-0.0.2/tests/test_utils.py
```

### Comparing `bayes_mapvar-0.0.1/LICENSE.txt` & `bayes_mapvar-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bayes_mapvar-0.0.1/PKG-INFO` & `bayes_mapvar-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayes_mapvar
-Version: 0.0.1
+Version: 0.0.2
 Summary: Bayesian Maximum a Posteriori/Variance estimation
 Home-page: UNKNOWN
 Author: Charles Lindsey
 Author-email: lindseycster@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `bayes_mapvar-0.0.1/setup.py` & `bayes_mapvar-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='bayes_mapvar',
     description='Bayesian Maximum a Posteriori/Variance estimation',
-    version='0.0.1',
+    version='0.0.2',
     author='Charles Lindsey',
     author_email='lindseycster@gmail.com',
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(where='src', exclude=['tests', 'tests.*']),
     package_dir={'': 'src'},
     install_requires=_load_requirements(),
```

### Comparing `bayes_mapvar-0.0.1/src/bayes_mapvar/map_utils.py` & `bayes_mapvar-0.0.2/src/bayes_mapvar/map_utils.py`

 * *Files identical despite different names*

### Comparing `bayes_mapvar-0.0.1/src/bayes_mapvar/mapvar.py` & `bayes_mapvar-0.0.2/src/bayes_mapvar/mapvar.py`

 * *Files identical despite different names*

### Comparing `bayes_mapvar-0.0.1/src/bayes_mapvar/var_utils.py` & `bayes_mapvar-0.0.2/src/bayes_mapvar/var_utils.py`

 * *Files identical despite different names*

### Comparing `bayes_mapvar-0.0.1/src/bayes_mapvar.egg-info/PKG-INFO` & `bayes_mapvar-0.0.2/src/bayes_mapvar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayes-mapvar
-Version: 0.0.1
+Version: 0.0.2
 Summary: Bayesian Maximum a Posteriori/Variance estimation
 Home-page: UNKNOWN
 Author: Charles Lindsey
 Author-email: lindseycster@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `bayes_mapvar-0.0.1/tests/test_utils.py` & `bayes_mapvar-0.0.2/tests/test_utils.py`

 * *Files identical despite different names*

