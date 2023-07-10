# Comparing `tmp/krakatoa-0.0.6.post1.tar.gz` & `tmp/krakatoa-0.0.6.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krakatoa-0.0.6.post1.tar", last modified: Wed Jul  5 18:18:26 2023, max compression
+gzip compressed data, was "krakatoa-0.0.6.post2.tar", last modified: Mon Jul 10 20:08:00 2023, max compression
```

## Comparing `krakatoa-0.0.6.post1.tar` & `krakatoa-0.0.6.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:18:26.504647 krakatoa-0.0.6.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-05 18:18:26.504647 krakatoa-0.0.6.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:18:26.504647 krakatoa-0.0.6.post1/krakatoa/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:18:26.504647 krakatoa-0.0.6.post1/krakatoa/future/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/future/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/future/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/future/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/future/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/future/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:18:26.504647 krakatoa-0.0.6.post1/krakatoa/models/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28354 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/models/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/models/_getmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/models/_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/models/autotune.py
--rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/models/quick.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:18:26.504647 krakatoa-0.0.6.post1/krakatoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-05 18:18:26.000000 krakatoa-0.0.6.post1/krakatoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-05 18:18:26.000000 krakatoa-0.0.6.post1/krakatoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:18:26.000000 krakatoa-0.0.6.post1/krakatoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-05 18:18:26.000000 krakatoa-0.0.6.post1/krakatoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 18:18:26.000000 krakatoa-0.0.6.post1/krakatoa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-05 18:18:26.504647 krakatoa-0.0.6.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:08:00.348557 krakatoa-0.0.6.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-10 20:08:00.348557 krakatoa-0.0.6.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:08:00.348557 krakatoa-0.0.6.post2/krakatoa/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:08:00.348557 krakatoa-0.0.6.post2/krakatoa/future/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/future/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/future/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/future/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/future/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/future/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:08:00.348557 krakatoa-0.0.6.post2/krakatoa/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28354 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/models/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/models/_getmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/models/_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/models/autotune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/models/quick.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:08:00.348557 krakatoa-0.0.6.post2/krakatoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-10 20:08:00.000000 krakatoa-0.0.6.post2/krakatoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-10 20:08:00.000000 krakatoa-0.0.6.post2/krakatoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:08:00.000000 krakatoa-0.0.6.post2/krakatoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-10 20:08:00.000000 krakatoa-0.0.6.post2/krakatoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 20:08:00.000000 krakatoa-0.0.6.post2/krakatoa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-10 20:08:00.348557 krakatoa-0.0.6.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/setup.py
```

### Comparing `krakatoa-0.0.6.post1/LICENSE` & `krakatoa-0.0.6.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post1/PKG-INFO` & `krakatoa-0.0.6.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: krakatoa
-Version: 0.0.6.post1
+Version: 0.0.6.post2
 Summary: Machine Learning high level package.
 Home-page: https://github.com/aitec-mp/krakatoa
-Download-URL: https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post1.tar.gz
+Download-URL: https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post2.tar.gz
 Author: Matheus de Prá Andrade
 Author-email: mpandrade@ucs.br
 License: MIT
 Keywords: krakatoa,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `krakatoa-0.0.6.post1/krakatoa/future/analysis.py` & `krakatoa-0.0.6.post2/krakatoa/future/analysis.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post1/krakatoa/future/evaluate.py` & `krakatoa-0.0.6.post2/krakatoa/future/evaluate.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post1/krakatoa/future/experiment.py` & `krakatoa-0.0.6.post2/krakatoa/future/experiment.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post1/krakatoa/future/preprocess.py` & `krakatoa-0.0.6.post2/krakatoa/future/preprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -290,7 +290,24 @@
             return True
         except Exception as e:
             print(e)
             return False
        
     def setTarget(self, target):
         self.target = target
+
+    def consistFormat(self, target='mongodb'):
+
+        if target == 'mongodb':
+
+            # Check for NaT values in 
+            for col in self.datetime_cols:
+                if self.dataset[col].isnull().sum() > 0:
+                    self.dataset[col] = self.dataset[col].astype('object').where(self.dataset[col].notnull(), None)
+
+            # Transform dataframe to list and records
+            records = self.dataset.to_dict('records')
+
+            return records
+        
+        else:
+            raise ValueError('Not implemented!')
```

### Comparing `krakatoa-0.0.6.post1/krakatoa/models/_config.py` & `krakatoa-0.0.6.post2/krakatoa/models/_config.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post1/krakatoa/models/_getmodels.py` & `krakatoa-0.0.6.post2/krakatoa/models/_getmodels.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post1/krakatoa/models/_metrics.py` & `krakatoa-0.0.6.post2/krakatoa/models/_metrics.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post1/krakatoa/models/autotune.py` & `krakatoa-0.0.6.post2/krakatoa/models/autotune.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post1/krakatoa/models/quick.py` & `krakatoa-0.0.6.post2/krakatoa/models/quick.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post1/krakatoa.egg-info/PKG-INFO` & `krakatoa-0.0.6.post2/krakatoa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: krakatoa
-Version: 0.0.6.post1
+Version: 0.0.6.post2
 Summary: Machine Learning high level package.
 Home-page: https://github.com/aitec-mp/krakatoa
-Download-URL: https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post1.tar.gz
+Download-URL: https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post2.tar.gz
 Author: Matheus de Prá Andrade
 Author-email: mpandrade@ucs.br
 License: MIT
 Keywords: krakatoa,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `krakatoa-0.0.6.post1/krakatoa.egg-info/SOURCES.txt` & `krakatoa-0.0.6.post2/krakatoa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post1/setup.py` & `krakatoa-0.0.6.post2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 setup(
   name = 'krakatoa',       
   packages = ['krakatoa', 'krakatoa/models', 'krakatoa/future'],  
-  version = '0.0.6post1',      
+  version = '0.0.6post2',      
   license='MIT',        
   description = 'Machine Learning high level package.',  
   long_description='Machine Learning high level package.',  
   author = 'Matheus de Prá Andrade',              
   author_email = 'mpandrade@ucs.br',    
   url = 'https://github.com/aitec-mp/krakatoa',  
-  download_url = 'https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post1.tar.gz',    
+  download_url = 'https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post2.tar.gz',    
   keywords = ['krakatoa', 'machine learning'],  
   install_requires=[    
           'scikit-learn',
           'numpy',
           'pandas',
           'xgboost',
           'seaborn'
```

