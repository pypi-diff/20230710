# Comparing `tmp/pedestal-inference-0.2.2.tar.gz` & `tmp/pedestal-inference-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pedestal-inference-0.2.2.tar", last modified: Wed Jul  5 15:41:17 2023, max compression
+gzip compressed data, was "pedestal-inference-0.2.3.tar", last modified: Mon Jul 10 17:41:27 2023, max compression
```

## Comparing `pedestal-inference-0.2.2.tar` & `pedestal-inference-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-05 15:41:17.115081 pedestal-inference-0.2.2/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1069 2022-04-07 11:51:39.000000 pedestal-inference-0.2.2/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)      979 2023-07-05 15:41:17.115081 pedestal-inference-0.2.2/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      270 2022-06-02 17:16:45.000000 pedestal-inference-0.2.2/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-05 15:41:17.115081 pedestal-inference-0.2.2/pedestal_inference.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)      979 2023-07-05 15:41:17.000000 pedestal-inference-0.2.2/pedestal_inference.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      400 2023-07-05 15:41:17.000000 pedestal-inference-0.2.2/pedestal_inference.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-07-05 15:41:17.000000 pedestal-inference-0.2.2/pedestal_inference.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      128 2023-07-05 15:41:17.000000 pedestal-inference-0.2.2/pedestal_inference.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        7 2023-07-05 15:41:17.000000 pedestal-inference-0.2.2/pedestal_inference.egg-info/top_level.txt
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-05 15:41:17.115081 pedestal-inference-0.2.2/pedinf/
--rw-rw-r--   0 chris     (1000) chris     (1000)     6452 2023-07-05 14:36:16.000000 pedestal-inference-0.2.2/pedinf/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    17094 2023-04-04 14:04:02.000000 pedestal-inference-0.2.2/pedinf/analysis.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1761 2023-06-16 12:58:40.000000 pedestal-inference-0.2.2/pedinf/diagnostics.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10546 2023-06-18 01:14:19.000000 pedestal-inference-0.2.2/pedinf/models.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5642 2023-06-18 01:49:12.000000 pedestal-inference-0.2.2/pedinf/spectrum.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      737 2023-07-05 15:33:14.000000 pedestal-inference-0.2.2/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)      954 2023-07-05 15:41:17.115081 pedestal-inference-0.2.2/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2021-11-05 18:05:19.000000 pedestal-inference-0.2.2/setup.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-05 15:41:17.115081 pedestal-inference-0.2.2/tests/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1309 2023-04-04 14:04:02.000000 pedestal-inference-0.2.2/tests/test_analysis.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2080 2023-04-04 14:04:02.000000 pedestal-inference-0.2.2/tests/test_models.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-10 17:41:27.512802 pedestal-inference-0.2.3/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1069 2022-04-07 11:51:39.000000 pedestal-inference-0.2.3/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)      983 2023-07-10 17:41:27.512802 pedestal-inference-0.2.3/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      270 2022-06-02 17:16:45.000000 pedestal-inference-0.2.3/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-10 17:41:27.508803 pedestal-inference-0.2.3/pedestal_inference.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      983 2023-07-10 17:41:27.000000 pedestal-inference-0.2.3/pedestal_inference.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      400 2023-07-10 17:41:27.000000 pedestal-inference-0.2.3/pedestal_inference.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-07-10 17:41:27.000000 pedestal-inference-0.2.3/pedestal_inference.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      128 2023-07-10 17:41:27.000000 pedestal-inference-0.2.3/pedestal_inference.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        7 2023-07-10 17:41:27.000000 pedestal-inference-0.2.3/pedestal_inference.egg-info/top_level.txt
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-10 17:41:27.512802 pedestal-inference-0.2.3/pedinf/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7022 2023-07-10 17:32:22.000000 pedestal-inference-0.2.3/pedinf/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    17094 2023-04-04 14:04:02.000000 pedestal-inference-0.2.3/pedinf/analysis.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3773 2023-07-10 17:32:22.000000 pedestal-inference-0.2.3/pedinf/diagnostics.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10546 2023-06-18 01:14:19.000000 pedestal-inference-0.2.3/pedinf/models.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5642 2023-07-10 17:32:22.000000 pedestal-inference-0.2.3/pedinf/spectrum.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      741 2023-07-10 17:38:46.000000 pedestal-inference-0.2.3/pyproject.toml
+-rw-rw-r--   0 chris     (1000) chris     (1000)      954 2023-07-10 17:41:27.512802 pedestal-inference-0.2.3/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2021-11-05 18:05:19.000000 pedestal-inference-0.2.3/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-10 17:41:27.512802 pedestal-inference-0.2.3/tests/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1309 2023-04-04 14:04:02.000000 pedestal-inference-0.2.3/tests/test_analysis.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2080 2023-04-04 14:04:02.000000 pedestal-inference-0.2.3/tests/test_models.py
```

### Comparing `pedestal-inference-0.2.2/LICENSE` & `pedestal-inference-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pedestal-inference-0.2.2/PKG-INFO` & `pedestal-inference-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pedestal-inference
-Version: 0.2.2
+Version: 0.2.3
 Summary: A collection of Python tools for plasma-edge Thomson-scattering analysis
 Home-page: https://github.com/C-bowman/pedestal-inference
 Author: Chris Bowman
 Author-email: Chris Bowman <chris.bowman.physics@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/C-bowman/pedestal-inference
-Project-URL: documentation, https://inference-tools.readthedocs.io
+Project-URL: documentation, https://pedestal-inference.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
```

### Comparing `pedestal-inference-0.2.2/pedestal_inference.egg-info/PKG-INFO` & `pedestal-inference-0.2.3/pedestal_inference.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pedestal-inference
-Version: 0.2.2
+Version: 0.2.3
 Summary: A collection of Python tools for plasma-edge Thomson-scattering analysis
 Home-page: https://github.com/C-bowman/pedestal-inference
 Author: Chris Bowman
 Author-email: Chris Bowman <chris.bowman.physics@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/C-bowman/pedestal-inference
-Project-URL: documentation, https://inference-tools.readthedocs.io
+Project-URL: documentation, https://pedestal-inference.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
```

### Comparing `pedestal-inference-0.2.2/pedinf/__init__.py` & `pedestal-inference-0.2.3/pedinf/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -146,14 +146,22 @@
         )
 
         de_result = differential_evolution(func=self.posterior.cost, bounds=self.bounds)
 
         return bfgs_mode if fmin < de_result.fun else de_result.x
 
 
+class FlatPrior:
+    def __call__(self, theta):
+        return 0.
+
+    def gradient(self, theta):
+        return 0.
+
+
 @dataclass
 class SpectrumData:
     spectra: ndarray
     errors: ndarray
     spatial_channels: ndarray
     time_index: int
     shot: int
@@ -191,13 +199,23 @@
         self.spectrum = spectrometer_model
         self.data = spectrum_data
 
         self.likelihood = likelihood(
             y_data=self.data.spectra.flatten(),
             sigma=self.data.errors.flatten(),
             forward_model=self.spectrum.predictions,
+            forward_model_jacobian=self.spectrum.predictions_jacobian
         )
 
-        self.prior = lambda x: 0.0 if prior is None else prior
+        self.prior = FlatPrior() if prior is None else prior
 
-    def __call__(self, theta):
+    def __call__(self, theta: ndarray) -> float:
         return self.likelihood(theta) + self.prior(theta)
+
+    def gradient(self, theta: ndarray) -> ndarray:
+        return self.likelihood.gradient(theta) + self.prior.gradient(theta)
+
+    def cost(self, theta: ndarray) -> float:
+        return -self.likelihood(theta) - self.prior(theta)
+
+    def cost_gradient(self, theta: ndarray) -> ndarray:
+        return -self.likelihood.gradient(theta) - self.prior.gradient(theta)
```

### Comparing `pedestal-inference-0.2.2/pedinf/analysis.py` & `pedestal-inference-0.2.3/pedinf/analysis.py`

 * *Files identical despite different names*

### Comparing `pedestal-inference-0.2.2/pedinf/models.py` & `pedestal-inference-0.2.3/pedinf/models.py`

 * *Files identical despite different names*

### Comparing `pedestal-inference-0.2.2/pedinf/spectrum.py` & `pedestal-inference-0.2.3/pedinf/spectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,23 +107,23 @@
         self.ln_te = ln_te_axes
         self.scattering_angle = scattering_angle_axes
         self.response = response
 
         # build the splines for all spatial / spectral channels
         n_positions, n_spectra, _, _ = self.response.shape
         self.splines = []
-        for i in range(n_positions):
+        for j in range(n_spectra):
             self.splines.append(
                 [
                     RectBivariateSpline(
                         x=self.ln_te[i, :],
                         y=self.scattering_angle[i, :],
                         z=self.response[i, j, :, :],
                     )
-                    for j in range(n_spectra)
+                    for i in range(n_positions)
                 ]
             )
 
     @classmethod
     def calculate_response(
         cls,
         wavelengths: ndarray,
```

### Comparing `pedestal-inference-0.2.2/pyproject.toml` & `pedestal-inference-0.2.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pedestal-inference"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="Chris Bowman", email="chris.bowman.physics@gmail.com" },
 ]
 description = "A collection of Python tools for plasma-edge Thomson-scattering analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -16,13 +16,13 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "numpy >= 1.8",
     "scipy >= 1.6.3",
-    "inference-tools >= 0.11.0",
+    "inference-tools >= 0.12.0",
 ]
 
 [project.urls]
 homepage = "https://github.com/C-bowman/pedestal-inference"
-documentation = "https://inference-tools.readthedocs.io"
+documentation = "https://pedestal-inference.readthedocs.io/"
```

### Comparing `pedestal-inference-0.2.2/setup.cfg` & `pedestal-inference-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pedestal-inference-0.2.2/tests/test_analysis.py` & `pedestal-inference-0.2.3/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `pedestal-inference-0.2.2/tests/test_models.py` & `pedestal-inference-0.2.3/tests/test_models.py`

 * *Files identical despite different names*

