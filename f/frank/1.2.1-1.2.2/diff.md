# Comparing `tmp/frank-1.2.1.tar.gz` & `tmp/frank-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/frank-1.2.1.tar", last modified: Fri Dec  2 19:05:42 2022, max compression
+gzip compressed data, was "frank-1.2.2.tar", last modified: Mon Jul 10 12:38:36 2023, max compression
```

## Comparing `frank-1.2.1.tar` & `frank-1.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 jeffjennings   (502) staff       (20)        0 2022-12-02 19:05:42.000000 frank-1.2.1/
--rw-r--r--   0 jeffjennings   (502) staff       (20)      320 2022-08-10 02:00:32.000000 frank-1.2.1/AUTHORS.rst
--rw-r--r--   0 jeffjennings   (502) staff       (20)     4420 2022-12-02 19:05:12.000000 frank-1.2.1/HISTORY.rst
--rw-r--r--   0 jeffjennings   (502) staff       (20)     7651 2022-11-09 21:11:25.000000 frank-1.2.1/LICENSE.txt
--rw-r--r--   0 jeffjennings   (502) staff       (20)      221 2022-11-09 21:11:25.000000 frank-1.2.1/MANIFEST.in
--rw-r--r--   0 jeffjennings   (502) staff       (20)     5598 2022-12-02 19:05:42.000000 frank-1.2.1/PKG-INFO
--rw-r--r--   0 jeffjennings   (502) staff       (20)     4473 2022-11-09 21:11:25.000000 frank-1.2.1/README.md
-drwxr-xr-x   0 jeffjennings   (502) staff       (20)        0 2022-12-02 19:05:42.000000 frank-1.2.1/frank/
--rw-r--r--   0 jeffjennings   (502) staff       (20)     1716 2022-12-02 19:05:12.000000 frank-1.2.1/frank/__init__.py
--rw-r--r--   0 jeffjennings   (502) staff       (20)     1024 2022-11-09 12:11:33.000000 frank-1.2.1/frank/constants.py
--rw-r--r--   0 jeffjennings   (502) staff       (20)     6712 2022-11-09 21:12:48.000000 frank-1.2.1/frank/debris_fitters.py
--rw-r--r--   0 jeffjennings   (502) staff       (20)     1722 2022-11-21 13:41:28.000000 frank-1.2.1/frank/default_parameters.json
--rw-r--r--   0 jeffjennings   (502) staff       (20)     7479 2022-11-11 20:32:11.000000 frank-1.2.1/frank/filter.py
--rw-r--r--   0 jeffjennings   (502) staff       (20)    33086 2022-11-21 13:41:28.000000 frank-1.2.1/frank/fit.py
--rw-r--r--   0 jeffjennings   (502) staff       (20)      626 2022-08-10 02:00:33.000000 frank-1.2.1/frank/frank.mplstyle
--rw-r--r--   0 jeffjennings   (502) staff       (20)    24895 2022-11-11 20:32:11.000000 frank-1.2.1/frank/geometry.py
--rw-r--r--   0 jeffjennings   (502) staff       (20)     7134 2022-11-11 20:32:11.000000 frank-1.2.1/frank/hankel.py
--rw-r--r--   0 jeffjennings   (502) staff       (20)     7395 2022-11-09 21:11:25.000000 frank-1.2.1/frank/io.py
--rw-r--r--   0 jeffjennings   (502) staff       (20)    47045 2022-11-09 21:11:25.000000 frank-1.2.1/frank/make_figs.py
--rw-r--r--   0 jeffjennings   (502) staff       (20)     9546 2022-11-11 20:32:11.000000 frank-1.2.1/frank/minimizer.py
--rw-r--r--   0 jeffjennings   (502) staff       (20)     5618 2022-11-21 13:41:28.000000 frank-1.2.1/frank/parameter_descriptions.json
--rw-r--r--   0 jeffjennings   (502) staff       (20)    12733 2022-11-09 21:11:25.000000 frank-1.2.1/frank/plot.py
--rw-r--r--   0 jeffjennings   (502) staff       (20)    31206 2022-11-11 20:32:11.000000 frank-1.2.1/frank/radial_fitters.py
--rw-r--r--   0 jeffjennings   (502) staff       (20)    41741 2022-11-16 19:45:15.000000 frank-1.2.1/frank/statistical_models.py
--rw-r--r--   0 jeffjennings   (502) staff       (20)    19865 2022-11-11 20:32:11.000000 frank-1.2.1/frank/tests.py
--rw-r--r--   0 jeffjennings   (502) staff       (20)    34592 2022-11-11 20:32:11.000000 frank-1.2.1/frank/utilities.py
-drwxr-xr-x   0 jeffjennings   (502) staff       (20)        0 2022-12-02 19:05:42.000000 frank-1.2.1/frank.egg-info/
--rw-r--r--   0 jeffjennings   (502) staff       (20)     5598 2022-12-02 19:05:40.000000 frank-1.2.1/frank.egg-info/PKG-INFO
--rw-r--r--   0 jeffjennings   (502) staff       (20)      579 2022-12-02 19:05:41.000000 frank-1.2.1/frank.egg-info/SOURCES.txt
--rw-r--r--   0 jeffjennings   (502) staff       (20)        1 2022-12-02 19:05:40.000000 frank-1.2.1/frank.egg-info/dependency_links.txt
--rw-r--r--   0 jeffjennings   (502) staff       (20)      188 2022-12-02 19:05:40.000000 frank-1.2.1/frank.egg-info/requires.txt
--rw-r--r--   0 jeffjennings   (502) staff       (20)        6 2022-12-02 19:05:40.000000 frank-1.2.1/frank.egg-info/top_level.txt
--rw-r--r--   0 jeffjennings   (502) staff       (20)     1458 2022-12-02 19:05:42.000000 frank-1.2.1/setup.cfg
--rw-r--r--   0 jeffjennings   (502) staff       (20)      115 2022-11-09 21:11:25.000000 frank-1.2.1/setup.py
+drwxr-xr-x   0 jj        (1000) jj        (1000)        0 2023-07-10 12:38:36.745163 frank-1.2.2/
+-rw-r--r--   0 jj        (1000) jj        (1000)      320 2023-01-17 16:44:29.000000 frank-1.2.2/AUTHORS.rst
+-rw-r--r--   0 jj        (1000) jj        (1000)     5528 2023-07-10 12:37:48.000000 frank-1.2.2/HISTORY.rst
+-rw-r--r--   0 jj        (1000) jj        (1000)     7651 2023-01-17 16:44:29.000000 frank-1.2.2/LICENSE.txt
+-rw-r--r--   0 jj        (1000) jj        (1000)      221 2023-01-17 16:44:29.000000 frank-1.2.2/MANIFEST.in
+-rw-r--r--   0 jj        (1000) jj        (1000)     5548 2023-07-10 12:38:36.745163 frank-1.2.2/PKG-INFO
+-rw-r--r--   0 jj        (1000) jj        (1000)     4473 2023-01-17 16:44:29.000000 frank-1.2.2/README.md
+drwxr-xr-x   0 jj        (1000) jj        (1000)        0 2023-07-10 12:38:36.745163 frank-1.2.2/frank/
+-rw-r--r--   0 jj        (1000) jj        (1000)     1716 2023-07-10 12:37:48.000000 frank-1.2.2/frank/__init__.py
+-rw-r--r--   0 jj        (1000) jj        (1000)      994 2023-07-10 12:37:48.000000 frank-1.2.2/frank/constants.py
+-rw-r--r--   0 jj        (1000) jj        (1000)     7016 2023-07-10 12:37:48.000000 frank-1.2.2/frank/debris_fitters.py
+-rw-r--r--   0 jj        (1000) jj        (1000)     1846 2023-07-10 12:37:48.000000 frank-1.2.2/frank/default_parameters.json
+-rw-r--r--   0 jj        (1000) jj        (1000)     8181 2023-07-10 12:37:48.000000 frank-1.2.2/frank/filter.py
+-rw-r--r--   0 jj        (1000) jj        (1000)    34922 2023-07-10 12:37:48.000000 frank-1.2.2/frank/fit.py
+-rw-r--r--   0 jj        (1000) jj        (1000)      626 2023-01-17 16:44:29.000000 frank-1.2.2/frank/frank.mplstyle
+-rw-r--r--   0 jj        (1000) jj        (1000)    24895 2023-05-22 12:19:40.000000 frank-1.2.2/frank/geometry.py
+-rw-r--r--   0 jj        (1000) jj        (1000)     9094 2023-07-10 12:37:48.000000 frank-1.2.2/frank/hankel.py
+-rw-r--r--   0 jj        (1000) jj        (1000)     7476 2023-07-10 12:37:48.000000 frank-1.2.2/frank/io.py
+-rw-r--r--   0 jj        (1000) jj        (1000)    48424 2023-06-21 17:10:10.000000 frank-1.2.2/frank/make_figs.py
+-rw-r--r--   0 jj        (1000) jj        (1000)     9546 2023-01-17 16:52:15.000000 frank-1.2.2/frank/minimizer.py
+-rw-r--r--   0 jj        (1000) jj        (1000)     6552 2023-07-10 12:37:48.000000 frank-1.2.2/frank/parameter_descriptions.json
+-rw-r--r--   0 jj        (1000) jj        (1000)    12715 2023-07-10 12:37:42.000000 frank-1.2.2/frank/plot.py
+-rw-r--r--   0 jj        (1000) jj        (1000)    33375 2023-07-10 12:37:48.000000 frank-1.2.2/frank/radial_fitters.py
+-rw-r--r--   0 jj        (1000) jj        (1000)    43205 2023-07-10 12:37:48.000000 frank-1.2.2/frank/statistical_models.py
+-rw-r--r--   0 jj        (1000) jj        (1000)    21928 2023-07-10 12:37:48.000000 frank-1.2.2/frank/tests.py
+-rw-r--r--   0 jj        (1000) jj        (1000)    35971 2023-07-10 12:37:48.000000 frank-1.2.2/frank/utilities.py
+drwxr-xr-x   0 jj        (1000) jj        (1000)        0 2023-07-10 12:38:36.745163 frank-1.2.2/frank.egg-info/
+-rw-r--r--   0 jj        (1000) jj        (1000)     5548 2023-07-10 12:38:36.000000 frank-1.2.2/frank.egg-info/PKG-INFO
+-rw-r--r--   0 jj        (1000) jj        (1000)      579 2023-07-10 12:38:36.000000 frank-1.2.2/frank.egg-info/SOURCES.txt
+-rw-r--r--   0 jj        (1000) jj        (1000)        1 2023-07-10 12:38:36.000000 frank-1.2.2/frank.egg-info/dependency_links.txt
+-rw-r--r--   0 jj        (1000) jj        (1000)      188 2023-07-10 12:38:36.000000 frank-1.2.2/frank.egg-info/requires.txt
+-rw-r--r--   0 jj        (1000) jj        (1000)        6 2023-07-10 12:38:36.000000 frank-1.2.2/frank.egg-info/top_level.txt
+-rw-r--r--   0 jj        (1000) jj        (1000)     1419 2023-07-10 12:38:36.745163 frank-1.2.2/setup.cfg
+-rw-r--r--   0 jj        (1000) jj        (1000)      115 2023-01-17 16:44:29.000000 frank-1.2.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `frank-1.2.1/HISTORY.rst` & `frank-1.2.2/HISTORY.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,38 @@
 .. :history:
 
 Changelog
 +++++++++
 
+v.1.2.2
++++++++
+*One bug fix, some code refactoring, a couple new functionalities, integrates scale-height fits into command-line UI*
+
+- default_parameters.json, parameter_descriptions.json:
+    - Adds parameters: 'convergence_failure', 'I_scale', 'save_figures', 'scale_height'
+- filter.py
+    - Breaks 'spectral_smoothing_matrix' out of 'CriticalFilter'; some restructuring of 'covariance_MAP' and 'log_prior'
+- fit.py
+    - Adds 'get_scale_height' function
+- hankel.py
+    - Adds 'interpolation_coefficients' and 'interpolate' functions
+- io.py
+    - Fixed a bug that was saving incorrect uncertainty for LogNormal brightness profile
+- make_figs.py
+    - Adds non-negative fit to figures
+- radial_fitters.py
+    - Adds 'convergence_failure' arg to FrankFitter
+    - Adds 'log_evidence_laplace' function to FrankFitter
+- statistical_models.py
+    - Adds 'DHT_coefficients' and 'interpolate' functions to 'VisibilityMapping'
+- test.py
+    - Adds tests for non-negative solver ('test_solve_non_negative') and solution object IO ('test_save_load_sol')
+- utilities.py
+    - Adds 'get_fit_stat_uncer' function
+
 v.1.2.1
 +++++++
 *Fixed a bug that caused non-python files to not be installed through pip*
 
 v.1.2.0
 +++++++
 *Introduction of log-normal fits, large amount of code refactoring to support both 'Gaussian' and 'LogNormal' methods*
```

### Comparing `frank-1.2.1/LICENSE.txt` & `frank-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `frank-1.2.1/PKG-INFO` & `frank-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: frank
-Version: 1.2.1
+Version: 1.2.2
 Summary: Frankenstein, the flux reconstructor
 Home-page: https://github.com/discsim/frank
 Author: Richard Booth, Jeff Jennings, Marco Tazzari
 Author-email: jjennings1519@gmail.com
 License: LGPLv3
 Project-URL: Bug Tracker, https://github.com/discsim/frank/issues
 Keywords: science,astronomy,interferometry
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs-build
 License-File: LICENSE.txt
 
 <p align="center">
    <img width = "800" src="https://github.com/discsim/frank/blob/master/docs/images/day_off.png?raw=true"/>
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: frank Version: 1.2.1 Summary: Frankenstein, the
+Metadata-Version: 2.1 Name: frank Version: 1.2.2 Summary: Frankenstein, the
 flux reconstructor Home-page: https://github.com/discsim/frank Author: Richard
 Booth, Jeff Jennings, Marco Tazzari Author-email: jjennings1519@gmail.com
 License: LGPLv3 Project-URL: Bug Tracker, https://github.com/discsim/frank/
 issues Keywords: science,astronomy,interferometry Classifier: Development
 Status :: 5 - Production/Stable Classifier: License :: OSI Approved :: GNU
 Lesser General Public License v3 (LGPLv3) Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
-Linux Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
-test Provides-Extra: docs-build License-File: LICENSE.txt
+Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
+text/markdown Provides-Extra: test Provides-Extra: docs-build License-File:
+LICENSE.txt
 [https://github.com/discsim/frank/blob/master/docs/images/day_off.png?raw=true]
     [https://img.shields.io/github/release/discsim/frank/all.svg]  [https://
                        img.shields.io/pypi/v/frank.svg]_
         _[https://img.shields.io/badge/changelog-detailed-blue]__[DOI]_
   _[https://github.com/discsim/frank/actions/workflows/tests.yml/badge.svg]__
    [https://github.com/discsim/frank/actions/workflows/docs.yml/badge.svg]__
              [https://discsim.github.io/frank/coverage/badge.svg]_
```

### Comparing `frank-1.2.1/README.md` & `frank-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `frank-1.2.1/frank/__init__.py` & `frank-1.2.2/frank/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>
 #
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 
 from frank import constants
 from frank import geometry
 from frank import hankel
 from frank import io
 from frank import radial_fitters
 from frank import debris_fitters
```

### Comparing `frank-1.2.1/frank/constants.py` & `frank-1.2.2/frank/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,12 +15,11 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>
 #
 """This module contains useful conversion constants."""
 
 import numpy as np
-from scipy.constants import c
 
 rad_to_arcsec = 3600 * 180 / np.pi
 sterad_to_arcsec = rad_to_arcsec ** 2
 deg_to_rad = np.pi / 180
```

### Comparing `frank-1.2.1/frank/debris_fitters.py` & `frank-1.2.2/frank/debris_fitters.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,14 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>
 #
 """This module contains methods for fitting a radial brightness profile to a set
   of deprojected visibities. Routines in this file assume that the emission is
   optically thin with a Gaussian vertical structure.
 """
-import abc
-from collections import defaultdict
-import logging
-import numpy as np
-
 from frank.radial_fitters import FourierBesselFitter, FrankFitter
 
 class FourierBesselDebrisFitter(FourierBesselFitter):
     """
     Fourier-Bessel series optically-thin model for fitting visibilities.
 
     The brightness model is :math:`I(R, z) = I(R) exp(-z^2/2H(R)^2)`, where
@@ -125,29 +120,37 @@
         Whether to check if the first (last) collocation point is smaller
         (larger) than the shortest (longest) deprojected baseline in the dataset
     store_iteration_diagnostics: bool, default = False
         Whether to store the power spectrum parameters and brightness profile
         for each fit iteration
     verbose:
         Whether to print notification messages
+    convergence_failure: string, default = 'raise'
+        Decide what to do when the frank model does not converge within max_iter.
+        Should be one of:
+        'raise'  : raise an error
+        'warn'   : print a warning message and continue
+        'ignore' : Ignore the error.
 
     References
     ----------
         Baddour & Chouinard (2015)
             DOI: https://doi.org/10.1364/JOSAA.32.000611
         Oppermann et al. (2013)
             DOI:  https://doi.org/10.1103/PhysRevE.87.032136
     """
 
     def __init__(self, Rmax, N, geometry, scale_height, nu=0, block_data=True,
                  block_size=10 ** 5, alpha=1.05, p_0=None, weights_smooth=1e-4,
                  tol=1e-3, method='Normal', I_scale=1e5, max_iter=2000, check_qbounds=True,
-                 store_iteration_diagnostics=False, verbose=True):
+                 store_iteration_diagnostics=False, verbose=True, 
+                 convergence_failure='raise'):
 
         # All functionality is provided by the base class. FrankDebrisFitter is just a 
         # sub-set of FrankFitter
         super(FrankDebrisFitter, self).__init__(
             Rmax, N, geometry, nu=nu, block_data=block_data,
             block_size=block_size, alpha=alpha, p_0=p_0, weights_smooth=weights_smooth,
             tol=tol, method=method, I_scale=I_scale, max_iter=max_iter, 
             check_qbounds=check_qbounds, store_iteration_diagnostics=store_iteration_diagnostics, 
-            assume_optically_thick=False, scale_height=scale_height, verbose=verbose)
+            assume_optically_thick=False, scale_height=scale_height, verbose=verbose,
+            convergence_failure=convergence_failure)
```

### Comparing `frank-1.2.1/frank/default_parameters.json` & `frank-1.2.2/frank/default_parameters.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9634680134680135%*

 * *Differences: {"'geometry'": "{'scale_height': None}",*

 * * "'hyperparameters'": "{'nonnegative': True, 'converge_failure': 'warn', 'I_scale': 100000.0}",*

 * * "'input_output'": "{'save_figures': True}"}*

```diff
@@ -13,31 +13,35 @@
         "dra": 0.0,
         "fit_inc_pa": true,
         "fit_phase_offset": true,
         "inc": 0.0,
         "initial_guess": false,
         "pa": 0.0,
         "rescale_flux": true,
+        "scale_height": null,
         "type": "gaussian"
     },
     "hyperparameters": {
+        "I_scale": 100000.0,
         "alpha": 1.05,
+        "converge_failure": "warn",
         "iter_tol": 0.001,
         "max_iter": 2000,
         "method": "Normal",
         "n": 300,
-        "nonnegative": false,
+        "nonnegative": true,
         "p0": null,
         "rout": 2.0,
         "wsmooth": 0.0001
     },
     "input_output": {
         "format": null,
         "iteration_diag": false,
         "save_dir": "",
+        "save_figures": true,
         "save_profile_fit": true,
         "save_solution": true,
         "save_uvtables": true,
         "save_vis_fit": true,
         "uvtable_filename": ""
     },
     "modify_data": {
```

### Comparing `frank-1.2.1/frank/filter.py` & `frank-1.2.2/frank/filter.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,16 +16,54 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>
 #
 import numpy as np
 import scipy.sparse
 
-from frank.constants import rad_to_arcsec
+def spectral_smoothing_matrix(DHT, weights):
+    r"""Compute the spectral smoothing prior matrix, Tij.
+    
+    .. math::
+        log P(p|q, w) = -1/2 q.T . Tij . q
+    
+    Parameters
+    ----------
+    DHT : DiscreteHankelTransform object
+        DHT to build the smoothing matrix for.
+    weights : float > 0
+        Weighting parameter used for the spectral smoothing matrix
+
+    Returns
+    -------
+    Tij : Sparse Matrix
+        Spectral smoothing p
+    """
+    log_q = np.log(DHT.q)
+    dc = (log_q[2:] - log_q[:-2]) / 2
+    de = np.diff(log_q)
+
+    N = DHT.size
+
+    Delta = np.zeros([3, N])
+    Delta[0, :-2] = 1 / (dc * de[:-1])
+    Delta[1, 1:-1] = - (1 / de[1:] + 1 / de[:-1]) / dc
+    Delta[2, 2:] = 1 / (dc * de[1:])
+
+    Delta = scipy.sparse.dia_matrix((Delta, [-1, 0, 1]),
+                                    shape=(N, N))
+
+    dce = np.zeros_like(log_q)
+    dce[1:-1] = dc
+    dce = scipy.sparse.dia_matrix((dce.reshape(1, -1), 0),
+                                    shape=(N, N))
+
+    Tij = Delta.T.dot(dce.dot(Delta))
 
+    return weights * Tij 
 
 class CriticalFilter:
     """Optimizer for power-spectrum priors.
 
     Parameters
     ----------
     DHT : DiscreteHankelTransform
@@ -50,39 +88,15 @@
 
         self._alpha = alpha
         self._p_0 = p_0
         self._rho = 1.0
 
         self._tol = tol
 
-        self._Tij = weights_smooth * self._build_smoothing_matrix()
-
-    def _build_smoothing_matrix(self):
-        log_q = np.log(self._DHT.q)
-        dc = (log_q[2:] - log_q[:-2]) / 2
-        de = np.diff(log_q)
-
-        N = self._DHT.size
-
-        Delta = np.zeros([3, N])
-        Delta[0, :-2] = 1 / (dc * de[:-1])
-        Delta[1, 1:-1] = - (1 / de[1:] + 1 / de[:-1]) / dc
-        Delta[2, 2:] = 1 / (dc * de[1:])
-
-        Delta = scipy.sparse.dia_matrix((Delta, [-1, 0, 1]),
-                                        shape=(N, N))
-
-        dce = np.zeros_like(log_q)
-        dce[1:-1] = dc
-        dce = scipy.sparse.dia_matrix((dce.reshape(1, -1), 0),
-                                      shape=(N, N))
-
-        Tij = Delta.T.dot(dce.dot(Delta))
-
-        return Tij 
+        self._Tij = spectral_smoothing_matrix(DHT, weights_smooth)
 
     def update_power_spectrum_multiple(self, fit, binning=None):
         """Estimate the best fit power spectrum given the current model fit.
         This version works when there are multiple fields being fit simultaneously.
         """
 
         Nfields, Np = fit.power_spectrum.shape
@@ -163,22 +177,25 @@
         return np.exp(tau)
 
     def check_convergence(self, pi_new, pi_old):
         """Determine whether the  power-spectrum iterations have converged"""
         return np.all(np.abs(pi_new - pi_old) <= self._tol * pi_new)
 
 
-    def covariance_MAP(self, fit):
+    def covariance_MAP(self, fit, ret_inv=False):
         """
         Covariance of the power spectrum at maximum likelihood
 
         Parameters
         ----------
         fit : _HankelRegressor
             Solution at maximum likelihood
+        ret_inv : bool, default=False
+            If True return the inverse covariance matrix instead. This 
+            avoids inverting the inverse covariace matrix
 
         Returns
         -------
         ps_cov : 2D array
             Covariance matrix of the power spectrum at maximum likelihood
 
         Notes
@@ -187,38 +204,43 @@
 
         """
         Ykm = self._DHT.coefficients()
 
         mq = np.dot(Ykm, fit.MAP)
 
         mqq = np.outer(mq, mq)
-        Dqq = np.dot(Ykm, fit.Dsolve(Ykm.T))
+        Dqq = np.dot(Ykm, np.dot(fit.covariance, Ykm.T))
 
         p = fit.power_spectrum
-        tau = np.log(p)
 
         hess = \
-            + np.diag(self._alpha - 1.0 + 0.5 * self._rho + self._Tij.dot(tau)) \
+            + np.diag(self._p_0/p + 0.5*(mq**2 + np.diag(Dqq))/p) \
             + self._Tij.todense() \
             - 0.5 * np.outer(1 / p, 1 / p) * (2 * mqq + Dqq) * Dqq
 
-        # Invert the Hessian
-        hess_chol = scipy.linalg.cho_factor(hess)
-        ps_cov = scipy.linalg.cho_solve(hess_chol, np.eye(self._DHT.size))
+        if ret_inv:
+            return hess 
+        else:
+            # Invert the Hessian
+            hess_chol = scipy.linalg.cho_factor(hess)
+            ps_cov = scipy.linalg.cho_solve(hess_chol, np.eye(self._DHT.size))
 
-        return ps_cov
+            return ps_cov
 
     def log_prior(self, p):
-        """
+        r"""
         Compute the log prior probability, log(P(p)),
 
         .. math:
-            `log[P(p)] ~ np.sum(p0/pi - alpha*np.log(p0/pi))
+            `log[P(p)] ~ - np.sum(p0/pi + (alpha-1)*np.log(p0/pi))
             - 0.5*np.log(p) (weights_smooth*T) np.log(p)`
 
+        Note that frank uses log(p) in the inference hence the probability
+        is normalized such that ..math:`\int P(p) d\log p = 1`.
+
         Parameters
         ----------
         p : array, size = N
             Power spectrum coefficients.
         
         Returns
         -------
@@ -228,14 +250,14 @@
         Notes
         -----
         Computed up to a normalizing constant that depends on alpha and p0
         """
 
         # Add the power spectrum prior term
         xi = self._p_0 / p
-        like = np.sum(xi - self._alpha * np.log(xi))
+        like = - np.sum(xi + (self._alpha-1) * np.log(xi))
 
         # Extra term due to spectral smoothness
         tau = np.log(p)
         like -= 0.5 * np.dot(tau, self._Tij.dot(tau))
 
         return like
```

### Comparing `frank-1.2.1/frank/fit.py` & `frank-1.2.2/frank/fit.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 #
 """This module runs Frankenstein to fit a source's 1D radial brightness profile.
    A default parameter file is used that specifies all options to run the fit
    and output results. Alternatively a custom parameter file can be provided.
 """
 
 import os
-import sys
 import time
 import json
 
 # Force frank to run on a single thread if we are using it as a library
 def _check_and_warn_if_parallel():
     """Check numpy is running in parallel"""
     num_threads = int(os.environ.get('OMP_NUM_THREADS', '1'))
@@ -34,15 +33,14 @@
         logging.warning("WARNING: You are running frank with "
                         "OMP_NUM_THREADS={}.".format(num_threads) +
                         "The code will likely run faster on a single thread.\n"
                         "Use 'unset OMP_NUM_THREADS' or "
                         "'export OMP_NUM_THREADS=1' to disable this warning.")
 
 import numpy as np
-
 import logging
 
 import frank
 from frank import io, geometry, make_figs, radial_fitters, utilities
 
 frank_path = os.path.dirname(frank.__file__)
 
@@ -132,14 +130,19 @@
         model['input_output']['save_dir'] = os.path.dirname(uv_path)
 
     # Add a save prefix to the .json parameter file for later use
     model['input_output']['save_prefix'] = save_prefix =  \
         os.path.join(model['input_output']['save_dir'],
                      os.path.splitext(os.path.basename(uv_path))[0])
 
+    if model['input_output']['save_figures'] is True:
+        model['input_output']['fig_save_prefix'] = save_prefix
+    else:
+        model['input_output']['fig_save_prefix'] = None
+
     log_path = save_prefix + '_frank_fit.log'
     frank.enable_logging(log_path)
 
     # Check whether the code runs in parallel now that the logging has been
     # initialized.
     _check_and_warn_if_parallel()
 
@@ -148,14 +151,27 @@
                  ' {}'.format(model['input_output']['uvtable_filename']))
 
     # Sanity check some of the .json parameters
     if model['hyperparameters']['method'] not in ["Normal", "LogNormal"]:
         err = ValueError("method should be 'Normal' or 'LogNormal'")
         raise err
 
+    if model['geometry']['scale_height'] is not None and \
+       model['hyperparameters']['method'] == 'LogNormal':
+        logging.warning("WARNING: 'scale_height' is not 'None' AND 'method' is "
+                        "'LogNormal'. It is suggested to use the 'Normal' method " 
+                        "for vertical inference.")
+
+    if model['hyperparameters']['nonnegative'] and \
+       model['hyperparameters']['method'] == 'LogNormal':
+        logging.warning("WARNING: 'nonnegative' is 'true' AND 'method' is "
+                        "'LogNormal' --> performing a LogNormal fit and setting "
+                        "'nonnegative' to 'false'")
+        model['hyperparameters']['nonnegative'] = False
+
     if model['hyperparameters']['method'] == 'LogNormal' and \
        model['hyperparameters']['p0'] is not None and \
        model['hyperparameters']['p0'] > 1e-30:
         err = ValueError("p0 = {}. If method is 'LogNormal', p0 should be "
                          "<~ 1e-35 (we recommend 1e-35)"
                          ".".format(model['hyperparameters']['p0']))
         raise err
@@ -362,14 +378,50 @@
 
     # Store geometry
     geom = geom.clone()
 
     return geom
 
 
+def get_scale_height(model):
+    """
+    Parse the functional form for disc scale-height in the parameter file
+
+    Parameters
+    ----------
+    model : dict
+        Dictionary containing model parameters the fit uses
+
+    Returns
+    -------
+    scale_height : function R --> H
+        Returns None if scale_height is 'null' in the input parameter file.
+        Else, returns a function for the vertical thickness of disc provided in 
+        the parameter file.
+
+    """
+
+    if model['geometry']['scale_height'] is None:
+        return
+
+    else:
+        if model['geometry']['rescale_flux']:
+            err = ValueError("scale_height should be 'null' if rescale_flux is 'true'")
+            raise err
+
+        def scale_height(R):
+            """Power-law with cutoff, unit=[arcsec]"""
+            vars = model['geometry']['scale_height']
+            h0, a, r0, b = vars['h0'], vars['a'], vars['r0'], vars['b']
+
+            return h0 * R ** a * np.exp(-(R / r0) ** b)
+
+        return scale_height
+
+
 def perform_fit(u, v, vis, weights, geom, model):
     r"""
     Deproject the observed visibilities and fit them for the brightness profile
 
     Parameters
     ----------
     u, v : array, unit = :math:`\lambda`
@@ -393,36 +445,42 @@
         Diagnostics of the fit iteration
         (see radial_fitters.FrankFitter.fit)
     """
 
     need_iterations = model['input_output']['iteration_diag'] or \
         model['plotting']['diag_plot']
 
+    scale_height = get_scale_height(model)
+
     t1 = time.time()
     FF = radial_fitters.FrankFitter(Rmax=model['hyperparameters']['rout'],
                                     N=model['hyperparameters']['n'],
                                     geometry=geom,
                                     alpha=model['hyperparameters']['alpha'],
                                     p_0=model['hyperparameters']['p0'],
                                     weights_smooth=model['hyperparameters']['wsmooth'],
                                     tol=model['hyperparameters']['iter_tol'],
                                     method=model['hyperparameters']['method'],
+                                    I_scale=model['hyperparameters']['I_scale'],
                                     max_iter=model['hyperparameters']['max_iter'],
                                     store_iteration_diagnostics=need_iterations,
+                                    convergence_failure=model['hyperparameters']['converge_failure'],
+                                    scale_height=scale_height,
                                     assume_optically_thick=model['geometry']['rescale_flux']
                                     )
 
     sol = FF.fit(u, v, vis, weights)
 
     if model['hyperparameters']['nonnegative'] and \
        model['hyperparameters']['method'] == 'Normal':
         # Add the best fit nonnegative solution to the fit's `sol` object
-        logging.info('  `nonnegative` is `true` in your parameter file --> '\
-                    'Storing the best fit nonnegative profile as the attribute `nonneg` in the `sol` object')
-        setattr(sol, '_nonneg', sol.solve_non_negative())
+        logging.info('  `nonnegative` is `true` in your parameter file --> '
+                    'Storing the best fit nonnegative profile as the attribute '
+                    '`nonneg` in the `sol` object')
+        setattr(sol, 'nonneg', sol.solve_non_negative())
 
     logging.info('    Time taken to fit profile (with {:.0e} visibilities and'
                  ' {:d} collocation points) {:.1f} sec'.format(len(u),
                                                                model['hyperparameters']['n'],
                                                                time.time() - t1)
                  )
 
@@ -491,15 +549,15 @@
 
     if len(alphas) in [1,2] and len(ws) in [1,2]:
         multifit_fig, multifit_axes = make_figs.make_multifit_fig(u=u, v=v, vis=vis,
                                                                weights=weights, sols=sols,
                                                                bin_widths=model['plotting']['bin_widths'],
                                                                dist=model['plotting']['distance'],
                                                                force_style=model['plotting']['force_style'],
-                                                               save_prefix=model['input_output']['save_prefix'],
+                                                               save_prefix=model['input_output']['fig_save_prefix'],
                                                                )
     else:
         logging.info('The multifit figure requires alpha and wsmooth to be lists of length <= 2.'
                      'Your lists are length {} and {} --> The multifit figure will not be made.'.format(len(alphas), len(ws)))
         multifit_fig, multifit_axes = None, None
 
     return multifit_fig, multifit_axes
@@ -563,74 +621,65 @@
             model['plotting']['full_plot'],
             model['plotting']['diag_plot'],
             model['analysis']['compare_profile']
             ]):
 
         logging.info('  Plotting results')
 
-        priors = {'alpha': sol.info['alpha'],\
-                  'wsmooth': sol.info['wsmooth'],\
-                  'Rmax': sol.info['Rmax'],\
-                  'N': sol.info['N'],\
-                  'p0': sol.info['p0']
-                  }
-
         if model['plotting']['deprojec_plot']:
             deproj_fig, deproj_axes = make_figs.make_deprojection_fig(u=u, v=v,
                                                              vis=vis, weights=weights,
                                                              geom=geom,
                                                              bin_widths=model['plotting']['bin_widths'],
                                                              force_style=model['plotting']['force_style'],
-                                                             save_prefix=model['input_output']['save_prefix']
+                                                             save_prefix=model['input_output']['fig_save_prefix']
                                                              )
 
             figs.append(deproj_fig)
             axes.append(deproj_axes)
 
         if model['plotting']['quick_plot']:
             quick_fig, quick_axes = make_figs.make_quick_fig(u=u, v=v, vis=vis,
                                                              weights=weights, sol=sol,
                                                              bin_widths=model['plotting']['bin_widths'],
-                                                             priors=priors,
                                                              dist=model['plotting']['distance'],
                                                              logx=model['plotting']['plot_in_logx'],
                                                              force_style=model['plotting']['force_style'],
-                                                             save_prefix=model['input_output']['save_prefix'],
+                                                             save_prefix=model['input_output']['fig_save_prefix'],
                                                              stretch=model['plotting']['stretch'],
                                                              gamma=model['plotting']['gamma'],
                                                              asinh_a=model['plotting']['asinh_a']
                                                              )
 
             figs.append(quick_fig)
             axes.append(quick_axes)
 
         if model['plotting']['full_plot']:
             full_fig, full_axes = make_figs.make_full_fig(u=u, v=v, vis=vis,
                                                           weights=weights, sol=sol,
                                                           bin_widths=model['plotting']['bin_widths'],
-                                                          priors=priors,
                                                           dist=model['plotting']['distance'],
                                                           logx=model['plotting']['plot_in_logx'],
                                                           force_style=model['plotting']['force_style'],
-                                                          save_prefix=model['input_output']['save_prefix'],
+                                                          save_prefix=model['input_output']['fig_save_prefix'],
                                                           norm_residuals=model['plotting']['norm_residuals'],
                                                           stretch=model['plotting']['stretch'],
                                                           gamma=model['plotting']['gamma'],
                                                           asinh_a=model['plotting']['asinh_a']
                                                           )
 
             figs.append(full_fig)
             axes.append(full_axes)
 
         if model['plotting']['diag_plot']:
             diag_fig, diag_axes, _ = make_figs.make_diag_fig(r=sol.r, q=sol.q,
                                                              iteration_diagnostics=iteration_diagnostics,
                                                              iter_plot_range=model['plotting']['iter_plot_range'],
                                                              force_style=model['plotting']['force_style'],
-                                                             save_prefix=model['input_output']['save_prefix']
+                                                             save_prefix=model['input_output']['fig_save_prefix']
                                                              )
 
             figs.append(diag_fig)
             axes.append(diag_axes)
 
         if model['analysis']['compare_profile']:
             dat = np.genfromtxt(model['analysis']['compare_profile']).T
@@ -666,15 +715,15 @@
                                                                         bin_widths=model['plotting']['bin_widths'],
                                                                         stretch=model['plotting']['stretch'],
                                                                         gamma=model['plotting']['gamma'],
                                                                         asinh_a=model['plotting']['asinh_a'],
                                                                         MAP_convolved=MAP_convolved,
                                                                         dist=model['plotting']['distance'],
                                                                         force_style=model['plotting']['force_style'],
-                                                                        save_prefix=model['input_output']['save_prefix']
+                                                                        save_prefix=model['input_output']['fig_save_prefix']
                                                                         )
 
             figs.append(clean_fig)
             axes.append(clean_axes)
 
     return figs, axes, model
 
@@ -724,29 +773,29 @@
 
         u_s, v_s, vis_s, w_s = utilities.draw_bootstrap_sample(
             u, v, vis, weights)
 
         sol, iteration_diagnostics = perform_fit(u_s, v_s, vis_s, w_s, geom, model)
 
         if model['hyperparameters']['nonnegative']:
-            profiles_bootstrap.append(sol._nonneg)
+            profiles_bootstrap.append(sol.nonneg)
         else:
             profiles_bootstrap.append(sol.I)
 
     bootstrap_path = model['input_output']['save_prefix'] + '_bootstrap.npz'
 
     logging.info(' Bootstrap complete. Saving fitted brightness profiles and'
                  ' the common set of collocation points')
 
     np.savez(bootstrap_path, r=sol.r, profiles=np.array(profiles_bootstrap))
 
     boot_fig, boot_axes = make_figs.make_bootstrap_fig(r=sol.r,
                                                        profiles=profiles_bootstrap,
                                                        force_style=model['plotting']['force_style'],
-                                                       save_prefix=model['input_output']['save_prefix']
+                                                       save_prefix=model['input_output']['fig_save_prefix']
                                                        )
 
     return boot_fig, boot_axes
 
 
 def main(*args):
     """Run the full Frankenstein pipeline to fit a dataset
```

### Comparing `frank-1.2.1/frank/frank.mplstyle` & `frank-1.2.2/frank/frank.mplstyle`

 * *Files identical despite different names*

### Comparing `frank-1.2.1/frank/geometry.py` & `frank-1.2.2/frank/geometry.py`

 * *Files identical despite different names*

### Comparing `frank-1.2.1/frank/hankel.py` & `frank-1.2.2/frank/hankel.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,21 +15,17 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>
 #
 """This module contains functions for computing the
 discrete Hankel transform (DHT).
 """
-
 import numpy as np
 from scipy.special import j0, j1, jn_zeros, jv
 
-from frank.constants import rad_to_arcsec
-
-
 class DiscreteHankelTransform(object):
     r"""
     Utilities for computing the discrete Hankel transform.
 
     This class provides the necessary interface to compute
     a discrete version of the Hankel transform (DHT):
 
@@ -202,14 +198,74 @@
         if q is None:
             return 0.5 * self._j_nN * norm * self._Ykm
 
         H = (norm * self._scale_factor) * \
             self._jnu0(np.outer(k * q, self._j_nk))
 
         return H
+    
+    def interpolation_coefficients(self, q, space='Real'):
+        """
+        Coefficients of the interpolation matrix, defined by
+            f(q) = np.dot(Y, f)
+
+        Parameters
+        ----------
+        q : array or None
+            The points at which to evaluate the interpolation.
+        space : { 'Real', 'Fourier' }, optional
+            Space in which the interpolation is done. If not supplied, 
+            'Real' is assumed.
+
+        Returns
+        -------
+        Y : array, size = (len(q), N)
+            The interpolation matrix
+        """
+        if space == 'Real':
+            x = np.atleast_1d(2*np.pi * q * self._Qmax)
+        elif space == 'Fourier':
+            x = np.atleast_1d(2*np.pi * q * self._Rmax)
+        else:
+            raise ValueError("Space must be one of 'Real' or 'Fourier', not "
+                             f"{space}.")
+
+        coeff = np.outer(np.where(x < self._j_nN, self._jnu0(x), 0),
+                         2*self._j_nk / self._jnup(self._j_nk))
+        Y = coeff / (self._j_nk.reshape(1,-1)**2 - x.reshape(-1, 1)**2)
+        
+        return Y
+
+    def interpolate(self, f, q, space='Real'):
+        """
+        Interpolate f (evaluated at the collocation points) to the new points,
+        pts, using interpolation that is consistent with the Fourier-Bessel
+        Series / Discrete Hankel Transform.
+
+        Parameters
+        ----------
+        f : array, size = N
+            Function to interpolate, evaluated at the collocation points:
+                f[k] = f(r_k) or f[k] = f(q_k)
+        q : array or None
+            The points at which to evaluate the interpolation.
+        space : { 'Real', 'Fourier' }, optional
+            Space in which the interpolation is done. If not supplied, 
+            'Real' is assumed.
+
+
+        Returns
+        -------
+        f_interp : array, size = len(q)
+            The interpolated results
+        """
+        Y = self.interpolation_coefficients(q, space)
+
+        return np.dot(Y, f)
+    
 
     @property
     def r(self):
         """Radius points"""
         return self._Rnk
 
     @property
```

### Comparing `frank-1.2.1/frank/io.py` & `frank-1.2.2/frank/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 """
 
 import os
 import numpy as np
 import pickle
 import logging
 
+from frank.utilities import get_fit_stat_uncer
+
 def load_uvtable(data_file):
     r"""
     Read in a UVTable with data to be fit
 
     Parameters
     ----------
     data_file : string
@@ -127,15 +129,16 @@
     Returns
     ----------
     sol : _HankelRegressor object
         frank solution object
         (see frank.radial_fitters.FrankFitter)
     """
 
-    sol = np.load(sol_file, allow_pickle=True)
+    with open(sol_file, 'rb') as f: 
+        sol = pickle.load(f)
 
     return sol
 
 
 def save_fit(u, v, vis, weights, sol, prefix, save_solution=True,
              save_profile_fit=True, save_vis_fit=True, save_uvtables=True,
              save_iteration_diag=False, iteration_diag=None,
@@ -188,16 +191,17 @@
             pickle.dump(sol, f)
 
     if save_iteration_diag:
         with open(prefix + '_frank_iteration_diagnostics.obj', 'wb') as f:
             pickle.dump(iteration_diag, f)
 
     if save_profile_fit:
+        unc = get_fit_stat_uncer(sol)
         np.savetxt(prefix + '_frank_profile_fit.txt',
-                   np.array([sol.r, sol.I, np.diag(sol.covariance)**.5]).T,
+                   np.array([sol.r, sol.I, unc]).T,
                    header='r [arcsec]\tI [Jy/sr]\tI_uncer [Jy/sr]')
 
     if save_vis_fit:
         np.savetxt(prefix + '_frank_vis_fit.' + format,
                    np.array([sol.q, sol.predict_deprojected(sol.q).real]).T,
                    header='Baseline [lambda]\tProjected Re(V) [Jy]')
```

### Comparing `frank-1.2.1/frank/make_figs.py` & `frank-1.2.2/frank/make_figs.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 import warnings
 warnings.filterwarnings('ignore', '.*handles with labels found.*')
 
 
 # Global settings for plots
 cs = ['#a4a4a4', 'k', '#f781bf', '#dede00']
 cs2 = ['#3498DB', '#984ea3', '#4daf4a', '#ff7f00']
-hist_cs = ['#e41a1c', '#999999', '#377eb8', '#ff7f00', '#4daf4a', '#f781bf',
+hist_cs = ['#377eb8', '#ff7f00', '#e41a1c', '#999999', '#4daf4a', '#f781bf',
            '#984ea3', '#dede00']
 multifit_cs = ['#e41a1c', '#999999', '#377eb8', '#ff7f00', '#4daf4a', '#f781bf',
                '#984ea3', '#dede00']
 ms = ['x', '+', '.', '1']
 
 
 class _DoNothingContextManager(object):
@@ -170,15 +170,15 @@
         plt.savefig(save_prefix + '_frank_deprojection.png', dpi=300,
                     bbox_inches='tight')
         plt.close()
 
     return fig, axes
 
 
-def make_quick_fig(u, v, vis, weights, sol, bin_widths, priors, dist=None,
+def make_quick_fig(u, v, vis, weights, sol, bin_widths, dist=None,
                    logx=False, force_style=True, save_prefix=None,
                    stretch='power', gamma=1.0, asinh_a=0.02, figsize=(8,6)):
     r"""
     Produce a simple figure showing just a Frankenstein fit, not any diagnostics
 
     Parameters
     ----------
@@ -190,17 +190,14 @@
         Weights assigned to observed visibilities, of the form
         :math:`1 / \sigma^2`
     sol : _HankelRegressor object
         Reconstructed profile using Maximum a posteriori power spectrum
         (see frank.radial_fitters.FrankFitter)
     bin_widths : list, unit = \lambda
         Bin widths in which to bin the observed visibilities
-    priors : dict
-        Dictionary with fit hyperparameters: 'alpha', 'wsmooth', 'Rmax', 'N', 'p0'.
-        Used for figure title
     dist : float, optional, unit = AU, default = None
         Distance to source, used to show second x-axis in [AU]
     logx : bool, default = False
         Whether to plot the visibility distributions in log(baseline)
     gamma : float, default = 1.0
         Index of power law normalization to apply to swept profile image's
         colormap (see matplotlib.colors.PowerNorm).
@@ -223,23 +220,23 @@
         The produced figure, including the GridSpec
     axes : Matplotlib `~.axes.Axes` class
         The axes of the produced figure
     """
 
     logging.info('    Making quick figure')
 
-    alpha, wsmooth, Rmax, N, p0 = priors['alpha'], priors['wsmooth'],\
-                                  priors['Rmax'], priors['N'], priors['p0']
+    Rmax, N, alpha, wsmooth, p0 = sol._info["Rmax"], sol._info["N"], \
+        sol._info["alpha"], sol._info["wsmooth"], sol._info["p0"]
 
     with frank_plotting_style_context_manager(force_style):
         gs = GridSpec(3, 2, hspace=0, bottom=.12)
         gs2 = GridSpec(3, 2, hspace=.2)
         fig = plt.figure(figsize=figsize)
-        fig.suptitle(r'Fit hyperparameters: $\alpha$={:.2f}, $w_{{smooth}}$={:.1e}, R$_{{max}}$={}, '\
-                     'N={}, p$_0$={:.0e}'.format(alpha, wsmooth, Rmax, N, p0))
+        fig.suptitle(r'Fit hyperparameters: $\alpha$={:.2f}, $w_{{smooth}}$={:.1e}, R$_{{max}}$={:.2f}, '
+                     'N={:0d}, p$_0$={:.0e}'.format(alpha, wsmooth, Rmax, N, p0))
 
         ax0 = fig.add_subplot(gs[0])
         ax1 = fig.add_subplot(gs[2])
 
         ax2 = fig.add_subplot(gs[1])
         ax3 = fig.add_subplot(gs[3])
 
@@ -262,44 +259,53 @@
         if dist:
             ax0_5 = plot_brightness_profile(sol.r, sol.I / 1e10, ax0, dist=dist, c='r')
             xlims = ax0.get_xlim()
             ax0_5.set_xlim(np.multiply(xlims, dist))
 
         plot_brightness_profile(sol.r, sol.I / 1e10, ax1, c='r', label='frank')
 
+        if hasattr(sol, 'nonneg'): 
+            plot_brightness_profile(sol.r, sol.nonneg / 1e10, ax0, ls='--', c='#009933', label='non-neg.')
+            plot_brightness_profile(sol.r, sol.nonneg / 1e10, ax1, ls='--', c='#009933', label='non-neg.')
+
+
         u_deproj, v_deproj, vis_deproj = sol.geometry.apply_correction(u, v, vis)
         baselines = (u_deproj**2 + v_deproj**2)**.5
         grid = np.logspace(np.log10(min(baselines.min(), sol.q[0])),
                            np.log10(max(baselines.max(), sol.q[-1])),
                            10**4)
 
         for i in range(len(bin_widths)):
             binned_vis = UVDataBinner(
                 baselines, vis_deproj, weights, bin_widths[i])
-            vis_re_kl = binned_vis.V.real * 1e3
-            vis_err_re_kl = binned_vis.error.real * 1e3
+            vis_re = binned_vis.V.real * 1e3
+            vis_err_re = binned_vis.error.real * 1e3
             vis_fit = sol.predict_deprojected(binned_vis.uv).real * 1e3
 
             for ax in [ax2, ax3]:
-                plot_vis_quantity(binned_vis.uv / 1e6, vis_re_kl, ax,
-                     vis_err_re_kl, c=cs[i],
+                plot_vis_quantity(binned_vis.uv / 1e6, vis_re, ax,
+                     vis_err_re, c=cs[i],
                      marker=ms[i], ls='None',
                      label=r'Obs., {:.0f} k$\lambda$ bins'.format(bin_widths[i]/1e3))
 
-        vis_fit_kl = sol.predict_deprojected(grid).real * 1e3
-        plot_vis_quantity(grid / 1e6, vis_fit_kl, ax2, c='r', label='frank', zorder=10)
+        vis_fit = sol.predict_deprojected(grid).real * 1e3
+        plot_vis_quantity(grid / 1e6, vis_fit, ax2, c='r', label='frank', zorder=10)
+
+        plot_vis_quantity(grid / 1e6, vis_fit, ax3, c='r', label='frank', zorder=10)
+
+        if hasattr(sol, 'nonneg'):
+            vis_fit_nonneg = sol.predict_deprojected(grid, I=sol.nonneg).real * 1e3
+            plot_vis_quantity(grid / 1e6, vis_fit_nonneg, ax2, ls='--', c='#009933', label='non-neg.', zorder=10)
+            plot_vis_quantity(grid / 1e6, vis_fit_nonneg, ax3, ls='--', c='#009933', label='non-neg.', zorder=10)
 
         # Make a guess of good y-bounds for zooming in on the visibility fit
-        # in linear-y
-        zoom_ylim_guess = abs(vis_fit_kl[int(.5 * len(vis_fit_kl)):]).max()
-        zoom_bounds = [-1.1 * zoom_ylim_guess, 1.1 * zoom_ylim_guess]
+        zoom_ylim_guess = vis_fit.mean()
+        zoom_bounds = [-1.5 * zoom_ylim_guess, 1.5 * zoom_ylim_guess]
         ax3.set_ylim(zoom_bounds)
 
-        plot_vis_quantity(grid / 1e6, vis_fit_kl, ax3, c='r', label='frank', zorder=10)
-
         vmax = sol.I.max()
         if stretch == 'asinh':
             vmin = max(0, min(sol.I))
             from astropy.visualization.mpl_normalize import simple_norm
             norm = simple_norm(sol.I, stretch='asinh', asinh_a=asinh_a, 
                                min_cut=vmin, max_cut=vmax)
         elif stretch == 'power':
@@ -314,15 +320,15 @@
         plot_2dsweep(sol.r, sol.I, ax=ax5, cmap='inferno', norm=norm,
                     project=True, geom=sol.geometry)
 
         ax1.set_xlabel('r ["]')
         ax0.set_ylabel(r'Brightness [$10^{10}$ Jy sr$^{-1}$]')
         ax1.set_ylabel(r'Brightness [$10^{10}$ Jy sr$^{-1}$]')
         ax1.set_yscale('log')
-        ax1.set_ylim(bottom=1e-3)
+        ax1.set_ylim(sol.I[sol.I > 0].min() * 0.9 / 1e10, sol.I.max() * 1.1 / 1e10)
 
         ax3.set_xlabel(r'Baseline [M$\lambda$]')
         ax2.set_ylabel('Re(V) [mJy]')
         ax3.set_ylabel('Re(V) [mJy]')
 
         if logx:
             ax2.set_xscale('log')
@@ -346,15 +352,15 @@
             plt.savefig(save_prefix + '_frank_fit_quick.png', dpi=300,
                         bbox_inches='tight')
             plt.close()
 
     return fig, axes
 
 
-def make_full_fig(u, v, vis, weights, sol, bin_widths, priors,
+def make_full_fig(u, v, vis, weights, sol, bin_widths,
                   dist=None, logx=False, force_style=True,
                   save_prefix=None, norm_residuals=False, stretch='power',
                   gamma=1.0, asinh_a=0.02, figsize=(8, 6)):
     r"""
     Produce a figure showing a Frankenstein fit and some useful diagnostics
 
     Parameters
@@ -367,17 +373,14 @@
         Weights assigned to observed visibilities, of the form
         :math:`1 / \sigma^2`
     sol : _HankelRegressor object
         Reconstructed profile using maximum a posteriori power spectrum
         (see frank.radial_fitters.FrankFitter)
     bin_widths : list, unit = \lambda
         Bin widths in which to bin the observed visibilities
-    priors : dict
-        Dictionary with fit hyperparameters: 'alpha', 'wsmooth', 'Rmax', 'N', 'p0'.
-        Used for figure title
     dist : float, optional, unit = AU, default = None
         Distance to source, used to show second x-axis in [AU]
     logx : bool, default = False
         Whether to plot the visibility distributions in log(baseline)
     force_style: bool, default = True
         Whether to use preconfigured matplotlib rcParams in generated figure
     save_prefix : string, default = None
@@ -403,24 +406,24 @@
         The produced figure, including the GridSpec
     axes : Matplotlib `~.axes.Axes` class
         The axes of the produced figure
     """
 
     logging.info('    Making full figure')
 
-    alpha, wsmooth, Rmax, N, p0 = priors['alpha'], priors['wsmooth'],\
-                                  priors['Rmax'], priors['N'], priors['p0']
+    Rmax, N, alpha, wsmooth, p0 = sol._info["Rmax"], sol._info["N"], \
+        sol._info["alpha"], sol._info["wsmooth"], sol._info["p0"]
 
     with frank_plotting_style_context_manager(force_style):
         gs = GridSpec(3, 3, hspace=0, wspace=0.25, left=0.06, right=0.98)
         gs1 = GridSpec(4, 3, hspace=0, wspace=0.25, left=0.06, right=0.98)
         gs2 = GridSpec(3, 3, hspace=.35, wspace=0.25, left=0.06, right=0.98)
         fig = plt.figure(figsize=figsize)
-        fig.suptitle(r'Fit hyperparameters: $\alpha$={:.2f}, $w_{{smooth}}$={:.1e}, R$_{{max}}$={}, '\
-                     'N={}, p$_0$={:.0e}'.format(alpha, wsmooth, Rmax, N, p0))
+        fig.suptitle(r'Fit hyperparameters: $\alpha$={:.2f}, $w_{{smooth}}$={:.1e}, R$_{{max}}$={:.2f}, '
+                     'N={:0d}, p$_0$={:.0e}'.format(alpha, wsmooth, Rmax, N, p0))
 
         ax0 = fig.add_subplot(gs[0])
         ax1 = fig.add_subplot(gs[3])
         ax2 = fig.add_subplot(gs2[6])
 
         ax3 = fig.add_subplot(gs[1])
         ax4 = fig.add_subplot(gs[4])
@@ -451,81 +454,101 @@
         if dist:
             ax0_5 = plot_brightness_profile(sol.r, sol.I / 1e10, ax0, dist=dist, c='r')
             xlims = ax0.get_xlim()
             ax0_5.set_xlim(np.multiply(xlims, dist))
 
         plot_brightness_profile(sol.r, sol.I / 1e10, ax1, c='r', label='frank')
 
+        if hasattr(sol, 'nonneg'): 
+            plot_brightness_profile(sol.r, sol.nonneg / 1e10, ax0, ls='--', c='#009933', label='non-neg.')
+            plot_brightness_profile(sol.r, sol.nonneg / 1e10, ax1, ls='--', c='#009933', label='non-neg.')
+
         # Apply deprojection to the provided (u, v) coordinates
         # and visibility amplitudes
         u_deproj, v_deproj, vis_deproj = sol.geometry.apply_correction(u, v, vis)
         baselines = (u_deproj**2 + v_deproj**2)**.5
         # Set a grid of baselines on which to plot the visibility domain frank fit
         grid = np.logspace(np.log10(min(baselines.min(), sol.q[0])),
                            np.log10(max(baselines.max(), sol.q[-1])), 10**4
                            )
-        # Map the frank visibility fit to `grid`, considering only the real component
-        # that frank fits
-        vis_fit_kl = sol.predict_deprojected(grid).real * 1e3
-
-        # Make a guess of good y-bounds for zooming in on the visibility fit
-        # in linear-y
-        zoom_ylim_guess = abs(vis_fit_kl[int(.5 * len(vis_fit_kl)):]).max()
-        zoom_bounds = [-1.1 * zoom_ylim_guess, 1.1 * zoom_ylim_guess]
-        ax4.set_ylim(zoom_bounds)
 
         # Bin the observed (real and imaginary components of the) visibilities
         # for plotting
         for i in range(len(bin_widths)):
             binned_vis = UVDataBinner(baselines, vis_deproj, weights, bin_widths[i])
-            vis_re_kl = binned_vis.V.real * 1e3
-            vis_im_kl = binned_vis.V.imag * 1e3
-            vis_err_re_kl = binned_vis.error.real * 1e3
-            vis_err_im_kl = binned_vis.error.imag * 1e3
+            vis_re = binned_vis.V.real * 1e3
+            vis_im = binned_vis.V.imag * 1e3
+            vis_err_re = binned_vis.error.real * 1e3
+            vis_err_im = binned_vis.error.imag * 1e3
             vis_fit = sol.predict_deprojected(binned_vis.uv).real * 1e3
+            if hasattr(sol, 'nonneg'):
+                vis_fit_nn = sol.predict_deprojected(binned_vis.uv, I=sol.nonneg).real * 1e3
 
             # Determine the visiblity domain frank fit residuals (and RMS error)
             # for Real(V)
-            resid = vis_re_kl - vis_fit
+            resid = vis_re - vis_fit
             if norm_residuals:
-                resid /= vis_re_kl
+                resid /= vis_re
             rmse = (np.mean(resid**2))**.5
+            if hasattr(sol, 'nonneg'):
+                resid_nn = vis_re - vis_fit_nn
+                if norm_residuals:
+                    resid_nn /= vis_re
+                rmse_nn = (np.mean(resid_nn**2))**.5
 
             # Plot the observed, binned visibilities (with errorbars) and the residuals
-            plot_vis_quantity(binned_vis.uv / 1e6, vis_re_kl, ax3, c=cs[i],
+            plot_vis_quantity(binned_vis.uv / 1e6, vis_re, ax3, c=cs[i],
                      marker=ms[i], ls='None',
                      label=r'Obs., {:.0f} k$\lambda$ bins'.format(bin_widths[i]/1e3))
 
-            plot_vis_quantity(binned_vis.uv / 1e6, vis_re_kl, ax4, c=cs[i],
+            plot_vis_quantity(binned_vis.uv / 1e6, vis_re, ax4, c=cs[i],
                      marker=ms[i], ls='None',
                      label=r'Obs., {:.0f} k$\lambda$ bins'.format(bin_widths[i]/1e3))
 
-            plot_vis_quantity(binned_vis.uv / 1e6, vis_im_kl, ax6, c=cs[i],
+            plot_vis_quantity(binned_vis.uv / 1e6, vis_im, ax6, c=cs[i],
                      marker=ms[i], ls='None',
                      label=r'Obs., {:.0f} k$\lambda$ bins'.format(bin_widths[i]/1e3))
 
-            plot_vis_quantity(binned_vis.uv / 1e6, resid, ax5, c=cs[i], marker=ms[i], ls='None',
+            plot_vis_quantity(binned_vis.uv / 1e6, resid, ax5, c='r', marker=ms[i], ls='None',
                            label=r'{:.0f} k$\lambda$ bins, RMSE {:.3f} mJy'.format(bin_widths[i]/1e3, rmse))
 
+            if hasattr(sol, 'nonneg'):
+                plot_vis_quantity(binned_vis.uv / 1e6, resid_nn, ax5, c='#009933', marker=ms[i], ls='None',
+                           label=r'{:.0f} k$\lambda$ bins, RMSE {:.3f} mJy'.format(bin_widths[i]/1e3, rmse_nn))                
+
             # Plot a histogram of the observed visibilties to examine how the
             # visibility count varies with baseline
             plot_vis_hist(binned_vis, ax8, rescale=1e6, color=hist_cs[i],
                           label=r'Obs., {:.0f} k$\lambda$ bins'.format(bin_widths[i]/1e3))
             # Plot the binned data signal-to-noise as a function of baseline
             plot_vis_quantity(binned_vis.uv / 1e6,
                           binned_vis.V.real**2 / binned_vis.error.real**2,
                           ax9, color=hist_cs[i], marker=ms[i], ls='None',
                           label=r'{:.0f} k$\lambda$ bins'.format(bin_widths[i]/1e3))
 
-        # Plot the visibility domain frank fit in log-y
-        plot_vis_quantity(grid / 1e6, vis_fit_kl, ax3, c='r', label='frank')
-        plot_vis_quantity(grid / 1e6, vis_fit_kl, ax4, c='r', label='frank')
+        # Map the frank visibility fit to `grid`, considering only the real component
+        # that frank fits
+        vis_fit = sol.predict_deprojected(grid).real * 1e3
+
+        # Plot the visibility domain frank fit
+        plot_vis_quantity(grid / 1e6, vis_fit, ax3, c='r', label='frank')
+        plot_vis_quantity(grid / 1e6, vis_fit, ax4, c='r', label='frank')
+
+        if hasattr(sol, 'nonneg'):
+            vis_fit_nonneg = sol.predict_deprojected(grid, I=sol.nonneg).real * 1e3
+            plot_vis_quantity(grid / 1e6, vis_fit_nonneg, ax3, ls='--', c='#009933', label='non-neg.')
+            plot_vis_quantity(grid / 1e6, vis_fit_nonneg, ax4, ls='--', c='#009933', label='non-neg.')
+
+        # Make a guess of good y-bounds for zooming in on the visibility fit
+        zoom_ylim_guess = vis_fit.mean()
+        zoom_bounds = [-1.5 * zoom_ylim_guess, 1.5 * zoom_ylim_guess]
+        ax4.set_ylim(zoom_bounds)
 
         # Plot the frank inferred power spectrum
-        plot_vis_quantity(sol.q / 1e6, sol.power_spectrum, ax7)
+        plot_vis_quantity(sol.q / 1e6, sol.power_spectrum, ax7, c='k')
 
         # Plot a sweep over 2\pi of the frank 1D fit
         # (analogous to a model image of the source)
         vmax = sol.I.max()
         if stretch == 'asinh':
             vmin = max(0, min(sol.I))
             from astropy.visualization.mpl_normalize import simple_norm
@@ -541,15 +564,15 @@
         plot_2dsweep(sol.r, sol.I, ax=ax2, cmap='inferno', norm=norm,
                     project=True, geom=sol.geometry)
 
         ax1.set_xlabel('r ["]')
         ax0.set_ylabel(r'Brightness [$10^{10}$ Jy sr$^{-1}$]')
         ax1.set_ylabel(r'Brightness [$10^{10}$ Jy sr$^{-1}$]')
         ax1.set_yscale('log')
-        ax1.set_ylim(bottom=1e-3)
+        ax1.set_ylim(sol.I[sol.I > 0].min() * 0.9 / 1e10, sol.I.max() * 1.1 / 1e10)
         ax2.set_xlabel('RA offset ["]')
         ax2.set_ylabel('Dec offset ["]')
 
         axs = [ax3, ax4, ax5, ax6, ax7, ax8, ax9]
         if logx:
             for aa in axs:
                 aa.set_xscale('log')
@@ -835,48 +858,48 @@
         baselines = (u_deproj**2 + v_deproj**2)**.5
         grid = np.logspace(np.log10(min(baselines.min(), sol.q[0])),
                            np.log10(max(baselines.max(), sol.q[-1])), 10**4
                            )
 
         for i in range(len(bin_widths)):
             binned_vis = UVDataBinner(baselines, vis_deproj, weights, bin_widths[i])
-            vis_re_kl = binned_vis.V.real * 1e3
-            vis_err_re_kl = binned_vis.error.real * 1e3
+            vis_re = binned_vis.V.real * 1e3
+            vis_err_re = binned_vis.error.real * 1e3
 
             if logy:
                 lab=r'Obs.>0, {:.0f} k$\lambda$ bins'.format(bin_widths[i]/1e3)
             else:
                 lab=r'Obs., {:.0f} k$\lambda$ bins'.format(bin_widths[i]/1e3)
-            plot_vis_quantity(binned_vis.uv / 1e6, vis_re_kl, ax1, c=cs[i],
+            plot_vis_quantity(binned_vis.uv / 1e6, vis_re, ax1, c=cs[i],
                      marker=ms[i], ls='None',
                      label=lab)
             if logy:
-                plot_vis_quantity(binned_vis.uv / 1e6, -vis_re_kl, ax1, c=cs2[i],
+                plot_vis_quantity(binned_vis.uv / 1e6, -vis_re, ax1, c=cs2[i],
                      marker=ms[i], ls='None',
                      label=r'Obs.<0, {:.0f} k$\lambda$ bins'.format(bin_widths[i]/1e3))
 
-        vis_fit_kl = sol.predict_deprojected(grid).real * 1e3
+        vis_fit = sol.predict_deprojected(grid).real * 1e3
 
         # Take the discrete Hankel transform of the CLEAN profile, using the same
         # collocation points for the DHT as those in the frank fit
         Inu_interp = np.interp(
             sol.r, clean_profile['r'], clean_profile['I'].real) * 1e3
-        clean_DHT_kl = sol.predict_deprojected(grid, I=Inu_interp)
+        clean_DHT = sol.predict_deprojected(grid, I=Inu_interp)
 
         if logy:
             lab = 'frank, >0'
             lab2 = 'DHT of CLEAN, >0'
         else:
             lab = 'frank'
             lab2 = 'DHT of CLEAN'
-        plot_vis_quantity(grid / 1e6, vis_fit_kl, ax1, c='r', label=lab)
-        plot_vis_quantity(grid / 1e6, clean_DHT_kl, ax1, c='b', label=lab2)
+        plot_vis_quantity(grid / 1e6, vis_fit, ax1, c='r', label=lab)
+        plot_vis_quantity(grid / 1e6, clean_DHT, ax1, c='b', label=lab2)
         if logy:
-            plot_vis_quantity(grid / 1e6, -vis_fit_kl, ax1, c='r', ls='--', label='frank, <0')
-            plot_vis_quantity(grid / 1e6, -clean_DHT_kl, ax1, c='b', ls='--', label='DHT of CLEAN, <0')
+            plot_vis_quantity(grid / 1e6, -vis_fit, ax1, c='r', ls='--', label='frank, <0')
+            plot_vis_quantity(grid / 1e6, -clean_DHT, ax1, c='b', ls='--', label='DHT of CLEAN, <0')
 
         if logx:
             ax1.set_xscale('log')
         ax1.set_xlim(right=1.2 * max(baselines) / 1e6)
 
         if logy:
             ax1.set_yscale('log')
@@ -1022,43 +1045,43 @@
         grid = np.logspace(np.log10(min(baselines.min(), sols[0].q[0])),
                            np.log10(max(baselines.max(), sols[0].q[-1])),
                            10**4)
 
         for i in range(len(bin_widths)):
             binned_vis = UVDataBinner(
                 baselines, vis_deproj, weights, bin_widths[i])
-            vis_re_kl = binned_vis.V.real * 1e3
-            vis_err_re_kl = binned_vis.error.real * 1e3
+            vis_re = binned_vis.V.real * 1e3
+            vis_err_re = binned_vis.error.real * 1e3
 
-            plot_vis_quantity(binned_vis.uv, vis_re_kl, ax2, c=cs[i],
+            plot_vis_quantity(binned_vis.uv, vis_re, ax2, c=cs[i],
                      marker=ms[i], ls='None', label=r'Obs., {:.0f} k$\lambda$ bins'.format(bin_widths[i]/1e3))
 
-            plot_vis_quantity(binned_vis.uv, vis_re_kl, ax3, c=cs[i],
+            plot_vis_quantity(binned_vis.uv, vis_re, ax3, c=cs[i],
                      marker=ms[i], ls='None',
                      label=r'Obs.>0, {:.0f} k$\lambda$ bins'.format(bin_widths[i]/1e3))
-            plot_vis_quantity(binned_vis.uv, -vis_re_kl, ax3, c=cs2[i],
+            plot_vis_quantity(binned_vis.uv, -vis_re, ax3, c=cs2[i],
                      marker=ms[i], ls='None',
                      label=r'Obs.<0, {:.0f} k$\lambda$ bins'.format(bin_widths[i]/1e3))
 
         # Overplot the multiple fits
         for ii in range(len(sols)):
             plot_brightness_profile(sols[ii].r, sols[ii].I / 1e10, ax0, c=multifit_cs[ii])#,
                 # label='alpha = {}, wsmooth = {}'.format(sols[ii].info['alpha'], sols[ii].info['wsmooth'])
             if dist and ii == len(sols) - 1:
                 ax0_5 = plot_brightness_profile(sols[ii].r, sols[ii].I / 1e10, ax0, dist=dist, c=multifit_cs[ii])
                 xlims = ax0.get_xlim()
                 ax0_5.set_xlim(np.multiply(xlims, dist))
 
             plot_brightness_profile(sols[ii].r, sols[ii].I / 1e10, ax1, c=multifit_cs[ii])
 
-            vis_fit_kl = sols[ii].predict_deprojected(grid).real * 1e3
-            plot_vis_quantity(grid, vis_fit_kl, ax2, c=multifit_cs[ii])
+            vis_fit = sols[ii].predict_deprojected(grid).real * 1e3
+            plot_vis_quantity(grid, vis_fit, ax2, c=multifit_cs[ii])
 
-            plot_vis_quantity(grid, vis_fit_kl, ax3, c=multifit_cs[ii])
-            plot_vis_quantity(grid, -vis_fit_kl, ax3, c=multifit_cs[ii], ls='--')
+            plot_vis_quantity(grid, vis_fit, ax3, c=multifit_cs[ii])
+            plot_vis_quantity(grid, -vis_fit, ax3, c=multifit_cs[ii], ls='--')
 
             plot_vis_quantity(sols[ii].q, sols[ii].power_spectrum, ax4, c=multifit_cs[ii])
 
         ax1.set_xlabel('r ["]')
         ax0.set_ylabel(r'Brightness [$10^{10}$ Jy sr$^{-1}$]')
         ax1.set_ylabel(r'Brightness [$10^{10}$ Jy sr$^{-1}$]')
         ax1.set_yscale('log')
```

### Comparing `frank-1.2.1/frank/minimizer.py` & `frank-1.2.2/frank/minimizer.py`

 * *Files identical despite different names*

### Comparing `frank-1.2.1/frank/parameter_descriptions.json` & `frank-1.2.2/frank/parameter_descriptions.json`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 {
   "input_output" : {
-    "uvtable_filename" : "UVTable with data to be fit (columns: u [\\lambda], v [\\lambda], Re(V) [Jy], Im(V) [Jy], weights [Jy^-2])",
+    "uvtable_filename" : "UVTable with data to be fit. An ASCII file should have columns of: u [\\lambda], v [\\lambda], Re(V) [Jy], Im(V) [Jy], weights [Jy^-2]. An npz file should have columns of: u [\\lambda], v [\\lambda], V [Jy; complex: real + imag * 1j], weights [Jy^-2])",
     "save_dir"         : "Directory in which output datafiles and figures are saved",
     "save_solution"    : "Whether to save `sol` object (see frank.radial_fitters.FrankFitter)",
     "save_profile_fit" : "Whether to save fitted brightness profile",
     "save_vis_fit"     : "Whether to save fitted visibility distribution",
     "save_uvtables"    : "Whether to save fitted and residual UV tables (these are reprojected)",
+    "save_figures"     : "Whether to save generated figures selected in 'plotting'",
     "iteration_diag"   : "Whether to return and save diagnostics of the fit iteration (needed for diag_plot)",
     "format"           : "Output file format. Default is the same as for 'uvtable_filename', else choose from 'npz' or 'txt'"
   },
 
   "modify_data" : {
     "baseline_range"   : "(Deprojected) baseline range outside of which visibilities are truncated, unit=[\\lambda]",
     "correct_weights"  : "Whether to estimate the data's weights (as they may be unknown for mock data)",
@@ -22,27 +23,30 @@
     "fit_phase_offset" : "Whether to fit for the phase center",
     "fit_inc_pa"       : "Whether to fit for the inclination and position angle",
     "initial_guess"    : "Whether to use the below values of `inc`, `pa`, `dra`, and `ddec` as an initial guess for the geometry (if `fit_phase_offset` is True or `fit_inc_pa` is True, the respective values below will be used. Guess is only used if `type` is 'gaussian' or 'nonparametric')",
     "inc"              : "Inclination, unit=[deg]",
     "pa"               : "Position angle, defined east of north, unit=[deg]",
     "dra"              : "Delta (offset from 0) right ascension, defined positive for offsets toward east, unit=[arcsec]",
     "ddec"             : "Delta declination, unit=[arcsec]",
-    "rescale_flux"     : "Whether to rescale the total flux to account for the source's inclination (see frank.geometry.rescale_total_flux)"
+    "rescale_flux"     : "Whether to rescale the total flux to account for the source's inclination (see frank.geometry.rescale_total_flux)",
+    "scale_height"     : "Parameter values for calcuating the vertical thickness of the disk in terms of its (assumed Gaussian) scale-height: 'h0', 'a', 'r0', 'b' in H(r) = h0 * r**a * np.exp(-(r/r0)**b). 'r0' should be in [arcsec]. Example (replace single- with double-quotes): {'h0': -1.0, 'a': 1.0, 'r0': 1.0, 'b': 1.0}",
   },
 
   "hyperparameters" : {
     "n"                : "Number of collocation points used in the fit (suggested range 100 - 300)",
     "rout"             : "Maximum disc radius in the fit (best to overestimate size of source), unit=[arcsec]",
     "alpha"            : "Order parameter for the power spectrum's inverse Gamma prior (suggested range 1.00 - 1.50). If a list, multiple fits will be performed and overplotted.",
     "p0"               : "Scale parameter for the power spectrum's inverse Gamma prior (suggested >0, <<1). If 'null', the code will internally choose a sensible value.",
     "wsmooth"          : "Strength of smoothing applied to the power spectrum (suggested range 10^-4 - 10^-1). If a list, multiple fits will be performed and overplotted.",
     "iter_tol"         : "Tolerance for fit iteration stopping criterion (suggested <<1)",
     "max_iter"         : "Maximum number of fit iterations",
-    "nonnegative"      : "Whether frank provides the mean (if false) or best fit nonnegative solution",
-    "method"           : "The fit method: 'Normal' to fit in linear brighness, 'LogNormal' to fit in logarithmic brightness"
+    "converge_failure" : "How to treat the case when the fit does not reach convergence by 'max_iter': one of ['raise', 'warn', 'ignore'] to respectively raise an error, raise a warning, or ignore.",    
+    "nonnegative"      : "Whether the best-fit nonnegative brightness profile is included in the frank fit solution object",
+    "method"           : "The fit method: 'Normal' to fit in linear brighness, 'LogNormal' to fit in logarithmic brightness",
+    "I_scale"          :  "Brightness scale, unit=[Jy/sr]. Only used if 'method' is 'LogNormal' -- the 'LogNormal' model produces I('rout') = 'I_scale'"
   },
 
   "plotting" : {
     "quick_plot"       : "Whether to make a figure showing the simplest plots of the fit",
     "full_plot"        : "Whether to make a figure more fully showing the fit and its diagnostics",
     "diag_plot"        : "Whether to make a diagnostic figure showing fit convergence metrics",
     "deprojec_plot"    : "Whether to make a figure showing the effect of deprojection on the (u, v) points and visibilities",
@@ -56,11 +60,11 @@
     "plot_in_logx"     : "Whether to plot visibility distributions in log(baseline) in 'quick_plot' and 'full_plot'",
     "norm_residuals"   : "Whether to normalize plotted visibility residuals in 'full_plot'"
   },
 
   "analysis" : {
     "compare_profile"  : "Path of file with comparison profile to be overplotted with frank fit (.txt or .dat). Columns: r [arcsec], I [Jy / sr], optional 3rd column with a single error [Jy / sr] or optional 3rd and 4th columns with lower and upper errors",
     "clean_beam"       : "Dictionary of B_major [arcsec], B_minor [arcsec], position angle [deg] of beam to convolve frank profile",
-    "bootstrap_ntrials": "Number of trials (dataset realizations) to perform in a bootstrap analysis",
+    "bootstrap_ntrials": "Number of trials (dataset realizations) to perform in a bootstrap analysis"
 
   }
 }
```

### Comparing `frank-1.2.1/frank/plot.py` & `frank-1.2.2/frank/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,16 +107,15 @@
 
     else:
         if low_uncer is not None:
             if high_uncer is None:
                 high_uncer = low_uncer * 1.
             ax.fill_between(fit_r, fit_i - low_uncer, fit_i + high_uncer, **kwargs)
 
-        else:
-            ax.plot(fit_r, fit_i, **kwargs)
+        ax.plot(fit_r, fit_i, **kwargs)
 
         ax.axhline(0, c='c', ls='--', zorder=10)
 
         if 'label' in kwargs:
             ax.legend(loc='best')
```

### Comparing `frank-1.2.1/frank/radial_fitters.py` & `frank-1.2.2/frank/radial_fitters.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   of deprojected visibities.
 """
 import abc
 from collections import defaultdict
 import logging
 import numpy as np
 
-from frank.constants import deg_to_rad, rad_to_arcsec
+from frank.constants import rad_to_arcsec
 from frank.filter import CriticalFilter
 from frank.hankel import DiscreteHankelTransform
 from frank.statistical_models import (
     GaussianModel, LogNormalMAPModel, VisibilityMapping
 )
 
 class FrankRadialFit(metaclass=abc.ABCMeta):
@@ -168,24 +168,17 @@
         The resulting brightness will be consistent with higher-resolution fits
         as long as the original fit has sufficient resolution. By sufficient
         resolution we simply mean that the missing terms in the Fourier-Bessel
         series are negligible, which will typically be the case if the
         brightness was obtained from a frank fit with 100 points or more.
         """
         Rpts = np.array(Rpts)
-        if I is None:
-            I = self.I
-        
-        V = self._vis_map.transform(I, direction='forward')
-        I = self._vis_map.transform(V, Rpts, direction='backward')
         
-        if np.any(Rpts > self.Rmax):
-            I[Rpts > self.Rmax] = 0
-
-        return I 
+        return self._vis_map.interpolate(I, Rpts, space='Real')
+  
 
     @abc.abstractproperty
     def MAP(self):
         pass
 
     @property
     def I(self):
@@ -674,30 +667,36 @@
     assume_optically_thick : bool, default = True
         Whether to correct the visibility amplitudes by a factor of
         1 / cos(inclination); see frank.geometry.rescale_total_flux
     scale_height : function R --> H, optional
         Specifies the vertical thickness of disc as a function of radius. Both
         R and H should be in arcsec. Assumes a Gaussian vertical structure. 
         Only works with assume_optically_thick=False
-    verbose:
+    verbose: bool
         Whether to print notification messages
+    convergence_failure: string, default = 'raise'
+        Decide what to do when the frank model does not converge within max_iter.
+        Should be one of:
+        'raise'  : raise an error
+        'warn'   : print a warning message and continue
+        'ignore' : Ignore the error.
 
     References
     ----------
         Baddour & Chouinard (2015)
             DOI: https://doi.org/10.1364/JOSAA.32.000611
         Oppermann et al. (2013)
             DOI:  https://doi.org/10.1103/PhysRevE.87.032136
     """
 
     def __init__(self, Rmax, N, geometry, nu=0, block_data=True,
                  block_size=10 ** 5, alpha=1.05, p_0=None, weights_smooth=1e-4,
                  tol=1e-3, method='Normal', I_scale=1e5, max_iter=2000, check_qbounds=True,
                  store_iteration_diagnostics=False, assume_optically_thick=True,
-                 scale_height=None, verbose=True):
+                 scale_height=None, verbose=True, convergence_failure='raise'):
 
         if method not in {'Normal', 'LogNormal'}:
             raise ValueError('FrankFitter supports following mehods:\n\t'
                              '{ "Normal", "LogNormal"}"')
         self._method = method
 
         super(FrankFitter, self).__init__(Rmax, N, geometry, nu, block_data,
@@ -719,15 +718,21 @@
             self._DHT, alpha, p_0, weights_smooth, tol
         )
 
         self._max_iter = max_iter
 
         self._store_iteration_diagnostics = store_iteration_diagnostics
 
-        self._info.update({'alpha' : alpha, 'wsmooth' : weights_smooth, 'p0' : p_0})
+        self._info.update({'alpha' : alpha, 'wsmooth' : weights_smooth, 
+            'p0' : p_0, 'method': method})
+        
+        if convergence_failure not in {'raise', 'warn', 'ignore'}:
+            raise ValueError("convergence_failure must be one of 'raise'," 
+                             f"'warn', or 'ignore', nor {convergence_failure}")
+        self._convergence_failure = convergence_failure
 
     def fit_method(self):
         """Name of the fit method"""
         return '{}: {} method'.format(type(self).__name__, self._method)
 
     def _fit(self):
         """Fit step. Computes the best fit given the pre-processed data"""
@@ -775,25 +780,44 @@
 
             if self._store_iteration_diagnostics:
                 self._iteration_diagnostics['power_spectrum'].append(pI)
                 self._iteration_diagnostics['MAP'].append(fit.MAP)
 
             count += 1
 
-        if self._verbose and logging.getLogger().isEnabledFor(logging.INFO):
-            print()
-
-            if count < self._max_iter:
+        # Check / report convergence
+        if count < self._max_iter:
+            if self._verbose and logging.getLogger().isEnabledFor(logging.INFO):
+                print()
                 logging.info('    Convergence criterion met at iteration'
                              ' {}'.format(count-1))
-            else:
+        else:
+            if self._verbose and logging.getLogger().isEnabledFor(logging.INFO):
+                print()
                 logging.info('    Convergence criterion not met; fit stopped at'
                              ' max_iter specified in your parameter file,'
                              ' {}'.format(self._max_iter))
 
+            msg = f'Convergence not met within {self._max_iter} '
+            msg += f'iterations.\nTry increasing max_iter, or '
+            msg += 'try increasing alpha since convergence can '
+            msg += 'be very slow for alpha close to 1.'
+            if self._convergence_failure == 'raise':
+                msg += '\nAlternatively set convergence_failure to'
+                msg += "'warn' or 'ignore' to continue despite the"
+                msg += 'failure.'
+                raise RuntimeError(msg)
+            elif self._convergence_failure == 'warn':
+                if logging.getLogger().isEnabledFor(logging.INFO):
+                    logging.info(msg)
+                else:    
+                    print(msg)
+            elif self._convergence_failure == 'ignore':           
+                pass
+
         if self._store_iteration_diagnostics:
             self._iteration_diagnostics['num_iterations'] = count
 
         # Save the best fit
         if self._method == "Normal":
             self._sol = FrankGaussianFit(self._vis_map, fit, self._info,
                                          geometry=self._geometry.clone())
@@ -920,14 +944,32 @@
         """
 
         if sol is None:
             sol = self.MAP_solution
 
         return self.log_prior(sol.power_spectrum) + sol.log_likelihood()
 
+    def log_evidence_laplace(self):
+        r"""Compute the evidence, p(V), for the best fit model.
+
+        Uses the Laplace approximation, I.e. we model the posterior p(p, V) as
+        a Gaussian in \tau = log(p) centered on p_MAP with the covariance 
+        determined by the curvate of log P(p,V) at p_MAP:
+            P_Laplace(\tau) ~ N(\tau-\tau_MAP, \Sigma) * p(V)
+        where p(V) is the approximated evidence. Here 
+            \Sigma_i,j = - d^2 \log(P) / d\tau_i d\tau_j
+        and p(V) is determined such that P_Lapace(\tau_MAP) = P(p_MAP, V).
+        """
+        Sigma_inv = self._filter.covariance_MAP(self._sol, ret_inv=True)
+
+        sign, logdet = np.linalg.slogdet(Sigma_inv/(2*np.pi))
+        laplace = self.log_likelihood() - 0.5*logdet
+
+        return laplace
+
     @property
     def MAP_solution(self):
         """Reconstruction for the maximum a posteriori power spectrum"""
         return self._sol
 
     @property
     def MAP_spectrum(self):
```

### Comparing `frank-1.2.1/frank/statistical_models.py` & `frank-1.2.2/frank/statistical_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,21 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>
 #
 
-
 import numpy as np
 import scipy.linalg
 import scipy.sparse
 import scipy.optimize
-from collections import defaultdict
 import logging
 
-from frank.hankel import DiscreteHankelTransform
 from frank.constants import rad_to_arcsec, deg_to_rad
-
 from frank.minimizer import LineSearch, MinimizeNewton
 
 class VisibilityMapping:
     r"""Builds the mapping between the visibility and image planes.
 
     VisibilityMapping generates the transform matrices :math:`H(q)` such that
     :math:`V_\nu(q) = H(q) I_\nu`. It also uses these to construct the design
@@ -98,19 +94,19 @@
             if self._verbose:
                 logging.info('  Assuming an optically thin model: *Not* scaling the '
                              'total flux to account for the source inclination')
         elif self._vis_model == 'debris':
             if scale_height is None:
                 raise ValueError('You requested a model with a non-zero scale height'
                                  ' but did not specify H(R) (scale_height=None)')
-            self._scale_height = scale_height
-            self._H2 = 0.5*(2*np.pi*scale_height(self.r) / rad_to_arcsec)**2
+            self._scale_height = scale_height(self.r)
+            self._H2 = 0.5*(2*np.pi*self._scale_height / rad_to_arcsec)**2
             
             if self._verbose:
-                logging.info('  Assuming an optically thin model but geometrically: '
+                logging.info('  Assuming an optically thin model but geometrically '
                              'thick model: *Not* scaling the total flux to account for '
                              'the source inclination')
    
     def map_visibilities(self, u, v, V, weights, frequencies=None, geometry=None):
         r"""
         Compute the matrices :math:`M` abd :math:`j` from the visibility data.
 
@@ -197,31 +193,29 @@
                 Nstep = int(self._chunk_size / self.size + 1)
             else:
                 Nstep = len(Vi)
 
             start = 0
             end = Nstep
             Ndata = len(Vi)
-            M = Ms[i]
-            j = js[i]
             while start < Ndata:
                 qs = qi[start:end]
                 ks = ki[start:end]
                 ws = wi[start:end]
                 Vs = Vi[start:end]
-
+                
                 X = self._get_mapping_coefficients(qs, ks)
 
                 wXT = np.array(X.T * ws, order='C')
 
-                M += np.dot(wXT, X)
-                j += np.dot(wXT, Vs)
+                Ms[i] += np.dot(wXT, X)
+                js[i] += np.dot(wXT, Vs)
 
                 start = end
-                end += Nstep
+                end = min(Ndata, end + Nstep)
 
         # Compute likelihood normalization H_0, i.e., the
         # log-likelihood of a source with I=0.
         H0 = 0.5 * np.sum(np.log(w / (2 * np.pi)) - V * w * V)
 
         if multi_freq:
             return {
@@ -231,14 +225,15 @@
                 'j' : js,
                 'null_likelihood' : H0,
                 'hash' : [True, self._DHT, geometry, self._vis_model, self._scale_height],
             }
         else: 
             return {
                 'mult_freq' : False,
+                'channels' : None,
                 'M' : Ms[0],
                 'j' : js[0],
                 'null_likelihood' : H0,
                 'hash' : [False, self._DHT, geometry, self._vis_model, self._scale_height],
             }
 
     def check_hash(self, hash, multi_freq=False, geometry=None):
@@ -274,15 +269,15 @@
 
         if self._scale_height is None:
             return hash[4] is None
         else:
             if hash[4] is None:
                 return False
             else:
-                return np.alltrue(self._scale_height(self.r) == hash[4](self.r))
+                return np.all(self._scale_height == hash[4])
 
 
     def predict_visibilities(self, I, q, k=None, geometry=None):
         r"""Compute the predicted visibilities given the brightness profile, I
         
         Parameters
         ----------
@@ -412,14 +407,62 @@
 
         """
         if direction == 'backward' and q is not None:
             q = q / rad_to_arcsec
             
         return self._DHT.transform(f, q, direction)
 
+    def DHT_coefficients(self, direction='forward'):
+        """Get the coefficients of the Discrete Hankel Transform.
+
+        The coefficients are defined by
+        .. math:
+            H[h] = np.dot(H, f)
+        
+        Parameters
+        ----------
+        direction : { 'forward', 'backward' }, optional
+            Direction of the transform. If not supplied, the forward
+            transform is used
+
+        Returns
+        -------
+        H : array, size = N or len(q) if supplied
+            The Hankel transform of the array f
+
+        """
+        return self._DHT.coefficients(direction=direction)
+    
+    def interpolate(self, f, r, space='Real'):
+        """
+        Interpolate f (evaluated at the collocation points) to the new points,
+        pts, using interpolation that is consistent with the Fourier-Bessel
+        Series / Discrete Hankel Transform.
+
+        Parameters
+        ----------
+        f : array, size = N
+            Function to interpolate, evaluated at the collocation points:
+                f[k] = f(r_k) or f[k] = f(q_k)
+        r : array or None
+            The points at which to evaluate the interpolation.
+        space : { 'Real', 'Fourier' }, optional
+            Space in which the interpolation is done. If not supplied, 
+            'Real' is assumed.
+
+
+        Returns
+        -------
+        f_interp : array, size = len(r)
+            The interpolated results
+        """
+        if space == 'Real':
+            r = r / rad_to_arcsec
+        return self._DHT.interpolate(f, r, space)
+
 
     def _get_mapping_coefficients(self, qs, ks, geometry=None, inverse=False):
         """Get :math:`H(q)`, such that :math:`V(q) = H(q) I_\nu`"""
         
         if self._vis_model == 'opt_thick':
             # Optically thick & geometrically thin
             if geometry is None:
@@ -496,18 +539,19 @@
         """Number of points in reconstruction"""
         return self._DHT.size
 
     @property
     def scale_height(self):
         "Vertial thickness of the disc, unit = arcsec"
         if self._scale_height is not None:
-            return self._scale_height(self.r)
+            return self._scale_height
         else:
             return None
 
+
 class GaussianModel:
     r"""
     Solves the linear regression problem to compute the posterior,
 
     .. math::
        P(I|q,V,p) \propto G(I-\mu, D),
```

### Comparing `frank-1.2.1/frank/tests.py` & `frank-1.2.2/frank/tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,24 +21,23 @@
 import numpy as np
 import os
 import json
 
 from frank.constants import rad_to_arcsec
 from frank.hankel import DiscreteHankelTransform
 from frank.radial_fitters import FourierBesselFitter, FrankFitter
+from frank.debris_fitters import FrankDebrisFitter
 from frank.geometry import (
     FixedGeometry, FitGeometryGaussian, FitGeometryFourierBessel
 )
-from frank.constants import deg_to_rad
 from frank.utilities import UVDataBinner, generic_dht
-from frank.io import load_uvtable, save_uvtable
+from frank.io import load_uvtable, save_uvtable, load_sol, save_fit
 from frank.statistical_models import VisibilityMapping
 from frank import fit
 
-
 def test_hankel_gauss():
     """Check the Hankel transform"""
 
     def gauss_real_space(r):
         x = r
         return np.exp(-0.5 * x * x)
 
@@ -90,14 +89,15 @@
                                )
     np.testing.assert_allclose(DHT.coefficients(q=DHT.r, direction='backward'),
                                DHT.coefficients(direction='backward'),
                                atol=1e-12, rtol=0,
                                err_msg="Cached inverse DHT Coeffs"
                                )
 
+
 def test_vis_mapping():
     def gauss_real_space(r):
         x = r 
         return np.exp(-0.5 * x * x)
 
     def gauss_vis_space(q):
         qs = (2 * np.pi) * q / rad_to_arcsec
@@ -125,14 +125,15 @@
 
     np.testing.assert_allclose(Iq, 2*Iq_dht,
                                atol=1e-5, rtol=0, err_msg="Forward DHT with generic_dht")
 
     np.testing.assert_allclose(Ir, 0.5*Ir_dht,
                                atol=1e-5, rtol=0, err_msg="Inverse DHT with generic_dht")
 
+
 def test_import_data():
     """Check the UVTable import function works for a .txt"""
     load_uvtable('docs/tutorials/test_datafile.txt')
 
 
 def load_AS209(uv_cut=None):
     """Load data for subsequent tests"""
@@ -153,15 +154,14 @@
                 continue
             cut_data[key] = uv_AS209_DSHARP[key][keep]
 
         uv_AS209_DSHARP = cut_data
 
     return uv_AS209_DSHARP, geometry
 
-
 def test_fit_geometry():
     """Check the geometry fit on a subset of the AS209 data"""
     AS209, _ = load_AS209()
     u, v, vis, weights = [AS209[k][::100] for k in ['u', 'v', 'V', 'weights']]
 
     inc_pa = [30.916257151011674, 85.46246241142246]
     phase_centre = [-0.6431627790617276e-3, -1.161768824369382e-3]
@@ -233,14 +233,15 @@
     np.testing.assert_allclose([geom.inc, geom.PA, 1e3 * geom.dRA,
                                1e3 * geom.dDec],
                               [33.83672738960381, 85.2562498368987,
                                -0.6431627790617276, -1.161768824369382],
                                rtol=1e-5,
                               err_msg="FourierBessel geometry fit (provided phase_centre)")
 
+
 def test_fourier_bessel_fitter():
     """Check FourierBesselFitter fitting routine with AS 209 dataset"""
     AS209, geometry = load_AS209()
 
     u, v, vis, weights = [AS209[k] for k in ['u', 'v', 'V', 'weights']]
 
     Rmax = 1.6
@@ -287,14 +288,15 @@
         -5.190942564982021451e+08,  5.100334030941848755e+08,
         -1.922568182176418006e+08,  8.067782715878820419e+07,
     ])
 
     np.testing.assert_allclose(sol.I, expected,
                                err_msg="Testing Frank Fit to AS 209")
 
+
 def test_two_stage_fit():
     """Check FrankFitter fitting routine with AS 209 dataset"""
     AS209, geometry = load_AS209(uv_cut=1e6)
 
     u, v, vis, weights = [AS209[k] for k in ['u', 'v', 'V', 'weights']]
 
     Rmax = 1.6
@@ -308,14 +310,39 @@
     preproc = FF.preprocess_visibilities(u, v, vis, weights)
     sol2 = FF.fit_preprocessed(preproc)
 
     np.testing.assert_equal(sol.I, sol2.I,
                             err_msg="Testing two-step fit")
 
 
+def test_solve_non_negative():
+    """Check FrankFitter fitting routine with non-negative fit using AS 209 dataset"""
+    AS209, geometry = load_AS209(uv_cut=1e6)
+
+    u, v, vis, weights = [AS209[k] for k in ['u', 'v', 'V', 'weights']]
+
+    Rmax = 1.6
+
+    FF = FrankFitter(Rmax, 20, geometry, alpha=1.05, weights_smooth=1e-2)
+
+    sol = FF.fit(u, v, vis, weights)
+    I_nn = sol.solve_non_negative()
+
+    expected = np.array([
+        2.42756717e+10, 1.28541672e+10, 1.90032938e+10, 8.31444339e+09,
+        1.30814112e+10, 1.59442160e+09, 2.93990783e+08, 5.29739902e+09,
+        1.24011568e+09, 5.40689479e+08, 1.97475180e+08, 2.12294162e+08,
+        4.45700329e+09, 1.67658919e+09, 8.61662448e+08, 3.81032165e+08,
+        2.41202443e+08, 7.68452028e+07, 0.00000000e+00, 2.86208170e+07
+    ])
+
+    np.testing.assert_allclose(I_nn, expected,
+                               err_msg="Testing Frank Fit to AS 209")
+
+
 def test_frank_fitter_log_normal():
     """Check FrankFitter fitting routine with AS 209 dataset"""
     AS209, geometry = load_AS209(uv_cut=1e6)
 
     u, v, vis, weights = [AS209[k] for k in ['u', 'v', 'V', 'weights']]
     
     Rmax = 1.6
@@ -329,15 +356,16 @@
         1.30516037e+10, 1.28158462e+09, 8.14949172e+08, 4.74472433e+09,
         1.66592277e+09, 3.39438704e+08, 1.56219080e+08, 4.42345087e+08,
         4.13155298e+09, 2.00246824e+09, 6.07773834e+08, 5.34020982e+08,
         1.80820913e+08, 7.71858927e+07, 2.89354816e+07, 2.45967370e+06,])
 
     np.testing.assert_allclose(sol.MAP, expected, rtol=7e-5,
                                err_msg="Testing Frank Log-Normal Fit to AS 209")
-                               
+
+
 def test_geom_deproject():
     """Check predict works properly with a different geometry"""
     AS209, geometry = load_AS209(uv_cut=1e6)
 
     u, v, vis, weights = [AS209[k] for k in ['u', 'v', 'V', 'weights']]
 
     Rmax = 1.6
@@ -358,14 +386,15 @@
         0.06555019,  0.01831576, -0.00173855,  0.00042803,
        -0.00322264,  0.00278782, -0.00978981,  0.00620259,
     ]
     
     np.testing.assert_allclose(V, Vexpected, rtol=2e-5, atol=1e-8,
                                err_msg="Testing predict with different geometry")
 
+
 def test_fit_geometry_inside():
     """Check the geometry fit embedded in a call to FrankFitter"""
     AS209, _ = load_AS209(uv_cut=1e6)
 
     u, v, vis, weights = [AS209[k][::100] for k in ['u', 'v', 'V', 'weights']]
 
     Rmax = 1.6
@@ -378,14 +407,15 @@
     geom = sol.geometry
     np.testing.assert_allclose([geom.inc, geom.PA, 1e3 * geom.dRA,
                                 1e3 * geom.dDec],
                                [34.50710460482996, 86.4699107557648,
                                 0.21017246809441995, -2.109586872914908],
                                err_msg="Gaussian geometry fit inside Frank fit")
 
+
 def test_throw_error_on_bad_q_range():
     """Check that frank correctly raises an error when the
     q range is bad."""
     AS209, geometry = load_AS209()
 
     u, v, vis, weights = [AS209[k][::100] for k in ['u', 'v', 'V', 'weights']]
 
@@ -396,14 +426,15 @@
 
     try:
         FF.fit(u, v, vis, weights)
         raise RuntimeError("Expected ValueError due to bad range")
     except ValueError:
         pass
 
+
 def test_uvbin():
     """Check the uv-data binning routine"""
     AS209, geometry = load_AS209()
 
     uv = np.hypot(*geometry.deproject(AS209['u'], AS209['v']))
 
     uvbin = UVDataBinner(uv, AS209['V'], AS209['weights'], 50e3)
@@ -422,14 +453,43 @@
     i = (uvbin.uv >= uvmin) & (uvbin.uv < uvmax)
 
     np.testing.assert_allclose(q, uvbin.uv[i])
     np.testing.assert_allclose(V, uvbin.V[i])
     np.testing.assert_allclose(w, uvbin.weights[i])
     np.testing.assert_allclose(len(widx), uvbin.bin_counts[i])
 
+def test_save_load_sol():
+    """Check saving/loading a frank 'sol' object"""
+    AS209, AS209_geometry = load_AS209(uv_cut=1e6)
+    u, v, vis, weights = [AS209[k][::100] for k in ['u', 'v', 'V', 'weights']]
+    Rmax, N = 1.6, 20
+
+    # generate a sol from a standard frank fit
+    FF = FrankFitter(Rmax, N, AS209_geometry, alpha=1.05, weights_smooth=1e-2)
+    sol = FF.fit(u, v, vis, weights)
+
+    # and from a frank debris fit (has additional keys over a standard fit sol)
+    FF_deb = FrankDebrisFitter(Rmax, N, AS209_geometry, lambda x : 0.05 * x, 
+                                alpha=1.05, weights_smooth=1e-2)
+    sol_deb = FF_deb.fit(u, v, vis, weights)
+
+    tmp_dir = '/tmp/frank/tests'
+    os.makedirs(tmp_dir, exist_ok=True)
+
+    save_prefix = [os.path.join(tmp_dir, 'standard'), os.path.join(tmp_dir, 'debris')]
+    sols = [sol, sol_deb]
+
+    for ii, jj in enumerate(save_prefix):
+        # save the 'sol' object 
+        save_fit(u, v, vis, weights, sols[ii], prefix=jj,
+            save_profile_fit=False, save_vis_fit=False, save_uvtables=False
+            )
+        # load it
+        load_sol(jj + '_frank_sol.obj')
+
 
 def _run_pipeline(geometry='gaussian', fit_phase_offset=True,
                    fit_inc_pa=True, make_figs=False,
                    multifit=False, bootstrap=False):
     """Check the full pipeline that performs a fit and outputs results"""
 
     # Build a subset of the data that we'll load during the fit
@@ -464,15 +524,15 @@
     geom['ddec'] = AS209_geometry.dDec
 
     if make_figs:
         params['plotting']['quick_plot'] = True
         params['plotting']['full_plot'] = True
         params['plotting']['diag_plot'] = True
         params['plotting']['deprojec_plot'] = True
-        params['plotting']['save_figs'] = True
+        params['input_output']['save_figures'] = False
         params['plotting']['distance'] = 121.
         params['plotting']['bin_widths'] = [1e5]
         params['plotting']['iter_plot_range'] = [0, 5]
         params['analysis']['compare_profile'] = 'docs/tutorials/AS209_clean_profile.txt'
         params['analysis']['clean_beam'] = {'bmaj'    : 0.03883,
                                             'bmin'    : 0.03818,
                                             'beam_pa' : 85.82243
```

### Comparing `frank-1.2.1/frank/utilities.py` & `frank-1.2.2/frank/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>
 #
 """This module has various functions useful for plotting and analyzing fit
 results.
 """
 import logging
 import numpy as np
-from scipy.fft import fftfreq
 from scipy.interpolate import interp1d
 
 from frank.constants import deg_to_rad, sterad_to_arcsec, rad_to_arcsec
 from frank.geometry import FixedGeometry
 from frank.hankel import DiscreteHankelTransform
 from frank.statistical_models import VisibilityMapping
 
@@ -87,15 +86,15 @@
 def jy_convert(x, conversion, bmaj=None, bmin=None):
     """
     Provide x as a brightness in one of the units [Jy / beam], [Jy / arcsec^2],
     [Jy / sterad] to convert x to another of these units
 
     Parameters
     ----------
-    x : float
+    x : array
         Brightness in one of: [Jy / beam], [Jy / arcsec^2], [Jy / sterad]
     conversion : { 'beam_sterad', 'beam_arcsec2', 'arcsec2_beam',
                    'arcsec2_sterad', 'sterad_beam', 'sterad_arcsec2'}
         The unit conversion to perform, e.g., 'beam_sterad' converts
         [Jy / beam] to [Jy / sterad]
     bmaj : float, optional
         Beam FWHM along the major axis [arcsec]
@@ -128,21 +127,61 @@
         converted = x / sterad_to_arcsec
     elif conversion == 'beam_sterad':
         converted = x / beam_solid_angle * sterad_to_arcsec
     elif conversion == 'sterad_beam':
         converted = x * beam_solid_angle / sterad_to_arcsec
     else:
         raise AttributeError("conversion must be one of {}"
-                             "".format(['beam_sterad', 'beam_arcsec',
-                             'arcsec_beam', 'arcsec_sterad',
-                             'sterad_beam', 'sterad_arcsec']))
+                             "".format(['beam_sterad', 'beam_arcsec2',
+                             'arcsec2_beam', 'arcsec2_sterad',
+                             'sterad_beam', 'sterad_arcsec2']))
 
     return converted
 
 
+def get_fit_stat_uncer(fit):
+    r"""
+    Retrieve a model brightness profile's statistical uncertainty (that due to 
+    the uncertainty on the observed baselines). This is only a lower bound on 
+    the total uncertainty (which also has a systematic contribution due to 
+    sparse sampling of the (u, v) plane).
+
+    Parameters
+    ----------
+    fit : FrankFitter result object
+        Fitted profile to obtain statistical uncertainty of 
+
+    Returns
+    -------
+    sigma: array
+        Statistical uncertainty on the fitted brightness, at the fitted radial
+        points.
+    """
+
+    if 'method' not in fit._info.keys():
+        raise AttributeError("'fit' object lacks '_info.method' key.")
+
+    if fit._info["method"] == "Normal":
+        sigma = np.sqrt(np.diag(fit.covariance))
+
+    elif fit._info["method"] == "LogNormal":
+        # convert stored variance from var(log(brightness)) to var(brightness).
+        # see Appendix A.2 in https://ui.adsabs.harvard.edu/abs/2016A%26A...586A..76J/abstract;
+        # https://en.wikipedia.org/wiki/Log-normal_distribution
+        log_variance = np.diag(fit.covariance)
+        lin_variance = (np.exp(log_variance) - 1) * np.exp(2 * np.log(fit.I))
+        sigma = np.sqrt(lin_variance)
+
+    else: 
+        raise ValueError("fit._info['method'] {} must be one of "
+            "['Normal', 'LogNormal']".format(fit._info['method']))
+
+    return sigma
+
+
 class UVDataBinner(object):
     r"""
     Average uv-data into bins of equal size.
 
     Compute the weighted mean of the visibilities in each bin
 
     Parameters
```

### Comparing `frank-1.2.1/frank.egg-info/PKG-INFO` & `frank-1.2.2/frank.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: frank
-Version: 1.2.1
+Version: 1.2.2
 Summary: Frankenstein, the flux reconstructor
 Home-page: https://github.com/discsim/frank
 Author: Richard Booth, Jeff Jennings, Marco Tazzari
 Author-email: jjennings1519@gmail.com
 License: LGPLv3
 Project-URL: Bug Tracker, https://github.com/discsim/frank/issues
 Keywords: science,astronomy,interferometry
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs-build
 License-File: LICENSE.txt
 
 <p align="center">
    <img width = "800" src="https://github.com/discsim/frank/blob/master/docs/images/day_off.png?raw=true"/>
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: frank Version: 1.2.1 Summary: Frankenstein, the
+Metadata-Version: 2.1 Name: frank Version: 1.2.2 Summary: Frankenstein, the
 flux reconstructor Home-page: https://github.com/discsim/frank Author: Richard
 Booth, Jeff Jennings, Marco Tazzari Author-email: jjennings1519@gmail.com
 License: LGPLv3 Project-URL: Bug Tracker, https://github.com/discsim/frank/
 issues Keywords: science,astronomy,interferometry Classifier: Development
 Status :: 5 - Production/Stable Classifier: License :: OSI Approved :: GNU
 Lesser General Public License v3 (LGPLv3) Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
-Linux Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
-test Provides-Extra: docs-build License-File: LICENSE.txt
+Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
+text/markdown Provides-Extra: test Provides-Extra: docs-build License-File:
+LICENSE.txt
 [https://github.com/discsim/frank/blob/master/docs/images/day_off.png?raw=true]
     [https://img.shields.io/github/release/discsim/frank/all.svg]  [https://
                        img.shields.io/pypi/v/frank.svg]_
         _[https://img.shields.io/badge/changelog-detailed-blue]__[DOI]_
   _[https://github.com/discsim/frank/actions/workflows/tests.yml/badge.svg]__
    [https://github.com/discsim/frank/actions/workflows/docs.yml/badge.svg]__
              [https://discsim.github.io/frank/coverage/badge.svg]_
```

### Comparing `frank-1.2.1/frank.egg-info/SOURCES.txt` & `frank-1.2.2/frank.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frank-1.2.1/setup.cfg` & `frank-1.2.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -15,28 +15,27 @@
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Operating System :: MacOS :: MacOS X
 	Operating System :: POSIX :: Linux
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 keywords = 
 	science
 	astronomy
 	interferometry
 
 [options]
 packages = frank
-python_requires = >=3.6
+python_requires = >=3.7
 install_requires = 
 	numpy>=1.12
 	matplotlib>=3.1.0
 	scipy>=1.2.0
 
 [options.package_data]
 * = default_parameters.json, parameter_descriptions.json, frank.mplstyle
```

