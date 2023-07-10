# Comparing `tmp/hds-stats-0.2.3.tar.gz` & `tmp/hds-stats-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hds-stats-0.2.3.tar", last modified: Sun Jun 18 16:49:46 2023, max compression
+gzip compressed data, was "hds-stats-0.3.0.tar", last modified: Mon Jul 10 05:31:45 2023, max compression
```

## Comparing `hds-stats-0.2.3.tar` & `hds-stats-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-06-18 16:49:46.260728 hds-stats-0.2.3/
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.2.3/LICENSE
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-06-18 16:49:46.260484 hds-stats-0.2.3/PKG-INFO
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.2.3/README.md
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-06-18 16:49:46.258219 hds-stats-0.2.3/hds_stats/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       82 2023-04-09 20:34:59.000000 hds-stats-0.2.3/hds_stats/__init__.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    11955 2023-06-18 16:25:20.000000 hds-stats-0.2.3/hds_stats/plot.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    27195 2023-06-18 16:48:47.000000 hds-stats-0.2.3/hds_stats/stat.py
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-06-18 16:49:46.260111 hds-stats-0.2.3/hds_stats.egg-info/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-06-18 16:49:46.000000 hds-stats-0.2.3/hds_stats.egg-info/PKG-INFO
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      263 2023-06-18 16:49:46.000000 hds-stats-0.2.3/hds_stats.egg-info/SOURCES.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-06-18 16:49:46.000000 hds-stats-0.2.3/hds_stats.egg-info/dependency_links.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       63 2023-06-18 16:49:46.000000 hds-stats-0.2.3/hds_stats.egg-info/requires.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-06-18 16:49:46.000000 hds-stats-0.2.3/hds_stats.egg-info/top_level.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.2.3/pyproject.toml
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-06-18 16:49:46.260815 hds-stats-0.2.3/setup.cfg
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     1178 2023-06-18 16:48:09.000000 hds-stats-0.2.3/setup.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 05:31:45.161097 hds-stats-0.3.0/
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.3.0/LICENSE
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-10 05:31:45.160854 hds-stats-0.3.0/PKG-INFO
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.3.0/README.md
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 05:31:45.158518 hds-stats-0.3.0/hds_stats/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       82 2023-04-09 20:34:59.000000 hds-stats-0.3.0/hds_stats/__init__.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     9625 2023-07-10 05:27:45.000000 hds-stats-0.3.0/hds_stats/ml.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    11955 2023-06-18 16:25:20.000000 hds-stats-0.3.0/hds_stats/plot.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    27195 2023-06-18 16:48:47.000000 hds-stats-0.3.0/hds_stats/stat.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 05:31:45.160479 hds-stats-0.3.0/hds_stats.egg-info/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-10 05:31:45.000000 hds-stats-0.3.0/hds_stats.egg-info/PKG-INFO
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      279 2023-07-10 05:31:45.000000 hds-stats-0.3.0/hds_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-07-10 05:31:45.000000 hds-stats-0.3.0/hds_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       72 2023-07-10 05:31:45.000000 hds-stats-0.3.0/hds_stats.egg-info/requires.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-07-10 05:31:45.000000 hds-stats-0.3.0/hds_stats.egg-info/top_level.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.3.0/pyproject.toml
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-07-10 05:31:45.161194 hds-stats-0.3.0/setup.cfg
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     1199 2023-07-10 05:29:41.000000 hds-stats-0.3.0/setup.py
```

### Comparing `hds-stats-0.2.3/LICENSE` & `hds-stats-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hds-stats-0.2.3/PKG-INFO` & `hds-stats-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.2.3
+Version: 0.3.0
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hds-stats
 Useful Functions for Statistics and Machine Learning
```

### Comparing `hds-stats-0.2.3/hds_stats/plot.py` & `hds-stats-0.3.0/hds_stats/plot.py`

 * *Files identical despite different names*

### Comparing `hds-stats-0.2.3/hds_stats/stat.py` & `hds-stats-0.3.0/hds_stats/stat.py`

 * *Files identical despite different names*

### Comparing `hds-stats-0.2.3/hds_stats.egg-info/PKG-INFO` & `hds-stats-0.3.0/hds_stats.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.2.3
+Version: 0.3.0
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hds-stats
 Useful Functions for Statistics and Machine Learning
```

### Comparing `hds-stats-0.2.3/setup.py` & `hds-stats-0.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 with open(file = 'README.md', mode = 'r', encoding = 'UTF-8') as file:
     long_description = file.read()
 
 setup(
     name = 'hds-stats',
-    version = '0.2.3',
+    version = '0.3.0',
     author = 'HelloDataScience',
     author_email = 'hellodatasciencekorea@gmail.com',
     
     description = 'Useful functions for Statistics and Machine Learning',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     
@@ -22,21 +22,22 @@
     license = 'MIT',
     classifiers = [
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     
-    python_requires = '>=3.6',
+    python_requires = '>=3.9',
     packages = find_packages(),
     package_dir = {'hds_stats': 'hds_stats'},
     py_modules = ['plot', 'stat'],
     install_requires = [
         'numpy', 
         'pandas', 
         'scipy', 
         'seaborn', 
         'matplotlib', 
         'statsmodels', 
-        'scikit-learn'
+        'scikit-learn', 
+        'graphviz'
     ],
 )
```

