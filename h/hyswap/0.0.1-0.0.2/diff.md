# Comparing `tmp/hyswap-0.0.1.tar.gz` & `tmp/hyswap-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyswap-0.0.1.tar", last modified: Mon Jun 12 12:25:06 2023, max compression
+gzip compressed data, was "hyswap-0.0.2.tar", last modified: Mon Jul 10 19:03:10 2023, max compression
```

## Comparing `hyswap-0.0.1.tar` & `hyswap-0.0.2.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.385591 hyswap-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.381591 hyswap-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.381591 hyswap-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-12 12:24:31.000000 hyswap-0.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-12 12:24:31.000000 hyswap-0.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-12 12:24:31.000000 hyswap-0.0.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-12 12:24:31.000000 hyswap-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-12 12:24:31.000000 hyswap-0.0.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-12 12:24:31.000000 hyswap-0.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-12 12:24:31.000000 hyswap-0.0.1/DISCLAIMER.md
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-12 12:24:31.000000 hyswap-0.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-12 12:25:06.385591 hyswap-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-12 12:24:31.000000 hyswap-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-12 12:24:31.000000 hyswap-0.0.1/code.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.381591 hyswap-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.381591 hyswap-0.0.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.381591 hyswap-0.0.1/docs/source/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/examples/cumulative_hydrograph_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/examples/flow_duration_curve_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/examples/raster_hydrograph_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/examples/streamflow_duration_hydrograph_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.381591 hyswap-0.0.1/docs/source/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/meta/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/meta/disclaimer.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/meta/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.381591 hyswap-0.0.1/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (123)    28371 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/reference/hyswap.png
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/reference/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.385591 hyswap-0.0.1/hyswap/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-12 12:24:31.000000 hyswap-0.0.1/hyswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 12:25:06.000000 hyswap-0.0.1/hyswap/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-12 12:24:31.000000 hyswap-0.0.1/hyswap/cumulative.py
--rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-06-12 12:24:31.000000 hyswap-0.0.1/hyswap/exceedance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-06-12 12:24:31.000000 hyswap-0.0.1/hyswap/percentiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-06-12 12:24:31.000000 hyswap-0.0.1/hyswap/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-06-12 12:24:31.000000 hyswap-0.0.1/hyswap/rasterhydrograph.py
--rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-06-12 12:24:31.000000 hyswap-0.0.1/hyswap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.385591 hyswap-0.0.1/hyswap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-12 12:25:06.000000 hyswap-0.0.1/hyswap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-12 12:25:06.000000 hyswap-0.0.1/hyswap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:25:06.000000 hyswap-0.0.1/hyswap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-12 12:25:06.000000 hyswap-0.0.1/hyswap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 12:25:06.000000 hyswap-0.0.1/hyswap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-12 12:24:31.000000 hyswap-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-12 12:24:31.000000 hyswap-0.0.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 12:24:31.000000 hyswap-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 12:25:06.385591 hyswap-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 12:24:31.000000 hyswap-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.385591 hyswap-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-12 12:24:31.000000 hyswap-0.0.1/tests/test_cumulative.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-06-12 12:24:31.000000 hyswap-0.0.1/tests/test_exceedance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-06-12 12:24:31.000000 hyswap-0.0.1/tests/test_percentiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-12 12:24:31.000000 hyswap-0.0.1/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-06-12 12:24:31.000000 hyswap-0.0.1/tests/test_rasterhydrograph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10450 2023-06-12 12:24:31.000000 hyswap-0.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:03:10.841017 hyswap-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:03:10.833017 hyswap-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:03:10.837017 hyswap-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-10 19:02:36.000000 hyswap-0.0.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-10 19:02:36.000000 hyswap-0.0.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-10 19:02:36.000000 hyswap-0.0.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-10 19:02:36.000000 hyswap-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-10 19:02:36.000000 hyswap-0.0.2/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-07-10 19:02:36.000000 hyswap-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-10 19:02:36.000000 hyswap-0.0.2/DISCLAIMER.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-10 19:02:36.000000 hyswap-0.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-10 19:03:10.841017 hyswap-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-10 19:02:36.000000 hyswap-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-10 19:02:36.000000 hyswap-0.0.2/code.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:03:10.837017 hyswap-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-10 19:02:36.000000 hyswap-0.0.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:03:10.837017 hyswap-0.0.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:02:36.000000 hyswap-0.0.2/docs/source/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-07-10 19:02:36.000000 hyswap-0.0.2/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:03:10.837017 hyswap-0.0.2/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-07-10 19:02:36.000000 hyswap-0.0.2/docs/source/examples/cumulative_hydrograph_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-07-10 19:02:36.000000 hyswap-0.0.2/docs/source/examples/flow_duration_curve_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-10 19:02:36.000000 hyswap-0.0.2/docs/source/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-10 19:02:36.000000 hyswap-0.0.2/docs/source/examples/raster_hydrograph_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-10 19:02:36.000000 hyswap-0.0.2/docs/source/examples/streamflow_duration_hydrograph_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-10 19:02:36.000000 hyswap-0.0.2/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:03:10.837017 hyswap-0.0.2/docs/source/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-10 19:02:36.000000 hyswap-0.0.2/docs/source/meta/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-10 19:02:36.000000 hyswap-0.0.2/docs/source/meta/disclaimer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17302 2023-07-10 19:02:36.000000 hyswap-0.0.2/docs/source/meta/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-10 19:02:36.000000 hyswap-0.0.2/docs/source/meta/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:03:10.837017 hyswap-0.0.2/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)    28371 2023-07-10 19:02:36.000000 hyswap-0.0.2/docs/source/reference/hyswap.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-10 19:02:36.000000 hyswap-0.0.2/docs/source/reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:03:10.841017 hyswap-0.0.2/hyswap/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-10 19:02:36.000000 hyswap-0.0.2/hyswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-10 19:03:10.000000 hyswap-0.0.2/hyswap/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-10 19:02:36.000000 hyswap-0.0.2/hyswap/cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-07-10 19:02:36.000000 hyswap-0.0.2/hyswap/exceedance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-07-10 19:02:36.000000 hyswap-0.0.2/hyswap/percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21034 2023-07-10 19:02:36.000000 hyswap-0.0.2/hyswap/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-07-10 19:02:36.000000 hyswap-0.0.2/hyswap/rasterhydrograph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19910 2023-07-10 19:02:36.000000 hyswap-0.0.2/hyswap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:03:10.841017 hyswap-0.0.2/hyswap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-10 19:03:10.000000 hyswap-0.0.2/hyswap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-10 19:03:10.000000 hyswap-0.0.2/hyswap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:03:10.000000 hyswap-0.0.2/hyswap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 19:03:10.000000 hyswap-0.0.2/hyswap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 19:03:10.000000 hyswap-0.0.2/hyswap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-10 19:02:36.000000 hyswap-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 19:02:36.000000 hyswap-0.0.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 19:02:36.000000 hyswap-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 19:03:10.841017 hyswap-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 19:02:36.000000 hyswap-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:03:10.841017 hyswap-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-10 19:02:36.000000 hyswap-0.0.2/tests/test_cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-10 19:02:36.000000 hyswap-0.0.2/tests/test_exceedance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-07-10 19:02:36.000000 hyswap-0.0.2/tests/test_percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-07-10 19:02:36.000000 hyswap-0.0.2/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-07-10 19:02:36.000000 hyswap-0.0.2/tests/test_rasterhydrograph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-07-10 19:02:36.000000 hyswap-0.0.2/tests/test_utils.py
```

### Comparing `hyswap-0.0.1/.github/workflows/build.yml` & `hyswap-0.0.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.1/.github/workflows/docs.yml` & `hyswap-0.0.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.1/.github/workflows/pypi.yml` & `hyswap-0.0.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.1/.gitignore` & `hyswap-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.1/.gitlab-ci.yml` & `hyswap-0.0.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.1/CONTRIBUTING.md` & `hyswap-0.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.1/DISCLAIMER.md` & `hyswap-0.0.2/DISCLAIMER.md`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.1/LICENSE.md` & `hyswap-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.1/PKG-INFO` & `hyswap-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyswap
-Version: 0.0.1
+Version: 0.0.2
 Summary: Analysis of surface water data.
 Author-email: USGS <comptools@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, this project is in the public domain in the United States because it contains materials that originally came from the United States Geological Survey, an agency of the United States Department of Interior.
         For more information, see the official USGS copyright policy at https://www.usgs.gov/information-policies-and-instructions/copyrights-and-credits.
@@ -39,15 +39,15 @@
 
 # hyswap - HYdrologic Surface Water Analysis Package
 
 [![USGS-category-image](https://img.shields.io/badge/USGS-Core-green.svg)](https://owi.usgs.gov/R/packages.html#core)
 [![pipeline-status-image](https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap/badges/main/pipeline.svg)](https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap/-/commits/main)
 [![coverage-report-image](https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap/badges/main/coverage.svg)](https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap/-/commits/main)
 [![PyPI version](https://badge.fury.io/py/hyswap.svg)](https://badge.fury.io/py/hyswap)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hyswap)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hyswap)](https://img.shields.io/pypi/pyversions/hyswap)
 
 ## Overview
 
 `hyswap` (HYdrologic Surface Water Analysis Package), is a Python package which provides a set of functions for manipulating and visualizing USGS water data.
 Specifically, a number of functions for calculating statistics (e.g., exceedance probabilities, daily historic percentiles) and generating related plots (e.g., flow duration curves, streamflow duration hydrographs) are available.
 These methods are provided in a modular fashion as individual functions, and are designed to give the user flexibility in implementation.
```

### Comparing `hyswap-0.0.1/README.md` & `hyswap-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # hyswap - HYdrologic Surface Water Analysis Package
 
 [![USGS-category-image](https://img.shields.io/badge/USGS-Core-green.svg)](https://owi.usgs.gov/R/packages.html#core)
 [![pipeline-status-image](https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap/badges/main/pipeline.svg)](https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap/-/commits/main)
 [![coverage-report-image](https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap/badges/main/coverage.svg)](https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap/-/commits/main)
 [![PyPI version](https://badge.fury.io/py/hyswap.svg)](https://badge.fury.io/py/hyswap)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hyswap)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hyswap)](https://img.shields.io/pypi/pyversions/hyswap)
 
 ## Overview
 
 `hyswap` (HYdrologic Surface Water Analysis Package), is a Python package which provides a set of functions for manipulating and visualizing USGS water data.
 Specifically, a number of functions for calculating statistics (e.g., exceedance probabilities, daily historic percentiles) and generating related plots (e.g., flow duration curves, streamflow duration hydrographs) are available.
 These methods are provided in a modular fashion as individual functions, and are designed to give the user flexibility in implementation.
```

### Comparing `hyswap-0.0.1/code.json` & `hyswap-0.0.2/code.json`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.1/docs/Makefile` & `hyswap-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.1/docs/source/conf.py` & `hyswap-0.0.2/docs/source/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -129,15 +129,19 @@
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
 # -- Options for linkcheck -------------------------------------------
 
 # Links to not "check" because they are problematic for the link checker
+# typically DOI links don't work
 linkcheck_ignore = [
-    r'https://doi.org/10.3133/wsp1542A'
+    r'https://doi.org/10.3133/wsp1542A',
+    r'https://doi.org/10.1029/2022WR031930',
+    r'https://pypi.org/project/hyswap/'
 ]
 
 linkcheck_exclude_documents = [
     r'meta/disclaimer*',
-    r'meta/contributing*'
+    r'meta/contributing*',
+    r'meta/installation*'
 ]
```

### Comparing `hyswap-0.0.1/docs/source/examples/cumulative_hydrograph_examples.rst` & `hyswap-0.0.2/docs/source/examples/cumulative_hydrograph_examples.rst`

 * *Files 12% similar despite different names*

```diff
@@ -118,14 +118,41 @@
     fig, ax = plt.subplots(figsize=(8, 5))
     ax = hyswap.plots.plot_cumulative_hydrograph(
         cdf, 2020, max_pct=True, min_pct=True,
         ax=ax, title='Cumulative Streamflow Hydrograph')
     plt.show()
 
 
+Visualizing Multiple Years of Data
+**********************************
+
+We are not limited to explicitly visualizing the cumulative streamflow from individual years.
+We can supply multiple `target_years` as a list, and each will be plotted as an individual cumulative discharge line with an associated label in the legend.
+Below is an example of this functionality wherein we plot the cumulative discharge for years 2010, 2015, and 2020.
+
+.. plot::
+    :context: reset
+    :include-source:
+
+    # get some data from the NWIS service
+    df, md = dataretrieval.nwis.get_dv(
+        '06803495', start='2000-01-01', end='2020-12-31')
+
+    # calculate the cumulative streamflow values per year
+    cdf = hyswap.cumulative.calculate_daily_cumulative_values(
+        df, '00060_Mean')
+
+    # plot the cumulative streamflow hydrograph
+    fig, ax = plt.subplots(figsize=(8, 5))
+    ax = hyswap.plots.plot_cumulative_hydrograph(
+        cdf, target_years=[2010, 2015, 2020],
+        ax=ax, title='Cumulative Streamflow Hydrograph')
+    plt.show()
+
+
 Customizing the Filled Envelope
 *******************************
 
 We can customize both the percentile thresholds between which a shaded area is plotted, as well as the color and transparency of the shaded area.
 The percentile thresholds used as the upper and lower-bound of the shaded area can be specified using the `envelope_pct` argument.
 The color and transparency, as well as other properties, of the filled region can be customized by passing keyword arguments to the :obj:`hyswap.plots.plot_cumulative_hydrograph` function, as those arguments are passed to the :meth:`matplotlib.axes.Axes.fill_between` function.
 We provide an example of doing this by filling between the 10th and 90th percentiles, and making the filled region red and semi-transparent.
```

### Comparing `hyswap-0.0.1/docs/source/examples/flow_duration_curve_examples.rst` & `hyswap-0.0.2/docs/source/examples/flow_duration_curve_examples.rst`

 * *Files 17% similar despite different names*

```diff
@@ -92,19 +92,64 @@
         # plot flow duration curve for this site
         ax = hyswap.plots.plot_flow_duration_curve(
             values, exp, ax=ax, label=f"USGS Site {site}"
         )
 
     # visualize the plot
     ax.set_title("Multiple USGS Flow Duration Curves")
+    ax.set_ylim(0.1, 1000)
     ax.legend(loc='best')
     plt.tight_layout()
     plt.show()
 
 
+Plotting Observations On Top of the Flow Duration Curve
+*******************************************************
+
+In this example we will plot the flow duration curve with the actual flow observations overlaid on top of the line.
+We will do this by utilizing the `observations` and `observation_probability` arguments.
+To make it obvious which points are observations, we will define them as small black circles by using the `scatter_kwargs` argument which allows us to pass keyword arguments through to the underlying :meth:`matplotlib.axes.Axes.scatter` function which is used to plot the observations.
+
+.. plot::
+    :context: reset
+    :include-source:
+
+    # get data from a single site
+    siteno = '06216900'
+    df, md = dataretrieval.nwis.get_dv(site=siteno, parameterCd='00060',
+                                    startDT='1900-01-01')
+    # filter to only approved data
+    df = hyswap.utils.filter_approved_data(df, '00060_Mean_cd')
+
+    # generate 10,000 evenly spaced values between the min and max
+    values = np.linspace(df['00060_Mean'].min(), df['00060_Mean'].max(), 10000)
+
+    # calculate exceedance probabilities
+    exceedance_probabilities = hyswap.exceedance.calculate_exceedance_probability_from_values_multiple(
+        values, df['00060_Mean'])
+
+    # calculate exceedance probabilities for the observations
+    obs_probs = hyswap.exceedance.calculate_exceedance_probability_from_values_multiple(
+        df['00060_Mean'], df['00060_Mean'])
+
+    # plot
+    fig, ax = plt.subplots(figsize=(8, 5))
+    # plot the flow duration curve
+    ax = hyswap.plots.plot_flow_duration_curve(
+        values, exceedance_probabilities, ax=ax,
+        observations=df['00060_Mean'],
+        observation_probabilities=obs_probs,
+        scatter_kwargs={'c': 'k', 's': 10, 'zorder': 10},
+        title=f'Flow Duration Curve for USGS Site {siteno}')
+
+    # show the plot
+    plt.tight_layout()
+    plt.show()
+
+
 Customizing Flow Duration Curve Plots
 *************************************
 
 In this example we will generate a synthetic set of exceedance probabilities from a statistical distribution to demonstrate how one can pass `**kwargs` to the :obj:`hyswap.plots.plot_flow_duration_curve` which are passed through to the underlying :meth:`matplotlib.axes.Axes.plot` and can be used to customize the line that is plotted.
 
 .. plot::
     :context: reset
```

### Comparing `hyswap-0.0.1/docs/source/examples/index.rst` & `hyswap-0.0.2/docs/source/examples/index.rst`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.1/docs/source/examples/raster_hydrograph_examples.rst` & `hyswap-0.0.2/docs/source/examples/raster_hydrograph_examples.rst`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.1/docs/source/examples/streamflow_duration_hydrograph_examples.rst` & `hyswap-0.0.2/docs/source/examples/streamflow_duration_hydrograph_examples.rst`

 * *Files 17% similar despite different names*

```diff
@@ -225,14 +225,85 @@
         title="Percentiles of Streamflow by Day of Year - Site 03586500",
         colors=['r', 'm', 'c', 'b']
     )
     plt.tight_layout()
     plt.show()
 
 
+Rolling Averages for Historic Daily Percentile Calculations
+***********************************************************
+
+In this example, rather than calculating historic daily percentile values based solely on the past values from that day of the year, we will calculate the historic daily percentile values based on rolling averages of the past values around that day.
+Under the hood this uses the :meth:`pandas.DataFrame.rolling` method to calculate the rolling average, with the default parameters.
+To show the effect of this, we will plot the historic daily percentile values for the daily (default) rolling average, 7-day rolling average, and the 28-day rolling average.
+
+.. plot::
+    :context: reset
+    :include-source:
+
+    # fetch historic data from NWIS
+    df, _ = dataretrieval.nwis.get_dv("03586500",
+                                        parameterCd="00060",
+                                        start="1776-01-01",
+                                        end="2022-12-31")
+
+    # calculate specific historic daily percentile thresholds for water years
+    percentiles_by_day = hyswap.percentiles.calculate_variable_percentile_thresholds_by_day(
+        df, "00060_Mean", data_type='daily', year_type="water"
+    )
+    percentiles_by_7day = hyswap.percentiles.calculate_variable_percentile_thresholds_by_day(
+        df, "00060_Mean", data_type='7-day', year_type="water"
+    )
+    percentiles_by_28day = hyswap.percentiles.calculate_variable_percentile_thresholds_by_day(
+        df, "00060_Mean", data_type='28-day', year_type="water"
+    )
+
+    # plotting percentiles by day with line shade between
+    fig, ax = plt.subplots(3, 1, figsize=(10, 18), sharex=True)
+    # filter down to data from 2022
+    df_year = df[df['index_year'] == 2022]
+    # plot daily percentiles
+    hyswap.plots.plot_duration_hydrograph(
+        percentiles_by_day,
+        df_year,
+        "00060_Mean",
+        "index_doy",
+        ax=ax[0],
+        data_label="Water Year 2022",
+        title="Percentiles of Streamflow by Day of Year - Site 03586500",
+        xlab="",
+        ylab="1-day Streamflow"
+    )
+    # plot 7-day percentiles
+    hyswap.plots.plot_duration_hydrograph(
+        percentiles_by_7day,
+        hyswap.utils.rolling_average(df_year, "00060_Mean", "7D"),
+        "00060_Mean",
+        "index_doy",
+        ax=ax[1],
+        data_label="Water Year 2022",
+        title="Percentiles of Streamflow by Day of Year (7-day rolling average) - Site 03586500",
+        xlab="",
+        ylab="7-day Streamflow"
+    )
+    # plot 28-day percentiles
+    hyswap.plots.plot_duration_hydrograph(
+        percentiles_by_28day,
+        hyswap.utils.rolling_average(df_year, "00060_Mean", "28D"),
+        "00060_Mean",
+        "index_doy",
+        ax=ax[2],
+        data_label="Water Year 2022",
+        title="Percentiles of Streamflow by Day of Year (28-day rolling average) - Site 03586500",
+        ylab="28-day Streamflow"
+    )
+    plt.tight_layout()
+    plt.show()
+
+
 Customizing Fill Areas
 **********************
 
 In this example we will customize the fill areas between the percentile thresholds by passing keyword arguments to the :obj:`hyswap.plots.plot_duration_hydrograph` function that are then passed through to the :meth:`matplotlib.axes.Axes.fill_between` function.
 Specifically we will set the `alpha` argument to 1.0 to make the fill areas opaque (the default value is 0.5 for some transparency).
 
 .. plot::
```

### Comparing `hyswap-0.0.1/docs/source/index.rst` & `hyswap-0.0.2/docs/source/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 .. toctree::
    :maxdepth: 1
 
    meta/installation
    examples/index
    meta/contributing
    meta/disclaimer
+   meta/glossary
    reference/index
```

### Comparing `hyswap-0.0.1/docs/source/meta/installation.rst` & `hyswap-0.0.2/docs/source/meta/installation.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,80 @@
 Installation
 ============
 
-All installation of the ``hyswap`` package must, at this time, be done
-**from source**. Here we provide instructions on how to do this, including
-both a "user" installation with minimal dependencies, as well as a "developer"
-installation that is "editable" and contains all of the dependencies needed
-to run the tests and build the package documentation.
+Installation instructions for the ``hyswap`` package are provided below.
+We provide instructions on recommended "user" installations with minimal dependencies, as well as how to install the package as a "developer" such that it is is "editable" and contains all of the dependencies needed to run the tests and build the package documentation.
 
 
 User Installation
 -----------------
 
-Below are the commands to install the ``hyswap`` package from source
-as a user. This installation will be static, and reflect the version of the
-package as it was at the time the code was downloaded.
+Below are two recommended installation methods for users of the ``hyswap`` package.
+
+
+Installation via ``pip``
+^^^^^^^^^^^^^^^^^^^^^^^^
+
+``hyswap`` is hosted on `pypi <https://pypi.org/project/hyswap/>`_ and can therefore be installed using ``pip``.
+This can be done with the following command:
+
+.. code-block:: bash
+
+    pip install hyswap
+
+It is possible to specify the specific version of the package you'd like to install with a command like:
+
+.. code-block:: bash
+
+    pip install hyswap==0.0.1
+
+
+Installation from source
+^^^^^^^^^^^^^^^^^^^^^^^^
+
+Below are the commands to install the ``hyswap`` package from source as a user.
+This installation will be static, and reflect the version of the package as it was at the time the code was downloaded.
 
 .. code-block:: bash
 
     git clone https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap.git
     cd hyswap
     pip install -r requirements.txt
     pip install .
 
 
 Developer Installation
 ----------------------
 
-Below are the commands to install the ``hyswap`` package from source
-as a developer. This installation will be "editable", meaning that any
-changes made to the source code will be reflected in the installed package
-without the need to reinstall. This installation will also contain all of the
-dependencies needed to run the tests and build the documentation.
+Below are the commands to install the ``hyswap`` package from source as a developer.
+This installation will be "editable", meaning that any changes made to the source code will be reflected in the installed package without the need to reinstall.
+This installation will also contain all of the dependencies needed to run the tests and build the documentation.
 
 .. code-block:: bash
 
     git clone https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap.git
     cd hyswap
     pip install -r requirements-dev.txt
     pip install -e .
 
-Once the installation is complete, the suite of tests can be run with a single
-command in the console:
+Once the installation is complete, the suite of unit tests can be run with a single command in the console:
 
 .. code-block:: bash
 
     pytest
 
 The documentation can be built and tested locally with the following commands:
 
 .. code-block:: bash
 
     cd docs
     make docs
 
 
-For a faster local documentation build you can skip running the documentation
-tests by running ``make html`` instead of ``make docs``.
+For a faster local documentation build you can skip running the documentation tests by running ``make html`` instead of ``make docs``.
 
-To run the linting and formatting checks locally, run the following commands
-from the root of the repository:
+To run the linting and formatting checks locally, run the following commands from the root of the repository:
 
 .. code-block:: bash
 
     flake8 .
     pydocstringformatter .
```

### Comparing `hyswap-0.0.1/docs/source/reference/hyswap.png` & `hyswap-0.0.2/docs/source/reference/hyswap.png`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.1/docs/source/reference/index.rst` & `hyswap-0.0.2/docs/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.1/hyswap/cumulative.py` & `hyswap-0.0.2/hyswap/cumulative.py`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.1/hyswap/exceedance.py` & `hyswap-0.0.2/hyswap/exceedance.py`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.1/hyswap/percentiles.py` & `hyswap-0.0.2/hyswap/percentiles.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Percentile calculation functions."""
 
 import numpy as np
 import pandas as pd
 from hyswap.utils import filter_data_by_time
 from hyswap.utils import calculate_metadata
 from hyswap.utils import define_year_doy_columns
+from hyswap.utils import set_data_type
+from hyswap.utils import rolling_average
 
 
 def calculate_fixed_percentile_thresholds(
         data,
         percentiles=np.array((0, 5, 10, 25, 75, 90, 95, 100)),
         method='weibull',
         **kwargs):
@@ -60,14 +62,15 @@
 
 def calculate_variable_percentile_thresholds_by_day(
         df,
         data_column_name,
         percentiles=[0, 5, 10, 25, 75, 90, 95, 100],
         method='weibull',
         date_column_name=None,
+        data_type='daily',
         year_type='calendar',
         min_years=10,
         **kwargs):
     """Calculate variable percentile thresholds of data by day of year.
 
     Parameters
     ----------
@@ -84,14 +87,21 @@
     method : str, optional
         Method to use to calculate percentiles. Default is 'weibull'.
 
     date_column_name : str, optional
         Name of column containing date information. If None, the index of
         `df` is used.
 
+    data_type : str, optional
+        The type of data. Must be one of 'daily', '7-day', '14-day', and
+        '28-day'. Default is 'daily'. If '7-day', '14-day', or '28-day' is
+        specified, the data will be averaged over the specified period. NaN
+        values will be used for any days that do not have data. If present,
+        NaN values will result in NaN values for the entire period.
+
     year_type : str, optional
         The type of year to use. Must be one of 'calendar', 'water', or
         'climate'. Default is 'calendar' which starts the year on January 1
         and ends on December 31. 'water' starts the year on October 1 and
         ends on September 30 of the following year which is the "water year".
         For example, October 1, 2010 to September 30, 2011 is "water year
         2011". 'climate' years begin on April 1 and end on March 31 of the
@@ -128,14 +138,17 @@
         >>> len(results.columns)  # 8 default percentiles
         8
     """
     # define year and day of year columns and convert date column to datetime
     # if necessary
     df = define_year_doy_columns(df, date_column_name=date_column_name,
                                  year_type=year_type, clip_leap_day=True)
+    # do rolling average for time as needed
+    data_type = set_data_type(data_type)
+    df = rolling_average(df, data_column_name, data_type)
     # based on date, get min and max day of year available
     min_day = np.nanmax((1, df.index.dayofyear.min()))
     max_day = np.nanmin((366, df.index.dayofyear.max() + 1))
     # make temporal index
     t_idx = np.arange(min_day, max_day)
     # initialize a DataFrame to hold percentiles by day of year
     percentiles_by_day = pd.DataFrame(index=t_idx, columns=percentiles)
```

### Comparing `hyswap-0.0.1/hyswap/plots.py` & `hyswap-0.0.2/hyswap/plots.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,40 +3,54 @@
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
 from hyswap.percentiles import calculate_variable_percentile_thresholds_by_day
 
 
 def plot_flow_duration_curve(
-        values, exceedance_probabilities, ax=None, title='Flow Duration Curve',
+        values, exceedance_probabilities,
+        observations=None, observation_probabilities=None,
+        ax=None, title='Flow Duration Curve',
         xlab='Exceedance Probability\n' +
-        '(Percent of Time Indicated Discharge was Equaled or Exceeded)',
-        ylab='Discharge, ft$^3$/s', grid=True, **kwargs):
+        '(Percentage of time indicated value was equaled or exceeded)',
+        ylab='Discharge, in Cubic Feet per Second', grid=True,
+        scatter_kwargs={}, **kwargs):
     """
     Make flow duration curve plot.
 
     Parameters
     ----------
     values : array-like
         Values to plot along y-axis.
     exceedance_probabilities : array-like
         Exceedance probabilities for each value, likely calculated from
         a function like :obj:`hyswap.exceedance.calculate_exceedance_probability_from_values_multiple`.
+    observations : list, numpy.ndarray, optional
+        List, numpy array or list-able set of flow observations. Optional, if
+        not provided the observations are not plotted.
+    observation_probabilities : list, numpy.ndarray, optional
+        Exceedance probabilities corresponding to each observation, likely
+        calculated from a function like
+        :obj:`hyswap.exceedance.calculate_exceedance_probability_from_values_multiple`.
+        Optional, if not provided observations are not plotted.
     ax : matplotlib.axes.Axes, optional
         Axes to plot on. If not provided, a new figure and axes will be
         created.
     title : str, optional
         Title for the plot. If not provided, the default title will be
         'Flow Duration Curve'.
     xlab : str, optional
         Label for the x-axis. If not provided, a default label will be used.
     ylab : str, optional
         Label for the y-axis. If not provided, a default label will be used.
     grid : bool, optional
         Whether to show grid lines on the plot. Default is True.
+    scatter_kwargs : dict
+        Dictionary containing keyword arguments to pass to the observations
+        plotting method, :meth:`matplotlib.axes.Axes.scatter`.
     **kwargs
         Keyword arguments passed to :meth:`matplotlib.axes.Axes.plot`.
 
     Returns
     -------
     matplotlib.axes.Axes
         Axes object containing the plot.
@@ -64,41 +78,56 @@
         >>> plt.show()
     """
     # Create axes if not provided
     if ax is None:
         _, ax = plt.subplots()
     # do plotting
     ax.plot(exceedance_probabilities*100, values, **kwargs)
+    if (observations is not None) and (observation_probabilities is not None):
+        ax.scatter(np.array(observation_probabilities)*100, observations,
+                   **scatter_kwargs)
     ax.set_xlabel(xlab)
     ax.set_ylabel(ylab)
     ax.set_title(title)
     # set log scales for x axis
     ax.set_yscale('log')
     # set limits for axes
     ax.set_xlim(0.1, 99.9)
     # set ticks for axes
     # always use same ticks for x-axis
     ax.set_xticks([0.1, 5, 10, 25, 50, 75, 90, 95, 99.9])
     ax.set_xticklabels([
         '0.1', '5', '10', '25', '50', '75', '90', '95', '99.9'])
     # get y-axis ticks and convert to comma-separated strings
     yticks = ax.get_yticks()
+    # min value is 0.1
+    # yticks = np.array([i for i in yticks if i >= 0.1])
+    # get logs for min/max values rounded to next lowest/highest
+    min_vals = np.log10(yticks[yticks <= np.min(values)])
+    if len(min_vals) > 0:
+        min_tick = min_vals[-1]
+    else:
+        min_tick = -1.0
+    max_tick = np.log10(yticks[yticks >= np.max(values)][0])
+    # set list of values using logs
+    yticks = list(10**np.arange(min_tick, max_tick+1))
     yticklabels = [f'{int(y):,}' for y in yticks]
     ax.set_yticks(yticks, labels=yticklabels)
+    ax.set_ylim(np.min(yticks), np.max(yticks))
     # add grid lines
     if grid:
         ax.grid(which='both', axis='both', alpha=0.5)
     # return the axes
     return ax
 
 
 def plot_raster_hydrograph(df_formatted, ax=None,
-                           title='Streamflow Raster Hydrograph',
+                           title='Raster Hydrograph',
                            xlab='Month', ylab='Year',
-                           cbarlab='Streamflow, cubic feet per second',
+                           cbarlab='Discharge, in Cubic Feet per Second',
                            **kwargs):
     """Make raster hydrograph plot.
 
     Parameters
     ----------
     df_formatted : pandas.DataFrame
         Formatted dataframe containing the raster hydrograph data.
@@ -112,15 +141,15 @@
         Label for the x-axis. If not provided, the default label will be
         'Month'.
     ylab : str, optional
         Label for the y-axis. If not provided, the default label will be
         'Year'.
     cbarlab : str, optional
         Label for the colorbar. If not provided, the default label will be
-        'Streamflow, cubic feet per second'.
+        'Discharge, in Cubic Feet per Second'.
     **kwargs
         Keyword arguments passed to :meth:`matplotlib.axes.Axes.imshow`.
 
     Returns
     -------
     matplotlib.axes.Axes
         Axes object containing the plot.
@@ -203,16 +232,16 @@
     return ax
 
 
 def plot_duration_hydrograph(percentiles_by_day, df, data_col, doy_col,
                              pct_list=[0, 5, 10, 25, 75, 90, 95, 100],
                              data_label=None, ax=None,
                              title="Duration Hydrograph",
-                             ylab="Discharge (cfs)", xlab="Month",
-                             colors=None, **kwargs):
+                             ylab="Discharge, in Cubic Feet per Second",
+                             xlab="Month", colors=None, **kwargs):
     """Make duration hydrograph plot.
 
     Parameters
     ----------
     percentiles_by_day : pandas.DataFrame
         Dataframe containing the percentiles by day.
     df : pandas.DataFrame
@@ -231,15 +260,15 @@
         Axes to plot on. If not provided, a new figure and axes will be
         created.
     title : str, optional
         Title for the plot. If not provided, the default title will be
         'Duration Hydrograph'.
     ylab : str, optional
         Label for the y-axis. If not provided, the default label will be
-        'Discharge (cfs)'.
+        'Discharge, in Cubic Feet per Second'.
     xlab : str, optional
         Label for the x-axis. If not provided, the default label will be
         'Month'.
     colors : list, optional
         List of colors to use for the lines. If not provided, a default
         list of colors will be used.
     **kwargs
@@ -331,31 +360,32 @@
     ax.set_yticks(yticks[1:-1], labels=yticklabels[1:-1])
     # two column legend
     ax.legend(loc="best", ncol=2)
     # return axes
     return ax
 
 
-def plot_cumulative_hydrograph(cumulative_percentiles, target_year,
+def plot_cumulative_hydrograph(cumulative_percentiles, target_years,
                                year_type='calendar',
                                envelope_pct=[25, 75],
                                max_pct=False, min_pct=False,
                                ax=None,
-                               title="Cumulative Discharge",
-                               ylab="Cumulative Discharge (cfs)",
+                               title="Cumulative Streamflow Hydrograph",
+                               ylab="Cumulative Streamflow, in Cubic Feet",
                                xlab="Month", **kwargs):
     """Make cumulative hydrograph plot.
 
     Parameters
     ----------
     cumulative_percentiles : pandas.DataFrame
         Dataframe containing the cumulative percentiles per year, output
         from :obj:`hyswap.cumulative.calculate_daily_cumulative_values`.
-    target_year : int
-        Target year to plot in black as the line.
+    target_years : int, or list
+        Target year(s) to plot in black as the line. Can provide a single year
+        as an integer, or a list of years.
     year_type : str, optional
         The type of year to use. Must be one of 'calendar', 'water', or
         'climate'. Default is 'calendar' which starts the year on January 1
         and ends on December 31. 'water' starts the year on October 1 and
         ends on September 30 of the following year which is the "water year".
         For example, October 1, 2010 to September 30, 2011 is "water year
         2011". 'climate' years begin on April 1 and end on March 31 of the
@@ -368,18 +398,18 @@
     min_pct : bool, optional
         If True, plot the minimum value as a dotted line. Default is False.
     ax : matplotlib.axes.Axes, optional
         Axes to plot on. If not provided, a new figure and axes will be
         created.
     title : str, optional
         Title for the plot. If not provided, the default title will be
-        'Cumulative Discharge'.
+        'Cumulative Streamflow Hydrograph'.
     ylab : str, optional
         Label for the y-axis. If not provided, the default label will be
-        'Cumulative Discharge (cfs)'.
+        'Cumulative Streamflow, in Cubic Feet'.
     xlab : str, optional
         Label for the x-axis. If not provided, the default label will be
         'Month'.
     **kwargs
         Keyword arguments passed to :meth:`matplotlib.axes.Axes.fill_between`.
 
     Returns
@@ -430,20 +460,26 @@
     # plot min/max if desired
     if min_pct:
         ax.plot(pdf.index.get_level_values(1), pdf[0], color='k',
                 alpha=0.5, linestyle=':', label="Minimum")
     if max_pct:
         ax.plot(pdf.index.get_level_values(1), pdf[100], color='k',
                 alpha=0.5, linestyle='--', label="Maximum")
-    # get data from target year
-    target_year_data = cumulative_percentiles.loc[
-        cumulative_percentiles['index_year'] == target_year]
-    # plot target year
-    ax.plot(target_year_data['index_doy'], target_year_data['cumulative'],
-            color='k', label=f"{target_year} Cumulative Discharge")
+    # handle target years
+    col_targets = ['k'] + list(matplotlib.colormaps['tab20'].colors)
+    if isinstance(target_years, int):
+        target_years = [target_years]  # make int a list
+    for i, target_year in enumerate(target_years):
+        # get data from target year
+        target_year_data = cumulative_percentiles.loc[
+            cumulative_percentiles['index_year'] == target_year]
+        # plot target year
+        ax.plot(target_year_data['index_doy'], target_year_data['cumulative'],
+                color=col_targets[i],
+                label=f"{target_year} Observed")
 
     # set labels
     ax.set_xlabel(xlab)
     ax.set_xlim(0, 365)
     # major xticks at first/end of each month
     months = [int(m.split('-')[0]) for m in pdf.index.get_level_values(1).to_list()]  # noqa: E501
     month_switch = np.where(np.diff(months) != 0)[0]
@@ -460,13 +496,14 @@
     ax.tick_params(axis='x', which='minor', length=0)
     # other labels
     ax.set_ylabel(ylab)
     ax.set_title(title)
     # get y-axis ticks and convert to comma-separated strings
     yticks = ax.get_yticks()
     yticklabels = [f'{int(y):,}' for y in yticks]
-    ax.set_yticks(yticks[1:-1], labels=yticklabels[1:-1])
+    ax.set_yticks(yticks[1:], labels=yticklabels[1:])
+    ax.set_ylim(0, yticks.max())
     # two column legend
     ax.legend(loc="best")
 
     # return
     return ax
```

### Comparing `hyswap-0.0.1/hyswap/rasterhydrograph.py` & `hyswap-0.0.2/hyswap/rasterhydrograph.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Raster hydrograph functionality."""
 
 import pandas as pd
 from hyswap.utils import rolling_average
 from hyswap.utils import define_year_doy_columns
+from hyswap.utils import set_data_type
 
 
 def format_data(df, data_column_name, date_column_name=None,
                 data_type='daily', year_type='calendar',
                 begin_year=None, end_year=None, **kwargs):
     """
     Format data for raster hydrograph.
@@ -87,15 +88,15 @@
     # calculate the date range
     date_range = _calculate_date_range(df, year_type, begin_year, end_year)
 
     # format date_range as YYYY-MM-DD
     date_range = date_range.strftime('%Y-%m-%d')
 
     # set data type
-    data_type = _set_data_type(data_type)
+    data_type = set_data_type(data_type)
 
     # make output data frame
     # calculation of rolling mean is done on the data column
     df_out = rolling_average(df, data_column_name, data_type, **kwargs)
 
     # convert date index to YYYY-MM-DD format
     df_out.index = df_out.index.strftime('%Y-%m-%d')
@@ -269,38 +270,7 @@
         begin_date = pd.to_datetime(str(begin_year-1) + '-04-01')
         end_date = pd.to_datetime(str(end_year) + '-03-31')
 
     # set date range
     date_range = pd.date_range(begin_date, end_date)
 
     return date_range
-
-
-def _set_data_type(data_type):
-    """Private function to set the data type.
-
-    Parameters
-    ----------
-    data_type : str
-        The type of data. Must be one of 'daily', '7-day', '14-day', and
-        '28-day'. If '7-day', '14-day', or '28-day' is
-        specified, the data will be averaged over the specified period. NaN
-        values will be used for any days that do not have data. If present,
-        NaN values will result in NaN values for the entire period.
-
-    Returns
-    -------
-    data_type : str
-        The formatted frequency string to be used with
-        pandas.DataFrame.rolling to calculate the average over the correct
-        temporal period.
-    """
-    if data_type == 'daily':
-        data_type = 'D'
-    elif data_type == '7-day':
-        data_type = '7D'
-    elif data_type == '14-day':
-        data_type = '14D'
-    elif data_type == '28-day':
-        data_type = '28D'
-
-    return data_type
```

### Comparing `hyswap-0.0.1/hyswap/utils.py` & `hyswap-0.0.2/hyswap/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -426,7 +426,111 @@
         [doy_index, month_day], names=['doy', 'month-day'])
     # slim down to just the columns used for the plot
     df_slim = df[source_pct_col]
     # rename columns
     df_slim.columns = target_pct_col
     # return the dataframe
     return df_slim
+
+
+def calculate_summary_statistics(df, data_col="00060_Mean"):
+    """
+    Calculate summary statistics for a site.
+
+    Parameters
+    ----------
+    df : pandas.DataFrame
+        DataFrame containing daily values for the site. Expected to be from
+        `dataretrieval.nwis.get_dv()`, or similar.
+
+    data_col : str, optional
+        Name of the column in the dv_df DataFrame that contains the data of
+        interest. Default is "00060_Mean" which is the mean daily discharge
+        column.
+
+    Returns
+    -------
+    summary_df : pandas.DataFrame
+        DataFrame containing summary statistics for the site.
+
+    Examples
+    --------
+    Get some NWIS data and apply the function to get the summary statistics.
+
+    .. doctest::
+
+        >>> df, _ = dataretrieval.nwis.get_dv(
+        ...     "03586500", parameterCd="00060",
+        ...     startDT="2010-01-01", endDT="2010-12-31")
+        >>> summary_df = utils.calculate_summary_statistics(df)
+        >>> summary_df.shape
+        (8, 1)
+        >>> print(summary_df)
+                    Summary Statistics
+        Site number           03586500
+        Begin date          2010-01-01
+        End date            2010-12-31
+        Count                      365
+        Minimum                   2.48
+        Mean                    207.43
+        Median                    82.5
+        Maximum                 3710.0
+    """
+    # make dictionary
+    summary_dict = {}
+    # populate it
+    # site number
+    summary_dict['Site number'] = str(int(df['site_no'][0])).zfill(8)
+    # dates
+    summary_dict['Begin date'] = df.index.min().strftime('%Y-%m-%d')
+    summary_dict['End date'] = df.index.max().strftime('%Y-%m-%d')
+    # count
+    summary_dict['Count'] = df[data_col].count()
+    # minimum
+    summary_dict['Minimum'] = df[data_col].min()
+    # mean
+    summary_dict['Mean'] = df[data_col].mean().round(2)
+    # median
+    summary_dict['Median'] = df[data_col].median()
+    # maximum
+    summary_dict['Maximum'] = df[data_col].max()
+
+    # make dataframe
+    summary_df = pd.DataFrame(summary_dict, index=[0])
+
+    # transpose and set column name
+    summary_df = summary_df.T
+    summary_df.columns = ['Summary Statistics']
+
+    # return dataframe
+    return summary_df
+
+
+def set_data_type(data_type):
+    """Function to set the data type for rolling averages.
+
+    Parameters
+    ----------
+    data_type : str
+        The type of data. Must be one of 'daily', '7-day', '14-day', and
+        '28-day'. If '7-day', '14-day', or '28-day' is
+        specified, the data will be averaged over the specified period. NaN
+        values will be used for any days that do not have data. If present,
+        NaN values will result in NaN values for the entire period.
+
+    Returns
+    -------
+    data_type : str
+        The formatted frequency string to be used with
+        pandas.DataFrame.rolling to calculate the average over the correct
+        temporal period.
+    """
+    if data_type == 'daily':
+        data_type = 'D'
+    elif data_type == '7-day':
+        data_type = '7D'
+    elif data_type == '14-day':
+        data_type = '14D'
+    elif data_type == '28-day':
+        data_type = '28D'
+
+    return data_type
```

### Comparing `hyswap-0.0.1/hyswap.egg-info/PKG-INFO` & `hyswap-0.0.2/hyswap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyswap
-Version: 0.0.1
+Version: 0.0.2
 Summary: Analysis of surface water data.
 Author-email: USGS <comptools@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, this project is in the public domain in the United States because it contains materials that originally came from the United States Geological Survey, an agency of the United States Department of Interior.
         For more information, see the official USGS copyright policy at https://www.usgs.gov/information-policies-and-instructions/copyrights-and-credits.
@@ -39,15 +39,15 @@
 
 # hyswap - HYdrologic Surface Water Analysis Package
 
 [![USGS-category-image](https://img.shields.io/badge/USGS-Core-green.svg)](https://owi.usgs.gov/R/packages.html#core)
 [![pipeline-status-image](https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap/badges/main/pipeline.svg)](https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap/-/commits/main)
 [![coverage-report-image](https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap/badges/main/coverage.svg)](https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap/-/commits/main)
 [![PyPI version](https://badge.fury.io/py/hyswap.svg)](https://badge.fury.io/py/hyswap)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hyswap)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hyswap)](https://img.shields.io/pypi/pyversions/hyswap)
 
 ## Overview
 
 `hyswap` (HYdrologic Surface Water Analysis Package), is a Python package which provides a set of functions for manipulating and visualizing USGS water data.
 Specifically, a number of functions for calculating statistics (e.g., exceedance probabilities, daily historic percentiles) and generating related plots (e.g., flow duration curves, streamflow duration hydrographs) are available.
 These methods are provided in a modular fashion as individual functions, and are designed to give the user flexibility in implementation.
```

### Comparing `hyswap-0.0.1/hyswap.egg-info/SOURCES.txt` & `hyswap-0.0.2/hyswap.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 docs/source/examples/cumulative_hydrograph_examples.rst
 docs/source/examples/flow_duration_curve_examples.rst
 docs/source/examples/index.rst
 docs/source/examples/raster_hydrograph_examples.rst
 docs/source/examples/streamflow_duration_hydrograph_examples.rst
 docs/source/meta/contributing.rst
 docs/source/meta/disclaimer.rst
+docs/source/meta/glossary.rst
 docs/source/meta/installation.rst
 docs/source/reference/hyswap.png
 docs/source/reference/index.rst
 hyswap/__init__.py
 hyswap/_version.py
 hyswap/cumulative.py
 hyswap/exceedance.py
```

### Comparing `hyswap-0.0.1/pyproject.toml` & `hyswap-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.1/tests/test_cumulative.py` & `hyswap-0.0.2/tests/test_cumulative.py`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.1/tests/test_exceedance.py` & `hyswap-0.0.2/tests/test_exceedance.py`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.1/tests/test_percentiles.py` & `hyswap-0.0.2/tests/test_percentiles.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,117 +1,168 @@
 """Tests for the percentiles functions."""
 import numpy as np
 import pandas as pd
 import pytest
 from hyswap import percentiles
 
 
-def test_calculate_fixed_percentile_thresholds():
-    """Test the calculate_fixed_percentile_thresholds function."""
-    # make some data
+class TestCalculateFixedPercentileThresholds:
+    # data value for all tests in this class
     data = np.arange(101)
-    # test the function
-    percentiles_ = percentiles.calculate_fixed_percentile_thresholds(
-        data, method='linear')
-    assert percentiles_.shape == (8,)
-    assert percentiles_ == pytest.approx((0, 5, 10, 25, 75, 90, 95, 100))
-    # set some percentile values as opposed to the defaults
-    percentiles_ = percentiles.calculate_fixed_percentile_thresholds(
-        data, percentiles=np.array((0, 10, 50, 90, 100)))
-    assert percentiles_.shape == (5,)
-    assert percentiles_ == pytest.approx((0, 9.2, 50, 90.8, 100))
-    # pass kwarg through to np.percentile
-    percentiles_ = percentiles.calculate_fixed_percentile_thresholds(
-        data, method='lower')
-    assert percentiles_.shape == (8,)
-    assert percentiles_ == pytest.approx((0, 5, 10, 25, 75, 90, 95, 100))
-
-
-def test_calculate_variable_percentile_thresholds_by_day():
-    """Test the calculate_variable_percentile_thresholds_by_day function."""
-    # make a dataframe
-    df = pd.DataFrame({
+
+    def test_calculate_fixed_percentile_thresholds_defaults(self):
+        """Test the calculate_fixed_percentile_thresholds function defaults."""
+        # test the function
+        percentiles_ = percentiles.calculate_fixed_percentile_thresholds(
+            self.data, method='linear')
+        assert percentiles_.shape == (8,)
+        assert percentiles_ == pytest.approx((0, 5, 10, 25, 75, 90, 95, 100))
+
+    def test_custom_percentiles(self):
+        # set some percentile values as opposed to the defaults
+        percentiles_ = percentiles.calculate_fixed_percentile_thresholds(
+            self.data, percentiles=np.array((0, 10, 50, 90, 100)))
+        assert percentiles_.shape == (5,)
+        assert percentiles_ == pytest.approx((0, 9.2, 50, 90.8, 100))
+
+    def test_kwargs_to_percentile(self):
+        # pass kwarg through to np.percentile
+        percentiles_ = percentiles.calculate_fixed_percentile_thresholds(
+            self.data, method='lower')
+        assert percentiles_.shape == (8,)
+        assert percentiles_ == pytest.approx((0, 5, 10, 25, 75, 90, 95, 100))
+
+
+class TestCalculateVariablePercentileThresholdsByDay:
+    # data for all tests in this class
+    small_df = pd.DataFrame({
         'data': np.arange(101),
         'date': pd.date_range('2019-01-01', '2019-04-11')})
-    # test the function
-    percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day(
-        df, 'data', date_column_name='date')
-    assert percentiles_.shape == (101, 8)
-    assert percentiles_.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100]
-    assert percentiles_.index.get_level_values(1).tolist()[0] == '01-01'
-    assert percentiles_.index.get_level_values(0).tolist()[0] == 1
-    # test the function with no date column and dates in the index
-    df = df.set_index('date')
-    percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day(
-        df, 'data')
-    assert percentiles_.shape == (101, 8)
-    assert percentiles_.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100]
-    assert percentiles_.index.get_level_values(1).tolist()[0] == '01-01'
-    assert percentiles_.index.get_level_values(0).tolist()[0] == 1
-    # test the function with a different set of percentiles
-    percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day(
-        df, 'data', percentiles=np.array((0, 10, 50, 90, 100)))
-    assert percentiles_.shape == (101, 5)
-    assert percentiles_.columns.tolist() == [0, 10, 50, 90, 100]
-    assert percentiles_.index.get_level_values(1).tolist()[0] == '01-01'
-    assert percentiles_.index.get_level_values(0).tolist()[0] == 1
-    # all percentiles should be NaN because demo dataset is 1 year only
-    assert percentiles_.isna().all().all()
-    # test the function with a different year type
-    percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day(
-        df, 'data', year_type='water')
-    assert percentiles_.shape == (101, 8)
-    assert percentiles_.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100]
-    assert percentiles_.index.get_level_values(1).tolist()[0] == '01-01'
-    assert percentiles_.index.get_level_values(0).tolist()[0] == 93
-    assert percentiles_.index.get_level_values(1).tolist()[-1] == '04-11'
-    assert percentiles_.index.get_level_values(0).tolist()[-1] == 193
-    # all percentiles should be NaN because demo dataset is 1 year only
-    assert percentiles_.isna().all().all()
-    # test the function with a different year type and a different set of
-    # percentiles
-    percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day(
-        df, 'data', year_type='climate',
-        percentiles=np.array((0, 10, 50, 90, 100)))
-    assert percentiles_.shape == (101, 5)
-    assert percentiles_.columns.tolist() == [0, 10, 50, 90, 100]
-    assert percentiles_.index.get_level_values(1).tolist()[0] == '04-01'
-    assert percentiles_.index.get_level_values(0).tolist()[0] == 1
-    # all percentiles should be NaN because demo dataset is 1 year only
-    assert percentiles_.isna().all().all()
-    # make a bigger dummy dataset so values are not NaN
-    df = pd.DataFrame({
+
+    bigger_df = pd.DataFrame({
         'data': np.random.random(
             len(pd.date_range('2000-01-01', '2020-12-31'))),
         'date': pd.date_range('2000-01-01', '2020-12-31')})
-    # test the function and check that the percentiles are not NaN
-    percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day(
-        df, 'data', date_column_name='date')
-    assert not percentiles_.isna().all().all()
-    # test a longer dummy set that exceeds 1 year
-    df = pd.DataFrame({
+
+    df_dummy = pd.DataFrame({
         'data': np.random.random(
             len(pd.date_range('2000-01-01', '2001-12-31'))),
         'date': pd.date_range('2000-01-01', '2001-12-31')})
-    # test the function
-    percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day(
-        df, 'data', date_column_name='date', year_type='water')
-    assert percentiles_.shape == (365, 8)
-    assert percentiles_.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100]
-    assert percentiles_.index.get_level_values(1).tolist()[0] == '10-01'
-    assert percentiles_.index.get_level_values(0).tolist()[0] == 1
-    assert percentiles_.index.get_level_values(1).tolist()[-1] == '09-30'
-    assert percentiles_.index.get_level_values(0).tolist()[-1] == 365
-    # test a longer dummy set that exceeds 1 year
-    df = pd.DataFrame({
+
+    df_dummy_alt = pd.DataFrame({
         'data': np.random.random(
             len(pd.date_range('2001-01-01', '2002-12-31'))),
         'date': pd.date_range('2001-01-01', '2002-12-31')})
-    # test the function
-    percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day(
-        df, 'data', date_column_name='date', year_type='water')
-    assert percentiles_.shape == (365, 8)
-    assert percentiles_.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100]
-    assert percentiles_.index.get_level_values(1).tolist()[0] == '10-01'
-    assert percentiles_.index.get_level_values(0).tolist()[0] == 1
-    assert percentiles_.index.get_level_values(1).tolist()[-1] == '09-30'
-    assert percentiles_.index.get_level_values(0).tolist()[-1] == 365
+
+    def test_calculate_variable_percentile_thresholds_by_day(self):
+        """Test with date column."""
+        # test the function
+        percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day( # noqa
+            self.small_df, 'data', date_column_name='date')
+        assert percentiles_.shape == (101, 8)
+        assert percentiles_.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100]
+        assert percentiles_.index.get_level_values(1).tolist()[0] == '01-01'
+        assert percentiles_.index.get_level_values(0).tolist()[0] == 1
+
+    def test_calculate_variable_percentile_thresholds_by_day_dateindex(self):
+        """Test with dates in the index."""
+        # test the function with no date column and dates in the index
+        self.small_df = self.small_df.set_index('date')
+        percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day( # noqa
+            self.small_df, 'data')
+        assert percentiles_.shape == (101, 8)
+        assert percentiles_.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100]
+        assert percentiles_.index.get_level_values(1).tolist()[0] == '01-01'
+        assert percentiles_.index.get_level_values(0).tolist()[0] == 1
+
+    def test_calculate_variable_percentile_thresholds_by_day_percentiles(self):
+        # test the function with a different set of percentiles
+        self.small_df = self.small_df.set_index('date')
+        percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day( # noqa
+            self.small_df, 'data', percentiles=np.array((0, 10, 50, 90, 100)))
+        assert percentiles_.shape == (101, 5)
+        assert percentiles_.columns.tolist() == [0, 10, 50, 90, 100]
+        assert percentiles_.index.get_level_values(1).tolist()[0] == '01-01'
+        assert percentiles_.index.get_level_values(0).tolist()[0] == 1
+        # all percentiles should be NaN because demo dataset is 1 year only
+        assert percentiles_.isna().all().all()
+
+    def test_calculate_variable_percentile_thresholds_by_day_year_type(self):
+        """Test with a different year type."""
+        # test the function with a different year type
+        self.small_df = self.small_df.set_index('date')
+        percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day( # noqa
+            self.small_df, 'data', year_type='water')
+        assert percentiles_.shape == (101, 8)
+        assert percentiles_.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100]
+        assert percentiles_.index.get_level_values(1).tolist()[0] == '01-01'
+        assert percentiles_.index.get_level_values(0).tolist()[0] == 93
+        assert percentiles_.index.get_level_values(1).tolist()[-1] == '04-11'
+        assert percentiles_.index.get_level_values(0).tolist()[-1] == 193
+        # all percentiles should be NaN because demo dataset is 1 year only
+        assert percentiles_.isna().all().all()
+
+    def test_calculate_variable_percentile_thresholds_by_day_year_type_percentiles(self): # noqa
+        # test the function with a different year type and a different set of
+        # percentiles
+        self.small_df = self.small_df.set_index('date')
+        percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day( # noqa
+            self.small_df, 'data', year_type='climate',
+            percentiles=np.array((0, 10, 50, 90, 100)))
+        assert percentiles_.shape == (101, 5)
+        assert percentiles_.columns.tolist() == [0, 10, 50, 90, 100]
+        assert percentiles_.index.get_level_values(1).tolist()[0] == '04-01'
+        assert percentiles_.index.get_level_values(0).tolist()[0] == 1
+        # all percentiles should be NaN because demo dataset is 1 year only
+        assert percentiles_.isna().all().all()
+
+    def test_non_nans(self):
+        """Test that the percentiles are not NaN."""
+        # test the function and check that the percentiles are not NaN
+        percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day( # noqa
+            self.bigger_df, 'data', date_column_name='date')
+        assert not percentiles_.isna().all().all()
+
+    def test_longer_dummy_set(self):
+        """Test with a longer dummy set."""
+        # test a longer dummy set that exceeds 1 year
+        # test the function
+        percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day( # noqa
+            self.df_dummy, 'data', date_column_name='date', year_type='water')
+        assert percentiles_.shape == (365, 8)
+        assert percentiles_.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100]
+        assert percentiles_.index.get_level_values(1).tolist()[0] == '10-01'
+        assert percentiles_.index.get_level_values(0).tolist()[0] == 1
+        assert percentiles_.index.get_level_values(1).tolist()[-1] == '09-30'
+        assert percentiles_.index.get_level_values(0).tolist()[-1] == 365
+
+    def test_longer_dummy_alt(self):
+        """Test with a different longer dummy set."""
+        # test a longer dummy set that exceeds 1 year
+        # test the function
+        percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day( # noqa
+            self.df_dummy_alt, 'data', date_column_name='date',
+            year_type='water')
+        assert percentiles_.shape == (365, 8)
+        assert percentiles_.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100]
+        assert percentiles_.index.get_level_values(1).tolist()[0] == '10-01'
+        assert percentiles_.index.get_level_values(0).tolist()[0] == 1
+        assert percentiles_.index.get_level_values(1).tolist()[-1] == '09-30'
+        assert percentiles_.index.get_level_values(0).tolist()[-1] == 365
+
+    def test_bigger_rolling_avg(self):
+        """Test rolling average."""
+        # function w/ daily percentiles
+        percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day( # noqa
+            self.bigger_df, 'data', date_column_name='date')
+        percentiles_7day = percentiles.calculate_variable_percentile_thresholds_by_day( # noqa
+            self.bigger_df, 'data', date_column_name='date',
+            data_type='7-day')
+        assert percentiles_.shape == (365, 8)
+        assert percentiles_7day.shape == (365, 8)
+        assert percentiles_.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100]
+        assert percentiles_7day.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100] # noqa
+        # check that the percentiles are not NaN
+        assert not percentiles_.isna().all().all()
+        assert not percentiles_7day.isna().all().all()
+        # check that the percentiles are not the same
+        assert not percentiles_.equals(percentiles_7day)
```

### Comparing `hyswap-0.0.1/tests/test_plots.py` & `hyswap-0.0.2/tests/test_plots.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     """Test the plot_flow_duration_curve function."""
     values = [1, 1.25, 2.5]
     exceedance_probabilities = exceedance.calculate_exceedance_probability_from_values_multiple(  # noqa: E501
         values, [1, 2, 3, 4])
     ax = plots.plot_flow_duration_curve(values, exceedance_probabilities)
     assert isinstance(ax, plt.Axes)
     assert ax.get_xlabel() == 'Exceedance Probability\n' + \
-        '(Percent of Time Indicated Discharge was Equaled or Exceeded)'
-    assert ax.get_ylabel() == 'Discharge, ft$^3$/s'
+        '(Percentage of time indicated value was equaled or exceeded)'
+    assert ax.get_ylabel() == 'Discharge, in Cubic Feet per Second'
     assert ax.get_title() == 'Flow Duration Curve'
     assert len(ax.lines) == 1
     assert len(ax.collections) == 0
     assert len(ax.patches) == 0
     assert len(ax.texts) == 0
     assert len(ax.artists) == 0
     assert len(ax.images) == 0
@@ -37,28 +37,42 @@
                                         ylab='Test Y Label')
     assert isinstance(ax, plt.Axes)
     assert ax.get_xlabel() == 'Test X Label'
     assert ax.get_ylabel() == 'Test Y Label'
     assert ax.get_title() == 'Test Title'
     assert len(ax.lines) == 1
     assert len(ax.collections) == 0
+    # make another plot with observations on it
+    ax = plots.plot_flow_duration_curve(values, exceedance_probabilities,
+                                        observations=[1, 2],
+                                        observation_probabilities=[0.5, 0.25],
+                                        title='Test Title',
+                                        xlab='Test X Label',
+                                        ylab='Test Y Label',
+                                        scatter_kwargs={'c': 'k'})
+    assert isinstance(ax, plt.Axes)
+    assert ax.get_xlabel() == 'Test X Label'
+    assert ax.get_ylabel() == 'Test Y Label'
+    assert ax.get_title() == 'Test Title'
+    assert len(ax.lines) == 1
+    assert len(ax.collections) == 1
     # close plot
     plt.close()
 
 
 def test_plot_raster_hydrograph():
     """Test the plot_raster_hydrograph function."""
     df = pd.DataFrame({'date': pd.date_range('1/1/2010', '12/31/2010'),
                        'data': np.random.rand(365)+100})
     df_formatted = rasterhydrograph.format_data(df, 'data', 'date')
     ax = plots.plot_raster_hydrograph(df_formatted)
     assert isinstance(ax, plt.Axes)
     assert ax.get_xlabel() == 'Month'
     assert ax.get_ylabel() == 'Year'
-    assert ax.get_title() == 'Streamflow Raster Hydrograph'
+    assert ax.get_title() == 'Raster Hydrograph'
     # make one with custom labels
     ax = plots.plot_raster_hydrograph(df_formatted, title='Test Title',
                                       xlab='Test X Label',
                                       ylab='Test Y Label')
     assert isinstance(ax, plt.Axes)
     assert ax.get_xlabel() == 'Test X Label'
     assert ax.get_ylabel() == 'Test Y Label'
@@ -74,15 +88,15 @@
     df.index = df['date']
     pct = percentiles.calculate_variable_percentile_thresholds_by_day(
         df, 'data')
     df['doy'] = df.index.dayofyear
     ax = plots.plot_duration_hydrograph(pct, df, 'data', 'doy')
     assert isinstance(ax, plt.Axes)
     assert ax.get_xlabel() == 'Month'
-    assert ax.get_ylabel() == 'Discharge (cfs)'
+    assert ax.get_ylabel() == 'Discharge, in Cubic Feet per Second'
     assert ax.get_title() == 'Duration Hydrograph'
     # make one with custom labels
     ax = plots.plot_duration_hydrograph(pct, df, 'data', 'doy',
                                         title='Test Title',
                                         xlab='Test X Label',
                                         ylab='Test Y Label',
                                         data_label='Test Data Label')
@@ -100,16 +114,16 @@
                        'data': np.random.rand(365)})
     df_cumulative = cumulative.calculate_daily_cumulative_values(
         df, 'data', date_column_name='date')
     # apply plot function
     ax = plots.plot_cumulative_hydrograph(df_cumulative, 2010)
     assert isinstance(ax, plt.Axes)
     assert ax.get_xlabel() == 'Month'
-    assert ax.get_ylabel() == 'Cumulative Discharge (cfs)'
-    assert ax.get_title() == 'Cumulative Discharge'
+    assert ax.get_ylabel() == 'Cumulative Streamflow, in Cubic Feet'
+    assert ax.get_title() == 'Cumulative Streamflow Hydrograph'
     assert len(ax.lines) == 1
     # make one with custom labels
     ax = plots.plot_cumulative_hydrograph(df_cumulative, 2010,
                                           title='Test Title',
                                           xlab='Test X Label',
                                           ylab='Test Y Label')
     assert isinstance(ax, plt.Axes)
@@ -118,13 +132,27 @@
     assert ax.get_title() == 'Test Title'
     assert len(ax.lines) == 1
     # make one with min/max lines plotted
     ax = plots.plot_cumulative_hydrograph(df_cumulative, 2010,
                                           max_pct=True, min_pct=True)
     assert isinstance(ax, plt.Axes)
     assert ax.get_xlabel() == 'Month'
-    assert ax.get_ylabel() == 'Cumulative Discharge (cfs)'
-    assert ax.get_title() == 'Cumulative Discharge'
+    assert ax.get_ylabel() == 'Cumulative Streamflow, in Cubic Feet'
+    assert ax.get_title() == 'Cumulative Streamflow Hydrograph'
     assert len(ax.lines) == 3
     assert len(ax.collections) == 1
+    # make one with multiple years of data plotted
+    _date = pd.date_range('1/1/2010', '12/31/2012')
+    df = pd.DataFrame({'date': _date,
+                       'data': np.random.rand(len(_date))})
+    df_cumulative = cumulative.calculate_daily_cumulative_values(
+        df, 'data', date_column_name='date')
+    ax = plots.plot_cumulative_hydrograph(df_cumulative, [2010, 2011],
+                                          max_pct=True, min_pct=True)
+    assert isinstance(ax, plt.Axes)
+    assert ax.get_xlabel() == 'Month'
+    assert ax.get_ylabel() == 'Cumulative Streamflow, in Cubic Feet'
+    assert ax.get_title() == 'Cumulative Streamflow Hydrograph'
+    assert len(ax.lines) == 4  # min/max, 2010 and 2011 lines
+    assert len(ax.collections) == 1
     # close plot
     plt.close()
```

### Comparing `hyswap-0.0.1/tests/test_rasterhydrograph.py` & `hyswap-0.0.2/tests/test_rasterhydrograph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 """Unit tests for the rasterhydrograph module."""
 import pytest
 import numpy as np
 import pandas as pd
 from hyswap import rasterhydrograph
 
 
-def test_set_data_type():
-    """Test the private function _set_data_type."""
-    assert rasterhydrograph._set_data_type('daily') == 'D'
-    assert rasterhydrograph._set_data_type('7-day') == '7D'
-    assert rasterhydrograph._set_data_type('14-day') == '14D'
-    assert rasterhydrograph._set_data_type('28-day') == '28D'
-
-
 def test_calculate_date_range():
     """Test the private function _calculate_date_range."""
     # define a data frame to use for testing
     dummy_dates = pd.date_range('2018-06-01', '2022-01-31')
     df = pd.DataFrame(
         {'date': dummy_dates, 'value': np.random.rand(len(dummy_dates)),
          'index_year': dummy_dates.year.tolist(),
```

### Comparing `hyswap-0.0.1/tests/test_utils.py` & `hyswap-0.0.2/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -244,7 +244,40 @@
     assert df_slim.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100]
     # check with climate year
     df_slim = utils.munge_nwis_stats(df, year_type='climate')
     assert df_slim.shape == (4, 8)
     assert len(df.columns) > len(df_slim.columns)
     assert 0 in df_slim.columns
     assert df_slim.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100]
+
+
+def test_calculate_summary_statistics():
+    """Test the calculate_summary_statistics function."""
+    # make test dataframe
+    df = pd.DataFrame({
+        'datetime': pd.date_range('2000-01-01', '2000-01-10'),
+        '00060_Mean': [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
+        'site_no': np.ones(10) * 12345678
+    })
+    # set datetime as index
+    df.set_index('datetime', inplace=True)
+    # use function
+    df_stats = utils.calculate_summary_statistics(df, '00060_Mean')
+    # check output
+    assert df_stats.shape == (8, 1)
+    assert df_stats.columns[0] == 'Summary Statistics'
+    assert df_stats.iloc[0, 0] == '12345678'
+    assert df_stats.iloc[1, 0] == '2000-01-01'
+    assert df_stats.iloc[2, 0] == '2000-01-10'
+    assert df_stats.iloc[3, 0] == 10
+    assert df_stats.iloc[4, 0] == 1
+    assert df_stats.iloc[5, 0] == 5.5
+    assert df_stats.iloc[6, 0] == 5.5
+    assert df_stats.iloc[7, 0] == 10
+
+
+def test_set_data_type():
+    """Test the function set_data_type."""
+    assert utils.set_data_type('daily') == 'D'
+    assert utils.set_data_type('7-day') == '7D'
+    assert utils.set_data_type('14-day') == '14D'
+    assert utils.set_data_type('28-day') == '28D'
```

