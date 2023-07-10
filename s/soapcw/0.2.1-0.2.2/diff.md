# Comparing `tmp/soapcw-0.2.1.tar.gz` & `tmp/soapcw-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soapcw-0.2.1.tar", last modified: Sun Jul  9 20:37:39 2023, max compression
+gzip compressed data, was "soapcw-0.2.2.tar", last modified: Mon Jul 10 10:00:37 2023, max compression
```

## Comparing `soapcw-0.2.1.tar` & `soapcw-0.2.2.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.945222 soapcw-0.2.1/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-05 17:01:34.000000 soapcw-0.2.1/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)     3508 2023-07-05 17:01:34.000000 soapcw-0.2.1/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-05 17:01:34.000000 soapcw-0.2.1/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-05 17:01:34.000000 soapcw-0.2.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-07-05 17:01:34.000000 soapcw-0.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2446 2023-07-09 20:37:39.946222 soapcw-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1377 2023-07-09 20:27:29.000000 soapcw-0.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.931222 soapcw-0.2.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)      605 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/authors.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.932222 soapcw-0.2.1/docs/cnn_usage/
--rw-rw-rw-   0 root         (0) root         (0)     5901 2023-07-09 19:50:12.000000 soapcw-0.2.1/docs/cnn_usage/data_generation.rst
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-07-09 19:50:12.000000 soapcw-0.2.1/docs/cnn_usage/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5625 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/cnn_usage/train_model.rst
--rwxrwxrwx   0 root         (0) root         (0)     4930 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/contributing.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/history.rst
--rw-rw-rw-   0 root         (0) root         (0)     1237 2023-07-09 19:50:12.000000 soapcw-0.2.1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      766 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.933222 soapcw-0.2.1/docs/neville_usage/
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-07-09 19:50:12.000000 soapcw-0.2.1/docs/neville_usage/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     6072 2023-07-09 19:50:12.000000 soapcw-0.2.1/docs/neville_usage/load_model.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.933222 soapcw-0.2.1/docs/pipeline_usage/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/pipeline_usage/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     6633 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/pipeline_usage/run_pipeline.rst
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/readme.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.934222 soapcw-0.2.1/docs/usage/
--rw-rw-rw-   0 root         (0) root         (0)      280 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/usage/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.935222 soapcw-0.2.1/pipeline/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 20:34:56.000000 soapcw-0.2.1/pipeline/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.935222 soapcw-0.2.1/pipeline/css/
--rw-rw-rw-   0 root         (0) root         (0)     3163 2023-07-05 17:01:34.000000 soapcw-0.2.1/pipeline/css/general.css
--rwxrwxrwx   0 root         (0) root         (0)     7001 2023-07-05 17:01:34.000000 soapcw-0.2.1/pipeline/make_dag_files_astro.py
--rwxrwxrwx   0 root         (0) root         (0)     6963 2023-07-05 17:01:34.000000 soapcw-0.2.1/pipeline/make_dag_files_lines.py
--rw-rw-rw-   0 root         (0) root         (0)    38283 2023-07-05 17:01:34.000000 soapcw-0.2.1/pipeline/make_html_page.py
--rwxrwxrwx   0 root         (0) root         (0)    37058 2023-07-06 15:04:52.000000 soapcw-0.2.1/pipeline/run_full_soap_astro.py
--rwxrwxrwx   0 root         (0) root         (0)    40172 2023-07-05 17:01:34.000000 soapcw-0.2.1/pipeline/run_full_soap_lines.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.936222 soapcw-0.2.1/pipeline/scripts/
--rw-rw-rw-   0 root         (0) root         (0)    18806 2023-07-05 17:01:34.000000 soapcw-0.2.1/pipeline/scripts/table_scripts.js
--rw-rw-rw-   0 root         (0) root         (0)     3367 2023-07-05 17:01:34.000000 soapcw-0.2.1/pipeline/soap_config_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-09 20:37:39.947222 soapcw-0.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4209 2023-07-05 17:01:34.000000 soapcw-0.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.939222 soapcw-0.2.1/soapcw/
--rw-rw-rw-   0 root         (0) root         (0)      619 2023-07-09 20:02:12.000000 soapcw-0.2.1/soapcw/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.941222 soapcw-0.2.1/soapcw/cnn/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cnn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4682 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cnn/cnn_data_dag_gen.py
--rwxrwxrwx   0 root         (0) root         (0)    17948 2023-07-06 15:04:52.000000 soapcw-0.2.1/soapcw/cnn/cnn_data_gen.py
--rw-rw-rw-   0 root         (0) root         (0)    12490 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cnn/generate_gaussian_train_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11006 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cnn/generate_test_data.py
--rw-rw-rw-   0 root         (0) root         (0)    20005 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cnn/generate_train_data.py
--rwxrwxrwx   0 root         (0) root         (0)     5822 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cnn/narrowband_sfts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.941222 soapcw-0.2.1/soapcw/cnn/pytorch/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cnn/pytorch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4307 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cnn/pytorch/load_models.py
--rw-rw-rw-   0 root         (0) root         (0)    15950 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cnn/pytorch/models.py
--rw-rw-rw-   0 root         (0) root         (0)    14625 2023-07-06 15:04:52.000000 soapcw-0.2.1/soapcw/cnn/train_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.942222 soapcw-0.2.1/soapcw/cw/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cw/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    43688 2023-07-08 20:43:38.000000 soapcw-0.2.1/soapcw/cw/generate_data.py
--rw-rw-rw-   0 root         (0) root         (0)    19576 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cw/load_sfts.py
--rw-rw-rw-   0 root         (0) root         (0)     8660 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cw/make_sfts.py
--rw-rw-rw-   0 root         (0) root         (0)     9450 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cw/sft.py
--rw-rw-rw-   0 root         (0) root         (0)     8567 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cw/timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)     1687 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cw/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.943222 soapcw-0.2.1/soapcw/line_aware_stat/
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/line_aware_stat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11721 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/line_aware_stat/gen_lookup.pyx
--rw-rw-rw-   0 root         (0) root         (0)    38004 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/line_aware_stat/gen_lookup_python.py
--rwxrwxrwx   0 root         (0) root         (0)     6514 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/line_aware_stat/save_lookup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.944222 soapcw-0.2.1/soapcw/neville/
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-07-09 19:50:12.000000 soapcw-0.2.1/soapcw/neville/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1898 2023-07-08 20:43:38.000000 soapcw-0.2.1/soapcw/neville/load_models.py
--rw-rw-rw-   0 root         (0) root         (0)    23724 2023-07-08 20:43:38.000000 soapcw-0.2.1/soapcw/neville/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2007 2023-07-09 19:50:12.000000 soapcw-0.2.1/soapcw/neville/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     4753 2023-07-08 20:43:38.000000 soapcw-0.2.1/soapcw/neville/truncated_gauss.py
--rw-rw-rw-   0 root         (0) root         (0)     4331 2023-07-08 20:43:38.000000 soapcw-0.2.1/soapcw/soap_config_parser.py
--rw-r--r--   0 root         (0) root         (0)  2271838 2023-07-09 20:37:39.000000 soapcw-0.2.1/soapcw/soapcw.c
--rw-rw-rw-   0 root         (0) root         (0)    65928 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/soapcw.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.944222 soapcw-0.2.1/soapcw/tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 20:34:56.000000 soapcw-0.2.1/soapcw/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2885 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/tools/plots.py
--rw-rw-rw-   0 root         (0) root         (0)     9044 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/tools/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.940222 soapcw-0.2.1/soapcw.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2446 2023-07-09 20:37:39.000000 soapcw-0.2.1/soapcw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2032 2023-07-09 20:37:39.000000 soapcw-0.2.1/soapcw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 20:37:39.000000 soapcw-0.2.1/soapcw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      484 2023-07-09 20:37:39.000000 soapcw-0.2.1/soapcw.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 20:37:39.000000 soapcw-0.2.1/soapcw.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-09 20:37:39.000000 soapcw-0.2.1/soapcw.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-09 20:37:39.000000 soapcw-0.2.1/soapcw.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.945222 soapcw-0.2.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)   445283 2023-07-05 17:01:34.000000 soapcw-0.2.1/tests/SNR_injections.ipynb
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-05 17:01:34.000000 soapcw-0.2.1/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1130 2023-07-05 17:01:34.000000 soapcw-0.2.1/tests/test_cwload.py
--rw-rw-rw-   0 root         (0) root         (0)     3602 2023-07-05 17:01:34.000000 soapcw-0.2.1/tests/test_line_aware_stat.py
--rw-rw-rw-   0 root         (0) root         (0)     4290 2023-07-05 17:01:34.000000 soapcw-0.2.1/tests/test_soap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:00:37.878473 soapcw-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-06 09:45:09.000000 soapcw-0.2.2/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3508 2023-07-06 09:45:09.000000 soapcw-0.2.2/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-06 09:45:09.000000 soapcw-0.2.2/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-06 09:45:09.000000 soapcw-0.2.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-07-06 09:45:09.000000 soapcw-0.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-07-10 10:00:37.878473 soapcw-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1377 2023-07-10 09:49:34.000000 soapcw-0.2.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:00:37.864472 soapcw-0.2.2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      605 2023-07-06 09:45:09.000000 soapcw-0.2.2/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-06 09:45:09.000000 soapcw-0.2.2/docs/authors.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:00:37.864472 soapcw-0.2.2/docs/cnn_usage/
+-rw-rw-rw-   0 root         (0) root         (0)     6264 2023-07-10 09:33:23.000000 soapcw-0.2.2/docs/cnn_usage/data_generation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-07-09 19:50:13.000000 soapcw-0.2.2/docs/cnn_usage/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5620 2023-07-10 09:33:23.000000 soapcw-0.2.2/docs/cnn_usage/train_model.rst
+-rwxrwxrwx   0 root         (0) root         (0)     4930 2023-07-06 09:45:09.000000 soapcw-0.2.2/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-06 09:45:09.000000 soapcw-0.2.2/docs/contributing.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-06 09:45:09.000000 soapcw-0.2.2/docs/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2023-07-10 09:33:23.000000 soapcw-0.2.2/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-06 09:45:09.000000 soapcw-0.2.2/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      766 2023-07-06 09:45:09.000000 soapcw-0.2.2/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:00:37.865472 soapcw-0.2.2/docs/neville_usage/
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-07-09 19:50:13.000000 soapcw-0.2.2/docs/neville_usage/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8053 2023-07-10 09:33:23.000000 soapcw-0.2.2/docs/neville_usage/load_model.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:00:37.866472 soapcw-0.2.2/docs/pipeline_usage/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-06 09:45:09.000000 soapcw-0.2.2/docs/pipeline_usage/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6807 2023-07-10 09:33:23.000000 soapcw-0.2.2/docs/pipeline_usage/run_pipeline.rst
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-06 09:45:09.000000 soapcw-0.2.2/docs/readme.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:00:37.867473 soapcw-0.2.2/docs/usage/
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-07-10 09:33:23.000000 soapcw-0.2.2/docs/usage/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:00:37.868472 soapcw-0.2.2/pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:58:24.000000 soapcw-0.2.2/pipeline/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:00:37.868472 soapcw-0.2.2/pipeline/css/
+-rw-rw-rw-   0 root         (0) root         (0)     3163 2023-07-06 09:45:09.000000 soapcw-0.2.2/pipeline/css/general.css
+-rwxrwxrwx   0 root         (0) root         (0)     7001 2023-07-06 09:45:09.000000 soapcw-0.2.2/pipeline/make_dag_files_astro.py
+-rwxrwxrwx   0 root         (0) root         (0)     6963 2023-07-06 09:45:09.000000 soapcw-0.2.2/pipeline/make_dag_files_lines.py
+-rw-rw-rw-   0 root         (0) root         (0)    38283 2023-07-06 09:45:09.000000 soapcw-0.2.2/pipeline/make_html_page.py
+-rwxrwxrwx   0 root         (0) root         (0)    37058 2023-07-06 15:04:53.000000 soapcw-0.2.2/pipeline/run_full_soap_astro.py
+-rwxrwxrwx   0 root         (0) root         (0)    40172 2023-07-06 09:45:09.000000 soapcw-0.2.2/pipeline/run_full_soap_lines.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:00:37.869472 soapcw-0.2.2/pipeline/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)    18806 2023-07-06 09:45:09.000000 soapcw-0.2.2/pipeline/scripts/table_scripts.js
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2023-07-06 09:45:09.000000 soapcw-0.2.2/pipeline/soap_config_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-10 10:00:37.879473 soapcw-0.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4209 2023-07-06 09:45:09.000000 soapcw-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:00:37.871472 soapcw-0.2.2/soapcw/
+-rw-rw-rw-   0 root         (0) root         (0)      619 2023-07-10 09:49:34.000000 soapcw-0.2.2/soapcw/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:00:37.873473 soapcw-0.2.2/soapcw/cnn/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/cnn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4682 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/cnn/cnn_data_dag_gen.py
+-rwxrwxrwx   0 root         (0) root         (0)    17948 2023-07-06 15:04:53.000000 soapcw-0.2.2/soapcw/cnn/cnn_data_gen.py
+-rw-rw-rw-   0 root         (0) root         (0)    12490 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/cnn/generate_gaussian_train_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11006 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/cnn/generate_test_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    20005 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/cnn/generate_train_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     5822 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/cnn/narrowband_sfts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:00:37.874473 soapcw-0.2.2/soapcw/cnn/pytorch/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/cnn/pytorch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4307 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/cnn/pytorch/load_models.py
+-rw-rw-rw-   0 root         (0) root         (0)    15950 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/cnn/pytorch/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    14625 2023-07-06 15:04:53.000000 soapcw-0.2.2/soapcw/cnn/train_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:00:37.875473 soapcw-0.2.2/soapcw/cw/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/cw/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    43688 2023-07-09 19:50:13.000000 soapcw-0.2.2/soapcw/cw/generate_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    19576 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/cw/load_sfts.py
+-rw-rw-rw-   0 root         (0) root         (0)     8660 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/cw/make_sfts.py
+-rw-rw-rw-   0 root         (0) root         (0)     9450 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/cw/sft.py
+-rw-rw-rw-   0 root         (0) root         (0)     8567 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/cw/timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1687 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/cw/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:00:37.875473 soapcw-0.2.2/soapcw/line_aware_stat/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/line_aware_stat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11721 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/line_aware_stat/gen_lookup.pyx
+-rw-rw-rw-   0 root         (0) root         (0)    38004 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/line_aware_stat/gen_lookup_python.py
+-rwxrwxrwx   0 root         (0) root         (0)     6514 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/line_aware_stat/save_lookup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:00:37.876473 soapcw-0.2.2/soapcw/neville/
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-07-09 19:50:13.000000 soapcw-0.2.2/soapcw/neville/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1898 2023-07-09 19:50:13.000000 soapcw-0.2.2/soapcw/neville/load_models.py
+-rw-rw-rw-   0 root         (0) root         (0)    23724 2023-07-09 19:50:13.000000 soapcw-0.2.2/soapcw/neville/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1950 2023-07-10 09:33:23.000000 soapcw-0.2.2/soapcw/neville/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     4753 2023-07-09 19:50:13.000000 soapcw-0.2.2/soapcw/neville/truncated_gauss.py
+-rw-rw-rw-   0 root         (0) root         (0)     4331 2023-07-09 19:50:13.000000 soapcw-0.2.2/soapcw/soap_config_parser.py
+-rw-r--r--   0 root         (0) root         (0)  2271838 2023-07-10 10:00:37.000000 soapcw-0.2.2/soapcw/soapcw.c
+-rw-rw-rw-   0 root         (0) root         (0)    65928 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/soapcw.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:00:37.876473 soapcw-0.2.2/soapcw/tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:58:24.000000 soapcw-0.2.2/soapcw/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2885 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/tools/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)     9044 2023-07-06 09:45:09.000000 soapcw-0.2.2/soapcw/tools/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:00:37.872473 soapcw-0.2.2/soapcw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-07-10 10:00:37.000000 soapcw-0.2.2/soapcw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-07-10 10:00:37.000000 soapcw-0.2.2/soapcw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 10:00:37.000000 soapcw-0.2.2/soapcw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      484 2023-07-10 10:00:37.000000 soapcw-0.2.2/soapcw.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 10:00:37.000000 soapcw-0.2.2/soapcw.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-10 10:00:37.000000 soapcw-0.2.2/soapcw.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-10 10:00:37.000000 soapcw-0.2.2/soapcw.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:00:37.878473 soapcw-0.2.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)   445283 2023-07-06 09:45:09.000000 soapcw-0.2.2/tests/SNR_injections.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-06 09:45:09.000000 soapcw-0.2.2/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2023-07-06 09:45:09.000000 soapcw-0.2.2/tests/test_cwload.py
+-rw-rw-rw-   0 root         (0) root         (0)     3602 2023-07-06 09:45:09.000000 soapcw-0.2.2/tests/test_line_aware_stat.py
+-rw-rw-rw-   0 root         (0) root         (0)     4290 2023-07-06 09:45:09.000000 soapcw-0.2.2/tests/test_soap.py
```

### Comparing `soapcw-0.2.1/CONTRIBUTING.rst` & `soapcw-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/LICENSE` & `soapcw-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/PKG-INFO` & `soapcw-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soapcw
-Version: 0.2.1
+Version: 0.2.2
 Summary: SOAP is a rapid algorithm to search for continuous sources of gravitational waves, with a wider application to long duration narrowband signals.
 Home-page: https://git.ligo.org/joseph.bayley/soapcw
 Author: Joe Bayley
 Author-email: joseph.bayley@glasgow.ac.uk
 License: MIT license
 Download-URL: https://git.ligo.org/joseph.bayley/soapcw/-/archive/0.1.2/soapcw-0.1.2.tar.gz
 Keywords: soapcw,soap,gravitational waves,pulsars,neutron stars,continuous waves
```

### Comparing `soapcw-0.2.1/README.rst` & `soapcw-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/docs/Makefile` & `soapcw-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/docs/cnn_usage/data_generation.rst` & `soapcw-0.2.2/docs/cnn_usage/data_generation.rst`

 * *Files 6% similar despite different names*

```diff
@@ -84,11 +84,17 @@
 This will create a set of sub and dag files to be used with condor, and it will call the program:
 
 .. code-block:: console
 
     $ soapcw-cnn-make-data
 
 
+One can also just use soapcw-cnn-make-data to generate the data without using condor or dags. This will still require and input config file and some other arguments.
 
+For example:
+
+.. code-block:: console
+
+    $ soapcw-cnn-make-data -c config.ini --band-min 100.0 --band-max 104.1 --band-width 0.1 --data-type train --run-type gauss --no-noise False --nperband 10
 
 
 .. _Github repo: https://git.ligo.org/joseph.bayley/soapcw
```

### Comparing `soapcw-0.2.1/docs/cnn_usage/train_model.rst` & `soapcw-0.2.2/docs/cnn_usage/train_model.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ============
-Pipeline usage
+CNN usage
 ============
 
 SOAP is usually run as a pipeline on the LIGO detectors, 
 both searching for astrophysical signals and as a detector characterisation tool.
 
 The machine learning part of this method, mostly using CNNs to reduce the impact of instrumental artefacts, and how to use it is described below.
```

### Comparing `soapcw-0.2.1/docs/conf.py` & `soapcw-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/docs/index.rst` & `soapcw-0.2.2/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
    
     usage/index
     cnn_usage/index
     neville_usage/index
     pipeline_usage/index
 
 
+
 Info
 =========
 
 .. toctree::
     :maxdepth: 1 
 
     modules
```

### Comparing `soapcw-0.2.1/docs/installation.rst` & `soapcw-0.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/docs/make.bat` & `soapcw-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/docs/neville_usage/load_model.rst` & `soapcw-0.2.2/docs/neville_usage/load_model.rst`

 * *Files 24% similar despite different names*

```diff
@@ -98,7 +98,48 @@
 		fdim=1                                            # dimensions to add after convolutional layer, default it 1 to add fmin of band 
 		n_channels=1                                      # number of channels input to cvae
 		dist_type = "gaussian"                            # distribution to use in latent dimension of cvae
 		
 		[code]
 		search_exec=soapcw-cnn-make-data                  # exec to create data
 
+
+Using the Model
+--------------
+For testing the model has a test function that will generate samples from the posterior distribution
+
+.. code-block:: python
+
+	neville_model.eval()  # put the model in eval mode
+	with torch.no_grad(): # dont compute gradients for this
+    	samps = neville_model.test(
+			tracks_input,             # torch tensor of input tracks (ntracks, nchannels, nsamples) 
+			freqs=fmins,              # torch tensor of base frequency for sub-bands corresponding to tracks
+			num_samples=5000,         # number of posterior samples to generate
+			transform_func=None,      # function to transform parameters, see below
+			return_latent = False,    # whether to return latent space samples also
+			par=None                  # injected parameters so latent space from q dsitribution can be returned
+			)
+
+The output of this function are:
+ - samps[0] = Normalised doppler parameters posterior samples 
+ - samps[1] = Transformed doppler parameters posterior samples (only if a transform function has beed specified)
+ - samps[2] = Track element posterior samples (i.e. samples from binomial distribution corresponding to probability that signal is consistent with that track element)
+
+In return latent argument is used the outputs are:
+ - samps[0] = Normalised doppler parameters posterior samples 
+ - samps[1] = Transformed doppler parameters posterior samples (only if a transform function has beed specified)
+ - samps[2] = samples from the latent space of the r encoder
+ - samps[3] = samples from the latent space of the q encoder
+ - samps[4] = Track element posterior samples (i.e. samples from binomial distribution corresponding to probability that signal is consistent with that track element)
+
+
+If using the transform function it should take in the samples and an index and output the transformed samples
+
+ .. code-block:: python
+	
+	def transform(samps, i):
+		lon = lon*2*np.pi
+		lat = lat*np.pi/2
+		f = f + 100.0
+		fdot = fdot*1e-9
+		return lon, lat, f, fdot
```

### Comparing `soapcw-0.2.1/docs/pipeline_usage/run_pipeline.rst` & `soapcw-0.2.2/docs/pipeline_usage/run_pipeline.rst`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 
 Once installed there are two scripts thats can be used to run the pipeline, first the astrophysical search:
 
 .. code-block:: console
 
     $ soapcw-run-soap-astro
 
-is the command which has a number of options. The majority of options are stored in a configuration files which might look something like:
+is the command which has a number of options. The majority of options are stored in a configuration files which might look something like below. 
+Note that currently this configuration file is slightly different from that of the machine learning config used in the cnn and Neville despite having similar inputs. 
 
 .. code-block:: console
 
     [general]
     root_dir = /home/joseph.bayley/repositories/soap/soap_pipeline/summary_pages/astrophysical/O3/
     temp_dir = /home/joseph.bayley/projects/soap_temp/
```

### Comparing `soapcw-0.2.1/pipeline/css/general.css` & `soapcw-0.2.2/pipeline/css/general.css`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/pipeline/make_dag_files_astro.py` & `soapcw-0.2.2/pipeline/make_dag_files_astro.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/pipeline/make_dag_files_lines.py` & `soapcw-0.2.2/pipeline/make_dag_files_lines.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/pipeline/make_html_page.py` & `soapcw-0.2.2/pipeline/make_html_page.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/pipeline/run_full_soap_astro.py` & `soapcw-0.2.2/pipeline/run_full_soap_astro.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/pipeline/run_full_soap_lines.py` & `soapcw-0.2.2/pipeline/run_full_soap_lines.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/pipeline/scripts/table_scripts.js` & `soapcw-0.2.2/pipeline/scripts/table_scripts.js`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/pipeline/soap_config_parser.py` & `soapcw-0.2.2/pipeline/soap_config_parser.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/setup.cfg` & `soapcw-0.2.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [bumpversion]
-current_version = 0.2.0
-new_version = 0.2.1
+current_version = 0.2.1
+new_version = 0.2.2
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
 
@@ -18,15 +18,15 @@
 [flake8]
 exclude = docs
 
 [aliases]
 
 [metadata]
 name = soapcw
-version = 0.2.1
+version = 0.2.2
 
 [options]
 packages = soapcw, pipeline
 
 [options.entry_points]
 console_scripts = 
 	soapcw-make-dag-files-lines = pipeline.make_dag_files_lines:main
```

### Comparing `soapcw-0.2.1/setup.py` & `soapcw-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/__init__.py` & `soapcw-0.2.2/soapcw/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import
 """Top-level package for soapcw."""
 
 __author__ = """Joe Bayley"""
 __email__ = 'joseph.bayley@glasgow.ac.uk'
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 from .soapcw import single_detector, two_detector, three_detector, single_detector_gaps
 from .tools import tools, plots
 from .cnn import __init__
 from .neville import __init__
 from .line_aware_stat import __init__
 from .cw import __init__
 from . import soap_config_parser
```

### Comparing `soapcw-0.2.1/soapcw/cnn/cnn_data_dag_gen.py` & `soapcw-0.2.2/soapcw/cnn/cnn_data_dag_gen.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/cnn/cnn_data_gen.py` & `soapcw-0.2.2/soapcw/cnn/cnn_data_gen.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/cnn/generate_gaussian_train_data.py` & `soapcw-0.2.2/soapcw/cnn/generate_gaussian_train_data.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/cnn/generate_test_data.py` & `soapcw-0.2.2/soapcw/cnn/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/cnn/generate_train_data.py` & `soapcw-0.2.2/soapcw/cnn/generate_train_data.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/cnn/narrowband_sfts.py` & `soapcw-0.2.2/soapcw/cnn/narrowband_sfts.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/cnn/pytorch/load_models.py` & `soapcw-0.2.2/soapcw/cnn/pytorch/load_models.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/cnn/pytorch/models.py` & `soapcw-0.2.2/soapcw/cnn/pytorch/models.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/cnn/train_model.py` & `soapcw-0.2.2/soapcw/cnn/train_model.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/cw/generate_data.py` & `soapcw-0.2.2/soapcw/cw/generate_data.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/cw/load_sfts.py` & `soapcw-0.2.2/soapcw/cw/load_sfts.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/cw/make_sfts.py` & `soapcw-0.2.2/soapcw/cw/make_sfts.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/cw/sft.py` & `soapcw-0.2.2/soapcw/cw/sft.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/cw/timeseries.py` & `soapcw-0.2.2/soapcw/cw/timeseries.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/cw/tools.py` & `soapcw-0.2.2/soapcw/cw/tools.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/line_aware_stat/gen_lookup.pyx` & `soapcw-0.2.2/soapcw/line_aware_stat/gen_lookup.pyx`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/line_aware_stat/gen_lookup_python.py` & `soapcw-0.2.2/soapcw/line_aware_stat/gen_lookup_python.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/line_aware_stat/save_lookup.py` & `soapcw-0.2.2/soapcw/line_aware_stat/save_lookup.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/neville/load_models.py` & `soapcw-0.2.2/soapcw/neville/load_models.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/neville/models.py` & `soapcw-0.2.2/soapcw/neville/models.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/neville/tools.py` & `soapcw-0.2.2/soapcw/neville/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,17 +23,15 @@
     lon = lon*2*np.pi
     lon = np.remainder(lon, 2*np.pi)
     lat = np.abs(lat)*(0.5*np.pi)
 
     f = f*width + fmin
     fdot = (fdot*2 - 1)*1e-9
 
-    alpha, delta = transform_ecliptic_geo(lon, lat)
-
-    return alpha, delta, f, fdot
+    return lon, lat, f, fdot
 
 def transform_normlonlat_alphadelta(fmin, width, lon, lat, f, fdot):
     """_summary_
 
     Args:
         fmin (_type_): _description_
         width (_type_): _description_
```

### Comparing `soapcw-0.2.1/soapcw/neville/truncated_gauss.py` & `soapcw-0.2.2/soapcw/neville/truncated_gauss.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/soap_config_parser.py` & `soapcw-0.2.2/soapcw/soap_config_parser.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/soapcw.c` & `soapcw-0.2.2/soapcw/soapcw.c`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/soapcw.pyx` & `soapcw-0.2.2/soapcw/soapcw.pyx`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/tools/plots.py` & `soapcw-0.2.2/soapcw/tools/plots.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw/tools/tools.py` & `soapcw-0.2.2/soapcw/tools/tools.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/soapcw.egg-info/PKG-INFO` & `soapcw-0.2.2/soapcw.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soapcw
-Version: 0.2.1
+Version: 0.2.2
 Summary: SOAP is a rapid algorithm to search for continuous sources of gravitational waves, with a wider application to long duration narrowband signals.
 Home-page: https://git.ligo.org/joseph.bayley/soapcw
 Author: Joe Bayley
 Author-email: joseph.bayley@glasgow.ac.uk
 License: MIT license
 Download-URL: https://git.ligo.org/joseph.bayley/soapcw/-/archive/0.1.2/soapcw-0.1.2.tar.gz
 Keywords: soapcw,soap,gravitational waves,pulsars,neutron stars,continuous waves
```

### Comparing `soapcw-0.2.1/soapcw.egg-info/SOURCES.txt` & `soapcw-0.2.2/soapcw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/tests/SNR_injections.ipynb` & `soapcw-0.2.2/tests/SNR_injections.ipynb`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/tests/test_cwload.py` & `soapcw-0.2.2/tests/test_cwload.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/tests/test_line_aware_stat.py` & `soapcw-0.2.2/tests/test_line_aware_stat.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.1/tests/test_soap.py` & `soapcw-0.2.2/tests/test_soap.py`

 * *Files identical despite different names*

