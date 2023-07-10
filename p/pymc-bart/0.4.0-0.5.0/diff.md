# Comparing `tmp/pymc_bart-0.4.0.tar.gz` & `tmp/pymc_bart-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymc_bart-0.4.0.tar", last modified: Fri Mar 17 17:05:31 2023, max compression
+gzip compressed data, was "pymc_bart-0.5.0.tar", last modified: Mon Jul 10 17:47:16 2023, max compression
```

## Comparing `pymc_bart-0.4.0.tar` & `pymc_bart-0.5.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 17:05:31.322672 pymc_bart-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-03-17 17:05:15.000000 pymc_bart-0.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-17 17:05:15.000000 pymc_bart-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-03-17 17:05:15.000000 pymc_bart-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-17 17:05:15.000000 pymc_bart-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-03-17 17:05:31.318673 pymc_bart-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-03-17 17:05:15.000000 pymc_bart-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 17:05:31.318673 pymc_bart-0.4.0/pymc_bart/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-17 17:05:15.000000 pymc_bart-0.4.0/pymc_bart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-03-17 17:05:15.000000 pymc_bart-0.4.0/pymc_bart/bart.py
--rw-r--r--   0 runner    (1001) docker     (123)    19343 2023-03-17 17:05:15.000000 pymc_bart-0.4.0/pymc_bart/pgbart.py
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-03-17 17:05:15.000000 pymc_bart-0.4.0/pymc_bart/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-03-17 17:05:15.000000 pymc_bart-0.4.0/pymc_bart/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 17:05:31.318673 pymc_bart-0.4.0/pymc_bart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-03-17 17:05:31.000000 pymc_bart-0.4.0/pymc_bart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-17 17:05:31.000000 pymc_bart-0.4.0/pymc_bart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 17:05:31.000000 pymc_bart-0.4.0/pymc_bart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-17 17:05:31.000000 pymc_bart-0.4.0/pymc_bart.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-17 17:05:31.000000 pymc_bart-0.4.0/pymc_bart.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-17 17:05:15.000000 pymc_bart-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-17 17:05:15.000000 pymc_bart-0.4.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-17 17:05:15.000000 pymc_bart-0.4.0/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-17 17:05:15.000000 pymc_bart-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 17:05:31.322672 pymc_bart-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-03-17 17:05:15.000000 pymc_bart-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 17:05:31.318673 pymc_bart-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-17 17:05:15.000000 pymc_bart-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-03-17 17:05:15.000000 pymc_bart-0.4.0/tests/test_bart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-03-17 17:05:15.000000 pymc_bart-0.4.0/tests/test_pgbart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-17 17:05:15.000000 pymc_bart-0.4.0/tests/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:47:16.811866 pymc_bart-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-10 17:47:16.811866 pymc_bart-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:47:16.807866 pymc_bart-0.5.0/pymc_bart/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/pymc_bart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/pymc_bart/bart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23435 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/pymc_bart/pgbart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/pymc_bart/split_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/pymc_bart/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27945 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/pymc_bart/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:47:16.807866 pymc_bart-0.5.0/pymc_bart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-10 17:47:16.000000 pymc_bart-0.5.0/pymc_bart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-10 17:47:16.000000 pymc_bart-0.5.0/pymc_bart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 17:47:16.000000 pymc_bart-0.5.0/pymc_bart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-10 17:47:16.000000 pymc_bart-0.5.0/pymc_bart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 17:47:16.000000 pymc_bart-0.5.0/pymc_bart.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 17:47:16.811866 pymc_bart-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:47:16.811866 pymc_bart-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/tests/test_bart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/tests/test_pgbart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/tests/test_split_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-10 17:47:07.000000 pymc_bart-0.5.0/tests/test_tree.py
```

### Comparing `pymc_bart-0.4.0/CODE_OF_CONDUCT.md` & `pymc_bart-0.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.4.0/CONTRIBUTING.md` & `pymc_bart-0.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.4.0/LICENSE` & `pymc_bart-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.4.0/PKG-INFO` & `pymc_bart-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc_bart
-Version: 0.4.0
+Version: 0.5.0
 Summary: Bayesian Additive Regression Trees for Probabilistic programming with PyMC
 Home-page: http://github.com/pymc-devs/pymc-bart
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -18,18 +18,18 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-Bayesian Additive Regression Trees for Probabilistic programming with PyMC
+# Bayesian Additive Regression Trees for Probabilistic programming with PyMC
 
 
-PyMC-BART extends [PyMC](https://github.com/pymc-devs/pymc) probabilistic programming framework to be able to define and solve models including a BART random variable. PyMC-BART also includes a few helpers function to aid with the interpretation of those models and perform variable selection. 
+PyMC-BART extends [PyMC](https://github.com/pymc-devs/pymc) probabilistic programming framework to be able to define and solve models including a BART random variable. PyMC-BART also includes a few helpers function to aid with the interpretation of those models and perform variable selection.
 
 
 ## Installation
 
 PyMC-BART is available on Conda-Forge. To set up a suitable Conda environment, run
 
 ```bash
```

### Comparing `pymc_bart-0.4.0/README.md` & `pymc_bart-0.5.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
-Bayesian Additive Regression Trees for Probabilistic programming with PyMC
+# Bayesian Additive Regression Trees for Probabilistic programming with PyMC
 
 
-PyMC-BART extends [PyMC](https://github.com/pymc-devs/pymc) probabilistic programming framework to be able to define and solve models including a BART random variable. PyMC-BART also includes a few helpers function to aid with the interpretation of those models and perform variable selection. 
+PyMC-BART extends [PyMC](https://github.com/pymc-devs/pymc) probabilistic programming framework to be able to define and solve models including a BART random variable. PyMC-BART also includes a few helpers function to aid with the interpretation of those models and perform variable selection.
 
 
 ## Installation
 
 PyMC-BART is available on Conda-Forge. To set up a suitable Conda environment, run
 
 ```bash
```

### Comparing `pymc_bart-0.4.0/pymc_bart/__init__.py` & `pymc_bart-0.5.0/pymc_bart/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 import pymc as pm
 
 from pymc_bart.bart import BART
 from pymc_bart.pgbart import PGBART
-from pymc_bart.utils import plot_convergence, plot_dependence, plot_variable_importance
+from pymc_bart.split_rules import ContinuousSplitRule, OneHotSplitRule, SubsetSplitRule
+from pymc_bart.utils import (
+    plot_convergence,
+    plot_pdp,
+    plot_ice,
+    plot_dependence,
+    plot_variable_importance,
+)
 
 __all__ = ["BART", "PGBART"]
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 
 pm.STEP_METHODS = list(pm.STEP_METHODS) + [PGBART]
```

### Comparing `pymc_bart-0.4.0/pymc_bart.egg-info/PKG-INFO` & `pymc_bart-0.5.0/pymc_bart.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc-bart
-Version: 0.4.0
+Version: 0.5.0
 Summary: Bayesian Additive Regression Trees for Probabilistic programming with PyMC
 Home-page: http://github.com/pymc-devs/pymc-bart
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -18,18 +18,18 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-Bayesian Additive Regression Trees for Probabilistic programming with PyMC
+# Bayesian Additive Regression Trees for Probabilistic programming with PyMC
 
 
-PyMC-BART extends [PyMC](https://github.com/pymc-devs/pymc) probabilistic programming framework to be able to define and solve models including a BART random variable. PyMC-BART also includes a few helpers function to aid with the interpretation of those models and perform variable selection. 
+PyMC-BART extends [PyMC](https://github.com/pymc-devs/pymc) probabilistic programming framework to be able to define and solve models including a BART random variable. PyMC-BART also includes a few helpers function to aid with the interpretation of those models and perform variable selection.
 
 
 ## Installation
 
 PyMC-BART is available on Conda-Forge. To set up a suitable Conda environment, run
 
 ```bash
```

### Comparing `pymc_bart-0.4.0/setup.py` & `pymc_bart-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import re
-
 from codecs import open
 from os.path import dirname, join, realpath
 
 from setuptools import find_packages, setup
 
 DISTNAME = "pymc_bart"
 DESCRIPTION = "Bayesian Additive Regression Trees for Probabilistic programming with PyMC"
```

### Comparing `pymc_bart-0.4.0/tests/__init__.py` & `pymc_bart-0.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.4.0/tests/test_bart.py` & `pymc_bart-0.5.0/tests/test_bart.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import numpy as np
 import pymc as pm
 import pytest
 from numpy.random import RandomState
 from numpy.testing import assert_almost_equal, assert_array_equal
+from pymc.initial_point import make_initial_point_fn
+from pymc.logprob.basic import joint_logp
 
 import pymc_bart as pmb
 
-from pymc.logprob.joint_logprob import joint_logp
-from pymc.initial_point import make_initial_point_fn
-
 
 def assert_moment_is_expected(model, expected, check_finite_logp=True):
     fn = make_initial_point_fn(
         model=model,
         return_transformed=False,
         default_strategy="moment",
     )
@@ -37,70 +36,90 @@
             )[0]
             .sum()
             .eval()
         )
         assert np.isfinite(logp_moment)
 
 
-def test_bart_vi():
+@pytest.mark.parametrize(
+    argnames="response",
+    argvalues=["constant", "linear"],
+    ids=["constant", "linear-response"],
+)
+def test_bart_vi(response):
     X = np.random.normal(0, 1, size=(250, 3))
     Y = np.random.normal(0, 1, size=250)
     X[:, 0] = np.random.normal(Y, 0.1)
 
     with pm.Model() as model:
-        mu = pmb.BART("mu", X, Y, m=10)
+        mu = pmb.BART("mu", X, Y, m=10, response=response)
         sigma = pm.HalfNormal("sigma", 1)
         y = pm.Normal("y", mu, sigma, observed=Y)
         idata = pm.sample(random_seed=3415)
         var_imp = (
             idata.sample_stats["variable_inclusion"]
             .stack(samples=("chain", "draw"))
             .mean("samples")
         )
         var_imp /= var_imp.sum()
         assert var_imp[0] > var_imp[1:].sum()
         assert_almost_equal(var_imp.sum(), 1)
 
 
-def test_missing_data():
+@pytest.mark.parametrize(
+    argnames="response",
+    argvalues=["constant", "linear"],
+    ids=["constant", "linear-response"],
+)
+def test_missing_data(response):
     X = np.random.normal(0, 1, size=(50, 2))
     Y = np.random.normal(0, 1, size=50)
     X[10:20, 0] = np.nan
 
     with pm.Model() as model:
-        mu = pmb.BART("mu", X, Y, m=10)
+        mu = pmb.BART("mu", X, Y, m=10, response=response)
         sigma = pm.HalfNormal("sigma", 1)
         y = pm.Normal("y", mu, sigma, observed=Y)
         idata = pm.sample(tune=100, draws=100, chains=1, random_seed=3415)
 
 
-def test_shared_variable():
+@pytest.mark.parametrize(
+    argnames="response",
+    argvalues=["constant", "linear"],
+    ids=["constant", "linear-response"],
+)
+def test_shared_variable(response):
     X = np.random.normal(0, 1, size=(50, 2))
     Y = np.random.normal(0, 1, size=50)
 
     with pm.Model() as model:
         data_X = pm.MutableData("data_X", X)
-        mu = pmb.BART("mu", data_X, Y, m=2)
+        mu = pmb.BART("mu", data_X, Y, m=2, response=response)
         sigma = pm.HalfNormal("sigma", 1)
         y = pm.Normal("y", mu, sigma, observed=Y, shape=mu.shape)
         idata = pm.sample(tune=100, draws=100, chains=2, random_seed=3415)
         ppc = pm.sample_posterior_predictive(idata)
         new_X = pm.set_data({"data_X": X[:3]})
         ppc2 = pm.sample_posterior_predictive(idata)
 
     assert ppc.posterior_predictive["y"].shape == (2, 100, 50)
     assert ppc2.posterior_predictive["y"].shape == (2, 100, 3)
 
 
-def test_shape():
+@pytest.mark.parametrize(
+    argnames="response",
+    argvalues=["constant", "linear"],
+    ids=["constant", "linear-response"],
+)
+def test_shape(response):
     X = np.random.normal(0, 1, size=(250, 3))
     Y = np.random.normal(0, 1, size=250)
 
     with pm.Model() as model:
-        w = pmb.BART("w", X, Y, m=2, shape=(2, 250))
+        w = pmb.BART("w", X, Y, m=2, response=response, shape=(2, 250))
         y = pm.Normal("y", w[0], pm.math.abs(w[1]), observed=Y)
         idata = pm.sample(random_seed=3415)
 
     assert model.initial_point()["w"].shape == (2, 250)
     assert idata.posterior.coords["w_dim_0"].data.size == 2
     assert idata.posterior.coords["w_dim_1"].data.size == 250
 
@@ -129,27 +148,43 @@
         assert pred_first.shape == (1, 10, 1)
 
     @pytest.mark.parametrize(
         "kwargs",
         [
             {},
             {
-                "kind": "pdp",
                 "samples": 2,
                 "xs_interval": "quantiles",
                 "xs_values": [0.25, 0.5, 0.75],
                 "var_discrete": [3],
             },
-            {"kind": "ice", "instances": 2},
-            {"var_idx": [0], "rug": False, "smooth": False, "color": "k"},
+            {"instances": 2},
+            {"var_idx": [0], "smooth": False, "color": "k"},
+            {"grid": (1, 2), "sharey": "none", "alpha": 1},
+        ],
+    )
+    def test_ice(self, kwargs):
+        pmb.plot_ice(self.mu, X=self.X, Y=self.Y, **kwargs)
+
+    @pytest.mark.parametrize(
+        "kwargs",
+        [
+            {},
+            {
+                "samples": 2,
+                "xs_interval": "quantiles",
+                "xs_values": [0.25, 0.5, 0.75],
+                "var_discrete": [3],
+            },
+            {"var_idx": [0], "smooth": False, "color": "k"},
             {"grid": (1, 2), "sharey": "none", "alpha": 1},
         ],
     )
     def test_pdp(self, kwargs):
-        pmb.plot_dependence(self.mu, X=self.X, Y=self.Y, **kwargs)
+        pmb.plot_pdp(self.mu, X=self.X, Y=self.Y, **kwargs)
 
     @pytest.mark.parametrize(
         "kwargs",
         [
             {},
             {"labels": ["A", "B", "C"], "samples": 2, "figsize": (6, 6)},
         ],
@@ -159,18 +194,18 @@
 
     def test_pdp_pandas_labels(self):
         pd = pytest.importorskip("pandas")
 
         X_names = ["norm1", "norm2", "binom"]
         X_pd = pd.DataFrame(self.X, columns=X_names)
         Y_pd = pd.Series(self.Y, name="response")
-        axes = pmb.plot_dependence(self.mu, X=X_pd, Y=Y_pd)
+        axes = pmb.plot_pdp(self.mu, X=X_pd, Y=Y_pd)
 
         figure = axes[0].figure
-        assert figure.texts[0].get_text() == "Predicted response"
+        assert figure.texts[0].get_text() == "Partial response"
         assert_array_equal([ax.get_xlabel() for ax in axes], X_names)
 
 
 @pytest.mark.parametrize(
     "size, expected",
     [
         (None, np.zeros(50)),
@@ -178,7 +213,34 @@
 )
 def test_bart_moment(size, expected):
     X = np.zeros((50, 2))
     Y = np.zeros(50)
     with pm.Model() as model:
         pmb.BART("x", X=X, Y=Y, size=size)
     assert_moment_is_expected(model, expected)
+
+
+@pytest.mark.parametrize(
+    argnames="separate_trees,split_rule",
+    argvalues=[
+        (False,pmb.ContinuousSplitRule),
+        (False,pmb.OneHotSplitRule),
+        (False,pmb.SubsetSplitRule),
+        (True,pmb.ContinuousSplitRule)
+    ],
+    ids=["continuous", "one-hot", "subset", "separate-trees"],
+)
+def test_categorical_model(separate_trees,split_rule):
+
+    Y = np.array([0, 0, 0, 1, 1, 1, 2, 2, 2])
+    X = np.concatenate([Y[:, None], np.random.randint(0, 6, size=(9, 4))], axis=1)
+
+    with pm.Model() as model:
+        lo = pmb.BART("logodds", X, Y, m=2, shape=(3, 9),
+            split_rules=[split_rule]*5,
+            separate_trees=separate_trees)
+        y = pm.Categorical("y", p=pm.math.softmax(lo.T, axis=-1), observed=Y)
+        idata = pm.sample(random_seed=3415, tune=300, draws=300)
+        idata = pm.sample_posterior_predictive(idata, predictions=True, extend_inferencedata=True)
+
+    # Fit should be good enough so right category is selected over 50% of time
+    assert (idata.predictions.y.median(["chain", "draw"]) == Y).all()
```

### Comparing `pymc_bart-0.4.0/tests/test_pgbart.py` & `pymc_bart-0.5.0/tests/test_pgbart.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 from unittest import TestCase
+import pytest
 import numpy as np
 import pymc as pm
+
 import pymc_bart as pmb
-from pymc_bart.pgbart import fast_mean, discrete_uniform_sampler, NormalSampler, UniformSampler
+from pymc_bart.pgbart import (
+    NormalSampler,
+    UniformSampler,
+    discrete_uniform_sampler,
+    fast_mean,
+    fast_linear_fit,
+)
 
 
 class TestSystematic(TestCase):
     def test_systematic(self):
         X = np.random.normal(0, 1, size=(250, 3))
         Y = np.random.normal(0, 1, size=250)
         X[:, 0] = np.random.normal(Y, 0.1)
@@ -17,15 +25,15 @@
             y = pm.Normal("y", mu, sigma, observed=Y)
             step = pmb.PGBART([mu])
 
         normalized_weights = np.array([0.5, 0.3, 0.2])
         indices = step.systematic(normalized_weights)
 
         self.assertEqual(len(indices), len(normalized_weights))
-        self.assertEqual(indices.dtype, np.int)
+        self.assertEqual(indices.dtype, np.int_)
         self.assertTrue(all(i >= 0 and i < len(normalized_weights) for i in indices))
 
         normalized_weights = np.array([0, 0.25, 0.75])
         indices = step.systematic(normalized_weights)
         self.assertTrue(all(i >= 1 and i < len(normalized_weights) for i in indices))
 
 
@@ -33,14 +41,31 @@
     values = np.random.uniform(size=10)
     np.testing.assert_almost_equal(fast_mean(values), np.mean(values))
 
     values = np.random.uniform(size=(2, 10))
     np.testing.assert_array_almost_equal(fast_mean(values), np.mean(values, 1))
 
 
+@pytest.mark.parametrize(
+    argnames="x,y,a_expected, b_expected",
+    argvalues=[
+        (np.array([1, 2, 3, 4, 5]), np.array([[1, 2, 3, 4, 5]]), 0.0, 1.0),
+        (np.array([1, 2, 3, 4, 5]), np.array([[1, 1, 1, 1, 1]]), 1.0, 0.0),
+    ],
+    ids=["1d-id", "1d-const"],
+)
+def test_fast_linear_fit(x, y, a_expected, b_expected):
+    y_fit, linear_params = fast_linear_fit(x, y, m=1, norm=np.zeros(1))
+    assert linear_params[0] == a_expected
+    assert linear_params[1] == b_expected
+    np.testing.assert_almost_equal(
+        actual=y_fit, desired=np.atleast_2d(a_expected + x * b_expected).T
+    )
+
+
 def test_discrete_uniform():
     sample = discrete_uniform_sampler(7)
     assert isinstance(sample, int)
     samples = np.array([discrete_uniform_sampler(7) for i in range(1000)])
     assert all(samples >= 0)
     assert all(samples < 7)
```

### Comparing `pymc_bart-0.4.0/tests/test_tree.py` & `pymc_bart-0.5.0/tests/test_tree.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import numpy as np
 
-from pymc_bart.tree import Node, get_depth
+from pymc_bart.tree import Node, get_idx_left_child, get_idx_right_child, get_depth
 
 
 def test_split_node():
-    split_node = Node.new_split_node(index=5, idx_split_variable=2, split_value=3.0)
-    assert split_node.index == 5
-    assert get_depth(split_node.index) == 2
+    index = 5
+    split_node = Node(idx_split_variable=2, value=3.0)
+    assert get_depth(index) == 2
     assert split_node.value == 3.0
     assert split_node.idx_split_variable == 2
     assert split_node.idx_data_points is None
-    assert split_node.get_idx_left_child() == 11
-    assert split_node.get_idx_right_child() == 12
+    assert get_idx_left_child(index) == 11
+    assert get_idx_right_child(index) == 12
     assert split_node.is_split_node() is True
     assert split_node.is_leaf_node() is False
 
 
 def test_leaf_node():
-    leaf_node = Node.new_leaf_node(index=5, value=3.14, idx_data_points=[1, 2, 3])
-    assert leaf_node.index == 5
-    assert get_depth(leaf_node.index) == 2
+    index = 5
+    leaf_node = Node.new_leaf_node(value=3.14, idx_data_points=[1, 2, 3])
+    assert get_depth(index) == 2
     assert leaf_node.value == 3.14
     assert leaf_node.idx_split_variable == -1
     assert np.array_equal(leaf_node.idx_data_points, [1, 2, 3])
-    assert leaf_node.get_idx_left_child() == 11
-    assert leaf_node.get_idx_right_child() == 12
+    assert get_idx_left_child(index) == 11
+    assert get_idx_right_child(index) == 12
     assert leaf_node.is_split_node() is False
     assert leaf_node.is_leaf_node() is True
```

