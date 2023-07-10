# Comparing `tmp/xeofs-1.0.1.tar.gz` & `tmp/xeofs-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeofs-1.0.1.tar", max compression
+gzip compressed data, was "xeofs-1.0.3.tar", max compression
```

## Comparing `xeofs-1.0.1.tar` & `xeofs-1.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1070 2023-07-07 02:48:04.371585 xeofs-1.0.1/LICENSE
--rw-r--r--   0        0        0     5580 2023-07-07 02:48:04.371585 xeofs-1.0.1/README.rst
--rw-r--r--   0        0        0     1138 2023-07-07 02:48:05.119587 xeofs-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       75 2023-07-07 02:48:04.415585 xeofs-1.0.1/xeofs/__init__.py
--rw-r--r--   0        0        0       70 2023-07-07 02:48:05.119587 xeofs-1.0.1/xeofs/_version.py
--rw-r--r--   0        0        0      219 2023-07-07 02:48:04.415585 xeofs-1.0.1/xeofs/models/__init__.py
--rw-r--r--   0        0        0     5791 2023-07-07 02:48:04.415585 xeofs-1.0.1/xeofs/models/_base_cross_model.py
--rw-r--r--   0        0        0     8790 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/models/_base_model.py
--rw-r--r--   0        0        0     3398 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/models/_base_rotator.py
--rw-r--r--   0        0        0     8778 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/models/decomposer.py
--rw-r--r--   0        0        0     7540 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/models/eof.py
--rw-r--r--   0        0        0     9859 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/models/eof_rotator.py
--rw-r--r--   0        0        0    24353 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/models/mca.py
--rw-r--r--   0        0        0    25201 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/models/mca_rotator.py
--rw-r--r--   0        0        0     2153 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/models/rotator_factory.py
--rw-r--r--   0        0        0        0 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/preprocessing/__init__.py
--rw-r--r--   0        0        0      812 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/preprocessing/_base_scaler.py
--rw-r--r--   0        0        0     3781 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/preprocessing/_base_stacker.py
--rw-r--r--   0        0        0    11193 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/preprocessing/scaler.py
--rw-r--r--   0        0        0    21232 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/preprocessing/stacker.py
--rw-r--r--   0        0        0        0 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/utils/__init__.py
--rw-r--r--   0        0        0      301 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/utils/constants.py
--rw-r--r--   0        0        0      631 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/utils/data_types.py
--rw-r--r--   0        0        0     5179 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/utils/rotation.py
--rw-r--r--   0        0        0     2201 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/utils/sanity_checks.py
--rw-r--r--   0        0        0     4681 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/utils/statistics.py
--rw-r--r--   0        0        0     6514 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/utils/xarray_utils.py
--rw-r--r--   0        0        0       41 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/validation/__init__.py
--rw-r--r--   0        0        0        1 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/validation/_base_bootstrapper.py
--rw-r--r--   0        0        0     4957 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/validation/bootstrapper.py
--rw-r--r--   0        0        0     6494 1970-01-01 00:00:00.000000 xeofs-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-10 14:25:12.149602 xeofs-1.0.3/LICENSE
+-rw-r--r--   0        0        0     6380 2023-07-10 14:25:12.149602 xeofs-1.0.3/README.rst
+-rw-r--r--   0        0        0     1137 2023-07-10 14:25:13.005613 xeofs-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       75 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-10 14:25:13.005613 xeofs-1.0.3/xeofs/_version.py
+-rw-r--r--   0        0        0      219 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/models/__init__.py
+-rw-r--r--   0        0        0     5791 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/models/_base_cross_model.py
+-rw-r--r--   0        0        0     8790 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/models/_base_model.py
+-rw-r--r--   0        0        0     3398 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/models/_base_rotator.py
+-rw-r--r--   0        0        0     8778 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/models/decomposer.py
+-rw-r--r--   0        0        0     7540 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/models/eof.py
+-rw-r--r--   0        0        0     9859 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/models/eof_rotator.py
+-rw-r--r--   0        0        0    24353 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/models/mca.py
+-rw-r--r--   0        0        0    25201 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/models/mca_rotator.py
+-rw-r--r--   0        0        0     2153 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/models/rotator_factory.py
+-rw-r--r--   0        0        0        0 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/preprocessing/__init__.py
+-rw-r--r--   0        0        0      812 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/preprocessing/_base_scaler.py
+-rw-r--r--   0        0        0     3781 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/preprocessing/_base_stacker.py
+-rw-r--r--   0        0        0    11193 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/preprocessing/scaler.py
+-rw-r--r--   0        0        0    21232 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/preprocessing/stacker.py
+-rw-r--r--   0        0        0        0 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/utils/__init__.py
+-rw-r--r--   0        0        0      301 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/utils/constants.py
+-rw-r--r--   0        0        0      631 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/utils/data_types.py
+-rw-r--r--   0        0        0     5179 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/utils/rotation.py
+-rw-r--r--   0        0        0     2201 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/utils/sanity_checks.py
+-rw-r--r--   0        0        0     4681 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/utils/statistics.py
+-rw-r--r--   0        0        0     6690 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/utils/xarray_utils.py
+-rw-r--r--   0        0        0       41 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/validation/__init__.py
+-rw-r--r--   0        0        0        1 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/validation/_base_bootstrapper.py
+-rw-r--r--   0        0        0     4957 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/validation/bootstrapper.py
+-rw-r--r--   0        0        0     7299 1970-01-01 00:00:00.000000 xeofs-1.0.3/PKG-INFO
```

### Comparing `xeofs-1.0.1/LICENSE` & `xeofs-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.1/README.rst` & `xeofs-1.0.3/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   :alt: xeofs logo
 
 
 |badge_build_status| |badge_docs_status| |badge_version_pypi| |badge_conda_version| |badge_downloads| |badge_coverage| |badge_license| |badge_zenodo|
 
 .. |badge_version_pypi| image:: https://img.shields.io/pypi/v/xeofs
    :alt: PyPI
-.. |badge_build_status| image:: https://img.shields.io/github/workflow/status/nicrie/xeofs/CI
+.. |badge_build_status| image:: https://img.shields.io/github/actions/workflow/status/nicrie/xeofs/CI.yml?branch=main
    :alt: GitHub Workflow Status (event)
 .. |badge_docs_status| image:: https://readthedocs.org/projects/xeofs/badge/?version=latest
    :target: https://xeofs.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 .. |badge_downloads_pypi| image:: https://img.shields.io/pypi/dm/xeofs
     :alt: PyPI - Downloads
 .. |badge_coverage| image:: https://codecov.io/gh/nicrie/xeofs/branch/main/graph/badge.svg?token=8040ZDH6U7
@@ -32,23 +32,35 @@
 
 
 
 
 Overview
 ---------------------
 
-``xeofs`` is a Python package that provides a platform for performing Empirical Orthogonal Function (EOF) analysis, a popular technique also known as Principal Component Analysis (PCA). It was born out of a necessity to process and analyse multi-dimensional Earth observation data, where the complexity extends beyond simple 2D matrices to include spatial (longitude, latitude, height), temporal (time, steps, lead times), and other dimensions.
+``xeofs`` is a Python package designed for Empirical Orthogonal Function (EOF) analysis, also known as Principal Component Analysis (PCA), 
+and related variants. The package stands out due to its capacity 
+to handle multi-dimensional Earth observation data, thereby optimizing the speed and efficiency of EOF analysis. 
+Here are the key strengths of ``xeofs``:
 
 The benefits of using ``xeofs`` include:
 
 - **Multi-dimensional Analysis**: Execute labeled EOF analysis with the extensive features of ``xarray``.
 - **Scalability**: Handle large datasets effectively with ``dask``.
 - **Speed**: Enjoy quick EOF analysis using ``scipy``'s randomized SVD.
+- **Variety of Methods**: Perform diverse variants of EOF analysis, including complex and rotated version, along with related techniques such as Maximum Covariance Analysis (MCA).
 - **Model Validation**: Validate models through bootstrapping.
 - **Modular Code Structure**: Incorporate new EOF variants with ease due to the package's modular structure.
+- **Flexible Data Formats**: Accepts a variety of ``xarray`` input types (``DataArray``, ``Dataset``, list of ``DataArray``).
+
+Compared to similar packages like eofs_, pyEOF_, and xMCA_, ``xeofs`` is more comprehensive and flexible, providing unique capabilities like handling fully multidimensional dimensions 
+(both samples and features) and a simple interface for bootstrapping. This makes ``xeofs`` a powerful one-stop-shop for most of your EOF analysis needs.
+
+.. _pyEOF: https://github.com/zhonghua-zheng/pyEOF
+.. _xMCA: https://github.com/Yefee/xMCA
+.. _eofs: https://github.com/ajdawson/eofs
 
 Installation
 ------------
 
 To install the package, use either of the following commands:
 
 .. code-block:: bash
@@ -141,15 +153,17 @@
 .. _Bueso: https://github.com/DiegoBueso/ROCK-PCA
 .. _Dawson: https://github.com/ajdawson/eofs
 .. _Yefee: https://github.com/Yefee/xMCA
 
 
 How to cite?
 ----------------------
-Please make sure that when using ``xeofs`` you always cite the **original source** of the method used. Additionally, if you find ``xeofs`` useful for your research, you may cite it as follows::
+When utilizing ``xeofs``, kindly remember to cite the original creators of the methods employed in your work. Additionally, if ``xeofs`` is proving useful in your research, I'd appreciate if you could acknowledge its use with the following citation:
+
+.. code-block:: bibtex
 
    @software{rieger_xeofs_2023,
      title = {xeofs: Multi-dimensional {EOF} analysis and variants in xarray},
      url = {https://github.com/nicrie/xeofs}
      version = {1.0.0},
      author = {Rieger, Niclas},
      date = {2023},
```

### Comparing `xeofs-1.0.1/pyproject.toml` & `xeofs-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "xeofs"
-version = "1.0.1"
+version = "1.0.3"
 description = "Collection of EOF analysis and related techniques for climate science"
 authors = ["Niclas Rieger <niclasrieger@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/nicrie/xeofs"
 repository = "https://github.com/nicrie/xeofs"
 documentation = "https://xeofs.readthedocs.io/en/latest/"
 
 [tool.poetry.dependencies]
-python = ">=3.10"
+python = "^3.10"
 numpy = ">=1.19.2"
 pandas = ">=1.4.1"
 xarray = ">=0.21.1"
 scikit-learn = ">=1.0.2"
 pooch = "^1.6.0"
 tqdm = "^4.64.0"
 dask = ">=2023.0.1"
@@ -22,18 +22,18 @@
 
 [tool.poetry.dev-dependencies]
 flake8 = "^4.0.1"
 pytest = "^7.0.1"
 coverage = "^6.3.1"
 netCDF4 = "^1.5.7"
 sphinx-gallery = "^0"
-sphinxawesome-theme = "^4"
 sphinx-design = "^0"
 nbsphinx = "^0"
 sphinx-copybutton = "^0"
+pydata-sphinx-theme = "^0"
 
 
 [build-system]
 requires = ["setuptools", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
```

### Comparing `xeofs-1.0.1/xeofs/models/_base_cross_model.py` & `xeofs-1.0.3/xeofs/models/_base_cross_model.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.1/xeofs/models/_base_model.py` & `xeofs-1.0.3/xeofs/models/_base_model.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.1/xeofs/models/_base_rotator.py` & `xeofs-1.0.3/xeofs/models/_base_rotator.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.1/xeofs/models/decomposer.py` & `xeofs-1.0.3/xeofs/models/decomposer.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.1/xeofs/models/eof.py` & `xeofs-1.0.3/xeofs/models/eof.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.1/xeofs/models/eof_rotator.py` & `xeofs-1.0.3/xeofs/models/eof_rotator.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.1/xeofs/models/mca.py` & `xeofs-1.0.3/xeofs/models/mca.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.1/xeofs/models/mca_rotator.py` & `xeofs-1.0.3/xeofs/models/mca_rotator.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.1/xeofs/models/rotator_factory.py` & `xeofs-1.0.3/xeofs/models/rotator_factory.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.1/xeofs/preprocessing/_base_scaler.py` & `xeofs-1.0.3/xeofs/preprocessing/_base_scaler.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.1/xeofs/preprocessing/_base_stacker.py` & `xeofs-1.0.3/xeofs/preprocessing/_base_stacker.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.1/xeofs/preprocessing/scaler.py` & `xeofs-1.0.3/xeofs/preprocessing/scaler.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.1/xeofs/preprocessing/stacker.py` & `xeofs-1.0.3/xeofs/preprocessing/stacker.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.1/xeofs/utils/data_types.py` & `xeofs-1.0.3/xeofs/utils/data_types.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.1/xeofs/utils/rotation.py` & `xeofs-1.0.3/xeofs/utils/rotation.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.1/xeofs/utils/sanity_checks.py` & `xeofs-1.0.3/xeofs/utils/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.1/xeofs/utils/statistics.py` & `xeofs-1.0.3/xeofs/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.1/xeofs/utils/xarray_utils.py` & `xeofs-1.0.3/xeofs/utils/xarray_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,16 +131,16 @@
     data: DataArray
         Hilbert transform of the input data.
 
     '''
     return xr.apply_ufunc(
         _hilbert_transform_with_padding,
         data,
-        input_core_dims=[['sample']],
-        output_core_dims=[['sample']],
+        input_core_dims=[['sample', 'feature']],
+        output_core_dims=[['sample', 'feature']],
         kwargs={'padding': padding, 'decay_factor': decay_factor},
         dask='parallelized',
         dask_gufunc_kwargs={'allow_rechunk': True}
     )
 
 def _np_sqrt_cos_lat_weights(data):
     '''Compute the square root of the cosine of the latitude.
@@ -200,14 +200,18 @@
         y = _pad_exp(y, decay_factor=decay_factor)
     
     y = hilbert(y, axis=0)
     
     if padding == 'exp':
         y = y[n_samples:2*n_samples]
 
+    # Padding can introduce a shift in the mean of the imaginary part
+    # of the Hilbert transform. Correct for this shift.
+    y = y - y.mean(axis=0)
+
     return y
 
 def _pad_exp(y, decay_factor=.2):
     '''Pad the input array with an exponential decay function.
 
     The start and end of the input array are padded with an exponential decay
     function falling to a reference line given by a linear fit of the data array.
```

### Comparing `xeofs-1.0.1/xeofs/validation/bootstrapper.py` & `xeofs-1.0.3/xeofs/validation/bootstrapper.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.1/PKG-INFO` & `xeofs-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: xeofs
-Version: 1.0.1
+Version: 1.0.3
 Summary: Collection of EOF analysis and related techniques for climate science
 Home-page: https://github.com/nicrie/xeofs
 License: MIT
 Author: Niclas Rieger
 Author-email: niclasrieger@gmail.com
-Requires-Python: >=3.10
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dask (>=2023.0.1)
 Requires-Dist: numpy (>=1.19.2)
 Requires-Dist: pandas (>=1.4.1)
@@ -29,15 +29,15 @@
   :alt: xeofs logo
 
 
 |badge_build_status| |badge_docs_status| |badge_version_pypi| |badge_conda_version| |badge_downloads| |badge_coverage| |badge_license| |badge_zenodo|
 
 .. |badge_version_pypi| image:: https://img.shields.io/pypi/v/xeofs
    :alt: PyPI
-.. |badge_build_status| image:: https://img.shields.io/github/workflow/status/nicrie/xeofs/CI
+.. |badge_build_status| image:: https://img.shields.io/github/actions/workflow/status/nicrie/xeofs/CI.yml?branch=main
    :alt: GitHub Workflow Status (event)
 .. |badge_docs_status| image:: https://readthedocs.org/projects/xeofs/badge/?version=latest
    :target: https://xeofs.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 .. |badge_downloads_pypi| image:: https://img.shields.io/pypi/dm/xeofs
     :alt: PyPI - Downloads
 .. |badge_coverage| image:: https://codecov.io/gh/nicrie/xeofs/branch/main/graph/badge.svg?token=8040ZDH6U7
@@ -57,23 +57,35 @@
 
 
 
 
 Overview
 ---------------------
 
-``xeofs`` is a Python package that provides a platform for performing Empirical Orthogonal Function (EOF) analysis, a popular technique also known as Principal Component Analysis (PCA). It was born out of a necessity to process and analyse multi-dimensional Earth observation data, where the complexity extends beyond simple 2D matrices to include spatial (longitude, latitude, height), temporal (time, steps, lead times), and other dimensions.
+``xeofs`` is a Python package designed for Empirical Orthogonal Function (EOF) analysis, also known as Principal Component Analysis (PCA), 
+and related variants. The package stands out due to its capacity 
+to handle multi-dimensional Earth observation data, thereby optimizing the speed and efficiency of EOF analysis. 
+Here are the key strengths of ``xeofs``:
 
 The benefits of using ``xeofs`` include:
 
 - **Multi-dimensional Analysis**: Execute labeled EOF analysis with the extensive features of ``xarray``.
 - **Scalability**: Handle large datasets effectively with ``dask``.
 - **Speed**: Enjoy quick EOF analysis using ``scipy``'s randomized SVD.
+- **Variety of Methods**: Perform diverse variants of EOF analysis, including complex and rotated version, along with related techniques such as Maximum Covariance Analysis (MCA).
 - **Model Validation**: Validate models through bootstrapping.
 - **Modular Code Structure**: Incorporate new EOF variants with ease due to the package's modular structure.
+- **Flexible Data Formats**: Accepts a variety of ``xarray`` input types (``DataArray``, ``Dataset``, list of ``DataArray``).
+
+Compared to similar packages like eofs_, pyEOF_, and xMCA_, ``xeofs`` is more comprehensive and flexible, providing unique capabilities like handling fully multidimensional dimensions 
+(both samples and features) and a simple interface for bootstrapping. This makes ``xeofs`` a powerful one-stop-shop for most of your EOF analysis needs.
+
+.. _pyEOF: https://github.com/zhonghua-zheng/pyEOF
+.. _xMCA: https://github.com/Yefee/xMCA
+.. _eofs: https://github.com/ajdawson/eofs
 
 Installation
 ------------
 
 To install the package, use either of the following commands:
 
 .. code-block:: bash
@@ -166,15 +178,17 @@
 .. _Bueso: https://github.com/DiegoBueso/ROCK-PCA
 .. _Dawson: https://github.com/ajdawson/eofs
 .. _Yefee: https://github.com/Yefee/xMCA
 
 
 How to cite?
 ----------------------
-Please make sure that when using ``xeofs`` you always cite the **original source** of the method used. Additionally, if you find ``xeofs`` useful for your research, you may cite it as follows::
+When utilizing ``xeofs``, kindly remember to cite the original creators of the methods employed in your work. Additionally, if ``xeofs`` is proving useful in your research, I'd appreciate if you could acknowledge its use with the following citation:
+
+.. code-block:: bibtex
 
    @software{rieger_xeofs_2023,
      title = {xeofs: Multi-dimensional {EOF} analysis and variants in xarray},
      url = {https://github.com/nicrie/xeofs}
      version = {1.0.0},
      author = {Rieger, Niclas},
      date = {2023},
```

