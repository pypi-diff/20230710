# Comparing `tmp/hds-stats-0.3.0.tar.gz` & `tmp/hds-stats-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hds-stats-0.3.0.tar", last modified: Mon Jul 10 05:31:45 2023, max compression
+gzip compressed data, was "hds-stats-0.3.1.tar", last modified: Mon Jul 10 06:14:46 2023, max compression
```

## Comparing `hds-stats-0.3.0.tar` & `hds-stats-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 05:31:45.161097 hds-stats-0.3.0/
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.3.0/LICENSE
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-10 05:31:45.160854 hds-stats-0.3.0/PKG-INFO
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.3.0/README.md
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 05:31:45.158518 hds-stats-0.3.0/hds_stats/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       82 2023-04-09 20:34:59.000000 hds-stats-0.3.0/hds_stats/__init__.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     9625 2023-07-10 05:27:45.000000 hds-stats-0.3.0/hds_stats/ml.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    11955 2023-06-18 16:25:20.000000 hds-stats-0.3.0/hds_stats/plot.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    27195 2023-06-18 16:48:47.000000 hds-stats-0.3.0/hds_stats/stat.py
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 05:31:45.160479 hds-stats-0.3.0/hds_stats.egg-info/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-10 05:31:45.000000 hds-stats-0.3.0/hds_stats.egg-info/PKG-INFO
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      279 2023-07-10 05:31:45.000000 hds-stats-0.3.0/hds_stats.egg-info/SOURCES.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-07-10 05:31:45.000000 hds-stats-0.3.0/hds_stats.egg-info/dependency_links.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       72 2023-07-10 05:31:45.000000 hds-stats-0.3.0/hds_stats.egg-info/requires.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-07-10 05:31:45.000000 hds-stats-0.3.0/hds_stats.egg-info/top_level.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.3.0/pyproject.toml
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-07-10 05:31:45.161194 hds-stats-0.3.0/setup.cfg
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     1199 2023-07-10 05:29:41.000000 hds-stats-0.3.0/setup.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:14:46.273087 hds-stats-0.3.1/
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.3.1/LICENSE
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-10 06:14:46.272845 hds-stats-0.3.1/PKG-INFO
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.3.1/README.md
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:14:46.270937 hds-stats-0.3.1/hds_stats/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      113 2023-07-10 06:13:09.000000 hds-stats-0.3.1/hds_stats/__init__.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     9625 2023-07-10 05:27:45.000000 hds-stats-0.3.1/hds_stats/ml.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    11955 2023-06-18 16:25:20.000000 hds-stats-0.3.1/hds_stats/plot.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    27195 2023-06-18 16:48:47.000000 hds-stats-0.3.1/hds_stats/stat.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:14:46.272472 hds-stats-0.3.1/hds_stats.egg-info/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-10 06:14:46.000000 hds-stats-0.3.1/hds_stats.egg-info/PKG-INFO
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      279 2023-07-10 06:14:46.000000 hds-stats-0.3.1/hds_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-07-10 06:14:46.000000 hds-stats-0.3.1/hds_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       72 2023-07-10 06:14:46.000000 hds-stats-0.3.1/hds_stats.egg-info/requires.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-07-10 06:14:46.000000 hds-stats-0.3.1/hds_stats.egg-info/top_level.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.3.1/pyproject.toml
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-07-10 06:14:46.273176 hds-stats-0.3.1/setup.cfg
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     1199 2023-07-10 06:13:22.000000 hds-stats-0.3.1/setup.py
```

### Comparing `hds-stats-0.3.0/LICENSE` & `hds-stats-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hds-stats-0.3.0/PKG-INFO` & `hds-stats-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.3.0
+Version: 0.3.1
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.3.0/hds_stats/ml.py` & `hds-stats-0.3.1/hds_stats/ml.py`

 * *Files identical despite different names*

### Comparing `hds-stats-0.3.0/hds_stats/plot.py` & `hds-stats-0.3.1/hds_stats/plot.py`

 * *Files identical despite different names*

### Comparing `hds-stats-0.3.0/hds_stats/stat.py` & `hds-stats-0.3.1/hds_stats/stat.py`

 * *Files identical despite different names*

### Comparing `hds-stats-0.3.0/hds_stats.egg-info/PKG-INFO` & `hds-stats-0.3.1/hds_stats.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.3.0
+Version: 0.3.1
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.3.0/setup.py` & `hds-stats-0.3.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 with open(file = 'README.md', mode = 'r', encoding = 'UTF-8') as file:
     long_description = file.read()
 
 setup(
     name = 'hds-stats',
-    version = '0.3.0',
+    version = '0.3.1',
     author = 'HelloDataScience',
     author_email = 'hellodatasciencekorea@gmail.com',
     
     description = 'Useful functions for Statistics and Machine Learning',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
```

