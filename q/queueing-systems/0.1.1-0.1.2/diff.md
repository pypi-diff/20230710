# Comparing `tmp/queueing_systems-0.1.1.tar.gz` & `tmp/queueing_systems-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "queueing_systems-0.1.1.tar", last modified: Mon Jul 10 19:26:37 2023, max compression
+gzip compressed data, was "queueing_systems-0.1.2.tar", last modified: Mon Jul 10 19:56:05 2023, max compression
```

## Comparing `queueing_systems-0.1.1.tar` & `queueing_systems-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 paulius    (501) staff       (20)        0 2023-07-10 19:26:36.000000 queueing_systems-0.1.1/
--rw-r--r--   0 paulius    (501) staff       (20)     1067 2023-07-10 00:45:03.000000 queueing_systems-0.1.1/LICENSE
--rw-r--r--   0 paulius    (501) staff       (20)     1159 2023-07-10 19:26:37.000000 queueing_systems-0.1.1/PKG-INFO
--rw-r--r--   0 paulius    (501) staff       (20)      537 2023-07-10 01:30:32.000000 queueing_systems-0.1.1/README.md
-drwxr-xr-x   0 paulius    (501) staff       (20)        0 2023-07-10 19:26:36.000000 queueing_systems-0.1.1/queueing_systems/
--rw-r--r--   0 paulius    (501) staff       (20)        0 2023-07-10 00:34:09.000000 queueing_systems-0.1.1/queueing_systems/__init__.py
--rw-r--r--   0 paulius    (501) staff       (20)    12465 2023-07-10 15:25:12.000000 queueing_systems-0.1.1/queueing_systems/functions.py
-drwxr-xr-x   0 paulius    (501) staff       (20)        0 2023-07-10 19:26:36.000000 queueing_systems-0.1.1/queueing_systems.egg-info/
--rw-r--r--   0 paulius    (501) staff       (20)     1159 2023-07-10 19:26:36.000000 queueing_systems-0.1.1/queueing_systems.egg-info/PKG-INFO
--rw-r--r--   0 paulius    (501) staff       (20)      284 2023-07-10 19:26:36.000000 queueing_systems-0.1.1/queueing_systems.egg-info/SOURCES.txt
--rw-r--r--   0 paulius    (501) staff       (20)        1 2023-07-10 19:26:36.000000 queueing_systems-0.1.1/queueing_systems.egg-info/dependency_links.txt
--rw-r--r--   0 paulius    (501) staff       (20)       24 2023-07-10 19:26:36.000000 queueing_systems-0.1.1/queueing_systems.egg-info/requires.txt
--rw-r--r--   0 paulius    (501) staff       (20)       17 2023-07-10 19:26:36.000000 queueing_systems-0.1.1/queueing_systems.egg-info/top_level.txt
--rw-r--r--   0 paulius    (501) staff       (20)       38 2023-07-10 19:26:37.000000 queueing_systems-0.1.1/setup.cfg
--rw-r--r--   0 paulius    (501) staff       (20)      902 2023-07-10 19:26:27.000000 queueing_systems-0.1.1/setup.py
+drwxr-xr-x   0 paulius    (501) staff       (20)        0 2023-07-10 19:56:04.000000 queueing_systems-0.1.2/
+-rw-r--r--   0 paulius    (501) staff       (20)     1067 2023-07-10 00:45:03.000000 queueing_systems-0.1.2/LICENSE
+-rw-r--r--   0 paulius    (501) staff       (20)     1159 2023-07-10 19:56:05.000000 queueing_systems-0.1.2/PKG-INFO
+-rw-r--r--   0 paulius    (501) staff       (20)      537 2023-07-10 01:30:32.000000 queueing_systems-0.1.2/README.md
+drwxr-xr-x   0 paulius    (501) staff       (20)        0 2023-07-10 19:56:04.000000 queueing_systems-0.1.2/queueing_systems/
+-rw-r--r--   0 paulius    (501) staff       (20)       24 2023-07-10 19:51:04.000000 queueing_systems-0.1.2/queueing_systems/__init__.py
+-rw-r--r--   0 paulius    (501) staff       (20)    12465 2023-07-10 15:25:12.000000 queueing_systems-0.1.2/queueing_systems/functions.py
+drwxr-xr-x   0 paulius    (501) staff       (20)        0 2023-07-10 19:56:04.000000 queueing_systems-0.1.2/queueing_systems.egg-info/
+-rw-r--r--   0 paulius    (501) staff       (20)     1159 2023-07-10 19:56:04.000000 queueing_systems-0.1.2/queueing_systems.egg-info/PKG-INFO
+-rw-r--r--   0 paulius    (501) staff       (20)      284 2023-07-10 19:56:04.000000 queueing_systems-0.1.2/queueing_systems.egg-info/SOURCES.txt
+-rw-r--r--   0 paulius    (501) staff       (20)        1 2023-07-10 19:56:04.000000 queueing_systems-0.1.2/queueing_systems.egg-info/dependency_links.txt
+-rw-r--r--   0 paulius    (501) staff       (20)       24 2023-07-10 19:56:04.000000 queueing_systems-0.1.2/queueing_systems.egg-info/requires.txt
+-rw-r--r--   0 paulius    (501) staff       (20)       17 2023-07-10 19:56:04.000000 queueing_systems-0.1.2/queueing_systems.egg-info/top_level.txt
+-rw-r--r--   0 paulius    (501) staff       (20)       38 2023-07-10 19:56:05.000000 queueing_systems-0.1.2/setup.cfg
+-rw-r--r--   0 paulius    (501) staff       (20)      902 2023-07-10 19:45:11.000000 queueing_systems-0.1.2/setup.py
```

### Comparing `queueing_systems-0.1.1/LICENSE` & `queueing_systems-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `queueing_systems-0.1.1/PKG-INFO` & `queueing_systems-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queueing_systems
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for queueing system parameter estimation using queueing theory
 Home-page: https://github.com/pauterv/queueing_systems
 Author: Paulius Tervydis
 Author-email: Paulius.Tervydis@ktu.lt
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `queueing_systems-0.1.1/README.md` & `queueing_systems-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `queueing_systems-0.1.1/queueing_systems/functions.py` & `queueing_systems-0.1.2/queueing_systems/functions.py`

 * *Files identical despite different names*

### Comparing `queueing_systems-0.1.1/queueing_systems.egg-info/PKG-INFO` & `queueing_systems-0.1.2/queueing_systems.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queueing-systems
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for queueing system parameter estimation using queueing theory
 Home-page: https://github.com/pauterv/queueing_systems
 Author: Paulius Tervydis
 Author-email: Paulius.Tervydis@ktu.lt
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `queueing_systems-0.1.1/setup.py` & `queueing_systems-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='queueing_systems',
-    version='0.1.1',
+    version='0.1.2',
     author='Paulius Tervydis',
     author_email='Paulius.Tervydis@ktu.lt',
     description='Python package for queueing system parameter estimation using queueing theory',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/pauterv/queueing_systems',
     packages=['queueing_systems'],
```

