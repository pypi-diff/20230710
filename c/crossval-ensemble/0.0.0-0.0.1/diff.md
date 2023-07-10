# Comparing `tmp/crossval_ensemble-0.0.0.tar.gz` & `tmp/crossval_ensemble-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossval_ensemble-0.0.0.tar", last modified: Mon Jul 10 08:46:12 2023, max compression
+gzip compressed data, was "crossval_ensemble-0.0.1.tar", last modified: Mon Jul 10 09:02:16 2023, max compression
```

## Comparing `crossval_ensemble-0.0.0.tar` & `crossval_ensemble-0.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 pa        (1000) pa        (1000)        0 2023-07-10 08:46:12.599448 crossval_ensemble-0.0.0/
--rw-rw-r--   0 pa        (1000) pa        (1000)     1516 2023-06-29 09:02:18.000000 crossval_ensemble-0.0.0/LICENSE
--rw-rw-r--   0 pa        (1000) pa        (1000)      457 2023-07-10 08:46:12.599448 crossval_ensemble-0.0.0/PKG-INFO
--rw-rw-r--   0 pa        (1000) pa        (1000)     1226 2023-07-07 16:06:51.000000 crossval_ensemble-0.0.0/README.md
-drwxrwxr-x   0 pa        (1000) pa        (1000)        0 2023-07-10 08:46:12.599448 crossval_ensemble-0.0.0/crossval_ensemble/
--rw-rw-r--   0 pa        (1000) pa        (1000)        0 2023-06-29 09:46:58.000000 crossval_ensemble-0.0.0/crossval_ensemble/__init__.py
--rw-rw-r--   0 pa        (1000) pa        (1000)     6414 2023-07-06 15:28:24.000000 crossval_ensemble-0.0.0/crossval_ensemble/crossval_pipeline.py
--rw-rw-r--   0 pa        (1000) pa        (1000)     3964 2023-06-30 13:58:02.000000 crossval_ensemble-0.0.0/crossval_ensemble/custom_pipeline.py
--rw-rw-r--   0 pa        (1000) pa        (1000)     2292 2023-07-06 16:06:36.000000 crossval_ensemble-0.0.0/crossval_ensemble/custom_transformed_target_regressor.py
-drwxrwxr-x   0 pa        (1000) pa        (1000)        0 2023-07-10 08:46:12.599448 crossval_ensemble-0.0.0/crossval_ensemble.egg-info/
--rw-rw-r--   0 pa        (1000) pa        (1000)      457 2023-07-10 08:46:12.000000 crossval_ensemble-0.0.0/crossval_ensemble.egg-info/PKG-INFO
--rw-rw-r--   0 pa        (1000) pa        (1000)      393 2023-07-10 08:46:12.000000 crossval_ensemble-0.0.0/crossval_ensemble.egg-info/SOURCES.txt
--rw-rw-r--   0 pa        (1000) pa        (1000)        1 2023-07-10 08:46:12.000000 crossval_ensemble-0.0.0/crossval_ensemble.egg-info/dependency_links.txt
--rw-rw-r--   0 pa        (1000) pa        (1000)      180 2023-07-10 08:46:12.000000 crossval_ensemble-0.0.0/crossval_ensemble.egg-info/requires.txt
--rw-rw-r--   0 pa        (1000) pa        (1000)       18 2023-07-10 08:46:12.000000 crossval_ensemble-0.0.0/crossval_ensemble.egg-info/top_level.txt
--rw-rw-r--   0 pa        (1000) pa        (1000)       38 2023-07-10 08:46:12.599448 crossval_ensemble-0.0.0/setup.cfg
--rw-rw-r--   0 pa        (1000) pa        (1000)      865 2023-07-07 15:56:15.000000 crossval_ensemble-0.0.0/setup.py
+drwxrwxr-x   0 pa        (1000) pa        (1000)        0 2023-07-10 09:02:16.084118 crossval_ensemble-0.0.1/
+-rw-rw-r--   0 pa        (1000) pa        (1000)     1516 2023-06-29 09:02:18.000000 crossval_ensemble-0.0.1/LICENSE
+-rw-rw-r--   0 pa        (1000) pa        (1000)      457 2023-07-10 09:02:16.084118 crossval_ensemble-0.0.1/PKG-INFO
+-rw-rw-r--   0 pa        (1000) pa        (1000)     1226 2023-07-07 16:06:51.000000 crossval_ensemble-0.0.1/README.md
+drwxrwxr-x   0 pa        (1000) pa        (1000)        0 2023-07-10 09:02:16.084118 crossval_ensemble-0.0.1/crossval_ensemble/
+-rw-rw-r--   0 pa        (1000) pa        (1000)        0 2023-06-29 09:46:58.000000 crossval_ensemble-0.0.1/crossval_ensemble/__init__.py
+-rw-rw-r--   0 pa        (1000) pa        (1000)     6414 2023-07-06 15:28:24.000000 crossval_ensemble-0.0.1/crossval_ensemble/crossval_pipeline.py
+-rw-rw-r--   0 pa        (1000) pa        (1000)     3964 2023-06-30 13:58:02.000000 crossval_ensemble-0.0.1/crossval_ensemble/custom_pipeline.py
+-rw-rw-r--   0 pa        (1000) pa        (1000)     2292 2023-07-06 16:06:36.000000 crossval_ensemble-0.0.1/crossval_ensemble/custom_transformed_target_regressor.py
+drwxrwxr-x   0 pa        (1000) pa        (1000)        0 2023-07-10 09:02:16.084118 crossval_ensemble-0.0.1/crossval_ensemble.egg-info/
+-rw-rw-r--   0 pa        (1000) pa        (1000)      457 2023-07-10 09:02:16.000000 crossval_ensemble-0.0.1/crossval_ensemble.egg-info/PKG-INFO
+-rw-rw-r--   0 pa        (1000) pa        (1000)      393 2023-07-10 09:02:16.000000 crossval_ensemble-0.0.1/crossval_ensemble.egg-info/SOURCES.txt
+-rw-rw-r--   0 pa        (1000) pa        (1000)        1 2023-07-10 09:02:16.000000 crossval_ensemble-0.0.1/crossval_ensemble.egg-info/dependency_links.txt
+-rw-rw-r--   0 pa        (1000) pa        (1000)      181 2023-07-10 09:02:16.000000 crossval_ensemble-0.0.1/crossval_ensemble.egg-info/requires.txt
+-rw-rw-r--   0 pa        (1000) pa        (1000)       18 2023-07-10 09:02:16.000000 crossval_ensemble-0.0.1/crossval_ensemble.egg-info/top_level.txt
+-rw-rw-r--   0 pa        (1000) pa        (1000)       38 2023-07-10 09:02:16.088117 crossval_ensemble-0.0.1/setup.cfg
+-rw-rw-r--   0 pa        (1000) pa        (1000)      866 2023-07-10 09:01:02.000000 crossval_ensemble-0.0.1/setup.py
```

### Comparing `crossval_ensemble-0.0.0/LICENSE` & `crossval_ensemble-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crossval_ensemble-0.0.0/README.md` & `crossval_ensemble-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `crossval_ensemble-0.0.0/crossval_ensemble/crossval_pipeline.py` & `crossval_ensemble-0.0.1/crossval_ensemble/crossval_pipeline.py`

 * *Files identical despite different names*

### Comparing `crossval_ensemble-0.0.0/crossval_ensemble/custom_pipeline.py` & `crossval_ensemble-0.0.1/crossval_ensemble/custom_pipeline.py`

 * *Files identical despite different names*

### Comparing `crossval_ensemble-0.0.0/crossval_ensemble/custom_transformed_target_regressor.py` & `crossval_ensemble-0.0.1/crossval_ensemble/custom_transformed_target_regressor.py`

 * *Files identical despite different names*

### Comparing `crossval_ensemble-0.0.0/setup.py` & `crossval_ensemble-0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='crossval_ensemble',
-    version='0.0.0',
+    version='0.0.1',
     description='A scikit-learn wrapper for CrossValidation Ensembles',
     long_description='CrossvalEnsemble is an ML library in Python that allows to create\
     CrossValidation Ensembles leveraging scikit-learn.',
     long_description_content_type='text/markdown',
     author='Pierre-Alexis Thoumieu',
     author_email='pierre-alexis@liberkeys.com',
     packages=find_packages(exclude=['tests']),
@@ -14,14 +14,14 @@
     install_requires=[
         'numpy>=1.25.0',
         'pandas>=2.0.3',
         'tqdm>=4.65.0',
         'python-dotenv>=1.0.0',
         'flake8>=6.0.0',
         'scikit-learn>=1.3.0',
-        'ipywidget>=8.0.6',
+        'ipywidgets>=8.0.6',
         'catboost>=1.2',
         'xgboost>=1.7.6',
         'lightgbm>=3.3.5',
         'sklearn-pandas>=2.2.0',
     ]
 )
```

