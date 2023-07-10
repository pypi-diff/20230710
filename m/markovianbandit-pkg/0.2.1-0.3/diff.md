# Comparing `tmp/markovianbandit-pkg-0.2.1.tar.gz` & `tmp/markovianbandit-pkg-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markovianbandit-pkg-0.2.1.tar", last modified: Mon Nov 21 10:52:27 2022, max compression
+gzip compressed data, was "markovianbandit-pkg-0.3.tar", last modified: Mon Jul 10 18:54:46 2023, max compression
```

## Comparing `markovianbandit-pkg-0.2.1.tar` & `markovianbandit-pkg-0.3.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 gast       (501) staff       (20)        0 2022-11-21 10:52:27.060588 markovianbandit-pkg-0.2.1/
--rw-r--r--   0 gast       (501) staff       (20)     1071 2021-11-19 10:04:40.000000 markovianbandit-pkg-0.2.1/LICENSE
--rw-r--r--   0 gast       (501) staff       (20)     2328 2022-11-21 10:52:27.060840 markovianbandit-pkg-0.2.1/PKG-INFO
--rw-r--r--   0 gast       (501) staff       (20)     1744 2022-11-21 09:02:37.000000 markovianbandit-pkg-0.2.1/README.md
--rw-r--r--   0 gast       (501) staff       (20)      103 2021-11-19 10:04:40.000000 markovianbandit-pkg-0.2.1/pyproject.toml
--rw-r--r--   0 gast       (501) staff       (20)      709 2022-11-21 10:52:27.061526 markovianbandit-pkg-0.2.1/setup.cfg
-drwxr-xr-x   0 gast       (501) staff       (20)        0 2022-11-21 10:52:27.052279 markovianbandit-pkg-0.2.1/src/
-drwxr-xr-x   0 gast       (501) staff       (20)        0 2022-11-21 10:52:27.057874 markovianbandit-pkg-0.2.1/src/markovianbandit/
--rw-r--r--   0 gast       (501) staff       (20)       30 2022-01-11 17:27:24.000000 markovianbandit-pkg-0.2.1/src/markovianbandit/__init__.py
--rw-r--r--   0 gast       (501) staff       (20)    11345 2022-11-21 08:51:46.000000 markovianbandit-pkg-0.2.1/src/markovianbandit/markovianbandit.py
--rw-r--r--   0 gast       (501) staff       (20)     7584 2022-11-21 08:51:46.000000 markovianbandit-pkg-0.2.1/src/markovianbandit/whittle_computation.py
-drwxr-xr-x   0 gast       (501) staff       (20)        0 2022-11-21 10:52:27.060199 markovianbandit-pkg-0.2.1/src/markovianbandit_pkg.egg-info/
--rw-r--r--   0 gast       (501) staff       (20)     2328 2022-11-21 10:52:27.000000 markovianbandit-pkg-0.2.1/src/markovianbandit_pkg.egg-info/PKG-INFO
--rw-r--r--   0 gast       (501) staff       (20)      344 2022-11-21 10:52:27.000000 markovianbandit-pkg-0.2.1/src/markovianbandit_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 gast       (501) staff       (20)        1 2022-11-21 10:52:27.000000 markovianbandit-pkg-0.2.1/src/markovianbandit_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 gast       (501) staff       (20)       16 2022-11-21 10:52:27.000000 markovianbandit-pkg-0.2.1/src/markovianbandit_pkg.egg-info/top_level.txt
+drwxr-xr-x   0 gast       (501) staff       (20)        0 2023-07-10 18:54:46.455644 markovianbandit-pkg-0.3/
+-rw-r--r--   0 gast       (501) staff       (20)     1071 2021-11-19 10:04:40.000000 markovianbandit-pkg-0.3/LICENSE
+-rw-r--r--   0 gast       (501) staff       (20)     2853 2023-07-10 18:54:46.455778 markovianbandit-pkg-0.3/PKG-INFO
+-rw-r--r--   0 gast       (501) staff       (20)     2271 2023-07-10 18:53:11.000000 markovianbandit-pkg-0.3/README.md
+-rw-r--r--   0 gast       (501) staff       (20)      103 2021-11-19 10:04:40.000000 markovianbandit-pkg-0.3/pyproject.toml
+-rw-r--r--   0 gast       (501) staff       (20)      707 2023-07-10 18:54:46.456394 markovianbandit-pkg-0.3/setup.cfg
+drwxr-xr-x   0 gast       (501) staff       (20)        0 2023-07-10 18:54:46.444614 markovianbandit-pkg-0.3/src/
+drwxr-xr-x   0 gast       (501) staff       (20)        0 2023-07-10 18:54:46.450391 markovianbandit-pkg-0.3/src/markovianbandit/
+-rw-r--r--   0 gast       (501) staff       (20)       30 2022-01-11 17:27:24.000000 markovianbandit-pkg-0.3/src/markovianbandit/__init__.py
+-rw-r--r--   0 gast       (501) staff       (20)    11345 2022-11-21 08:51:46.000000 markovianbandit-pkg-0.3/src/markovianbandit/markovianbandit.py
+-rw-r--r--   0 gast       (501) staff       (20)     7932 2023-07-10 18:43:12.000000 markovianbandit-pkg-0.3/src/markovianbandit/whittle_computation.py
+drwxr-xr-x   0 gast       (501) staff       (20)        0 2023-07-10 18:54:46.453069 markovianbandit-pkg-0.3/src/markovianbandit_pkg.egg-info/
+-rw-r--r--   0 gast       (501) staff       (20)     2853 2023-07-10 18:54:46.000000 markovianbandit-pkg-0.3/src/markovianbandit_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 gast       (501) staff       (20)      399 2023-07-10 18:54:46.000000 markovianbandit-pkg-0.3/src/markovianbandit_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 gast       (501) staff       (20)        1 2023-07-10 18:54:46.000000 markovianbandit-pkg-0.3/src/markovianbandit_pkg.egg-info/dependency_links.txt
+-rw-r--r--   0 gast       (501) staff       (20)       16 2023-07-10 18:54:46.000000 markovianbandit-pkg-0.3/src/markovianbandit_pkg.egg-info/top_level.txt
+drwxr-xr-x   0 gast       (501) staff       (20)        0 2023-07-10 18:54:46.454914 markovianbandit-pkg-0.3/tests/
+-rw-r--r--   0 gast       (501) staff       (20)      334 2022-11-21 08:51:46.000000 markovianbandit-pkg-0.3/tests/test_nonindexable.py
+-rw-r--r--   0 gast       (501) staff       (20)     4369 2022-11-21 08:51:46.000000 markovianbandit-pkg-0.3/tests/test_nonregression.py
```

### Comparing `markovianbandit-pkg-0.2.1/LICENSE` & `markovianbandit-pkg-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `markovianbandit-pkg-0.2.1/README.md` & `markovianbandit-pkg-0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -47,11 +47,28 @@
     print("Model of size", dim, "computed in", time.time() - ts, "seconds")
 ```
 
 ## Authors
 
 Nicolas Gast and Kimang Khun. 
 
+## History version
+
+- 0.3 (July 10, 2023): 
+  - handle multichain case by testing when matrix inversion fails
+  - correct treatment of possibly infinite indices
+  - correction of a bug when dividing by 0.
+  - addition of an absolute tolerance to be more robust
+
+- 0.2 (Nov 21, 2022)
+  - simplification of how the discount is treated
+  - function to avoid recomputation of indices
+  - new indexability test
+
+- 0.1 (Jan 11, 2021)
+  - Many small optimization (code about 50% faster)
+
+- 0.0.5 (Nov 19, 2021). First public release.
 ## Reference
 
 "Testing Indexability and Computing Whittle and Gittins Index in Subcubic Time" by Nicolas Gast, Kimang Khun and Bruno Gaujal.
 https://arxiv.org/abs/2203.05207
```

### Comparing `markovianbandit-pkg-0.2.1/setup.cfg` & `markovianbandit-pkg-0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = markovianbandit-pkg
-version = 0.2.1
+version = 0.3
 author = Nicolas Gast
 author_email = nicolas.gast@inria.fr
 description = Library to compute Gittins and Whittle index for Markovian Bandits
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.inria.fr/markovianbandit/markovianbandit
 project_urls =
```

### Comparing `markovianbandit-pkg-0.2.1/src/markovianbandit/markovianbandit.py` & `markovianbandit-pkg-0.3/src/markovianbandit/markovianbandit.py`

 * *Files identical despite different names*

### Comparing `markovianbandit-pkg-0.2.1/src/markovianbandit/whittle_computation.py` & `markovianbandit-pkg-0.3/src/markovianbandit/whittle_computation.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 INDEXABLE_BUT_NOT_STRONGLY = 1
 STRONGLY_INDEXABLE = 2
 MULTICHAIN = -1
 
 # make numpy raise division by zero and 0/0 error
 np.seterr(divide='raise', invalid='raise')
 
+def multichain_message(whittle_idx):
+    """
+    Message to be printed when the arm is multichain. 
+    """
+    print("The arm is multichain! -> try with discount factor 0.99999999 to get an approximate answer.")
+    return MULTICHAIN, whittle_idx
+
 def initialize_X_from_update(beta_P0, beta_P1, beta, X, pi, atol):
     """
     Compute Delta*A_inv as defined in Algorithm 2 of the paper
     and store the product in matrix X
     """
     dim = beta_P0.shape[0]
     i0 = 0 # state having null bias in non-discounted case
@@ -44,39 +51,43 @@
             elif 1.0-y[i] > atol: mu_i_k[i] = current_mu + z[i]/(1.0-y[i])
             else: mu_i_k[i] = np.inf
     valid_idx = np.where( (mu_i_k > current_mu + atol) ) [0]
     if len(valid_idx)>0:
         argmin = mu_i_k[valid_idx].argmin()
         return valid_idx[argmin], mu_i_k[valid_idx[argmin]]
     else:
-        return -1, current_mu
+        # if no valid index is found, this means that there is a draw -> we return the first available index.
+        return 0, current_mu 
 
 @jit
 def update_W(W, sigma, X, k, atol, check_indexability=True, k0=0):
     n = X.shape[0]
     V = np.copy(X[:, sigma])
     if check_indexability:
         for l in range(k0+1, k):
             c = V[n-l]
             for i in range(n):
                 V[i] = V[i] - c * W[l-1, i]
         c = 1.0 + V[n-k]
-        if abs(c) < atol: raise ZeroDivisionError
+        if abs(c) < atol:
+            raise ZeroDivisionError
         for i in range(n):
             W[k-1, i] = V[i] / c
     else:
         for l in range(k0+1, k):
             c = V[n-l]
             for i in range(n-l+1):
                 V[i] = V[i] - c * W[l-1, i]
         c = 1.0 + V[n-k]
-        if abs(c) < atol: raise ZeroDivisionError
+        if abs(c) < atol:
+            raise ZeroDivisionError
         for i in range(n-k):
             W[k-1, i] = V[i] / c
 
+
 def compute_whittle_indices(P0, P1, R0, R1, beta=1, check_indexability=True, verbose=False, atol=1e-12, number_of_updates='2n**0.1'):
     """
     Implementation of Algorithm 2 of the paper
     Test whether the problem is indexable
     and compute Whittle indices when the problem is indexable
     The indices are computed in increasing order
 
@@ -106,19 +117,19 @@
     k0 = 0
     if number_of_updates == '2n**0.1':
         number_of_updates = int(2*dim**0.1)
     frequency_of_update = int(dim / max(1, number_of_updates))
 
     try:
         initialize_X_from_update(beta_P0, beta_P1, beta, X, pi, atol)
-    except np.linalg.LinAlgError as e:
-        if 'Matrix is singular' in str(e):
-            print("The arm is multichain!")
-            return MULTICHAIN, whittle_idx
-        else: raise e
+    except np.linalg.LinAlgError as error:
+        if 'Matrix is singular' in str(error):
+            return multichain_message(whittle_idx)
+        else:
+            raise error
     y = np.zeros(dim)
     z = R1 - R0 + X.dot(R1)
     argmin = np.argmin(z)
     sigma = sorted_sigmas[argmin]
     whittle_idx[sigma] = z[sigma]
     z -= whittle_idx[sigma]
 
@@ -141,33 +152,32 @@
 
         """
         2. If needed, we re-compute the matrix "beta times X". This should not be done too often.
         """
         if k > k0 + frequency_of_update:
             try:
                 initialize_X_from_update(beta_P0, beta_P1, beta, X, pi, atol)
-            except np.linalg.LinAlgError as e:
-                if 'Matrix is singular' in str(e):
-                    print("The arm is multichain!")
-                    return MULTICHAIN, whittle_idx
-                else: raise e
+            except np.linalg.LinAlgError as error:
+                if k < dim-1 and 'Matrix is singular' in str(error):
+                    return multichain_message(whittle_idx)
+                else:
+                    raise error
             for i in range(dim):
                 sorted_X[i] = np.copy(X[sorted_sigmas[i]])
             X = np.copy(sorted_X)
             k0 = k-1
         pi[sigma] = 0
 
         """
         3. We perform the recursive operations to compute beta*X, beta*y and beta*z.
         """
         try:
             update_W(W, sigma, X, k, atol, check_indexability, k0)
         except ZeroDivisionError:
-            print("The arm is multichain!")
-            return MULTICHAIN, whittle_idx
+            return multichain_message(whittle_idx)
         y += (1.0 - y[dim-k])*W[k-1]
         argmin, mu_min_k = find_mu_min(y[0:dim-k], z[0:dim-k], whittle_idx[sigma], atol)
         if np.isinf(mu_min_k):
             one_minus_y = 1.0 - y[dim-k:]
             if (one_minus_y < -atol).any() or (np.nonzero(abs(one_minus_y)<atol)[0] == np.nonzero(abs(z[dim-k:])<atol)[0]).any():
                 is_indexable = NON_INDEXABLE
                 print("Not indexable!")
```

