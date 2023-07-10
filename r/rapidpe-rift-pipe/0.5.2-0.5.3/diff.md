# Comparing `tmp/rapidpe_rift_pipe-0.5.2.tar.gz` & `tmp/rapidpe_rift_pipe-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpe_rift_pipe-0.5.2.tar", last modified: Tue Jul  4 01:46:55 2023, max compression
+gzip compressed data, was "rapidpe_rift_pipe-0.5.3.tar", last modified: Mon Jul 10 17:48:28 2023, max compression
```

## Comparing `rapidpe_rift_pipe-0.5.2.tar` & `rapidpe_rift_pipe-0.5.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 01:46:55.902635 rapidpe_rift_pipe-0.5.2/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1128 2023-07-04 01:46:55.902635 rapidpe_rift_pipe-0.5.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 01:46:55.895635 rapidpe_rift_pipe-0.5.2/bin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 01:46:55.897635 rapidpe_rift_pipe-0.5.2/bin/postscripts/
--rw-rw-rw-   0 root         (0) root         (0)    10056 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/bin/postscripts/compute_posterior.py
--rwxrwxrwx   0 root         (0) root         (0)    12423 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/bin/postscripts/convert_result_to_txt.py
--rw-rw-rw-   0 root         (0) root         (0)     6342 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/bin/postscripts/cprofile_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     5579 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/bin/postscripts/create_summarypage.py
--rw-rw-rw-   0 root         (0) root         (0)     3724 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/bin/postscripts/plot_skymap.py
--rw-rw-rw-   0 root         (0) root         (0)     1440 2023-07-04 01:46:55.902635 rapidpe_rift_pipe-0.5.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 01:46:55.895635 rapidpe_rift_pipe-0.5.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 01:46:55.900635 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-04 01:12:23.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    47573 2023-07-04 01:12:23.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    18705 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 01:46:55.901635 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/config_files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 01:46:43.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/config_files/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 01:46:55.901635 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 01:46:43.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4536 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
--rwxrwxrwx   0 root         (0) root         (0)    31454 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/jacobians.py
--rw-rw-rw-   0 root         (0) root         (0)     9701 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     4719 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/pastro.py
--rw-rw-rw-   0 root         (0) root         (0)    27677 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/postscript_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/search_bias_bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 01:46:55.901635 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 01:46:43.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/static/stylesheet.css
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/test_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-06-14 05:13:15.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 01:46:55.901635 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1128 2023-07-04 01:46:55.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1317 2023-07-04 01:46:55.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 01:46:55.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-04 01:46:55.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-07-04 01:46:55.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-04 01:46:55.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 01:46:55.000000 rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:48:28.739685 rapidpe_rift_pipe-0.5.3/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-07-10 17:48:28.739685 rapidpe_rift_pipe-0.5.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:48:28.732685 rapidpe_rift_pipe-0.5.3/bin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:48:28.735685 rapidpe_rift_pipe-0.5.3/bin/postscripts/
+-rw-rw-rw-   0 root         (0) root         (0)    10056 2023-07-07 05:15:05.000000 rapidpe_rift_pipe-0.5.3/bin/postscripts/compute_posterior.py
+-rwxrwxrwx   0 root         (0) root         (0)    12423 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/bin/postscripts/convert_result_to_txt.py
+-rw-rw-rw-   0 root         (0) root         (0)     6342 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/bin/postscripts/cprofile_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     5579 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/bin/postscripts/create_summarypage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/bin/postscripts/plot_skymap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2023-07-10 17:48:28.740685 rapidpe_rift_pipe-0.5.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:48:28.733685 rapidpe_rift_pipe-0.5.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:48:28.737685 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-09 11:30:28.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    47573 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    18705 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:48:28.738685 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/config_files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:48:18.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/config_files/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:48:28.739685 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:48:18.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4536 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
+-rwxrwxrwx   0 root         (0) root         (0)    31454 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/jacobians.py
+-rw-rw-rw-   0 root         (0) root         (0)     9701 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4719 2023-07-07 05:15:05.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/pastro.py
+-rw-rw-rw-   0 root         (0) root         (0)    27677 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/postscript_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/search_bias_bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:48:28.739685 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:48:18.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/static/stylesheet.css
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/test_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:48:28.738685 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-07-10 17:48:28.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-07-10 17:48:28.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 17:48:28.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-10 17:48:28.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-10 17:48:28.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-10 17:48:28.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 17:48:28.000000 rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe.egg-info/zip-safe
```

### Comparing `rapidpe_rift_pipe-0.5.2/COPYING` & `rapidpe_rift_pipe-0.5.3/COPYING`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.2/PKG-INFO` & `rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
-Name: rapidpe_rift_pipe
-Version: 0.5.2
+Name: rapidpe-rift-pipe
+Version: 0.5.3
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 License-File: COPYING
```

### Comparing `rapidpe_rift_pipe-0.5.2/bin/postscripts/compute_posterior.py` & `rapidpe_rift_pipe-0.5.3/bin/postscripts/compute_posterior.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.2/bin/postscripts/convert_result_to_txt.py` & `rapidpe_rift_pipe-0.5.3/bin/postscripts/convert_result_to_txt.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.2/bin/postscripts/cprofile_summary.py` & `rapidpe_rift_pipe-0.5.3/bin/postscripts/cprofile_summary.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.2/bin/postscripts/create_summarypage.py` & `rapidpe_rift_pipe-0.5.3/bin/postscripts/create_summarypage.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.2/bin/postscripts/plot_skymap.py` & `rapidpe_rift_pipe-0.5.3/bin/postscripts/plot_skymap.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.2/setup.cfg` & `rapidpe_rift_pipe-0.5.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 license = GPL-2+
 classifiers = 
 	Development Status :: 3 - Alpha
 	License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 	Intended Audience :: Science/Research
 	Natural Language :: English
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: Scientific/Engineering
 	Topic :: Scientific/Engineering :: Astronomy
 	Topic :: Scientific/Engineering :: Physics
 
 [options]
@@ -28,15 +27,15 @@
 	numpy
 	matplotlib
 	h5py
 	tabulate
 	astropy
 	lalsuite
 	gwpy>=3.0.4
-	rift==0.0.15.8
+	rift==0.0.15.9
 	rapid_pe>=0.1.0,<0.2.0
 scripts = 
 	bin/postscripts/convert_result_to_txt.py
 	bin/postscripts/create_summarypage.py
 	bin/postscripts/compute_posterior.py
 	bin/postscripts/plot_skymap.py
 	bin/postscripts/cprofile_summary.py
```

### Comparing `rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/cli.py` & `rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/cli.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/config.py` & `rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json` & `rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/create_submit_dag_one_event.py` & `rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/create_submit_dag_one_event.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/jacobians.py` & `rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/jacobians.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/modules.py` & `rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/modules.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/pastro.py` & `rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/pastro.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/postscript_utils.py` & `rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/postscript_utils.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/profiling.py` & `rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/profiling.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/search_bias_bounds.py` & `rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/search_bias_bounds.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/static/stylesheet.css` & `rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/static/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe/test_config.py` & `rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe/test_config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe.egg-info/PKG-INFO` & `rapidpe_rift_pipe-0.5.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
-Name: rapidpe-rift-pipe
-Version: 0.5.2
+Name: rapidpe_rift_pipe
+Version: 0.5.3
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 License-File: COPYING
```

### Comparing `rapidpe_rift_pipe-0.5.2/src/rapidpe_rift_pipe.egg-info/SOURCES.txt` & `rapidpe_rift_pipe-0.5.3/src/rapidpe_rift_pipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

