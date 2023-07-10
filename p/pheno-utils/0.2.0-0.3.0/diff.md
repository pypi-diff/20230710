# Comparing `tmp/pheno-utils-0.2.0.tar.gz` & `tmp/pheno-utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.2.0.tar", last modified: Mon May  1 18:49:32 2023, max compression
+gzip compressed data, was "pheno-utils-0.3.0.tar", last modified: Mon Jul 10 19:35:18 2023, max compression
```

## Comparing `pheno-utils-0.2.0.tar` & `pheno-utils-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-05-01 18:49:32.461170 pheno-utils-0.2.0/
--rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.2.0/LICENSE
--rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.2.0/MANIFEST.in
--rw-r--r--   0 alondmnt   (501) staff       (20)     1553 2023-05-01 18:49:32.458503 pheno-utils-0.2.0/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      504 2023-05-01 07:16:03.000000 pheno-utils-0.2.0/README.md
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-05-01 18:49:32.449280 pheno-utils-0.2.0/pheno_utils/
--rw-r--r--   0 alondmnt   (501) staff       (20)      355 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/__init__.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    16451 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/_modidx.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/age_reference_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     5300 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/basic_analysis.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2789 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/basic_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     7865 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/cgm_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     3599 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/config.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    17656 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/data_loader.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/dates_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2113 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/ecg_analysis.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     7691 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/meta_loader.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    13210 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/sleep_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     1586 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/subset_loader.py
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-05-01 18:49:32.456084 pheno-utils-0.2.0/pheno_utils.egg-info/
--rw-r--r--   0 alondmnt   (501) staff       (20)     1553 2023-05-01 18:49:32.000000 pheno-utils-0.2.0/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      681 2023-05-01 18:49:32.000000 pheno-utils-0.2.0/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-05-01 18:49:32.000000 pheno-utils-0.2.0/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-05-01 18:49:32.000000 pheno-utils-0.2.0/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.2.0/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 alondmnt   (501) staff       (20)      143 2023-05-01 18:49:32.000000 pheno-utils-0.2.0/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-05-01 18:49:32.000000 pheno-utils-0.2.0/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)     1085 2023-05-01 18:46:30.000000 pheno-utils-0.2.0/settings.ini
--rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-05-01 18:49:32.461742 pheno-utils-0.2.0/setup.cfg
--rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:35:17.997520 pheno-utils-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-07-10 19:35:17.986651 pheno-utils-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      489 2023-06-21 16:13:16.000000 pheno-utils-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:35:17.816806 pheno-utils-0.3.0/pheno_utils/
+-rw-r--r--   0 root         (0) root         (0)      342 2023-07-10 19:27:56.000000 pheno-utils-0.3.0/pheno_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17797 2023-07-10 19:27:56.000000 pheno-utils-0.3.0/pheno_utils/_modidx.py
+-rw-r--r--   0 root         (0) root         (0)    16963 2023-07-10 19:27:56.000000 pheno-utils-0.3.0/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 root         (0) root         (0)     5322 2023-07-10 19:27:56.000000 pheno-utils-0.3.0/pheno_utils/basic_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     2870 2023-07-10 19:27:56.000000 pheno-utils-0.3.0/pheno_utils/basic_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2517 2023-07-10 19:27:56.000000 pheno-utils-0.3.0/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 root         (0) root         (0)     7865 2023-07-10 19:27:56.000000 pheno-utils-0.3.0/pheno_utils/cgm_plots.py
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-07-10 19:27:56.000000 pheno-utils-0.3.0/pheno_utils/cohort_selector.py
+-rw-r--r--   0 root         (0) root         (0)     3594 2023-07-10 19:27:56.000000 pheno-utils-0.3.0/pheno_utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-07-10 19:27:56.000000 pheno-utils-0.3.0/pheno_utils/dates_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-10 19:27:56.000000 pheno-utils-0.3.0/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     7754 2023-07-10 19:27:56.000000 pheno-utils-0.3.0/pheno_utils/meta_loader.py
+-rw-r--r--   0 root         (0) root         (0)    19887 2023-07-10 19:27:56.000000 pheno-utils-0.3.0/pheno_utils/pheno_loader.py
+-rw-r--r--   0 root         (0) root         (0)    13210 2023-07-10 19:27:56.000000 pheno-utils-0.3.0/pheno_utils/sleep_plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:35:17.973025 pheno-utils-0.3.0/pheno_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-07-10 19:35:16.000000 pheno-utils-0.3.0/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      684 2023-07-10 19:35:16.000000 pheno-utils-0.3.0/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 19:35:16.000000 pheno-utils-0.3.0/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-10 19:35:16.000000 pheno-utils-0.3.0/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.0/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      143 2023-07-10 19:35:16.000000 pheno-utils-0.3.0/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-10 19:35:16.000000 pheno-utils-0.3.0/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-07-10 19:30:36.000000 pheno-utils-0.3.0/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 19:35:18.004232 pheno-utils-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2560 2023-06-21 16:13:16.000000 pheno-utils-0.3.0/setup.py
```

### Comparing `pheno-utils-0.2.0/LICENSE` & `pheno-utils-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.2.0/PKG-INFO` & `pheno-utils-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.2.0
+Version: 0.3.0
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
-Description: pheno-utils
-        ================
-        
-        <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
-        
-        Viz functions, loaders, mergers.
-        
-        WORK IN PROGRESS
-        
-        ## Install
-        
-        ``` sh
-        pip install pheno_utils
-        ```
-        
-        ## How to use
-        
-        Examples:
-        
-        ``` python
-        data = generate_synthetic_data(n=1000)
-        hist_ecdf_plots(data=data, col="val1")
-        ```
-        
-        ![](index_files/figure-commonmark/cell-2-output-1.png)
-        
-        ``` python
-        age_refplots = GenderAgeRefPlot(data, "val1")
-        age_refplots.plot()
-        ```
-        
-        ![](index_files/figure-commonmark/cell-3-output-1.png)
-        
 Keywords: nbdev jupyter notebook python
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# pheno-utils
+
+<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
+
+Viz functions, loaders, mergers.
+
+WORK IN PROGRESS
+
+## Install
+
+``` sh
+pip install pheno_utils
+```
+
+## How to use
+
+Examples:
+
+``` python
+data = generate_synthetic_data(n=1000)
+hist_ecdf_plots(data=data, col="val1")
+```
+
+![](index_files/figure-commonmark/cell-2-output-1.png)
+
+``` python
+age_refplots = GenderAgeRefPlot(data, "val1")
+age_refplots.plot()
+```
+
+![](index_files/figure-commonmark/cell-3-output-1.png)
```

### Comparing `pheno-utils-0.2.0/pheno_utils/_modidx.py` & `pheno-utils-0.3.0/pheno_utils/_modidx.py`

 * *Files 25% similar despite different names*

```diff
@@ -52,48 +52,24 @@
                                                                                     'pheno_utils/cgm_plots.py'),
                                        'pheno_utils.cgm_plots.CGMPlot.plot_gluc': ( 'cgm_plots.html#cgmplot.plot_gluc',
                                                                                     'pheno_utils/cgm_plots.py'),
                                        'pheno_utils.cgm_plots.CGMPlot.plot_sleep': ( 'cgm_plots.html#cgmplot.plot_sleep',
                                                                                      'pheno_utils/cgm_plots.py'),
                                        'pheno_utils.cgm_plots.CGMPlot.prep_plot': ( 'cgm_plots.html#cgmplot.prep_plot',
                                                                                     'pheno_utils/cgm_plots.py')},
+            'pheno_utils.cohort_selector': { 'pheno_utils.cohort_selector.CohortSelector': ( 'cohort_selector.html#cohortselector',
+                                                                                             'pheno_utils/cohort_selector.py'),
+                                             'pheno_utils.cohort_selector.CohortSelector.__init__': ( 'cohort_selector.html#cohortselector.__init__',
+                                                                                                      'pheno_utils/cohort_selector.py'),
+                                             'pheno_utils.cohort_selector.CohortSelector.select': ( 'cohort_selector.html#cohortselector.select',
+                                                                                                    'pheno_utils/cohort_selector.py')},
             'pheno_utils.config': { 'pheno_utils.config.generate_synthetic_data': ( 'config.html#generate_synthetic_data',
                                                                                     'pheno_utils/config.py'),
                                     'pheno_utils.config.generate_synthetic_data_like': ( 'config.html#generate_synthetic_data_like',
                                                                                          'pheno_utils/config.py')},
-            'pheno_utils.data_loader': { 'pheno_utils.data_loader.DataLoader': ( 'data_loader.html#dataloader',
-                                                                                 'pheno_utils/data_loader.py'),
-                                         'pheno_utils.data_loader.DataLoader.__concat__': ( 'data_loader.html#dataloader.__concat__',
-                                                                                            'pheno_utils/data_loader.py'),
-                                         'pheno_utils.data_loader.DataLoader.__get_dataset_path__': ( 'data_loader.html#dataloader.__get_dataset_path__',
-                                                                                                      'pheno_utils/data_loader.py'),
-                                         'pheno_utils.data_loader.DataLoader.__get_file_path__': ( 'data_loader.html#dataloader.__get_file_path__',
-                                                                                                   'pheno_utils/data_loader.py'),
-                                         'pheno_utils.data_loader.DataLoader.__getitem__': ( 'data_loader.html#dataloader.__getitem__',
-                                                                                             'pheno_utils/data_loader.py'),
-                                         'pheno_utils.data_loader.DataLoader.__init__': ( 'data_loader.html#dataloader.__init__',
-                                                                                          'pheno_utils/data_loader.py'),
-                                         'pheno_utils.data_loader.DataLoader.__load_age_sex__': ( 'data_loader.html#dataloader.__load_age_sex__',
-                                                                                                  'pheno_utils/data_loader.py'),
-                                         'pheno_utils.data_loader.DataLoader.__load_dataframes__': ( 'data_loader.html#dataloader.__load_dataframes__',
-                                                                                                     'pheno_utils/data_loader.py'),
-                                         'pheno_utils.data_loader.DataLoader.__load_dictionary__': ( 'data_loader.html#dataloader.__load_dictionary__',
-                                                                                                     'pheno_utils/data_loader.py'),
-                                         'pheno_utils.data_loader.DataLoader.__load_one_dataframe__': ( 'data_loader.html#dataloader.__load_one_dataframe__',
-                                                                                                        'pheno_utils/data_loader.py'),
-                                         'pheno_utils.data_loader.DataLoader.__repr__': ( 'data_loader.html#dataloader.__repr__',
-                                                                                          'pheno_utils/data_loader.py'),
-                                         'pheno_utils.data_loader.DataLoader.__str__': ( 'data_loader.html#dataloader.__str__',
-                                                                                         'pheno_utils/data_loader.py'),
-                                         'pheno_utils.data_loader.DataLoader.describe_field': ( 'data_loader.html#dataloader.describe_field',
-                                                                                                'pheno_utils/data_loader.py'),
-                                         'pheno_utils.data_loader.DataLoader.get': ( 'data_loader.html#dataloader.get',
-                                                                                     'pheno_utils/data_loader.py'),
-                                         'pheno_utils.data_loader.DataLoader.load_sample_data': ( 'data_loader.html#dataloader.load_sample_data',
-                                                                                                  'pheno_utils/data_loader.py')},
             'pheno_utils.dates_plots': { 'pheno_utils.dates_plots.dates_dist_plot': ( 'date_plots.html#dates_dist_plot',
                                                                                       'pheno_utils/dates_plots.py')},
             'pheno_utils.ecg_analysis': { 'pheno_utils.ecg_analysis.get_hrv_df': ( 'ecg_analysis.html#get_hrv_df',
                                                                                    'pheno_utils/ecg_analysis.py'),
                                           'pheno_utils.ecg_analysis.vis_ecg': ('ecg_analysis.html#vis_ecg', 'pheno_utils/ecg_analysis.py')},
             'pheno_utils.meta_loader': { 'pheno_utils.meta_loader.MetaLoader': ( 'meta_loader.html#metaloader',
                                                                                  'pheno_utils/meta_loader.py'),
@@ -111,19 +87,51 @@
                                                                                           'pheno_utils/meta_loader.py'),
                                          'pheno_utils.meta_loader.MetaLoader.__str__': ( 'meta_loader.html#metaloader.__str__',
                                                                                          'pheno_utils/meta_loader.py'),
                                          'pheno_utils.meta_loader.MetaLoader.get': ( 'meta_loader.html#metaloader.get',
                                                                                      'pheno_utils/meta_loader.py'),
                                          'pheno_utils.meta_loader.MetaLoader.load': ( 'meta_loader.html#metaloader.load',
                                                                                       'pheno_utils/meta_loader.py')},
+            'pheno_utils.pheno_loader': { 'pheno_utils.pheno_loader.PhenoLoader': ( 'pheno_loader.html#phenoloader',
+                                                                                    'pheno_utils/pheno_loader.py'),
+                                          'pheno_utils.pheno_loader.PhenoLoader.__concat__': ( 'pheno_loader.html#phenoloader.__concat__',
+                                                                                               'pheno_utils/pheno_loader.py'),
+                                          'pheno_utils.pheno_loader.PhenoLoader.__get_dataset_path__': ( 'pheno_loader.html#phenoloader.__get_dataset_path__',
+                                                                                                         'pheno_utils/pheno_loader.py'),
+                                          'pheno_utils.pheno_loader.PhenoLoader.__get_dictionary_file_path__': ( 'pheno_loader.html#phenoloader.__get_dictionary_file_path__',
+                                                                                                                 'pheno_utils/pheno_loader.py'),
+                                          'pheno_utils.pheno_loader.PhenoLoader.__get_file_path__': ( 'pheno_loader.html#phenoloader.__get_file_path__',
+                                                                                                      'pheno_utils/pheno_loader.py'),
+                                          'pheno_utils.pheno_loader.PhenoLoader.__getitem__': ( 'pheno_loader.html#phenoloader.__getitem__',
+                                                                                                'pheno_utils/pheno_loader.py'),
+                                          'pheno_utils.pheno_loader.PhenoLoader.__init__': ( 'pheno_loader.html#phenoloader.__init__',
+                                                                                             'pheno_utils/pheno_loader.py'),
+                                          'pheno_utils.pheno_loader.PhenoLoader.__load_age_sex__': ( 'pheno_loader.html#phenoloader.__load_age_sex__',
+                                                                                                     'pheno_utils/pheno_loader.py'),
+                                          'pheno_utils.pheno_loader.PhenoLoader.__load_dataframes__': ( 'pheno_loader.html#phenoloader.__load_dataframes__',
+                                                                                                        'pheno_utils/pheno_loader.py'),
+                                          'pheno_utils.pheno_loader.PhenoLoader.__load_dictionary__': ( 'pheno_loader.html#phenoloader.__load_dictionary__',
+                                                                                                        'pheno_utils/pheno_loader.py'),
+                                          'pheno_utils.pheno_loader.PhenoLoader.__load_one_dataframe__': ( 'pheno_loader.html#phenoloader.__load_one_dataframe__',
+                                                                                                           'pheno_utils/pheno_loader.py'),
+                                          'pheno_utils.pheno_loader.PhenoLoader.__repr__': ( 'pheno_loader.html#phenoloader.__repr__',
+                                                                                             'pheno_utils/pheno_loader.py'),
+                                          'pheno_utils.pheno_loader.PhenoLoader.__str__': ( 'pheno_loader.html#phenoloader.__str__',
+                                                                                            'pheno_utils/pheno_loader.py'),
+                                          'pheno_utils.pheno_loader.PhenoLoader.describe_field': ( 'pheno_loader.html#phenoloader.describe_field',
+                                                                                                   'pheno_utils/pheno_loader.py'),
+                                          'pheno_utils.pheno_loader.PhenoLoader.get': ( 'pheno_loader.html#phenoloader.get',
+                                                                                        'pheno_utils/pheno_loader.py'),
+                                          'pheno_utils.pheno_loader.PhenoLoader.load_sample_data': ( 'pheno_loader.html#phenoloader.load_sample_data',
+                                                                                                     'pheno_utils/pheno_loader.py'),
+                                          'pheno_utils.pheno_loader.PhenoLoader.replace_bulk_data_path': ( 'pheno_loader.html#phenoloader.replace_bulk_data_path',
+                                                                                                           'pheno_utils/pheno_loader.py')},
             'pheno_utils.sleep_plots': { 'pheno_utils.sleep_plots.format_xticks': ( 'sleep_plots.html#format_xticks',
                                                                                     'pheno_utils/sleep_plots.py'),
                                          'pheno_utils.sleep_plots.get_legend_colors': ( 'sleep_plots.html#get_legend_colors',
                                                                                         'pheno_utils/sleep_plots.py'),
                                          'pheno_utils.sleep_plots.plot_channels': ( 'sleep_plots.html#plot_channels',
                                                                                     'pheno_utils/sleep_plots.py'),
                                          'pheno_utils.sleep_plots.plot_events': ( 'sleep_plots.html#plot_events',
                                                                                   'pheno_utils/sleep_plots.py'),
                                          'pheno_utils.sleep_plots.plot_sleep': ( 'sleep_plots.html#plot_sleep',
-                                                                                 'pheno_utils/sleep_plots.py')},
-            'pheno_utils.subset_loader': { 'pheno_utils.subset_loader.load_subset': ( 'subset_loader.html#load_subset',
-                                                                                      'pheno_utils/subset_loader.py')}}}
+                                                                                 'pheno_utils/sleep_plots.py')}}}
```

### Comparing `pheno-utils-0.2.0/pheno_utils/age_reference_plots.py` & `pheno-utils-0.3.0/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.2.0/pheno_utils/basic_analysis.py` & `pheno-utils-0.3.0/pheno_utils/basic_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import pandas as pd
 import matplotlib.pyplot as plt
 import seaborn as sns
 from typing import List, Any, Dict, Union, Optional
 
 
 # %% ../nbs/07_basic_analysis.ipynb 5
-from .config import *
+from .config import generate_synthetic_data
 
 # %% ../nbs/07_basic_analysis.ipynb 6
 def custom_describe(df: pd.DataFrame) -> pd.DataFrame:
     """
     Generates a custom summary statistics dataframe for mixed data types.
     
     Args:
```

### Comparing `pheno-utils-0.2.0/pheno_utils/basic_plots.py` & `pheno-utils-0.3.0/pheno_utils/basic_plots.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 import matplotlib.pyplot as plt
 import seaborn as sns
 from typing import Optional
 from PIL import Image
 from smart_open import open
 
 # %% ../nbs/01_basic_plots.ipynb 4
-from .config import *
+from pheno_utils.config import (
+    FEMALE_COLOR, 
+    MALE_COLOR, 
+    generate_synthetic_data
+    )
 
 # %% ../nbs/01_basic_plots.ipynb 5
 def hist_ecdf_plots(data: pd.DataFrame, col: str, feature_str: Optional[str] = None,
                     gender_col: str = "sex") -> None:
     """
     Plots histograms and empirical cumulative distribution functions (ECDFs) from a DataFrame
     for a specific column.
```

### Comparing `pheno-utils-0.2.0/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.3.0/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.2.0/pheno_utils/cgm_plots.py` & `pheno-utils-0.3.0/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.2.0/pheno_utils/config.py` & `pheno-utils-0.3.0/pheno_utils/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_config.ipynb.
 
 # %% auto 0
 __all__ = ['REF_COLOR', 'FEMALE_COLOR', 'MALE_COLOR', 'ALL_COLOR', 'GLUC_COLOR', 'FOOD_COLOR', 'DATASETS_PATH', 'COHORT',
-           'POPULATION_DATASET', 'ERROR_ACTION', 'CONFIG_FILES', 'generate_synthetic_data',
+           'EVENTS_DATASET', 'ERROR_ACTION', 'CONFIG_FILES', 'BULK_DATA_PATH', 'generate_synthetic_data',
            'generate_synthetic_data_like']
 
 # %% ../nbs/00_config.ipynb 3
 import os
-
+import json
 import numpy as np
 import pandas as pd
 
 # %% ../nbs/00_config.ipynb 4
 REF_COLOR = "k"
 FEMALE_COLOR = "C1"
 MALE_COLOR = "C0"
 ALL_COLOR = "C5"
 
 GLUC_COLOR = "C0"
 FOOD_COLOR = "C1"
 
 DATASETS_PATH = '/home/ec2-user/studies/hpp/'
-COHORT = '10k'
-POPULATION_DATASET = 'population'
+COHORT = None
+EVENTS_DATASET = 'events'
 ERROR_ACTION = 'raise'
-CONFIG_FILES = ['.pheno/config', '~/.pheno/config', '/efs/.pheno/config']
+CONFIG_FILES = ['.pheno/config.json', '~/.pheno/config.json', '/efs/.pheno/config.json']
+BULK_DATA_PATH = {}
+
 
 for cf in CONFIG_FILES:
     cf = os.path.expanduser(cf)
     if not os.path.isfile(cf):
         continue
-    with open(cf, 'r') as f:
-        for line in f:
-            if line.startswith('DATASETS_PATH'):
-                DATASETS_PATH = line.split('=')[1].strip()
-            elif line.startswith('POPULATION_DATASET'):
-                POPULATION_DATASET = line.split('=')[1].strip()
-            elif line.startswith('COHORT'):
-                COHORT = line.split('=')[1].strip()
-                if (len(COHORT) == 0) or (COHORT == 'None'):
-                    COHORT = None
-            elif line.startswith('ERROR_ACTION'):
-                ERROR_ACTION = line.split('=')[1].strip()
+
+    f = open(cf)
+    config = json.load(f)
+    
+    if 'DATASETS_PATH' in config:
+        DATASETS_PATH = config['DATASETS_PATH']
+    if 'BULK_DATA_PATH' in config:
+        BULK_DATA_PATH = config['BULK_DATA_PATH']
+    if 'EVENTS_DATASET' in config:
+        EVENTS_DATASET = config['EVENTS_DATASET']
+    if 'COHORT' in config:
+        if config['COHORT'] == 0 or config['COHORT']=='None' or config['COHORT']==None :
+            COHORT = None
+    if 'ERROR_ACTION' in config:
+        ERROR_ACTION = config['ERROR_ACTION']
     break
 
 
 # %% ../nbs/00_config.ipynb 5
 def generate_synthetic_data(n: int = 1000) -> pd.DataFrame:
     """
     Generates a sample DataFrame containing age, gender, and value data.
```

### Comparing `pheno-utils-0.2.0/pheno_utils/data_loader.py` & `pheno-utils-0.3.0/pheno_utils/pheno_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,46 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/05_data_loader.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/05_pheno_loader.ipynb.
 
 # %% auto 0
-__all__ = ['DataLoader']
+__all__ = ['PhenoLoader']
 
-# %% ../nbs/05_data_loader.ipynb 3
+# %% ../nbs/05_pheno_loader.ipynb 3
 from glob import glob
 import os
 import re
 from typing import List, Any, Dict, Union
 import warnings
+import logging
 
 import numpy as np
 import pandas as pd
 
-# %% ../nbs/05_data_loader.ipynb 4
-from .config import *
-from .basic_analysis import *
-from .basic_plots import *
+# %% ../nbs/05_pheno_loader.ipynb 4
+from pheno_utils.config import (
+    DATASETS_PATH,
+    COHORT, 
+    EVENTS_DATASET, 
+    ERROR_ACTION, 
+    BULK_DATA_PATH
+    )
+from .basic_analysis import custom_describe
+from .basic_plots import show_fundus
 
-# %% ../nbs/05_data_loader.ipynb 5
-class DataLoader:
+# %% ../nbs/05_pheno_loader.ipynb 5
+class PhenoLoader:
     """
     Class to load multiple tables from a dataset and allows to easily access
     their fields.
 
     Args:
     
         dataset (str): The name of the dataset to load.
         base_path (str, optional): The base path where the data is stored. Defaults to DATASETS_PATH.
         cohort (str, optional): The name of the cohort within the dataset. Defaults to COHORT.
-        age_sex_dataset (str, optional): The name of the dataset to use for computing age and sex. Defaults to POPULATION_DATASET.
+        age_sex_dataset (str, optional): The name of the dataset to use for computing age and sex. Defaults to EVENTS_DATASET.
         skip_dfs (list, optional): A list of tables (or substrings that match to tables) to skip when loading the data. Defaults to [].
         unique_index (bool, optional): Whether to ensure the index of the data is unique. Defaults to False.
         valid_dates (bool, optional): Whether to ensure that all timestamps in the data are valid dates. Defaults to False.
         valid_stage (bool, optional): Whether to ensure that all research stages in the data are valid. Defaults to False.
         flexible_field_search (bool, optional): Whether to allow regex field search. Defaults to False.
         errors (str, optional): Whether to raise an error or issue a warning if missing data is encountered.
             Possible values are 'raise', 'warn' and 'ignore'. Defaults to 'raise'.
@@ -57,27 +64,27 @@
     """
 
     def __init__(
         self,
         dataset: str,
         base_path: str = DATASETS_PATH,
         cohort: str = COHORT,
-        age_sex_dataset: str = POPULATION_DATASET,
+        age_sex_dataset: str = EVENTS_DATASET,
         skip_dfs: List[str] = [],
         unique_index: bool = False,
         valid_dates: bool = False,
         valid_stage: bool = False,
         flexible_field_search: bool = False,
         errors: str = ERROR_ACTION,
     ) -> None:
         self.dataset = dataset
         self.cohort = cohort
         self.base_path = base_path
         self.dataset_path = self.__get_dataset_path__(self.dataset)
-        if self.dataset != age_sex_dataset:
+        if self.dataset not in [age_sex_dataset, 'population']:
             self.age_sex_dataset = age_sex_dataset
         else:
             self.age_sex_dataset = None
         self.skip_dfs = skip_dfs
         self.unique_index = unique_index
         self.valid_dates = valid_dates
         self.valid_stage = valid_stage
@@ -121,17 +128,18 @@
         if array_index is not None:
             if not isinstance(array_index, list):
                 array_index = [array_index]
             query_str += ' and array_index in @array_index'
 
         sample = self[[field_name] + ['participant_id']].query(query_str)
         col = sample.columns[0]  # can be different from field_name is a parent_dataframe is implied
-        sample = sample.astype({col: str})
+        sample = sample.astype({col: str})  
         missing_participants = np.setdiff1d(participant_id, sample['participant_id'].unique())
-        sample = self.dataset_path + '/' + sample.iloc[:, 0]
+        sample = sample.loc[:, col]
+        
 
         if len(missing_participants):
             if self.errors == 'raise':
                 raise ValueError(f'Missing samples: {missing_participants}')
             elif self.errors == 'warn':
                 warnings.warn(f'Missing samples: {missing_participants}')
             if len(sample) == 0:
@@ -204,22 +212,28 @@
         """
         if flexible is None:
             flexible = self.flexible_field_search
         if isinstance(fields, str):
             fields = [fields]
 
         # check whether any field points to a parent_dataframe
-        has_parent = self.dict.loc[self.dict.index.isin(fields), 'parent_dataframe'].dropna()
-        fields += has_parent.unique().tolist()
+        # has_parent = self.dict.loc[self.dict.index.isin(fields), 'parent_dataframe'].dropna()
+        seen_fields = set()
+        parent_dict = self.dict.loc[self.dict.index.isin(fields), 'parent_dataframe'].dropna().to_dict()
+        fields = [parent_dict.get(field, field) for field in fields]
+        fields = [field for field in fields if field not in seen_fields and not seen_fields.add(field)]
+        # fields += has_parent.unique().tolist()
+        flexi_fields = list()
 
         data = pd.DataFrame()
         for df in self.dfs.values():
             if flexible:
                 # use fuzzy matching including regex to find fields
                 fields_in_col = np.unique([col for f in fields for col in df.columns if re.search(f, col)])
+                flexi_fields += fields_in_col.tolist()
             else:
                 fields_in_col = df.columns.intersection(fields).difference(data.columns)
             if len(fields_in_col):
                 data = self.__concat__(data, df[fields_in_col])
 
             fields_in_index = np.setdiff1d(np.intersect1d(df.index.names, fields), data.columns)
             for field in fields_in_index:
@@ -232,17 +246,40 @@
 
         not_found = np.setdiff1d(fields, data.columns)
         if len(not_found) and not flexible:
             if self.errors == 'raise':
                 raise KeyError(f'Fields not found: {not_found}')
             elif self.errors == 'warn':
                 warnings.warn(f'Fields not found: {not_found}')
+        
+        data = self.replace_bulk_data_path(data, fields)
+        
+        cols_order = [field for field in fields if field in data.columns]
+        cols_order += [field for field in flexi_fields if (field in data.columns and field not in fields)]
+
+        return data[cols_order]
+    
+
+    def replace_bulk_data_path(self, data, fields):
+        bulk_fields = self.dict.loc[self.dict.index.isin(fields)].query('item_type == "Bulk"')
+        cols = [col for col in bulk_fields.index.to_list() if col in data.columns] 
+        dataset_bulk_data_path = {k:v.format(dataset=self.dataset) for k, v in BULK_DATA_PATH.items()}
+        category_cols = self.dict.loc[self.dict.index.isin(fields)].query('pandas_dtype == "category"').index
+    
+        for col in category_cols: 
+            data[col] = data[col].astype(str)
 
+        data[cols] = data[cols].replace(dataset_bulk_data_path, regex=True)
+        for col in category_cols: 
+            data[col] = data[col].astype('category')
+            
         return data
 
+
+
     def __concat__(self, df1, df2):
         if df1.empty:
             return df2
         if df2.empty:
             return df1
         return df1.join(df2, how='outer')
 
@@ -324,41 +361,48 @@
     def __load_dataframes__(self) -> None:
         """
         Load all tables in the dataset dictionary.
         """
         self.dfs = {}
         self.fields = set()
         for relative_location in self.dict['relative_location'].dropna().unique():
+            # parquet_name = relative_location.split(os.sep)[-1]
+            parquet_name = os.sep.join(relative_location.split(os.sep)[2:])
+            
             if any([pattern in relative_location for pattern in self.skip_dfs]):
                 print(f'Skipping {relative_location}')
                 continue
-            df = self.__load_one_dataframe__(relative_location)
+            df = self.__load_one_dataframe__(parquet_name)
             if df is None:
                 continue
-            self.dfs[relative_location.split('.')[0]] = df
+            table_name = parquet_name.split('.')[0].split(os.sep)[-1]
+            self.dfs[table_name] = df
             if not df.index.is_unique:
-                print('Warning: index is not unique for', relative_location)
-            self.fields |= set(self.dfs[relative_location.split('.')[0]].columns.tolist())
+                print('Warning: index is not unique for', parquet_name)
+            self.fields |= set(self.dfs[table_name].columns.tolist())
         self.fields = sorted(list(self.fields))
 
     def __load_one_dataframe__(self, relative_location: str) -> pd.DataFrame:
         """
         Load one dataframe.
 
         Args:
             relative_location (str): the location of the dataframe
 
         Returns:
             pd.DataFrame: the loaded dataframe
         """
+    
         df_path = os.path.join(self.dataset_path, relative_location)
+        
         try:
             data =  pd.read_parquet(df_path)
         except Exception as err:
             if self.errors == 'raise':
+                warnings.warn(f'Error loading {df_path}:\n{err}')
                 raise err
             if self.errors == 'warn':
                 warnings.warn(f'Error loading {df_path}:\n{err}')
             return None
 
         # set the order of columns according to the dictionary
         dict_columns = self.dict.index.intersection(data.columns)
@@ -379,15 +423,15 @@
 
         return data
 
     def __load_dictionary__(self) -> None:
         """
         Load dataset dictionary.
         """
-        self.dict = pd.read_csv(self.__get_file_path__(self.dataset, 'csv'))\
+        self.dict = pd.read_csv(self.__get_dictionary_file_path__(self.dataset))\
             .set_index('tabular_field_name')
         self.fields = self.dict.index.tolist()
 
     def __get_file_path__(self, dataset: str, extension: str) -> str:
         """
         Get the file path for a dataset and an extension.
 
@@ -399,14 +443,29 @@
             str: the path to the file
         """
         path = os.path.join(self.dataset_path, '*.' + extension)
         if path.startswith('s3://'):
            return path
         return glob(path)[0]
 
+    def __get_dictionary_file_path__(self, dataset: str) -> str:
+        """
+        Get the file path for data dictionary.
+
+        Args:
+            dataset (str): the name of the dataset
+
+        Returns:
+            str: the path to the file
+        """
+        path = os.path.join(self.dataset_path, f'{dataset}_data_dictionary.csv')
+        if path.startswith('s3://'):
+           return path
+        return glob(path)[0]
+
     def __get_dataset_path__(self, dataset):
         """
         Get the dataset path.
         
         Args:
             dataset (str): the name of the dataset
 
@@ -426,13 +485,13 @@
             return_summary (Bool): whether to return the summary dataframe
         
         Returns:
             pd.DataFrame: Data for the specified fields from all tables
         """
         if isinstance(fields, str):
             fields = [fields]
-            
+        
         summary_df = pd.concat([self.dict.loc[fields,:].T,
                                 custom_describe(self[fields])])
         display(summary_df)
         if return_summary:
             return summary_df
```

### Comparing `pheno-utils-0.2.0/pheno_utils/dates_plots.py` & `pheno-utils-0.3.0/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.2.0/pheno_utils/ecg_analysis.py` & `pheno-utils-0.3.0/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.2.0/pheno_utils/meta_loader.py` & `pheno-utils-0.3.0/pheno_utils/meta_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,20 @@
 import warnings
 
 import numpy as np
 import pandas as pd
 import dask.dataframe as dd
 
 # %% ../nbs/11_meta_loader.ipynb 4
-from .config import *
-from .data_loader import DataLoader as PhenoLoader
+from pheno_utils.config import (
+    DATASETS_PATH, 
+    COHORT, 
+    ERROR_ACTION
+    )
+from .pheno_loader import PhenoLoader
 
 # %% ../nbs/11_meta_loader.ipynb 5
 class MetaLoader:
     """
     Class to load multiple dictionaries and allows to easily access the relevant fields.
 
     Args:
@@ -49,14 +53,15 @@
         flexible_field_search: bool = False,
         errors: str = ERROR_ACTION,
         **kwargs,
     ) -> None:
         self.cohort = cohort
         self.base_path = base_path
         self.dataset_path = self.__get_dataset_path__()
+        
         self.flexible_field_search = flexible_field_search
         self.errors = errors
         self.kwargs = kwargs
 
         self.__load_dictionaries__()
 
     def load(self, fields: Union[str,List[str]], flexible: bool=None, prop: str='tabular_field_name') -> pd.DataFrame:
```

### Comparing `pheno-utils-0.2.0/pheno_utils/sleep_plots.py` & `pheno-utils-0.3.0/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.2.0/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.3.0/pheno_utils.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.2.0
+Version: 0.3.0
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
-Description: pheno-utils
-        ================
-        
-        <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
-        
-        Viz functions, loaders, mergers.
-        
-        WORK IN PROGRESS
-        
-        ## Install
-        
-        ``` sh
-        pip install pheno_utils
-        ```
-        
-        ## How to use
-        
-        Examples:
-        
-        ``` python
-        data = generate_synthetic_data(n=1000)
-        hist_ecdf_plots(data=data, col="val1")
-        ```
-        
-        ![](index_files/figure-commonmark/cell-2-output-1.png)
-        
-        ``` python
-        age_refplots = GenderAgeRefPlot(data, "val1")
-        age_refplots.plot()
-        ```
-        
-        ![](index_files/figure-commonmark/cell-3-output-1.png)
-        
 Keywords: nbdev jupyter notebook python
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# pheno-utils
+
+<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
+
+Viz functions, loaders, mergers.
+
+WORK IN PROGRESS
+
+## Install
+
+``` sh
+pip install pheno_utils
+```
+
+## How to use
+
+Examples:
+
+``` python
+data = generate_synthetic_data(n=1000)
+hist_ecdf_plots(data=data, col="val1")
+```
+
+![](index_files/figure-commonmark/cell-2-output-1.png)
+
+``` python
+age_refplots = GenderAgeRefPlot(data, "val1")
+age_refplots.plot()
+```
+
+![](index_files/figure-commonmark/cell-3-output-1.png)
```

### Comparing `pheno-utils-0.2.0/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.3.0/pheno_utils.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 pheno_utils/__init__.py
 pheno_utils/_modidx.py
 pheno_utils/age_reference_plots.py
 pheno_utils/basic_analysis.py
 pheno_utils/basic_plots.py
 pheno_utils/blandaltman_plots.py
 pheno_utils/cgm_plots.py
+pheno_utils/cohort_selector.py
 pheno_utils/config.py
-pheno_utils/data_loader.py
 pheno_utils/dates_plots.py
 pheno_utils/ecg_analysis.py
 pheno_utils/meta_loader.py
+pheno_utils/pheno_loader.py
 pheno_utils/sleep_plots.py
-pheno_utils/subset_loader.py
 pheno_utils.egg-info/PKG-INFO
 pheno_utils.egg-info/SOURCES.txt
 pheno_utils.egg-info/dependency_links.txt
 pheno_utils.egg-info/entry_points.txt
 pheno_utils.egg-info/not-zip-safe
 pheno_utils.egg-info/requires.txt
 pheno_utils.egg-info/top_level.txt
```

### Comparing `pheno-utils-0.2.0/settings.ini` & `pheno-utils-0.3.0/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = pheno-utils
 lib_name = %(repo)s
-version = 0.2.0
+version = 0.3.0
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = pheno_utils
```

### Comparing `pheno-utils-0.2.0/setup.py` & `pheno-utils-0.3.0/setup.py`

 * *Files identical despite different names*

