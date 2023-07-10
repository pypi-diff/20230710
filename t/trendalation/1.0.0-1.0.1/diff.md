# Comparing `tmp/trendalation-1.0.0.tar.gz` & `tmp/trendalation-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trendalation-1.0.0.tar", last modified: Mon Jul 10 01:47:35 2023, max compression
+gzip compressed data, was "trendalation-1.0.1.tar", last modified: Mon Jul 10 01:53:58 2023, max compression
```

## Comparing `trendalation-1.0.0.tar` & `trendalation-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-10 01:47:35.677561 trendalation-1.0.0/
--rw-r--r--   0 raghavsaboo   (501) staff       (20)     1084 2023-07-08 16:44:54.000000 trendalation-1.0.0/LICENSE.rst
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      556 2023-07-10 01:47:35.677626 trendalation-1.0.0/PKG-INFO
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      872 2023-07-08 16:44:54.000000 trendalation-1.0.0/README.md
--rw-r--r--   0 raghavsaboo   (501) staff       (20)       93 2023-07-08 17:30:19.000000 trendalation-1.0.0/pyproject.toml
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      107 2023-07-10 01:47:35.677850 trendalation-1.0.0/setup.cfg
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      787 2023-07-10 01:47:24.000000 trendalation-1.0.0/setup.py
-drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-10 01:47:35.675118 trendalation-1.0.0/src/
-drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-10 01:47:35.676574 trendalation-1.0.0/src/trendalation/
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      118 2023-07-10 01:46:20.000000 trendalation-1.0.0/src/trendalation/__init__.py
--rw-r--r--   0 raghavsaboo   (501) staff       (20)     5885 2023-07-10 01:30:01.000000 trendalation-1.0.0/src/trendalation/classification.py
--rw-r--r--   0 raghavsaboo   (501) staff       (20)     1479 2023-07-10 01:30:01.000000 trendalation-1.0.0/src/trendalation/metrics.py
--rw-r--r--   0 raghavsaboo   (501) staff       (20)       22 2023-07-10 01:37:36.000000 trendalation-1.0.0/src/trendalation/version.py
-drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-10 01:47:35.677410 trendalation-1.0.0/src/trendalation.egg-info/
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      556 2023-07-10 01:47:35.000000 trendalation-1.0.0/src/trendalation.egg-info/PKG-INFO
--rw-r--r--   0 raghavsaboo   (501) staff       (20)      374 2023-07-10 01:47:35.000000 trendalation-1.0.0/src/trendalation.egg-info/SOURCES.txt
--rw-r--r--   0 raghavsaboo   (501) staff       (20)        1 2023-07-10 01:47:35.000000 trendalation-1.0.0/src/trendalation.egg-info/dependency_links.txt
--rw-r--r--   0 raghavsaboo   (501) staff       (20)       25 2023-07-10 01:47:35.000000 trendalation-1.0.0/src/trendalation.egg-info/requires.txt
--rw-r--r--   0 raghavsaboo   (501) staff       (20)       13 2023-07-10 01:47:35.000000 trendalation-1.0.0/src/trendalation.egg-info/top_level.txt
+drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-10 01:53:58.931574 trendalation-1.0.1/
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)     1084 2023-07-08 16:44:54.000000 trendalation-1.0.1/LICENSE.rst
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      556 2023-07-10 01:53:58.931639 trendalation-1.0.1/PKG-INFO
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      872 2023-07-08 16:44:54.000000 trendalation-1.0.1/README.md
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)       93 2023-07-08 17:30:19.000000 trendalation-1.0.1/pyproject.toml
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      107 2023-07-10 01:53:58.931860 trendalation-1.0.1/setup.cfg
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      787 2023-07-10 01:53:48.000000 trendalation-1.0.1/setup.py
+drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-10 01:53:58.929013 trendalation-1.0.1/src/
+drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-10 01:53:58.930637 trendalation-1.0.1/src/trendalation/
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      118 2023-07-10 01:46:20.000000 trendalation-1.0.1/src/trendalation/__init__.py
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)     6775 2023-07-10 01:52:16.000000 trendalation-1.0.1/src/trendalation/classification.py
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)     1479 2023-07-10 01:30:01.000000 trendalation-1.0.1/src/trendalation/metrics.py
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)       22 2023-07-10 01:37:36.000000 trendalation-1.0.1/src/trendalation/version.py
+drwxr-xr-x   0 raghavsaboo   (501) staff       (20)        0 2023-07-10 01:53:58.931426 trendalation-1.0.1/src/trendalation.egg-info/
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      556 2023-07-10 01:53:58.000000 trendalation-1.0.1/src/trendalation.egg-info/PKG-INFO
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)      374 2023-07-10 01:53:58.000000 trendalation-1.0.1/src/trendalation.egg-info/SOURCES.txt
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)        1 2023-07-10 01:53:58.000000 trendalation-1.0.1/src/trendalation.egg-info/dependency_links.txt
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)       25 2023-07-10 01:53:58.000000 trendalation-1.0.1/src/trendalation.egg-info/requires.txt
+-rw-r--r--   0 raghavsaboo   (501) staff       (20)       13 2023-07-10 01:53:58.000000 trendalation-1.0.1/src/trendalation.egg-info/top_level.txt
```

### Comparing `trendalation-1.0.0/LICENSE.rst` & `trendalation-1.0.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `trendalation-1.0.0/PKG-INFO` & `trendalation-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trendalation
-Version: 1.0.0
+Version: 1.0.1
 Home-page: https://github.com/kartikeysinha/trendalation
 Author: ['Raghav Saboo', 'Kartikey Sinha']
 Author-email: raghs2000@gmail.com
 License: MIT
 Keywords: anomaly detection,procrustes,time-series,trends
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `trendalation-1.0.0/README.md` & `trendalation-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `trendalation-1.0.0/setup.py` & `trendalation-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='trendalation',
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     python_requires=">=3.8",
-    version='1.0.0',
+    version='1.0.1',
     license='MIT',
     author=['Raghav Saboo', 'Kartikey Sinha'],
     author_email='raghs2000@gmail.com',
     url='https://github.com/kartikeysinha/trendalation',
     keywords=['anomaly detection', 'procrustes', 'time-series', 'trends'],
     install_requires=[
         'numpy',
```

### Comparing `trendalation-1.0.0/src/trendalation/classification.py` & `trendalation-1.0.1/src/trendalation/classification.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,55 +7,52 @@
 
 class ProcClassifier:
     def __init__(self) -> None:
         self.ref_curve, self.width, self.thresh = None, None, None
         self.is_fitted = False
         
     def _proc_error(self, trace):
-        '''
+        """
         Returns the procrustes error against the fitted reference curve for a given trace.
 
                 Parameters
                 ----------
                 trace : {array-like} of shape (n_features,)
                     The training input samples. Internally, it will be converted to
                     ``dtype=np.float32``.
 
                 Returns
                 -------
                 error : float 
                     Procrustes error for the trace against the reference curve.
-        '''
-        # if not self.is_fitted:
-        #     raise Exception("Error: Fit model before making predictions")
-    
+        """    
         _, _, disparity = procrustes(self.ref_curve.reshape(-1, 1), trace.reshape(-1, 1))
         return disparity
     
     def _normalize_trace(self, trace):
-        '''
+        """
         Normalize a trace with respect to itself => (trace - mean(trace)) / std(trace)
 
                 Parameters
                 ----------
                 trace : {array-like} of shape (n_features,)
                     The training input samples. Internally, it will be converted to
                     ``dtype=np.float32``.
 
                 Returns
                 -------
                 trace : array-like of shape (n_sampn_featuresles,)
                     Normalized trace.
-        '''
+        """
         mean = np.mean(trace)
         std = np.std(trace)
         return (trace - mean) / std
 
     def fit(self, X, y=None, threshold=None, normalize=True, ci_width=3.0):
-        '''
+        """
         Build a Procrustes Analysis powered classifier from the training set (X, y).
 
                 Parameters
                 ----------
                 X : {array-like, sparse matrix} of shape (n_samples, n_features)
                     The training input samples. Internally, it will be converted to
                     ``dtype=np.float32``.
@@ -77,15 +74,15 @@
                 ci_width : float, default=3.0
                     Confidence interval width parameter. Defaults to 3.0 which corresponds to
                     a 99% confidence interval.
 
                 Returns
                 -------
                 None
-        '''
+        """
         
         # Convert to 2d numpy array
         X_train = np.array(X, dtype=np.float64, copy=True)
         if X_train.ndim == 1:
             X_train = X.reshape(1, -1)
             
         # Normalize each trace with respect to itself
@@ -112,38 +109,64 @@
             fpr, tpr, thresholds = metrics.roc_curve(y, errors, pos_label=1)
             optimal_idx = np.argmax(tpr - fpr)
             self.thresh = thresholds[optimal_idx]
         elif self.thresh is None:
             self.thresh = np.percentile(errors, 0.75)
 
         # Mark estimator as fitted 
-        self.is_fitted = True
+        self.is_fitted = True        
+    
+    def _predict_preproc(self, X):
+        """
+        Preprocing for prediction.
+        """
+        if not self.is_fitted:
+            raise Exception("Error: Fit model before making predictions")
+        
+        # Convert to 2d numpy array
+        X = np.array(X, dtype=np.float64, copy=True)
+        if X.ndim == 1:
+            X = X.reshape(1, -1)
+        
+        # Compute procrustes error for each curve
+        errors = np.array([self._proc_error(x) for x in X])
 
+        return (errors - self.thresh).round(5)
+    
     def predict(self, X):
-        '''
+        """
         Classify traces based on the trained estimator (X).
 
                 Parameters
                 ----------
                 X : {array-like, sparse matrix} of shape (n_samples, n_features)
                     The training input samples. Internally, it will be converted to
                     ``dtype=np.float32``.
 
                 Returns
                 -------
                 y : array-like of shape (n_samples,)
                     The predicted label values (binary class labels) as integers with 1 
                     representing an anomaly.
-        '''
-        if not self.is_fitted:
-            raise Exception("Error: Fit model before making predictions")
-        
-        # Convert to 2d numpy array
-        X = np.array(X, dtype=np.float64, copy=True)
-        if X.ndim == 1:
-            X = X.reshape(1, -1)
-        
-        # Compute procrustes error for each curve
-        errors = np.array([self._proc_error(x) for x in X])
-        preds = np.where(errors > self.thresh, 1.0, 0.0)
-        
+        """
+        errors_less_threshold = self._predict_preproc(X)
+        preds = np.where(errors_less_threshold > 0.0, 1.0, 0.0)
         return preds
+
+    def predict_score(self, X):
+        """
+        Score to quantify how well the traces adapt to the trained estimator (X).
+        Score represents error, so the lesser the better.
+
+                Parameters
+                ----------
+                X : {array-like, sparse matrix} of shape (n_samples, n_features)
+                    The training input samples. Internally, it will be converted to
+                    ``dtype=np.float32``.
+
+                Returns
+                -------
+                y : array-like of shape (n_samples,)
+                    The mean squared error of the transformed curve with thee reference curve.
+                    The lesser the value, the closer the curve is to the reference curve.
+        """
+        return self._predict_preproc(X)
```

### Comparing `trendalation-1.0.0/src/trendalation/metrics.py` & `trendalation-1.0.1/src/trendalation/metrics.py`

 * *Files identical despite different names*

### Comparing `trendalation-1.0.0/src/trendalation.egg-info/PKG-INFO` & `trendalation-1.0.1/src/trendalation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trendalation
-Version: 1.0.0
+Version: 1.0.1
 Home-page: https://github.com/kartikeysinha/trendalation
 Author: ['Raghav Saboo', 'Kartikey Sinha']
 Author-email: raghs2000@gmail.com
 License: MIT
 Keywords: anomaly detection,procrustes,time-series,trends
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

