# Comparing `tmp/mflike-0.8.4.tar.gz` & `tmp/mflike-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mflike-0.8.4.tar", last modified: Tue May 30 14:51:08 2023, max compression
+gzip compressed data, was "mflike-0.9.0.tar", last modified: Mon Jul 10 12:38:28 2023, max compression
```

## Comparing `mflike-0.8.4.tar` & `mflike-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:51:08.155874 mflike-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-30 14:51:04.000000 mflike-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-30 14:51:04.000000 mflike-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-30 14:51:08.155874 mflike-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-30 14:51:04.000000 mflike-0.8.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:51:08.155874 mflike-0.8.4/mflike/
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-05-30 14:51:04.000000 mflike-0.8.4/mflike/MFLike.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-30 14:51:04.000000 mflike-0.8.4/mflike/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-30 14:51:08.155874 mflike-0.8.4/mflike/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-05-30 14:51:04.000000 mflike-0.8.4/mflike/mflike.py
--rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-05-30 14:51:04.000000 mflike-0.8.4/mflike/theoryforge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:51:08.155874 mflike-0.8.4/mflike.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-30 14:51:08.000000 mflike-0.8.4/mflike.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-30 14:51:08.000000 mflike-0.8.4/mflike.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:51:08.000000 mflike-0.8.4/mflike.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 14:51:08.000000 mflike-0.8.4/mflike.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 14:51:08.000000 mflike-0.8.4/mflike.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:51:08.000000 mflike-0.8.4/mflike.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-30 14:51:08.155874 mflike-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-30 14:51:04.000000 mflike-0.8.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-05-30 14:51:04.000000 mflike-0.8.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:38:28.271775 mflike-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-10 12:38:24.000000 mflike-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 12:38:24.000000 mflike-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-10 12:38:28.271775 mflike-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-10 12:38:24.000000 mflike-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:38:28.271775 mflike-0.9.0/mflike/
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-10 12:38:24.000000 mflike-0.9.0/mflike/MFLike.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-10 12:38:24.000000 mflike-0.9.0/mflike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-10 12:38:28.271775 mflike-0.9.0/mflike/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13748 2023-07-10 12:38:24.000000 mflike-0.9.0/mflike/mflike.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18736 2023-07-10 12:38:24.000000 mflike-0.9.0/mflike/theoryforge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:38:28.271775 mflike-0.9.0/mflike.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-10 12:38:28.000000 mflike-0.9.0/mflike.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-10 12:38:28.000000 mflike-0.9.0/mflike.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:38:28.000000 mflike-0.9.0/mflike.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-10 12:38:28.000000 mflike-0.9.0/mflike.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 12:38:28.000000 mflike-0.9.0/mflike.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:38:28.000000 mflike-0.9.0/mflike.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-10 12:38:28.271775 mflike-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-10 12:38:24.000000 mflike-0.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-07-10 12:38:24.000000 mflike-0.9.0/versioneer.py
```

### Comparing `mflike-0.8.4/LICENSE` & `mflike-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mflike-0.8.4/PKG-INFO` & `mflike-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mflike
-Version: 0.8.4
+Version: 0.9.0
 Summary: SO LAT multi-frequency likelihood for cobaya
 Home-page: https://github.com/simonsobs/LAT_MFLike
 Author: Simons Observatory Collaboration Power Spectrum Group aka so_ps 1 & 2
 License: BSD license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -91,14 +91,16 @@
 ``mflike_example.yaml`` file) using the combination of TT, TE and EE spectra (*i.e.*
 ``polarizations: ['TT', 'TE', 'ET', 'EE']``). The results will be stored in the ``chains/mcmc``
 directory.
 
 Simulation releases
 -------------------
 
+- ``v0.8`` release has spectra produced with high accuracy camb parameters up to ``ell = 9000``, the foreground components are integrated in frequency using top-hat bandpasses, stored in the ``sacc`` files
+
 - ``v0.7.1`` is a bugfix release of ``v0.7`` release where the mono-frequency and dirac bandpasses
   have been correctly set with the ``sacc`` files
 
 - ``v0.7`` release includes the ACT like foregrounds. Simulation parameters are also stored within ``sacc`` metadata and the associated ``dict`` file can be viewed `here <https://gist.github.com/xgarrido/5d2fdbe4232cfa9ad1156ee30baa7811>`_.
 
 - ``v0.6`` release make use of CMB map based simulations (see https://github.com/simonsobs/map_based_simulations/blob/master/201911_lensed_cmb/README.md). Only temperature foregrounds were considered.
```

### Comparing `mflike-0.8.4/README.rst` & `mflike-0.9.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -72,14 +72,16 @@
 ``mflike_example.yaml`` file) using the combination of TT, TE and EE spectra (*i.e.*
 ``polarizations: ['TT', 'TE', 'ET', 'EE']``). The results will be stored in the ``chains/mcmc``
 directory.
 
 Simulation releases
 -------------------
 
+- ``v0.8`` release has spectra produced with high accuracy camb parameters up to ``ell = 9000``, the foreground components are integrated in frequency using top-hat bandpasses, stored in the ``sacc`` files
+
 - ``v0.7.1`` is a bugfix release of ``v0.7`` release where the mono-frequency and dirac bandpasses
   have been correctly set with the ``sacc`` files
 
 - ``v0.7`` release includes the ACT like foregrounds. Simulation parameters are also stored within ``sacc`` metadata and the associated ``dict`` file can be viewed `here <https://gist.github.com/xgarrido/5d2fdbe4232cfa9ad1156ee30baa7811>`_.
 
 - ``v0.6`` release make use of CMB map based simulations (see https://github.com/simonsobs/map_based_simulations/blob/master/201911_lensed_cmb/README.md). Only temperature foregrounds were considered.
```

### Comparing `mflike-0.8.4/mflike/MFLike.yaml` & `mflike-0.9.0/mflike/MFLike.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # A simple cobaya likelihood for SO/LAT
 
-data_folder: MFLike/v0.7.1
+data_folder: MFLike/v0.8
 # Path to the input SACC file, containing, minimally,
 # information about the different tracers (i.e. frequency
 # bands) and the set of power spectra.
 input_file: null
 # If cov_Bbl_file is null, then the previous file should
 # also contain bandpower window functions and covariance
 # matrix. Otherwise they'll be read from this file.
@@ -19,18 +19,18 @@
 # Specify default set of spectra and scale cuts
 # to be used
 defaults:
   # Which spectra?
   polarizations: [TT, TE, ET, EE]
   # Scale cuts (in ell) for each spectrum
   scales:
-    TT: [50, 5000]
-    TE: [50, 5000]
-    ET: [50, 5000]
-    EE: [50, 5000]
+    TT: [30, 9000]
+    TE: [30, 9000]
+    ET: [30, 9000]
+    EE: [30, 9000]
   # If True, TE' = (TE + ET) / 2 will be used
   # instead of TE and ET separately.
   symmetrize: false
 
 data:
   # List the names and frequencies of all the
   # relevant experiments.
@@ -67,15 +67,16 @@
 #     bandwidth can be a list if you want a different width for each band
 #     e.g. bandwidth: [0.3,0.2,0.3] for 3 bands
 # when top_hat_band is a null dict: no top-hat band is built and
 # bandpasses read from sacc file. Band integration is performed accordingly
 # (if bandpass in sacc is a single freq, no band integration)
 # the default is to read bandpasses from file, to build top-hat uncomment the
 # parameters of the block!
-# Bandpass has to be in RJ units
+# Bandpass has to be divided by nu^2 if measured with respect to a RJ source
+# the nu^2 factor is set back again in the _bandpass_construction function
 top_hat_band:
 #  nsteps: 1
 #  bandwidth: 0
 
 # uncomment the block to include a systematic template
 # to be read from external file at "rootname"
 # default is systematic_template to be a null dict
```

### Comparing `mflike-0.8.4/mflike/mflike.py` & `mflike-0.9.0/mflike/mflike.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from cobaya.tools import are_different_params_lists
 
 from .theoryforge import TheoryForge
 
 
 class MFLike(InstallableLikelihood):
     _url = "https://portal.nersc.gov/cfs/sobs/users/MFLike_data"
-    _release = "v0.7.1"
+    _release = "v0.8"
     install_options = {"download_url": f"{_url}/{_release}.tar.gz"}
 
     # attributes set from .yaml
     input_file: Optional[str]
     cov_Bbl_file: Optional[str]
     data: dict
     defaults: dict
```

### Comparing `mflike-0.8.4/mflike/theoryforge.py` & `mflike-0.9.0/mflike/theoryforge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import os
 from itertools import product
 
 import numpy as np
 from cobaya.log import LoggedError
 
 
-# Converts from cmb units to brightness.
-# There is an additional nu**2 factor to convert the bandpasses
-# from RJ to brightness units.
+# Converts from cmb temperature to differential source intensity
+# (see eq. 8 of https://arxiv.org/abs/1303.5070).
+# The bandpass transmission needs to be divided by
+# nu^2 if measured with respect to a RJ source.
+# This factor is already included here.
 # Numerical factors not included,
 # it needs proper normalization when used.
 def _cmb2bb(nu):
     # NB: numerical factors not included
     from scipy import constants
 
     T_CMB = 2.72548
@@ -77,15 +79,17 @@
                 if self.bandint_nsteps > 1 and np.any(np.array(self.bandint_width) == 0):
                     raise LoggedError(
                         self.log, "One band has width = 0, set a positive width and run again"
                     )
 
     # Takes care of the bandpass construction. It returns a list of nu-transmittance
     # for each frequency or an array with the effective freqs.
-    # bandpasses saved in the sacc file have to be in RJ units
+    # bandpasses saved in the sacc file have to be divided by nu^2
+    # if measured with respect to a RJ source.
+    # This factor is already included in the _cmb2bb function
     def _bandpass_construction(self, **params):
         data_are_monofreq = False
         self.bandint_freqs = []
         for iexp, exp in enumerate(self.experiments):
             bandpar = f"bandint_shift_{exp}"
             # Only temperature bandpass for the time being
             bands = self.bands[f"{exp}_s0"]
```

### Comparing `mflike-0.8.4/mflike.egg-info/PKG-INFO` & `mflike-0.9.0/mflike.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mflike
-Version: 0.8.4
+Version: 0.9.0
 Summary: SO LAT multi-frequency likelihood for cobaya
 Home-page: https://github.com/simonsobs/LAT_MFLike
 Author: Simons Observatory Collaboration Power Spectrum Group aka so_ps 1 & 2
 License: BSD license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -91,14 +91,16 @@
 ``mflike_example.yaml`` file) using the combination of TT, TE and EE spectra (*i.e.*
 ``polarizations: ['TT', 'TE', 'ET', 'EE']``). The results will be stored in the ``chains/mcmc``
 directory.
 
 Simulation releases
 -------------------
 
+- ``v0.8`` release has spectra produced with high accuracy camb parameters up to ``ell = 9000``, the foreground components are integrated in frequency using top-hat bandpasses, stored in the ``sacc`` files
+
 - ``v0.7.1`` is a bugfix release of ``v0.7`` release where the mono-frequency and dirac bandpasses
   have been correctly set with the ``sacc`` files
 
 - ``v0.7`` release includes the ACT like foregrounds. Simulation parameters are also stored within ``sacc`` metadata and the associated ``dict`` file can be viewed `here <https://gist.github.com/xgarrido/5d2fdbe4232cfa9ad1156ee30baa7811>`_.
 
 - ``v0.6`` release make use of CMB map based simulations (see https://github.com/simonsobs/map_based_simulations/blob/master/201911_lensed_cmb/README.md). Only temperature foregrounds were considered.
```

### Comparing `mflike-0.8.4/setup.py` & `mflike-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `mflike-0.8.4/versioneer.py` & `mflike-0.9.0/versioneer.py`

 * *Files identical despite different names*

