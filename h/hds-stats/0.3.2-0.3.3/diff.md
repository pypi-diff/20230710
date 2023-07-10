# Comparing `tmp/hds-stats-0.3.2.tar.gz` & `tmp/hds-stats-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hds-stats-0.3.2.tar", last modified: Mon Jul 10 06:26:14 2023, max compression
+gzip compressed data, was "hds-stats-0.3.3.tar", last modified: Mon Jul 10 06:40:04 2023, max compression
```

## Comparing `hds-stats-0.3.2.tar` & `hds-stats-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:26:14.970065 hds-stats-0.3.2/
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.3.2/LICENSE
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-10 06:26:14.969794 hds-stats-0.3.2/PKG-INFO
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.3.2/README.md
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:26:14.967868 hds-stats-0.3.2/hds_stats/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      113 2023-07-10 06:13:09.000000 hds-stats-0.3.2/hds_stats/__init__.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     9586 2023-07-10 06:25:27.000000 hds-stats-0.3.2/hds_stats/ml.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    11955 2023-06-18 16:25:20.000000 hds-stats-0.3.2/hds_stats/plot.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    27195 2023-06-18 16:48:47.000000 hds-stats-0.3.2/hds_stats/stat.py
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:26:14.969405 hds-stats-0.3.2/hds_stats.egg-info/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-10 06:26:14.000000 hds-stats-0.3.2/hds_stats.egg-info/PKG-INFO
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      279 2023-07-10 06:26:14.000000 hds-stats-0.3.2/hds_stats.egg-info/SOURCES.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-07-10 06:26:14.000000 hds-stats-0.3.2/hds_stats.egg-info/dependency_links.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       72 2023-07-10 06:26:14.000000 hds-stats-0.3.2/hds_stats.egg-info/requires.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-07-10 06:26:14.000000 hds-stats-0.3.2/hds_stats.egg-info/top_level.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.3.2/pyproject.toml
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-07-10 06:26:14.970178 hds-stats-0.3.2/setup.cfg
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     1199 2023-07-10 06:25:39.000000 hds-stats-0.3.2/setup.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:40:04.166552 hds-stats-0.3.3/
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.3.3/LICENSE
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-10 06:40:04.166293 hds-stats-0.3.3/PKG-INFO
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.3.3/README.md
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:40:04.162988 hds-stats-0.3.3/hds_stats/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      113 2023-07-10 06:13:09.000000 hds-stats-0.3.3/hds_stats/__init__.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     9586 2023-07-10 06:25:27.000000 hds-stats-0.3.3/hds_stats/ml.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    11955 2023-06-18 16:25:20.000000 hds-stats-0.3.3/hds_stats/plot.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    27424 2023-07-10 06:38:52.000000 hds-stats-0.3.3/hds_stats/stat.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:40:04.165885 hds-stats-0.3.3/hds_stats.egg-info/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-10 06:40:04.000000 hds-stats-0.3.3/hds_stats.egg-info/PKG-INFO
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      279 2023-07-10 06:40:04.000000 hds-stats-0.3.3/hds_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-07-10 06:40:04.000000 hds-stats-0.3.3/hds_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       72 2023-07-10 06:40:04.000000 hds-stats-0.3.3/hds_stats.egg-info/requires.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-07-10 06:40:04.000000 hds-stats-0.3.3/hds_stats.egg-info/top_level.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.3.3/pyproject.toml
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-07-10 06:40:04.166650 hds-stats-0.3.3/setup.cfg
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     1199 2023-07-10 06:39:02.000000 hds-stats-0.3.3/setup.py
```

### Comparing `hds-stats-0.3.2/LICENSE` & `hds-stats-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hds-stats-0.3.2/PKG-INFO` & `hds-stats-0.3.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.3.2
+Version: 0.3.3
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.3.2/hds_stats/ml.py` & `hds-stats-0.3.3/hds_stats/ml.py`

 * *Files identical despite different names*

### Comparing `hds-stats-0.3.2/hds_stats/plot.py` & `hds-stats-0.3.3/hds_stats/plot.py`

 * *Files identical despite different names*

### Comparing `hds-stats-0.3.2/hds_stats/stat.py` & `hds-stats-0.3.3/hds_stats/stat.py`

 * *Files 1% similar despite different names*

```diff
@@ -609,26 +609,36 @@
     from sklearn.metrics import mean_absolute_percentage_error
     
     MSE = mean_squared_error(
         y_true = y_true, 
         y_pred = y_pred
     )
     
-    RMSE = MSE**(1/2)
+    RMSE = mean_squared_error(
+        y_true = y_true, 
+        y_pred = y_pred, 
+        squared = True
+    )
+    
+    minus_count = pd.Series(data = y_pred).lt(0).sum()
     
-    minus_count = y_pred.lt(0).sum()
     if minus_count > 0:
         MSLE = None
         RMSLE = None
     else:
         MSLE = mean_squared_log_error(
             y_true = y_true, 
             y_pred = y_pred
         )
-        RMSLE = MSLE ** (1/2)
+        
+        RMSLE = mean_squared_log_error(
+            y_true = y_true, 
+            y_pred = y_pred, 
+            squared = True
+        )
     
     MAE = mean_absolute_error(
         y_true = y_true, 
         y_pred = y_pred
     )
     
     MAPE = mean_absolute_percentage_error(
```

### Comparing `hds-stats-0.3.2/hds_stats.egg-info/PKG-INFO` & `hds-stats-0.3.3/hds_stats.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.3.2
+Version: 0.3.3
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.3.2/setup.py` & `hds-stats-0.3.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 with open(file = 'README.md', mode = 'r', encoding = 'UTF-8') as file:
     long_description = file.read()
 
 setup(
     name = 'hds-stats',
-    version = '0.3.2',
+    version = '0.3.3',
     author = 'HelloDataScience',
     author_email = 'hellodatasciencekorea@gmail.com',
     
     description = 'Useful functions for Statistics and Machine Learning',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
```

