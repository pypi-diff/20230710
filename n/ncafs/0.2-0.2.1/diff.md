# Comparing `tmp/ncafs-0.2.tar.gz` & `tmp/ncafs-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ncafs-0.2.tar", last modified: Sun Oct 10 18:29:54 2021, max compression
+gzip compressed data, was "ncafs-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ncafs-0.2.tar` & `ncafs-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,8 @@
-drwxr-xr-x   0 pedropaiva   (501) staff       (20)        0 2021-10-10 18:29:53.000000 ncafs-0.2/
--rw-r--r--   0 pedropaiva   (501) staff       (20)     1519 2021-09-05 19:19:38.000000 ncafs-0.2/LICENSE
--rw-r--r--   0 pedropaiva   (501) staff       (20)     2694 2021-10-10 18:29:53.000000 ncafs-0.2/PKG-INFO
--rw-r--r--   0 pedropaiva   (501) staff       (20)     1970 2021-09-19 19:14:33.000000 ncafs-0.2/README.md
-drwxr-xr-x   0 pedropaiva   (501) staff       (20)        0 2021-10-10 18:29:53.000000 ncafs-0.2/ncafs/
--rw-r--r--   0 pedropaiva   (501) staff       (20)       33 2021-09-04 14:39:06.000000 ncafs-0.2/ncafs/__init__.py
--rw-r--r--   0 pedropaiva   (501) staff       (20)     6231 2021-10-10 18:22:06.000000 ncafs-0.2/ncafs/base.py
--rw-r--r--   0 pedropaiva   (501) staff       (20)     5524 2021-10-07 02:21:53.000000 ncafs-0.2/ncafs/core.py
-drwxr-xr-x   0 pedropaiva   (501) staff       (20)        0 2021-10-10 18:29:53.000000 ncafs-0.2/ncafs.egg-info/
--rw-r--r--   0 pedropaiva   (501) staff       (20)     2694 2021-10-10 18:29:45.000000 ncafs-0.2/ncafs.egg-info/PKG-INFO
--rw-r--r--   0 pedropaiva   (501) staff       (20)      226 2021-10-10 18:29:46.000000 ncafs-0.2/ncafs.egg-info/SOURCES.txt
--rw-r--r--   0 pedropaiva   (501) staff       (20)        1 2021-10-10 18:29:45.000000 ncafs-0.2/ncafs.egg-info/dependency_links.txt
--rw-r--r--   0 pedropaiva   (501) staff       (20)       73 2021-10-10 18:29:45.000000 ncafs-0.2/ncafs.egg-info/requires.txt
--rw-r--r--   0 pedropaiva   (501) staff       (20)        6 2021-10-10 18:29:45.000000 ncafs-0.2/ncafs.egg-info/top_level.txt
--rw-r--r--   0 pedropaiva   (501) staff       (20)       79 2021-10-10 18:29:53.000000 ncafs-0.2/setup.cfg
--rw-r--r--   0 pedropaiva   (501) staff       (20)     1068 2021-10-10 18:29:29.000000 ncafs-0.2/setup.py
+-rw-r--r--   0        0        0     1970 2023-07-10 14:07:04.672171 ncafs-0.2.1/README.md
+-rw-r--r--   0        0        0       56 2023-07-10 14:07:04.672171 ncafs-0.2.1/ncafs/__init__.py
+-rw-r--r--   0        0        0     6227 2023-07-10 14:07:04.672171 ncafs-0.2.1/ncafs/base.py
+-rw-r--r--   0        0        0     5490 2023-07-10 14:07:04.672171 ncafs-0.2.1/ncafs/core.py
+-rw-r--r--   0        0        0     2277 2023-07-10 14:07:04.672171 ncafs-0.2.1/ncafs/tests/test_functional.py
+-rw-r--r--   0        0        0      689 2023-07-10 14:07:04.672171 ncafs-0.2.1/ncafs/tests/test_unit.py
+-rw-r--r--   0        0        0      943 2023-07-10 14:07:04.672171 ncafs-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2837 1970-01-01 00:00:00.000000 ncafs-0.2.1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ncafs-0.2/PKG-INFO` & `ncafs-0.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: ncafs
-Version: 0.2
-Summary: Neighborhood Component Analysis Feature Selection
-Home-page: https://gitlab.com/pedro.paiva/ncafs
-Author: Pedro Paiva
-Author-email: paiva@ita.br
-License: BSD 3-Clause
-Download-URL: https://gitlab.com/pedro.paiva/ncafs/-/archive/v0.2/ncafs-v0.2.tar.gz
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # NCAFS
 
 _Neighborhood Component Analysis Feature Selection_
 
 NCAFS is a non-parametric algorithm based on k-nearest neighbors (kNN), which learns a feature weighting 
 vector by minimizing the expected leave-one-out error with a regularization term. NCA was originally 
 proposed in [1], which inspired the feature selection method for classification presented in [2]. It was 
@@ -85,9 +65,7 @@
 
 1. Goldberger, J., Hinton, G., Roweis, S., Salakhutdinov, R. (2005). Neighbourhood Components Analysis. Advances in Neural Information Processing Systems. 17, 513-520.
 2. Yang, W., Wang, K., & Zuo, W. (2012). Neighborhood component feature selection for high-dimensional data. J. Comput., 7(1), 161-168.
 3. Amankwaa-Kyeremeh, B., Greet, C., Zanin, M., Skinner, W. and Asamoah, R. K., (2020), Selecting key
    predictor parameters for regression analysis using modified Neighbourhood Component Analysis (NCA)
    Algorithm. Proceedings of 6th UMaT Biennial International Mining and Mineral Conference, Tarkwa, Ghana,
    pp. 320-325.
-
-
```

### Comparing `ncafs-0.2/README.md` & `ncafs-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: ncafs
+Version: 0.2.1
+Summary: Neighborhood Component Analysis Feature Selection
+Author-email: Pedro Paiva <paiva@ita.br>
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Intended Audience :: Science/Research
+Requires-Dist: scikit-learn>=0.23
+Requires-Dist: setuptools>=52.0.0
+Requires-Dist: numpy>=1.20
+Requires-Dist: scipy>=1.6
+Requires-Dist: pytest>=6.0 ; extra == "dev"
+Requires-Dist: notebook>=6.4 ; extra == "dev"
+Requires-Dist: jupyterlab>=3.5.3 ; extra == "dev"
+Project-URL: repository, https://gitlab.com/pedro.paiva/ncafs
+Provides-Extra: dev
+
 # NCAFS
 
 _Neighborhood Component Analysis Feature Selection_
 
 NCAFS is a non-parametric algorithm based on k-nearest neighbors (kNN), which learns a feature weighting 
 vector by minimizing the expected leave-one-out error with a regularization term. NCA was originally 
 proposed in [1], which inspired the feature selection method for classification presented in [2]. It was 
@@ -65,7 +88,8 @@
 
 1. Goldberger, J., Hinton, G., Roweis, S., Salakhutdinov, R. (2005). Neighbourhood Components Analysis. Advances in Neural Information Processing Systems. 17, 513-520.
 2. Yang, W., Wang, K., & Zuo, W. (2012). Neighborhood component feature selection for high-dimensional data. J. Comput., 7(1), 161-168.
 3. Amankwaa-Kyeremeh, B., Greet, C., Zanin, M., Skinner, W. and Asamoah, R. K., (2020), Selecting key
    predictor parameters for regression analysis using modified Neighbourhood Component Analysis (NCA)
    Algorithm. Proceedings of 6th UMaT Biennial International Mining and Mineral Conference, Tarkwa, Ghana,
    pp. 320-325.
+
```

### Comparing `ncafs-0.2/ncafs/base.py` & `ncafs-0.2.1/ncafs/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     check_X_y,
     check_array,
     check_is_fitted,
     check_scalar
 )
 
 
-class BaseNCAFS(TransformerMixin, BaseEstimator, ABC):
+class NCAFS(TransformerMixin, BaseEstimator, ABC):
     """
 
     Parameters
     ----------
     n_features_to_select : int (optional, default=None)
         Number of features which must be selected.
     threshold : float (optional, default=0.1)
```

### Comparing `ncafs-0.2/ncafs/core.py` & `ncafs-0.2.1/ncafs/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Tuple
 
 import numpy as np
 from scipy.optimize import minimize
 from scipy.spatial.distance import pdist, squareform
 
-from .base import BaseNCAFS
+from .base import NCAFS
 
 
 def exponential_kernel(z: np.ndarray, sigma: float) -> np.ndarray:
     """
     Exponential kernel.
 
     Parameters
@@ -46,15 +46,16 @@
     # matrix to hold pairwise distances between samples in each feature
     N, M = X.shape
     dists = np.zeros((M, N, N))
     for j in range(M):
         dists[j] = squareform(
             pdist(
                 X[:, j].reshape(-1, 1),
-                metric=metric)
+                metric=metric
+            )
         )
     return dists
 
 
 def add_pseudocount(v: np.ndarray) -> np.ndarray:
     """
     Adds pseudocount to avoid zero-value elements in a vector.
@@ -77,16 +78,21 @@
             pseudocount = np.exp(-20)
         else:
             pseudocount = np.min(v[~mask])
         v[mask] += pseudocount
     return v
 
 
-def cost_nca(w: np.ndarray, feat_dist: np.ndarray, y_loss: np.ndarray,
-             sigma: float = 1, alpha: float = 1) -> Tuple[float, np.ndarray]:
+def cost_nca(
+        w: np.ndarray,
+        feat_dist: np.ndarray,
+        y_loss: np.ndarray,
+        sigma: float = 1.0,
+        alpha: float = 1.0
+) -> Tuple[float, np.ndarray]:
     """
     Cost function for NCA model.
 
     Parameters
     ----------
     w : array of shape (n_features,)
         weights array
@@ -127,59 +133,63 @@
     s2 = np.sum(y_loss * p * feat_dist, axis=(1, 2)).reshape(-1, 1)
     grad = 2 * ((1 / sigma) * (s1 - s2) * (1 / N) + alpha) * w
     grad = grad.reshape(-1)
 
     return cost, grad
 
 
-class NCAFSR(BaseNCAFS):
+class NCAFSR(NCAFS):
     """
     Neighborhood Component Analysis Feature Selection for regression targets.
     """
 
     def _fit(self, X: np.ndarray, y: np.ndarray, w0: np.ndarray) -> np.ndarray:
         n_feat = X.shape[1]
         X_dist = pairwise_feature_distance(X, metric=self.metric)
         y_dist = squareform(pdist(y.reshape(-1, 1), metric=self.metric))
 
         if self.alpha is None:
             alpha = self._estimate_alpha(n_feat, y)
         else:
             alpha = self.alpha
         args = (X_dist, y_dist, self.sigma, alpha)
-        result = minimize(cost_nca, w0, args,
-                          method=self.solver,
-                          jac=True,
-                          options=dict(disp=False),
-                          bounds=[self.bounds] * n_feat)
+        result = minimize(
+            cost_nca, w0, args,
+            method=self.solver,
+            jac=True,
+            options=dict(disp=False),
+            bounds=[self.bounds] * n_feat
+        )
         return np.abs(result['x'])
 
     @staticmethod
     def _estimate_alpha(n_feat: int, y: np.ndarray) -> float:
         return 0.01 * np.log10(n_feat) * y.std()
 
 
-class NCAFSC(BaseNCAFS):
+class NCAFSC(NCAFS):
     """
     Neighborhood Component Analysis Feature Selection for classification targets.
     """
 
     def _fit(self, X: np.ndarray, y: np.ndarray, w0: np.ndarray) -> np.ndarray:
         n_feat = X.shape[1]
         X_dist = pairwise_feature_distance(X, metric=self.metric)
         y_dist = squareform(pdist(y.reshape(-1, 1), metric=lambda u, v: 1 - (u == v)))
 
         if self.alpha is None:
             alpha = self._estimate_alpha(n_feat, y)
         else:
             alpha = self.alpha
         args = (X_dist, y_dist, self.sigma, alpha)
-        result = minimize(cost_nca, w0, args,
-                          method=self.solver,
-                          jac=True,
-                          options=dict(disp=False),
-                          bounds=[self.bounds] * n_feat)
+        result = minimize(
+            cost_nca, w0, args,
+            method=self.solver,
+            jac=True,
+            options=dict(disp=False),
+            bounds=[self.bounds] * n_feat
+        )
         return np.abs(result['x'])
 
     @staticmethod
     def _estimate_alpha(n_feat: int, y: np.ndarray) -> float:
         return 0.01 / max(1, np.log10(n_feat))
```

