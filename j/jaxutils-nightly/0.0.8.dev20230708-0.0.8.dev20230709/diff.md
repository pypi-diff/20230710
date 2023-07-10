# Comparing `tmp/jaxutils-nightly-0.0.8.dev20230708.tar.gz` & `tmp/jaxutils-nightly-0.0.8.dev20230709.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20230708.tar", last modified: Sat Jul  8 00:06:39 2023, max compression
+gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20230709.tar", last modified: Sun Jul  9 00:06:35 2023, max compression
```

## Comparing `jaxutils-nightly-0.0.8.dev20230708.tar` & `jaxutils-nightly-0.0.8.dev20230709.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-08 00:06:39.336575 jaxutils-nightly-0.0.8.dev20230708/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-07-08 00:06:39.336575 jaxutils-nightly-0.0.8.dev20230708/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3004 2023-07-08 00:06:31.000000 jaxutils-nightly-0.0.8.dev20230708/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-08 00:06:39.336575 jaxutils-nightly-0.0.8.dev20230708/jaxutils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2023-07-08 00:06:31.000000 jaxutils-nightly-0.0.8.dev20230708/jaxutils/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2023-07-08 00:06:39.336575 jaxutils-nightly-0.0.8.dev20230708/jaxutils/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2023-07-08 00:06:31.000000 jaxutils-nightly-0.0.8.dev20230708/jaxutils/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2023-07-08 00:06:31.000000 jaxutils-nightly-0.0.8.dev20230708/jaxutils/data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2023-07-08 00:06:31.000000 jaxutils-nightly-0.0.8.dev20230708/jaxutils/dict.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2023-07-08 00:06:31.000000 jaxutils-nightly-0.0.8.dev20230708/jaxutils/parameters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2023-07-08 00:06:31.000000 jaxutils-nightly-0.0.8.dev20230708/jaxutils/pytree.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-08 00:06:39.336575 jaxutils-nightly-0.0.8.dev20230708/jaxutils_nightly.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-07-08 00:06:39.000000 jaxutils-nightly-0.0.8.dev20230708/jaxutils_nightly.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-07-08 00:06:39.000000 jaxutils-nightly-0.0.8.dev20230708/jaxutils_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-08 00:06:39.000000 jaxutils-nightly-0.0.8.dev20230708/jaxutils_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-07-08 00:06:39.000000 jaxutils-nightly-0.0.8.dev20230708/jaxutils_nightly.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-07-08 00:06:39.000000 jaxutils-nightly-0.0.8.dev20230708/jaxutils_nightly.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2023-07-08 00:06:39.336575 jaxutils-nightly-0.0.8.dev20230708/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-07-08 00:06:31.000000 jaxutils-nightly-0.0.8.dev20230708/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2023-07-08 00:06:31.000000 jaxutils-nightly-0.0.8.dev20230708/versioneer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-09 00:06:35.968086 jaxutils-nightly-0.0.8.dev20230709/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-07-09 00:06:35.968086 jaxutils-nightly-0.0.8.dev20230709/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3004 2023-07-09 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230709/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-09 00:06:35.968086 jaxutils-nightly-0.0.8.dev20230709/jaxutils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2023-07-09 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230709/jaxutils/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2023-07-09 00:06:35.968086 jaxutils-nightly-0.0.8.dev20230709/jaxutils/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2023-07-09 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230709/jaxutils/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2023-07-09 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230709/jaxutils/data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2023-07-09 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230709/jaxutils/dict.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2023-07-09 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230709/jaxutils/parameters.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2023-07-09 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230709/jaxutils/pytree.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-09 00:06:35.964086 jaxutils-nightly-0.0.8.dev20230709/jaxutils_nightly.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-07-09 00:06:35.000000 jaxutils-nightly-0.0.8.dev20230709/jaxutils_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-07-09 00:06:35.000000 jaxutils-nightly-0.0.8.dev20230709/jaxutils_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-09 00:06:35.000000 jaxutils-nightly-0.0.8.dev20230709/jaxutils_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-07-09 00:06:35.000000 jaxutils-nightly-0.0.8.dev20230709/jaxutils_nightly.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-07-09 00:06:35.000000 jaxutils-nightly-0.0.8.dev20230709/jaxutils_nightly.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2023-07-09 00:06:35.968086 jaxutils-nightly-0.0.8.dev20230709/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-07-09 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230709/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2023-07-09 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230709/versioneer.py
```

### Comparing `jaxutils-nightly-0.0.8.dev20230708/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20230709/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20230708
+Version: 0.0.8.dev20230709
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20230708/README.md` & `jaxutils-nightly-0.0.8.dev20230709/README.md`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230708/jaxutils/__init__.py` & `jaxutils-nightly-0.0.8.dev20230709/jaxutils/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230708/jaxutils/config.py` & `jaxutils-nightly-0.0.8.dev20230709/jaxutils/config.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230708/jaxutils/data.py` & `jaxutils-nightly-0.0.8.dev20230709/jaxutils/data.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230708/jaxutils/dict.py` & `jaxutils-nightly-0.0.8.dev20230709/jaxutils/dict.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230708/jaxutils/parameters.py` & `jaxutils-nightly-0.0.8.dev20230709/jaxutils/parameters.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230708/jaxutils/pytree.py` & `jaxutils-nightly-0.0.8.dev20230709/jaxutils/pytree.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230708/jaxutils_nightly.egg-info/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20230709/jaxutils_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20230708
+Version: 0.0.8.dev20230709
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20230708/setup.py` & `jaxutils-nightly-0.0.8.dev20230709/setup.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230708/versioneer.py` & `jaxutils-nightly-0.0.8.dev20230709/versioneer.py`

 * *Files identical despite different names*

