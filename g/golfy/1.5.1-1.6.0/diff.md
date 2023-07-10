# Comparing `tmp/golfy-1.5.1.tar.gz` & `tmp/golfy-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golfy-1.5.1.tar", last modified: Fri Jul  7 15:59:15 2023, max compression
+gzip compressed data, was "golfy-1.6.0.tar", last modified: Mon Jul 10 19:45:27 2023, max compression
```

## Comparing `golfy-1.5.1.tar` & `golfy-1.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-07 15:59:15.653431 golfy-1.5.1/
--rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-1.5.1/LICENSE
--rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-07 15:59:15.653286 golfy-1.5.1/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)     1317 2023-07-06 20:51:05.000000 golfy-1.5.1/README.md
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-07 15:59:15.651398 golfy-1.5.1/golfy/
--rw-r--r--   0 iskander   (501) staff       (20)      357 2023-07-07 15:58:21.000000 golfy-1.5.1/golfy/__init__.py
--rw-r--r--   0 iskander   (501) staff       (20)     5492 2023-07-06 20:50:21.000000 golfy-1.5.1/golfy/deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)     8479 2023-07-07 14:29:26.000000 golfy-1.5.1/golfy/initialization.py
--rw-r--r--   0 iskander   (501) staff       (20)     8453 2023-07-07 14:00:59.000000 golfy-1.5.1/golfy/optimization.py
--rw-r--r--   0 iskander   (501) staff       (20)     4089 2023-07-07 14:00:08.000000 golfy-1.5.1/golfy/solution.py
--rw-r--r--   0 iskander   (501) staff       (20)      270 2023-07-03 19:32:27.000000 golfy-1.5.1/golfy/types.py
--rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-1.5.1/golfy/util.py
--rw-r--r--   0 iskander   (501) staff       (20)     3632 2023-07-03 19:39:30.000000 golfy-1.5.1/golfy/validity.py
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-07 15:59:15.651938 golfy-1.5.1/golfy.egg-info/
--rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-07 15:59:15.000000 golfy-1.5.1/golfy.egg-info/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)      415 2023-07-07 15:59:15.000000 golfy-1.5.1/golfy.egg-info/SOURCES.txt
--rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-07 15:59:15.000000 golfy-1.5.1/golfy.egg-info/dependency_links.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:59:15.000000 golfy-1.5.1/golfy.egg-info/requires.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:59:15.000000 golfy-1.5.1/golfy.egg-info/top_level.txt
--rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-07 15:56:30.000000 golfy-1.5.1/pyproject.toml
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-1.5.1/requirements.txt
--rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-07 15:59:15.653468 golfy-1.5.1/setup.cfg
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-07 15:59:15.652892 golfy-1.5.1/tests/
--rw-r--r--   0 iskander   (501) staff       (20)      884 2023-07-06 20:33:42.000000 golfy-1.5.1/tests/test_deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)     1660 2023-07-07 14:04:35.000000 golfy-1.5.1/tests/test_init.py
--rw-r--r--   0 iskander   (501) staff       (20)      203 2023-07-03 19:41:20.000000 golfy-1.5.1/tests/test_optimize.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-10 19:45:27.521258 golfy-1.6.0/
+-rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-1.6.0/LICENSE
+-rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-10 19:45:27.521122 golfy-1.6.0/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)     1317 2023-07-06 20:51:05.000000 golfy-1.6.0/README.md
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-10 19:45:27.519090 golfy-1.6.0/golfy/
+-rw-r--r--   0 iskander   (501) staff       (20)      630 2023-07-10 19:41:36.000000 golfy-1.6.0/golfy/__init__.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5141 2023-07-10 19:45:10.000000 golfy-1.6.0/golfy/deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)     8479 2023-07-07 14:29:26.000000 golfy-1.6.0/golfy/initialization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     8453 2023-07-07 14:00:59.000000 golfy-1.6.0/golfy/optimization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4089 2023-07-07 14:00:08.000000 golfy-1.6.0/golfy/solution.py
+-rw-r--r--   0 iskander   (501) staff       (20)      270 2023-07-03 19:32:27.000000 golfy-1.6.0/golfy/types.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-1.6.0/golfy/util.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3632 2023-07-03 19:39:30.000000 golfy-1.6.0/golfy/validity.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-10 19:45:27.519730 golfy-1.6.0/golfy.egg-info/
+-rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-10 19:45:27.000000 golfy-1.6.0/golfy.egg-info/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)      415 2023-07-10 19:45:27.000000 golfy-1.6.0/golfy.egg-info/SOURCES.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-10 19:45:27.000000 golfy-1.6.0/golfy.egg-info/dependency_links.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-10 19:45:27.000000 golfy-1.6.0/golfy.egg-info/requires.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-10 19:45:27.000000 golfy-1.6.0/golfy.egg-info/top_level.txt
+-rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-10 19:33:19.000000 golfy-1.6.0/pyproject.toml
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-1.6.0/requirements.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-10 19:45:27.521292 golfy-1.6.0/setup.cfg
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-10 19:45:27.520815 golfy-1.6.0/tests/
+-rw-r--r--   0 iskander   (501) staff       (20)      884 2023-07-06 20:33:42.000000 golfy-1.6.0/tests/test_deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1660 2023-07-07 14:04:35.000000 golfy-1.6.0/tests/test_init.py
+-rw-r--r--   0 iskander   (501) staff       (20)      203 2023-07-03 19:41:20.000000 golfy-1.6.0/tests/test_optimize.py
```

### Comparing `golfy-1.5.1/LICENSE` & `golfy-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `golfy-1.5.1/PKG-INFO` & `golfy-1.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 1.5.1
+Version: 1.6.0
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `golfy-1.5.1/README.md` & `golfy-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `golfy-1.5.1/golfy/deconvolution.py` & `golfy-1.6.0/golfy/deconvolution.py`

 * *Files 8% similar despite different names*

```diff
@@ -120,14 +120,16 @@
 def solve_linear_system(
     linear_system: LinearSystem,
     min_peptide_activity: float = 1.0,
     leave_on_out=True,
     sparse_solution=True,
     verbose=False,
 ) -> DeconvolutionResult:
+    from sklearn.linear_model import Lasso, Ridge
+
     A = linear_system.A
     b = linear_system.b
     num_pools, num_peptides_with_constant = A.shape
     num_peptides = num_peptides_with_constant - 1
     row_indices = list(range(num_pools))
     if leave_on_out:
         loo_indices = row_indices
@@ -138,37 +140,27 @@
     frac_hit = np.zeros(num_peptides)
 
     for loo_idx in loo_indices:
         subset_indices = np.array([i for i in row_indices if i != loo_idx])
         A_subset = A[subset_indices, :]
         b_subset = b[subset_indices]
         if sparse_solution:
-            # L1 minimizatin to get a small set of confident active peptides
-            import sklearn.linear_model
-
-            lasso = sklearn.linear_model.Lasso(fit_intercept=False)
+            # L1 minimization to get a small set of confident active peptides
+            lasso = Lasso(fit_intercept=False, positive=True)
             lasso.fit(A_subset, b_subset)
             x_with_offset = lasso.coef_
-            x, c = x_with_offset[:-1], x_with_offset[-1]
-            if verbose:
-                print("x = %s" % (x,))
-                print("c = %s" % (c,))
         else:
-            # least squares non-sparse solution, works horribly, have fun
-            x_with_offset, residuals, rank, singular_values = np.linalg.lstsq(
-                A, b, rcond=None
-            )
-            x, c = x_with_offset[:-1], x_with_offset[-1]
-            if verbose:
-                print("x = %s" % (x[:-1],))
-                print("c = %f" % (c,))
-                print("residuals = %s" % (residuals,))
-                print("rank = %s" % (rank,))
-                print("singular_values = %s" % (singular_values,))
-
+            # this will work horribly, have fun
+            ridge = Ridge(fit_intercept=False, positive=True)
+            ridge.fit(A_subset, b_subset)
+            x_with_offset = ridge.coef_
+        if verbose:
+            print("x = %s" % (x,))
+            print("c = %s" % (c,))
+        x, c = x_with_offset[:-1], x_with_offset[-1]
         avg_activity += x
         frac_hit += (x > min_peptide_activity).astype(float)
 
     avg_activity /= len(loo_indices)
     frac_hit /= len(loo_indices)
     high_confidence_hits = set(np.where(frac_hit > 0.5)[0])
```

### Comparing `golfy-1.5.1/golfy/initialization.py` & `golfy-1.6.0/golfy/initialization.py`

 * *Files identical despite different names*

### Comparing `golfy-1.5.1/golfy/optimization.py` & `golfy-1.6.0/golfy/optimization.py`

 * *Files identical despite different names*

### Comparing `golfy-1.5.1/golfy/solution.py` & `golfy-1.6.0/golfy/solution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.5.1/golfy/util.py` & `golfy-1.6.0/golfy/util.py`

 * *Files identical despite different names*

### Comparing `golfy-1.5.1/golfy/validity.py` & `golfy-1.6.0/golfy/validity.py`

 * *Files identical despite different names*

### Comparing `golfy-1.5.1/golfy.egg-info/PKG-INFO` & `golfy-1.6.0/golfy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 1.5.1
+Version: 1.6.0
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `golfy-1.5.1/pyproject.toml` & `golfy-1.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `golfy-1.5.1/tests/test_deconvolution.py` & `golfy-1.6.0/tests/test_deconvolution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.5.1/tests/test_init.py` & `golfy-1.6.0/tests/test_init.py`

 * *Files identical despite different names*

