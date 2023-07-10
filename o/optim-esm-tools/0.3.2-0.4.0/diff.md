# Comparing `tmp/optim_esm_tools-0.3.2.tar.gz` & `tmp/optim_esm_tools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optim_esm_tools-0.3.2.tar", last modified: Fri Jul  7 14:47:25 2023, max compression
+gzip compressed data, was "optim_esm_tools-0.4.0.tar", last modified: Mon Jul 10 06:59:24 2023, max compression
```

## Comparing `optim_esm_tools-0.3.2.tar` & `optim_esm_tools-0.4.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:47:25.310311 optim_esm_tools-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-07-07 14:47:25.310311 optim_esm_tools-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:47:25.310311 optim_esm_tools-0.3.2/optim_esm_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/_test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:47:25.310311 optim_esm_tools-0.3.2/optim_esm_tools/analyze/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/analyze/calculate_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/analyze/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/analyze/cmip_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/analyze/find_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/analyze/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/analyze/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    23233 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/analyze/region_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/analyze/tipping_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/analyze/xarray_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:47:25.310311 optim_esm_tools-0.3.2/optim_esm_tools/cmip_files/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/cmip_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/optim_esm_conf.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:47:25.310311 optim_esm_tools-0.3.2/optim_esm_tools/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/plotting/map_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/plotting/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:47:25.310311 optim_esm_tools-0.3.2/optim_esm_tools/synda_files/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/synda_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/synda_files/format_synda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/synda_files/synda_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/optim_esm_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:47:25.310311 optim_esm_tools-0.3.2/optim_esm_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-07-07 14:47:24.000000 optim_esm_tools-0.3.2/optim_esm_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-07 14:47:25.000000 optim_esm_tools-0.3.2/optim_esm_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:47:24.000000 optim_esm_tools-0.3.2/optim_esm_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:47:24.000000 optim_esm_tools-0.3.2/optim_esm_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 14:47:24.000000 optim_esm_tools-0.3.2/optim_esm_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 14:47:24.000000 optim_esm_tools-0.3.2/optim_esm_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-07 14:47:25.314311 optim_esm_tools-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:47:25.310311 optim_esm_tools-0.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/test/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/test/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/test/test_find_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/test/test_pangeo_download.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/test/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/test/test_region_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/test/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/test/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-07 14:47:16.000000 optim_esm_tools-0.3.2/test/test_xarray_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:59:24.923272 optim_esm_tools-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-07-10 06:59:24.927272 optim_esm_tools-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:59:24.919272 optim_esm_tools-0.4.0/optim_esm_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/_test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:59:24.923272 optim_esm_tools-0.4.0/optim_esm_tools/analyze/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/analyze/calculate_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/analyze/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/analyze/cmip_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/analyze/find_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/analyze/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/analyze/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23233 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/analyze/region_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/analyze/tipping_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/analyze/xarray_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:59:24.923272 optim_esm_tools-0.4.0/optim_esm_tools/cmip_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/cmip_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/optim_esm_conf.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:59:24.923272 optim_esm_tools-0.4.0/optim_esm_tools/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/plotting/map_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/plotting/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:59:24.923272 optim_esm_tools-0.4.0/optim_esm_tools/synda_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/synda_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/synda_files/format_synda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/synda_files/synda_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/optim_esm_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:59:24.919272 optim_esm_tools-0.4.0/optim_esm_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-07-10 06:59:24.000000 optim_esm_tools-0.4.0/optim_esm_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-10 06:59:24.000000 optim_esm_tools-0.4.0/optim_esm_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 06:59:24.000000 optim_esm_tools-0.4.0/optim_esm_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 06:59:24.000000 optim_esm_tools-0.4.0/optim_esm_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 06:59:24.000000 optim_esm_tools-0.4.0/optim_esm_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 06:59:24.000000 optim_esm_tools-0.4.0/optim_esm_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-10 06:59:24.927272 optim_esm_tools-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:59:24.923272 optim_esm_tools-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/test/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/test/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/test/test_find_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/test/test_pangeo_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/test/test_region_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/test/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/test/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-10 06:59:20.000000 optim_esm_tools-0.4.0/test/test_xarray_tools.py
```

### Comparing `optim_esm_tools-0.3.2/PKG-INFO` & `optim_esm_tools-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim_esm_tools
-Version: 0.3.2
+Version: 0.4.0
 Summary: Tools for OptimESM
 Home-page: https://github.com/JoranAngevaare/optim_esm_tools
 Author: Joran R. Angevaare
 License: UNKNOWN
 Description: # OptimESM
         [![Coverage Status](https://coveralls.io/repos/github/JoranAngevaare/optim_esm_tools/badge.svg)](https://coveralls.io/github/JoranAngevaare/optim_esm_tools)
         [![PyPI version shields.io](https://img.shields.io/pypi/v/optim-esm-tools.svg)](https://pypi.python.org/pypi/optim-esm-tools/)
@@ -15,14 +15,21 @@
         Getting started with OptimESM
         
         Selection of tools and tricks for [OptimESM](https://cordis.europa.eu/project/id/101081193) project.
         
         J.R. Angevaare (KNMI)
         
         
+        0.4.0 / 2023-07-07
+        ------------------
+        *  Technical release related to the setup of the package relating to the config
+        
+        **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v0.3.0...v0.4.0
+        
+        
         0.3.0 / 2023-07-05
         ------------------
         * Remove old setup by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/77
         * Area calculation  & percentile recombination & weighted clustering by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/76
         
         
         **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v0.2.2...v0.3.0
```

### Comparing `optim_esm_tools-0.3.2/README.md` & `optim_esm_tools-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/optim_esm_tools/_test_utils.py` & `optim_esm_tools-0.4.0/optim_esm_tools/_test_utils.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/optim_esm_tools/analyze/calculate_metric.py` & `optim_esm_tools-0.4.0/optim_esm_tools/analyze/calculate_metric.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/optim_esm_tools/analyze/clustering.py` & `optim_esm_tools-0.4.0/optim_esm_tools/analyze/clustering.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/optim_esm_tools/analyze/cmip_handler.py` & `optim_esm_tools-0.4.0/optim_esm_tools/analyze/cmip_handler.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/optim_esm_tools/analyze/find_matches.py` & `optim_esm_tools-0.4.0/optim_esm_tools/analyze/find_matches.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/optim_esm_tools/analyze/io.py` & `optim_esm_tools-0.4.0/optim_esm_tools/analyze/io.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/optim_esm_tools/analyze/region_finding.py` & `optim_esm_tools-0.4.0/optim_esm_tools/analyze/region_finding.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/optim_esm_tools/analyze/tipping_criteria.py` & `optim_esm_tools-0.4.0/optim_esm_tools/analyze/tipping_criteria.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/optim_esm_tools/analyze/xarray_tools.py` & `optim_esm_tools-0.4.0/optim_esm_tools/analyze/xarray_tools.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/optim_esm_tools/config.py` & `optim_esm_tools-0.4.0/optim_esm_tools/config.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/optim_esm_tools/optim_esm_conf.ini` & `optim_esm_tools-0.4.0/optim_esm_tools/optim_esm_conf.ini`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/optim_esm_tools/plotting/map_maker.py` & `optim_esm_tools-0.4.0/optim_esm_tools/plotting/map_maker.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/optim_esm_tools/synda_files/format_synda.py` & `optim_esm_tools-0.4.0/optim_esm_tools/synda_files/format_synda.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/optim_esm_tools/synda_files/synda_files.py` & `optim_esm_tools-0.4.0/optim_esm_tools/synda_files/synda_files.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/optim_esm_tools/utils.py` & `optim_esm_tools-0.4.0/optim_esm_tools/utils.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/optim_esm_tools.egg-info/PKG-INFO` & `optim_esm_tools-0.4.0/optim_esm_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim-esm-tools
-Version: 0.3.2
+Version: 0.4.0
 Summary: Tools for OptimESM
 Home-page: https://github.com/JoranAngevaare/optim_esm_tools
 Author: Joran R. Angevaare
 License: UNKNOWN
 Description: # OptimESM
         [![Coverage Status](https://coveralls.io/repos/github/JoranAngevaare/optim_esm_tools/badge.svg)](https://coveralls.io/github/JoranAngevaare/optim_esm_tools)
         [![PyPI version shields.io](https://img.shields.io/pypi/v/optim-esm-tools.svg)](https://pypi.python.org/pypi/optim-esm-tools/)
@@ -15,14 +15,21 @@
         Getting started with OptimESM
         
         Selection of tools and tricks for [OptimESM](https://cordis.europa.eu/project/id/101081193) project.
         
         J.R. Angevaare (KNMI)
         
         
+        0.4.0 / 2023-07-07
+        ------------------
+        *  Technical release related to the setup of the package relating to the config
+        
+        **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v0.3.0...v0.4.0
+        
+        
         0.3.0 / 2023-07-05
         ------------------
         * Remove old setup by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/77
         * Area calculation  & percentile recombination & weighted clustering by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/76
         
         
         **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v0.2.2...v0.3.0
```

### Comparing `optim_esm_tools-0.3.2/optim_esm_tools.egg-info/SOURCES.txt` & `optim_esm_tools-0.4.0/optim_esm_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/setup.py` & `optim_esm_tools-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 readme = open('README.md').read()
 history = open('HISTORY.md').read()
 requirements = open_requirements('requirements.txt')
 
 setuptools.setup(
     name='optim_esm_tools',
-    version='0.3.2',
+    version='0.4.0',
     description='Tools for OptimESM',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     author='Joran R. Angevaare',
     url='https://github.com/JoranAngevaare/optim_esm_tools',
     packages=setuptools.find_packages(),
     package_dir={
```

### Comparing `optim_esm_tools-0.3.2/test/test_clustering.py` & `optim_esm_tools-0.4.0/test/test_clustering.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/test/test_find_matches.py` & `optim_esm_tools-0.4.0/test/test_find_matches.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/test/test_region_finding.py` & `optim_esm_tools-0.4.0/test/test_region_finding.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/test/test_utils.py` & `optim_esm_tools-0.4.0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/test/test_viewer.py` & `optim_esm_tools-0.4.0/test/test_viewer.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/test/test_workflow.py` & `optim_esm_tools-0.4.0/test/test_workflow.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.3.2/test/test_xarray_tools.py` & `optim_esm_tools-0.4.0/test/test_xarray_tools.py`

 * *Files identical despite different names*

