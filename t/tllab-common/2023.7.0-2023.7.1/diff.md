# Comparing `tmp/tllab_common-2023.7.0.tar.gz` & `tmp/tllab_common-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tllab_common-2023.7.0.tar", max compression
+gzip compressed data, was "tllab_common-2023.7.1.tar", max compression
```

## Comparing `tllab_common-2023.7.0.tar` & `tllab_common-2023.7.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2023.7.0/LICENSE
--rw-r--r--   0        0        0      770 2021-11-19 15:34:09.296030 tllab_common-2023.7.0/README.md
--rw-r--r--   0        0        0      890 2023-07-04 13:05:29.543945 tllab_common-2023.7.0/pyproject.toml
--rw-r--r--   0        0        0      461 2023-04-26 07:34:18.368614 tllab_common-2023.7.0/tllab_common/__init__.py
--rwxr-xr-x   0        0        0    10047 2022-09-20 13:24:57.600406 tllab_common-2023.7.0/tllab_common/findcells.py
--rw-r--r--   0        0        0     6333 2023-06-01 13:22:00.139940 tllab_common-2023.7.0/tllab_common/fit.py
--rw-r--r--   0        0        0    10422 2023-04-26 14:30:00.605612 tllab_common-2023.7.0/tllab_common/misc.py
--rw-r--r--   0        0        0      187 2021-10-14 16:27:02.346127 tllab_common-2023.7.0/tllab_common/transform.txt
--rw-r--r--   0        0        0     9202 2022-08-08 15:25:51.713820 tllab_common-2023.7.0/tllab_common/transforms.py
--rwxr-xr-x   0        0        0    70080 2023-07-04 13:03:46.359987 tllab_common-2023.7.0/tllab_common/wimread.py
--rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 tllab_common-2023.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2023.7.1/LICENSE
+-rw-r--r--   0        0        0      770 2021-11-19 15:34:09.296030 tllab_common-2023.7.1/README.md
+-rw-r--r--   0        0        0      890 2023-07-10 14:35:05.698052 tllab_common-2023.7.1/pyproject.toml
+-rw-r--r--   0        0        0      461 2023-04-26 07:34:18.368614 tllab_common-2023.7.1/tllab_common/__init__.py
+-rwxr-xr-x   0        0        0    10047 2022-09-20 13:24:57.600406 tllab_common-2023.7.1/tllab_common/findcells.py
+-rw-r--r--   0        0        0     7220 2023-07-10 12:51:15.183521 tllab_common-2023.7.1/tllab_common/fit.py
+-rw-r--r--   0        0        0    10422 2023-04-26 14:30:00.605612 tllab_common-2023.7.1/tllab_common/misc.py
+-rw-r--r--   0        0        0      187 2021-10-14 16:27:02.346127 tllab_common-2023.7.1/tllab_common/transform.txt
+-rw-r--r--   0        0        0     9202 2022-08-08 15:25:51.713820 tllab_common-2023.7.1/tllab_common/transforms.py
+-rwxr-xr-x   0        0        0    70080 2023-07-04 13:03:46.359987 tllab_common-2023.7.1/tllab_common/wimread.py
+-rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 tllab_common-2023.7.1/PKG-INFO
```

### Comparing `tllab_common-2023.7.0/LICENSE` & `tllab_common-2023.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.7.0/README.md` & `tllab_common-2023.7.1/README.md`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.7.0/pyproject.toml` & `tllab_common-2023.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tllab_common"
-version = "2023.7.0"
+version = "2023.7.1"
 description = "Common code for the Lenstra lab."
 authors = ["Lenstra lab NKI <t.lenstra@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["burst", "transcription"]
 include = ["transform.txt"]
 repository = "https://github.com/Lenstralab/tllab_common"
```

### Comparing `tllab_common-2023.7.0/tllab_common/findcells.py` & `tllab_common-2023.7.1/tllab_common/findcells.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.7.0/tllab_common/fit.py` & `tllab_common-2023.7.1/tllab_common/fit.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,17 +9,15 @@
     def __init__(self, x, y, w=None, log_scale=False):
         x = np.asarray(x)
         y = np.asarray(y)
         if w is None:
             w = np.ones_like(x)
         else:
             w = np.asarray(w)
-        self.x = x[y > 0]
-        self.y = y[y > 0]
-        self.w = w[y > 0]
+        self.x, self.y, self.w = nonnan(x, y, w)
         self.log_scale = log_scale
         self.n = len(x)
         self.p_ci95 = None
         self.r_squared = None
         self.chi_squared = None
         self.r_squared_adjusted = None
 
@@ -41,23 +39,25 @@
     @abstractmethod
     def fun(p, x):
         pass
 
     def evaluate(self, x=None):
         if x is None:
             x = np.linspace(np.nanmin(self.x), np.nanmax(self.x))
-        return x, self.fun(self.p, x)
+        else:
+            x = np.asarray(x)
+        return x.real, self.fun(self.p, x)
 
     def get_cost_fun(self):
         if self.log_scale:
             def cost(p):
-                return np.sum(self.w * np.log(self.y / self.fun(p, self.x)) ** 2)
+                return np.sum(np.abs(self.w * np.log(self.y / self.fun(p, self.x)) ** 2))
         else:
             def cost(p):
-                return np.sum(self.w * (self.y - self.fun(p, self.x)) ** 2)
+                return np.sum(np.abs(self.w * (self.y - self.fun(p, self.x)) ** 2))
         return cost
 
     @cached_property
     def r(self):
         if len(self.x):
             r = minimize(self.get_cost_fun(), self.p0, method='Nelder-Mead', bounds=self.bounds)
         else:
@@ -86,14 +86,16 @@
 
     def ftest(self, fit2):
         """ returns the p-value for the hypothesis that fit2 is the better fit,
             assuming fit2 is the fit with more free parameters
             if the fits are swapped the p-value will be negative """
         if not np.all(self.x == fit2.x):
             raise ValueError('Only two fits on the same data can be compared.')
+        if self.n_p == fit2.n_p:
+            raise ValueError('The two fits cannot have the same number of parameters.')
         rss1 = self.get_cost_fun()(self.p)
         rss2 = fit2.get_cost_fun()(fit2.p)
         swapped = np.argmin((self.n_p, fit2.n_p))
         if swapped and rss1 > rss2:
             return -1
         elif not swapped and rss1 < rss2:
             return 1
@@ -110,16 +112,16 @@
     bounds = ((0, None), (0, None))
 
     @property
     def p0(self):
         """ y = a*exp(-t/tau)
             return a, tau
         """
-        q = np.polyfit(self.x, np.log(self.y), 1)
-        return [np.clip(value, *bound) for value, bound in zip((np.exp(q[1]), -1 / q[0]), self.bounds)]
+        q = np.polyfit(*finite(self.x.astype('complex'), np.log(self.y.astype('complex'))), 1)
+        return [np.clip(value.real, *bound) for value, bound in zip((np.exp(q[1]), -1 / q[0]), self.bounds)]
 
     @staticmethod
     def fun(p, x):
         return p[0] * np.exp(-x / p[1])
 
 
 class Exponential2(Fit):
@@ -138,14 +140,40 @@
                 for value, bound in zip((y0, 1 - q[0], q[1] / 3, q[1]), self.bounds)]
 
     @staticmethod
     def fun(p, x):
         return p[0] * (p[1] * np.exp(-x / p[2]) + (1 - p[1]) * np.exp(-x / p[3]))
 
 
+class Powerlaw(Fit):
+    n_p = 2
+
+    @property
+    def p0(self):
+        """ y = (x/tau)^alpha
+            return alpha, tau
+        """
+        q = np.polyfit(*finite(np.log(self.x.astype('complex')), np.log(self.y.astype('complex'))), 1)
+        return q[0].real, np.exp(-q[1] / q[0]).real
+
+    @staticmethod
+    def fun(p, x):
+        return ((x.astype('complex') / p[1]) ** p[0]).real
+
+
+def finite(*args):
+    idx = np.prod([np.isfinite(arg) for arg in args], 0).astype(bool)
+    return [arg[idx] for arg in args]
+
+
+def nonnan(*args):
+    idx = np.prod([~np.isnan(arg) for arg in args], 0).astype(bool)
+    return [arg[idx] for arg in args]
+
+
 def fminerr(fun, a, y, args=(), w=None, diffstep=1e-6):
     """ Error estimation of a fit
 
         Inputs:
         fun:  function which was fitted to data
         a:    function parameters
         y:    ydata
@@ -181,15 +209,15 @@
 
     # calculate R^2
     sstot = np.sum((y - np.nanmean(y)) ** 2)
     ssres = np.sum((y - f0) ** 2)
     r_squared = 1 - ssres / sstot
 
     # calculate derivatives
-    deriv = np.zeros((n_data, n_par))
+    deriv = np.zeros((n_data, n_par), dtype='complex')
     for i in range(n_par):
         ah = a.copy()
         ah[i] = a[i] * (1 + diffstep) + eps
         f = np.array(fun(ah, *args)).flatten()
         deriv[:, i] = (f - f0) / (ah[i] - a[i]) * w
 
     hesse = np.matmul(deriv.T, deriv)
@@ -197,8 +225,8 @@
     try:
         if np.linalg.matrix_rank(hesse) == np.shape(hesse)[0]:
             da = np.sqrt(chisq * np.diag(np.linalg.inv(hesse)))
         else:
             da = np.sqrt(chisq * np.diag(np.linalg.pinv(hesse)))
     except (Exception,):
         da = np.full_like(a, np.nan)
-    return chisq, 1.96 * da, r_squared
+    return chisq.real, 1.96 * da.real, r_squared.real
```

### Comparing `tllab_common-2023.7.0/tllab_common/misc.py` & `tllab_common-2023.7.1/tllab_common/misc.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.7.0/tllab_common/transforms.py` & `tllab_common-2023.7.1/tllab_common/transforms.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.7.0/tllab_common/wimread.py` & `tllab_common-2023.7.1/tllab_common/wimread.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.7.0/PKG-INFO` & `tllab_common-2023.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tllab-common
-Version: 2023.7.0
+Version: 2023.7.1
 Summary: Common code for the Lenstra lab.
 Home-page: https://github.com/Lenstralab/tllab_common
 License: GPLv3
 Keywords: burst,transcription
 Author: Lenstra lab NKI
 Author-email: t.lenstra@nki.nl
 Requires-Python: >=3.8,<4.0
```

