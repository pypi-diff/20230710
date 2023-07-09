# Comparing `tmp/trendalation-0.1.8.tar.gz` & `tmp/trendalation-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trendalation-0.1.8.tar", last modified: Sun Jul  9 22:04:54 2023, max compression
+gzip compressed data, was "trendalation-0.1.9.tar", last modified: Sun Jul  9 22:08:59 2023, max compression
```

## Comparing `trendalation-0.1.8.tar` & `trendalation-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-09 22:04:54.021059 trendalation-0.1.8/
--rw-r--r--   0 raghavsaboo   (501) staff       (20)     1084 2023-07-08 16:44:54.000000 trendalation-0.1.8/LICENSE.rst
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      550 2023-07-09 22:04:54.021135 trendalation-0.1.8/PKG-INFO
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      872 2023-07-08 16:44:54.000000 trendalation-0.1.8/README.md
--rw-r--r--   0 raghavsaboo   (501) staff       (20)       93 2023-07-08 17:30:19.000000 trendalation-0.1.8/pyproject.toml
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      107 2023-07-09 22:04:54.021359 trendalation-0.1.8/setup.cfg
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      801 2023-07-09 20:52:07.000000 trendalation-0.1.8/setup.py
-drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-09 22:04:54.018839 trendalation-0.1.8/trendalation/
-drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-09 22:04:54.020915 trendalation-0.1.8/trendalation/trendalation.egg-info/
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      550 2023-07-09 22:04:54.000000 trendalation-0.1.8/trendalation/trendalation.egg-info/PKG-INFO
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      299 2023-07-09 22:04:54.000000 trendalation-0.1.8/trendalation/trendalation.egg-info/SOURCES.txt
--rw-r--r--   0 raghavsaboo   (501) staff       (20)        1 2023-07-09 22:04:54.000000 trendalation-0.1.8/trendalation/trendalation.egg-info/dependency_links.txt
--rw-r--r--   0 raghavsaboo   (501) staff       (20)       25 2023-07-09 22:04:54.000000 trendalation-0.1.8/trendalation/trendalation.egg-info/requires.txt
--rw-r--r--   0 raghavsaboo   (501) staff       (20)        1 2023-07-09 22:04:54.000000 trendalation-0.1.8/trendalation/trendalation.egg-info/top_level.txt
+drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-09 22:08:59.426144 trendalation-0.1.9/
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)     1084 2023-07-08 16:44:54.000000 trendalation-0.1.9/LICENSE.rst
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      550 2023-07-09 22:08:59.426214 trendalation-0.1.9/PKG-INFO
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      872 2023-07-08 16:44:54.000000 trendalation-0.1.9/README.md
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)       93 2023-07-08 17:30:19.000000 trendalation-0.1.9/pyproject.toml
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      107 2023-07-09 22:08:59.426457 trendalation-0.1.9/setup.cfg
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      801 2023-07-09 22:08:49.000000 trendalation-0.1.9/setup.py
+drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-09 22:08:59.424298 trendalation-0.1.9/trendalation/
+drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-09 22:08:59.425995 trendalation-0.1.9/trendalation/trendalation.egg-info/
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      550 2023-07-09 22:08:59.000000 trendalation-0.1.9/trendalation/trendalation.egg-info/PKG-INFO
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      299 2023-07-09 22:08:59.000000 trendalation-0.1.9/trendalation/trendalation.egg-info/SOURCES.txt
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)        1 2023-07-09 22:08:59.000000 trendalation-0.1.9/trendalation/trendalation.egg-info/dependency_links.txt
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)       25 2023-07-09 22:08:59.000000 trendalation-0.1.9/trendalation/trendalation.egg-info/requires.txt
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)        1 2023-07-09 22:08:59.000000 trendalation-0.1.9/trendalation/trendalation.egg-info/top_level.txt
```

### Comparing `trendalation-0.1.8/LICENSE.rst` & `trendalation-0.1.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `trendalation-0.1.8/PKG-INFO` & `trendalation-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trendalation
-Version: 0.1.8
+Version: 0.1.9
 Home-page: https://github.com/kartikeysinha/trendalation
 Author: Raghav Saboo, Kartikey Sinha
 Author-email: raghs2000@gmail.com
 License: MIT
 Keywords: anomaly detection,procrustes,time-series,trends
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `trendalation-0.1.8/README.md` & `trendalation-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `trendalation-0.1.8/setup.py` & `trendalation-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='trendalation',
     package_dir={"": "trendalation"},
     packages=find_packages(where="trendalation"),
     python_requires=">=3.8",
-    version='0.1.8',
+    version='0.1.9',
     license='MIT',
     author="Raghav Saboo, Kartikey Sinha",
     author_email='raghs2000@gmail.com',
     url='https://github.com/kartikeysinha/trendalation',
     keywords=['anomaly detection', 'procrustes', 'time-series', 'trends'],
     install_requires=[
         'numpy',
```

### Comparing `trendalation-0.1.8/trendalation/trendalation.egg-info/PKG-INFO` & `trendalation-0.1.9/trendalation/trendalation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trendalation
-Version: 0.1.8
+Version: 0.1.9
 Home-page: https://github.com/kartikeysinha/trendalation
 Author: Raghav Saboo, Kartikey Sinha
 Author-email: raghs2000@gmail.com
 License: MIT
 Keywords: anomaly detection,procrustes,time-series,trends
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

