# Comparing `tmp/yet_another_wizz-2.5.tar.gz` & `tmp/yet_another_wizz-2.5.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yet_another_wizz-2.5.tar", last modified: Sun Jul  9 16:12:24 2023, max compression
+gzip compressed data, was "yet_another_wizz-2.5.post0.tar", last modified: Mon Jul 10 08:18:48 2023, max compression
```

## Comparing `yet_another_wizz-2.5.tar` & `yet_another_wizz-2.5.post0.tar`

### file list

```diff
@@ -1,84 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.595285 yet_another_wizz-2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-09 16:12:24.595285 yet_another_wizz-2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 16:12:24.595285 yet_another_wizz-2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.563283 yet_another_wizz-2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.563283 yet_another_wizz-2.5/src/yaw/
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.567283 yet_another_wizz-2.5/src/yaw/catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/catalogs/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/catalogs/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/catalogs/linkage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.567283 yet_another_wizz-2.5/src/yaw/catalogs/scipy/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/catalogs/scipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/catalogs/scipy/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/catalogs/scipy/kdtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/catalogs/scipy/patches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.571283 yet_another_wizz-2.5/src/yaw/catalogs/treecorr/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/catalogs/treecorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/catalogs/treecorr/catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.575284 yet_another_wizz-2.5/src/yaw/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/config/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/config/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)    14657 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/config/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/config/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/config/resampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/config/scales.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.579284 yet_another_wizz-2.5/src/yaw/core/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12375 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/cosmology.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/math.c
--rw-r--r--   0 runner    (1001) docker     (123)    10827 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.579284 yet_another_wizz-2.5/src/yaw/correlation/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/correlation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40621 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/correlation/corrfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/correlation/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)    41926 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/correlation/paircounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/deprecated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.583284 yet_another_wizz-2.5/src/yaw/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   129479 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/examples/auto_reference.hdf
--rw-r--r--   0 runner    (1001) docker     (123)   123032 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/examples/auto_unknown_1.hdf
--rw-r--r--   0 runner    (1001) docker     (123)   100475 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/examples/cross_1.hdf
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)    22441 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/redshifts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.583284 yet_another_wizz-2.5/src/yaw_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.587284 yet_another_wizz-2.5/src/yaw_cli/commandline/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/commandline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/commandline/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/commandline/subcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/commandline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.591284 yet_another_wizz-2.5/src/yaw_cli/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17836 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/pipeline/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/pipeline/default_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/pipeline/directories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/pipeline/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/pipeline/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/pipeline/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    16034 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/pipeline/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15241 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/pipeline/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/pipeline/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.591284 yet_another_wizz-2.5/src/yet_another_wizz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-09 16:12:24.000000 yet_another_wizz-2.5/src/yet_another_wizz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-09 16:12:24.000000 yet_another_wizz-2.5/src/yet_another_wizz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 16:12:24.000000 yet_another_wizz-2.5/src/yet_another_wizz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-09 16:12:24.000000 yet_another_wizz-2.5/src/yet_another_wizz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-09 16:12:24.000000 yet_another_wizz-2.5/src/yet_another_wizz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-09 16:12:24.000000 yet_another_wizz-2.5/src/yet_another_wizz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.342015 yet_another_wizz-2.5.post0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-10 08:18:48.342015 yet_another_wizz-2.5.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 08:18:48.342015 yet_another_wizz-2.5.post0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.318014 yet_another_wizz-2.5.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.322014 yet_another_wizz-2.5.post0/src/yaw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.322014 yet_another_wizz-2.5.post0/src/yaw/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/linkage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.326015 yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/kdtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/patches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.326015 yet_another_wizz-2.5.post0/src/yaw/catalogs/treecorr/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/treecorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15092 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/treecorr/catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.330015 yet_another_wizz-2.5.post0/src/yaw/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14829 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/resampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/scales.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.334015 yet_another_wizz-2.5.post0/src/yaw/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9967 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16139 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/cosmology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/math.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.334015 yet_another_wizz-2.5.post0/src/yaw/correlation/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/correlation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40475 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/correlation/corrfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/correlation/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41424 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/correlation/paircounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/deprecated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.334015 yet_another_wizz-2.5.post0/src/yaw/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129479 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/examples/auto_reference.hdf
+-rw-r--r--   0 runner    (1001) docker     (123)   123032 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/examples/auto_unknown_1.hdf
+-rw-r--r--   0 runner    (1001) docker     (123)   100475 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/examples/cross_1.hdf
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22413 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/redshifts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.338015 yet_another_wizz-2.5.post0/src/yaw_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.338015 yet_another_wizz-2.5.post0/src/yaw_cli/commandline/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/commandline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/commandline/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17458 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/commandline/subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/commandline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.338015 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17790 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/default_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18945 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.342015 yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-10 08:18:48.000000 yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-10 08:18:48.000000 yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 08:18:48.000000 yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 08:18:48.000000 yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-10 08:18:48.000000 yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 08:18:48.000000 yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/top_level.txt
```

### Comparing `yet_another_wizz-2.5/LICENSE` & `yet_another_wizz-2.5.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5/PKG-INFO` & `yet_another_wizz-2.5.post0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-Metadata-Version: 2.1
-Name: yet_another_wizz
-Version: 2.5
-Summary: Implementation of the Schmidt et al. (2013) clustering redshift method and wrapper scripts to produce cross-correlation (CC) redshifts.
-Home-page: https://github.com/jlvdb/yet_another_wizz.git
-Author-email: Jan Luca van den Busch <jlvdb@astro.ruhr-uni-bochum.de>
-License: GPL-3.0-or-later
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Astronomy
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: plot
-Provides-Extra: docs
-Provides-Extra: dev
-License-File: LICENSE
-
 yet_another_wizz
 ================
 
+.. image:: https://badge.fury.io/py/yet-another-wizz.svg
+    :target: https://badge.fury.io/py/yet-another-wizz
+.. image:: https://readthedocs.org/projects/yet-another-wizz/badge/?version=latest
+    :target: https://yet-another-wizz.readthedocs.io/en/latest/?badge=latest
+.. image:: https://github.com/jlvdb/yet_another_wizz/actions/workflows/run-tests.yml/badge.svg
+    :target: https://github.com/jlvdb/yet_another_wizz/actions/workflows/run-tests.yml
+.. image:: https://codecov.io/gh/jlvdb/yet_another_wizz/branch/main/graph/badge.svg?token=PC41ME2AR8
+    :target: https://codecov.io/gh/jlvdb/yet_another_wizz
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+    :target: https://pycqa.github.io/isort/
+
 
 *yet_another_wizz* is a python package to efficiently compute cross-correlation
 redshifts, also know as clustering redshifts and is hosted on github:
 
 - code: https://github.com/jlvdb/yet_another_wizz.git
 - docs: https://yet-another-wizz.readthedocs.io/
 - PyPI: https://pypi.org/project/yet_another_wizz/
@@ -67,15 +62,15 @@
 Reporting bugs and requesting features
 --------------------------------------
 
 For bug reports or requesting new features, please use the github issue page:
 
 https://github.com/jlvdb/yet_another_wizz/issues
 
-    
+
 **Maintainers:**
 
 - Jan Luca van den Busch
   (*author*, Ruhr-Universität Bochum, Astronomisches Institut)
 
 
 Acknowledgements
```

### Comparing `yet_another_wizz-2.5/pyproject.toml` & `yet_another_wizz-2.5.post0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -32,30 +32,41 @@
     "astropy",
     "treecorr>=4.3",
     "emcee",
     "matplotlib",
 ]
 
 [project.scripts]
-yaw_cli = "yaw_cli:__main__"
+yaw_cli = "yaw_cli:Commandline.main"
 
 [project.optional-dependencies]
 plot = ["matplotlib"]
 docs = [
     "sphinx",
     "sphinx-design",
     "sphinx-copybutton",
     "pydata-sphinx-theme",
 ]
-dev = [
+test = [
     "typing_extensions",
     "more_itertools",
-    "yet_another_wizz[docs]",
-    "pytest",
     "coverage",
+    "pytest",
+    "pytest-cov",
+]
+style = [
+    "black",
+    "isort",
+    "flake8",
+    "pre-commit",
+]
+dev = [
+    "yet_another_wizz[docs]",
+    "yet_another_wizz[test]",
+    "yet_another_wizz[style]",
     "ipykernel",
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "yaw.__version__"}
 
 [tool.setuptools.packages.find]
@@ -69,7 +80,26 @@
     "examples/*.smp",
 ]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra -q"
 testpaths = ["tests"]
+
+[tool.isort]
+profile = "black"
+
+[tool.black]
+include = ".pyi?$"
+exclude = """
+/(
+    .git
+    | .hg
+    | .mypy_cache
+    | .tox
+    | .venv
+    | _build
+    | buck-out
+    | build
+    | dist
+)/
+"""
```

### Comparing `yet_another_wizz-2.5/src/yaw/catalogs/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 The most important member is the catalog factory class :obj:`NewCatalog`,
 which provides an interface to create new catalog instances for each of the
 supported correlation measurement backends. The :obj:`BaseCatalog` defines the
 common catalogue interface and must be subclasses by all other backend
 implementations.
 """
 
+# make backends available and make sure they are registered
 from yaw.catalogs.catalog import BaseCatalog
 from yaw.catalogs.factory import NewCatalog
 from yaw.catalogs.linkage import PatchLinkage
 
-# make backends available and make sure they are registered
-from yaw.catalogs import scipy, treecorr
+# isort: split
+from yaw.catalogs import scipy, treecorr  # noqa
 
+__all__ = ["BaseCatalog", "NewCatalog", "PatchLinkage"]
```

### Comparing `yet_another_wizz-2.5/src/yaw/catalogs/catalog.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,22 @@
 from numpy.typing import NDArray
 
 from yaw.core.coordinates import Coordinate, CoordSky, DistSky
 from yaw.core.utils import long_num_format
 
 if TYPE_CHECKING:  # pragma: no cover
     from pandas import DataFrame
+
     from yaw.catalogs import PatchLinkage
     from yaw.config import Configuration, ResamplingConfig
     from yaw.correlation.paircounts import NormalisedCounts
     from yaw.redshifts import HistData
 
+__all__ = ["BaseCatalog"]
+
 
 _Tcat = TypeVar("_Tcat", bound="BaseCatalog")
 
 
 class BackendError(Exception):
     pass
 
@@ -45,17 +48,18 @@
     _backends = dict()
 
     def __init_subclass__(cls, **kwargs):
         """Handles the backend subclass registration."""
         super().__init_subclass__(**kwargs)
         if not cls.__name__.endswith("Catalog"):
             raise BackendError(
-                f"subclasses of 'BaseCatalog' must follow naming convention "
-                f"'[Backend name]Catalog for registration (e.g. ScipyCatalog "
-                f"-> 'scipy')")
+                "subclasses of 'BaseCatalog' must follow naming convention "
+                "'[Backend name]Catalog for registration (e.g. ScipyCatalog "
+                "-> 'scipy')"
+            )
         backend = cls.__name__.strip("Catalog").lower()
         cls._backends[backend] = cls
 
     @abstractmethod
     def __init__(
         self,
         data: DataFrame,
@@ -64,18 +68,18 @@
         *,
         patch_name: str | None = None,
         patch_centers: BaseCatalog | Coordinate | None = None,
         n_patches: int | None = None,
         redshift_name: str | None = None,
         weight_name: str | None = None,
         cache_directory: str | None = None,
-        progress: bool = False
+        progress: bool = False,
     ) -> None:
         """Build a catalogue from in-memory data.
-        
+
         Catalogs should be instantiated through the factory class, see
         :meth:`yaw.catalogs.NewCatalog.from_dataframe`."""
         pass
 
     @classmethod
     def from_file(
         cls,
@@ -86,18 +90,18 @@
         *,
         redshift: str | None = None,
         weight: str | None = None,
         sparse: int | None = None,
         cache_directory: str | None = None,
         file_ext: str | None = None,
         progress: bool = False,
-        **kwargs
+        **kwargs,
     ) -> BaseCatalog:
         """Build a catalogue from data file.
-        
+
         Catalogs should be instantiated through the factory class, see
         :meth:`yaw.catalogs.NewCatalog.from_file`."""
         columns = [c for c in [ra, dec, redshift, weight] if c is not None]
         if isinstance(patches, str):
             columns.append(patches)
             patch_kwarg = dict(patch_name=patches)
         elif isinstance(patches, int):
@@ -106,73 +110,78 @@
             patch_kwarg = dict(patch_centers=patches)
         elif isinstance(patches, BaseCatalog):
             patch_kwarg = dict(patch_centers=patches.centers)
         else:
             raise TypeError(
                 "'patches' must be either of type 'str' (col. name), 'int' "
                 "(number of patches), or 'Catalog' or 'Coordinate' (specify "
-                "centers)")
+                "centers)"
+            )
 
         cls._logger.info(f"reading catalog file '{filepath}'")
         data = apd.read_auto(filepath, columns=columns, ext=file_ext, **kwargs)
         if sparse is not None:
             cls._logger.debug(f"sparse sampling data {sparse}x")
             data = data[::sparse]
         return cls(
-            data, ra, dec, **patch_kwarg,
+            data,
+            ra,
+            dec,
+            **patch_kwarg,
             redshift_name=redshift,
             weight_name=weight,
             cache_directory=cache_directory,
-            progress=progress)
+            progress=progress,
+        )
 
     @abstractclassmethod
-    def from_cache(
-        cls,
-        cache_directory: str,
-        progress: bool = False
-    ) -> BaseCatalog:
+    def from_cache(cls, cache_directory: str, progress: bool = False) -> BaseCatalog:
         """Restore the catalogue from its cache directory.
-        
+
         Catalogs should be instantiated through the factory class, see
         :meth:`yaw.catalogs.NewCatalog.from_cache`."""
         cls._logger.info(f"restoring from cache directory '{cache_directory}'")
 
     def __repr__(self) -> str:
         name = self.__class__.__name__
         args = dict(
             loaded=self.is_loaded(),
             nobjects=len(self),
             npatches=self.n_patches,
-            redshifts=self.has_redshifts())
+            redshifts=self.has_redshifts(),
+        )
         arg_str = ", ".join(f"{k}={v}" for k, v in args.items())
         return f"{name}({arg_str})"
 
     @abstractmethod
-    def __len__(self) -> int: pass
+    def __len__(self) -> int:
+        pass
 
     @abstractmethod
-    def __getitem__(self, item: int) -> Any: pass
+    def __getitem__(self, item: int) -> Any:
+        pass
 
     @abstractproperty
     def ids(self) -> list[int]:
         """Return a list of unique patch indices in the catalog."""
         pass
 
     @abstractmethod
     def n_patches(self) -> int:
         """The number of spatial patches of this catalogue."""
         pass
 
     @abstractmethod
-    def __iter__(self) -> Iterator: pass
+    def __iter__(self) -> Iterator:
+        pass
 
     @abstractmethod
     def is_loaded(self) -> bool:
         """Indicates whether the catalog data is loaded.
-        
+
         Always ``True`` if no cache is used. If the catalog is unloaded, data
         will be read from cache every time data is accessed."""
         pass
 
     @abstractmethod
     def load(self) -> None:
         """Permanently load data from cache into memory.
@@ -196,15 +205,15 @@
     def has_weights(self) -> bool:
         """Indicates whether the :meth:`weights` attribute holds data."""
         pass
 
     @property
     def pos(self) -> CoordSky:
         """Get a vector of the object sky positions in radians.
-        
+
         Returns:
             :obj:`yaw.core.coordinates.CoordSky`
         """
         return CoordSky(self.ra, self.dec)
 
     @abstractproperty
     def ra(self) -> NDArray[np.float_]:
@@ -250,41 +259,41 @@
     def get_totals(self) -> NDArray[np.float_]:
         """Get an array of the sum of weights or number of objects in each
         patch."""
 
     @abstractproperty
     def centers(self) -> CoordSky:
         """Get a vector of sky coordinates of the patch centers in radians.
-        
+
         Returns:
             :obj:`yaw.core.coordinates.CoordSky`
         """
         pass
 
     @abstractproperty
     def radii(self) -> DistSky:
         """Get a vector of angular separations in radians that describe the
         patch sizes.
 
         The radius of the patch is defined as the maximum angular distance of
         any object from the patch center.
-                
+
         Returns:
             :obj:`yaw.core.coordinates.DistSky`
         """
         pass
 
     @abstractmethod
     def correlate(
         self,
         config: Configuration,
         binned: bool,
         other: _Tcat = None,
         linkage: PatchLinkage | None = None,
-        progress: bool = False
+        progress: bool = False,
     ) -> NormalisedCounts | dict[str, NormalisedCounts]:
         """Count pairs between objects at a given separation and in bins of
         redshift.
 
         If another catalog instance is passed to ``other``, then pairs are
         formed between these catalogues (cross), otherwise pairs are formed with
         the catalog (auto). Pairs are counted in bins of redshift, as defined in
@@ -317,30 +326,31 @@
         1. If no second catalogue is provided, pairs are counted within the
            catalogue while applying the redshift binning.
         2. If a second catalogue is provided and ``binned=True``, pairs are
            counted between the catalogues and the binning is applied to both
            cataluges.
         3. If a second catalogue is provided and ``binned=False``, the redshift
            binning is not applied to the second catalogue, otherwise above.
-        
+
         The catalogue from the calling instance of :meth:`correlate` has always
         redshift binning applied.
         """
         n1 = long_num_format(len(self))
         n2 = long_num_format(len(self) if other is None else len(other))
         self._logger.debug(
             f"correlating with {'' if binned else 'un'}binned catalog "
-            f"({n1}x{n2}) in {config.binning.zbin_num} redshift bins")
+            f"({n1}x{n2}) in {config.binning.zbin_num} redshift bins"
+        )
 
     @abstractmethod
     def true_redshifts(
         self,
         config: Configuration,
         sampling_config: ResamplingConfig | None = None,
-        progress: bool = False
+        progress: bool = False,
     ) -> HistData:
         """
         Compute a histogram of the object redshifts from the binning defined in
         the provided configuration.
 
         Args:
             config (:obj:`~yaw.config.Configuration`):
```

### Comparing `yet_another_wizz-2.5/src/yaw/catalogs/factory.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 
 from typing import TYPE_CHECKING
 
 from yaw.catalogs.catalog import BackendError, BaseCatalog
 
 if TYPE_CHECKING:  # pragma: no cover
     from pandas import DataFrame
+
     from yaw.core.coordinates import Coordinate
 
+__all__ = ["NewCatalog"]
+
 
 class NewCatalog:
     """Factory class for data catalogues implemented by the backends.
 
     A catalogue provides all the functionality to compute pair counts for
     correlation measurements by implementing an interface to the object
     positions, spatial patches for error estimation, and data management if the
@@ -36,15 +39,15 @@
     individual spatial patches) can be read back into memory on demand.
 
     .. Warning::
 
         - The ``scipy`` backend does not preserve the order the input data, but
           instead groups objects by there spatial patch.
         - The ``treecorr`` backend does currently not support restoration from
-          cache.    
+          cache.
     """
 
     def __init__(self, backend: str = "scipy") -> None:
         """Create a new catalogue factory.
 
         Args:
             backend (:obj:`str`):
@@ -69,33 +72,33 @@
         *,
         patch_name: str | None = None,
         patch_centers: BaseCatalog | Coordinate | None = None,
         n_patches: int | None = None,
         redshift_name: str | None = None,
         weight_name: str | None = None,
         cache_directory: str | None = None,
-        progress: bool = False
+        progress: bool = False,
     ) -> BaseCatalog:
         """Build a catalogue from in-memory data.
-        
+
         Specify the names of the required and or available columns in a
         :obj:`pandas.DataFrame`. Additional parameters control the creation
         spatial patches used for error estimates. Patches can be assigned based
         on a column in the data frame (``patch_name``), constructed from a set
         of existing patch centers (``patch_centers``), or generated with
         `k`-means clustering (``n_patches``).
 
         Args:
             data (:obj:`pandas.Dataframe`):
                 Holds the catalog data.
             ra_name (:obj:`str`):
                 Name of the column with right ascension data in degrees.
             dec_name (:obj:`str`):
                 Name of the column with declination data in degress.
-        
+
         Keyword Args:
             patch_name (:obj:`str`, optional):
                 Name of the column that specifies the patch index, i.e.
                 assigning each object to a spatial patch. Index starts counting
                 from 0 (see :ref:`patches`).
             patch_centers (:obj:`~yaw.catalogs.BaseCatalog`, :obj:`~yaw.core.coordinates.Coordinate`, optional):
                 Assign objects to existing patch centers based on their
@@ -136,30 +139,31 @@
             dec_name,
             patch_name=patch_name,
             patch_centers=patch_centers,
             n_patches=n_patches,
             redshift_name=redshift_name,
             weight_name=weight_name,
             cache_directory=cache_directory,
-            progress=progress)
+            progress=progress,
+        )
 
     def from_file(
         self,
         filepath: str,
         patches: str | int | BaseCatalog | Coordinate,
         ra: str,
         dec: str,
         *,
         redshift: str | None = None,
         weight: str | None = None,
         sparse: int | None = None,
         cache_directory: str | None = None,
         file_ext: str | None = None,
         progress: bool = False,
-        **kwargs
+        **kwargs,
     ) -> BaseCatalog:
         """
         Build catalogue from data file.
 
         Loads the input file and constructs the catalogue using the specified
         column names.
 
@@ -171,15 +175,15 @@
                 are read from the file. If `int`, generates this number of
                 patches. Otherwise assign objects based on existing patch
                 centers from a catalog instance or a coordinate vector.
             ra (:obj:`str`):
                 Name of the column with right ascension data in degrees.
             dec (:obj:`str`):
                 Name of the column with declination data in degress.
-        
+
         Keyword Args:
             redshift (:obj:`str`, optional):
                 Name of the column with point-redshift estimates.
             weight (:obj:`str`, optional):
                 Name of the column with object weights.
             sparse (:obj:`int`, optional):
                 Load every N-th row of the input data.
@@ -216,21 +220,18 @@
             dec,
             redshift=redshift,
             weight=weight,
             sparse=sparse,
             cache_directory=cache_directory,
             file_ext=file_ext,
             progress=progress,
-            **kwargs)
+            **kwargs,
+        )
 
-    def from_cache(
-        self,
-        cache_directory: str,
-        progress: bool = False
-    ) -> BaseCatalog:
+    def from_cache(self, cache_directory: str, progress: bool = False) -> BaseCatalog:
         """
         Restore the catalogue from its cache directory.
 
         Args:
             cache_directory (:obj:`str`):
                 Path to the cache directory.
             progress (:obj:`bool`, optional):
```

### Comparing `yet_another_wizz-2.5/src/yaw/catalogs/linkage.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/linkage.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from yaw.core.coordinates import Dist3D, DistSky
 from yaw.core.cosmology import r_kpc_to_angle
 
 if TYPE_CHECKING:  # pragma: no cover
     from yaw.catalogs import BaseCatalog
     from yaw.config import Configuration
 
+__all__ = ["PatchLinkage"]
+
 
 logger = logging.getLogger(__name__)
 
 
 LINK_ZMIN = 0.05
 """The reference redshift at which the maximum angular size is computed."""
 
@@ -29,34 +31,27 @@
     This class is useful to generate pairs of patches that need to be paired
     for pair count measurements for a given maximum angular search radius.
     Patches that are separated by more than the sum of their radii and the
     maximum search radius do not contribute any pair counts and can be
     discarded.
     """
 
-    def __init__(
-        self,
-        patch_tuples: list[PatchIDs]
-    ) -> None:
+    def __init__(self, patch_tuples: list[PatchIDs]) -> None:
         """Populate a patch linkage container.
 
         To create a new linkage, use the :meth:`from_setup` method.
 
         Args:
             patch_tuples (list[:obj:`~yaw.core.containers.PatchIDs`]):
                 List of patch pairs that need to be visited to count pairs.
         """
         self.pairs = patch_tuples
 
     @classmethod
-    def from_setup(
-        cls,
-        config: Configuration,
-        catalog: BaseCatalog
-    ) -> PatchLinkage:
+    def from_setup(cls, config: Configuration, catalog: BaseCatalog) -> PatchLinkage:
         """Generate a new patch linkage.
 
         Compute a maximum angular separation for at low redshift for the scales
         provided in the configuration. Generate a list of all patch pairs that
         are separated by less than this maximum separation (factoring in the
         size of the patches).
 
@@ -71,15 +66,16 @@
             :obj:`PatchLinkage`
         """
         # determine the additional overlap from the spatial query
         if config.backend.crosspatch:
             # estimate maximum query radius at low, but non-zero redshift
             z_ref = max(LINK_ZMIN, config.binning.zmin)
             max_query_radius = r_kpc_to_angle(
-                config.scales.as_array(), z_ref, config.cosmology).max()
+                config.scales.as_array(), z_ref, config.cosmology
+            ).max()
         else:
             max_query_radius = 0.0  # only relevant for cross-patch
         max_query_radius = DistSky(max_query_radius)
 
         logger.debug(f"computing patch linkage with {max_query_radius=:.3e}")
         centers_3d = catalog.centers.to_3d().values
         radii = catalog.radii.values
@@ -90,16 +86,16 @@
 
         # check which patches overlap when factoring in the query radius
         overlaps = dist_mat_3d.to_sky() < (size_sum + max_query_radius)
         patch_pairs = []
         for id1, overlap in enumerate(overlaps):
             patch_pairs.extend((id1, id2) for id2 in np.where(overlap)[0])
         logger.debug(
-            f"found {len(patch_pairs)} patch links "
-            f"for {catalog.n_patches} patches")
+            f"found {len(patch_pairs)} patch links " f"for {catalog.n_patches} patches"
+        )
         return cls(patch_pairs)
 
     def __len__(self) -> int:
         return len(self.pairs)
 
     def __repr__(self) -> str:
         name = self.__class__.__name__
@@ -115,21 +111,17 @@
         return len(patches)
 
     @property
     def density(self) -> float:
         """Get ratio of the number of linked patch pairs compared to all
         possible combinations."""
         n = self.n_patches
-        return len(self) / (n*n)
+        return len(self) / (n * n)
 
-    def get_pairs(
-        self,
-        auto: bool,
-        crosspatch: bool = True
-    ) -> list[PatchIDs]:
+    def get_pairs(self, auto: bool, crosspatch: bool = True) -> list[PatchIDs]:
         """Get a list of linked patch pairs.
 
         Args:
             auto (:obj:`bool`):
                 For autocorrelation measurements, only visit patch pairs where
                 patch ID1 >= ID2.
             crosspatch (:obj:`bool`):
@@ -146,31 +138,30 @@
                 pairs = self.pairs
         else:
             pairs = [(i, j) for i, j in self.pairs if i == j]
         return pairs
 
     @staticmethod
     def _parse_collections(
-        collection1: BaseCatalog,
-        collection2: BaseCatalog | None = None
+        collection1: BaseCatalog, collection2: BaseCatalog | None = None
     ) -> tuple[bool, BaseCatalog, BaseCatalog]:
         auto = collection2 is None
         if auto:
             collection2 = collection1
         return auto, collection1, collection2
 
     def get_matrix(
         self,
         collection1: BaseCatalog,
         collection2: BaseCatalog | None = None,
-        crosspatch: bool = True
+        crosspatch: bool = True,
     ) -> NDArray[np.bool_]:
         """Convert the list of linked patches to a boolean matrix indicating if
         two patches are linked.
-        
+
         Depending on if one or two catalogs are provided as input, the result
         resembles a cross- or autocorrelation patch linkage. This is the only
         purpose of the inputs.
 
         Args:
             collection1 (:obj:`BaseCatalog`):
                 First catalog for patch linkage.
@@ -185,31 +176,32 @@
 
         .. Warning::
 
             The patch centers of both catalogues must be (very close to)
             identical.
         """
         auto, collection1, collection2 = self._parse_collections(
-            collection1, collection2)
+            collection1, collection2
+        )
         pairs = self.get_pairs(auto, crosspatch)
         # make a boolean matrix indicating the exisiting patch combinations
         n_patches = self.n_patches
         matrix = np.zeros((n_patches, n_patches), dtype=np.bool_)
         for pair in pairs:
             matrix[pair] = True
         return matrix
 
     def get_patches(
         self,
         collection1: BaseCatalog,
         collection2: BaseCatalog | None = None,
-        crosspatch: bool = True
+        crosspatch: bool = True,
     ) -> tuple[list[BaseCatalog], list[BaseCatalog]]:
         """Return linked pairs of patch data ready for processing.
-        
+
         Instead of returning a list of patch index pairs, the actual patch data
         is returned in two aligned list, where item 1 form the first list is
         linked to item 1 of the second list. Depending on if one or two catalogs
         are provided as input, the result resembles a cross- or autocorrelation
         patch linkage.
 
         Args:
@@ -227,15 +219,16 @@
 
         .. Warning::
 
             The patch centers of both catalogues must be (very close to)
             identical.
         """
         auto, collection1, collection2 = self._parse_collections(
-            collection1, collection2)
+            collection1, collection2
+        )
         pairs = self.get_pairs(auto, crosspatch)
         # generate the patch lists
         patches1 = []
         patches2 = []
         for id1, id2 in pairs:
             patches1.append(collection1[id1])
             patches2.append(collection2[id2])
```

### Comparing `yet_another_wizz-2.5/src/yaw/catalogs/scipy/catalog.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/catalog.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 from __future__ import annotations
 
 import itertools
 import os
 from collections.abc import Iterator, Sequence
-from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
 
 from yaw.catalogs import BaseCatalog, PatchLinkage
 from yaw.catalogs.scipy.patches import (
-    PatchCatalog, patch_id_from_path, create_patches, assign_patches)
+    PatchCatalog,
+    assign_patches,
+    create_patches,
+    patch_id_from_path,
+)
 from yaw.config import Configuration, ResamplingConfig
 from yaw.core.containers import PatchCorrelationData, PatchIDs
-from yaw.core.coordinates import Coordinate, Coord3D, CoordSky, DistSky
+from yaw.core.coordinates import Coord3D, Coordinate, CoordSky, DistSky
 from yaw.core.cosmology import Scale
 from yaw.core.logging import TimedLog
 from yaw.core.parallel import ParallelHelper
-from yaw.core.utils import (
-    LimitTracker, job_progress_bar, long_num_format)
+from yaw.core.utils import LimitTracker, job_progress_bar, long_num_format
 from yaw.correlation.paircounts import (
-    NormalisedCounts, PatchedCount, PatchedTotal, pack_results)
+    NormalisedCounts,
+    PatchedCount,
+    PatchedTotal,
+    pack_results,
+)
 from yaw.redshifts import HistData
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import NDArray
     from pandas import DataFrame
+
     from yaw.core.cosmology import TypeCosmology
 
+__all__ = ["ScipyCatalog"]
+
 
 def _count_pairs_thread(
     patch1: PatchCatalog,
     patch2: PatchCatalog,
     scales: Sequence[Scale],
     cosmology: TypeCosmology,
     z_bins: NDArray[np.float_],
     bin1: bool = True,
     bin2: bool = False,
     dist_weight_scale: float | None = None,
-    dist_weight_res: int = 50
+    dist_weight_res: int = 50,
 ) -> PatchCorrelationData:
     """Implementes the pair counting between two patches.
 
     Bins the data as needed and builds the KDTrees for the pair finding.
     Converts the physical scales to angles for the given cosmology and redshift
     and counts the pairs. Pairs are recoreded for each set of scales and stored
     in a PatchCorrelationData object.
@@ -63,34 +72,34 @@
     # count pairs, iterate through the bins and count pairs between the trees
     counts = np.empty((len(scales), len(z_intervals)))
     totals1 = np.empty(len(z_intervals))
     totals2 = np.empty(len(z_intervals))
     for i, (intv, tree1, tree2) in enumerate(zip(z_intervals, trees1, trees2)):
         # if bin1 is False and bin2 is False, these will still give different
         # counts since the angle for scales is chaning
-        angles = [
-            scale.to_radian(intv.mid, cosmology) for scale in scales]
+        angles = [scale.to_radian(intv.mid, cosmology) for scale in scales]
         counts[:, i] = tree1.count(
             tree2,
             scales=angles,
             dist_weight_scale=dist_weight_scale,
-            weight_res=dist_weight_res)
+            weight_res=dist_weight_res,
+        )
         totals1[i] = tree1.total
         totals2[i] = tree2.total
     counts = {str(scale): count for scale, count in zip(scales, counts)}
     return PatchCorrelationData(
         patches=PatchIDs(patch1.id, patch2.id),
         totals1=totals1,
         totals2=totals2,
-        counts=counts)
+        counts=counts,
+    )
 
 
 def _histogram_thread(
-    patch: PatchCatalog,
-    z_bins: NDArray[np.float_]
+    patch: PatchCatalog, z_bins: NDArray[np.float_]
 ) -> NDArray[np.float_]:
     """Computes a redshift histogram for a single PatchCatalog and returns the
     counts as array."""
     is_loaded = patch.is_loaded()
     patch.load()
     counts, _ = np.histogram(patch.redshifts, z_bins, weights=patch.weights)
     if not is_loaded:
@@ -100,15 +109,15 @@
 
 class ScipyCatalog(BaseCatalog):
     """An implementation of the :obj:`BaseCatalog` using a wrapper around
     :obj:`scipy.spatial.cKDTree` for the pair counting, which is implemented in
     :obj:`yaw.catalogs.scipy.kdtree`. Fully supports caching.
 
     .. Note::
-    
+
         This is currently the default backend and has the best support and
         performance. Currently, trees cannot be shared across the
         multiprocessing interface and must be rebuilt every time a patch is
         used for pair counting again.
     """
 
     def __init__(
@@ -119,15 +128,15 @@
         *,
         patch_name: str | None = None,
         patch_centers: BaseCatalog | Coordinate | None = None,
         n_patches: int | None = None,
         redshift_name: str | None = None,
         weight_name: str | None = None,
         cache_directory: str | None = None,
-        progress: bool = True
+        progress: bool = True,
     ) -> None:
         if len(data) == 0:
             raise ValueError("data catalog is empty")
         # check if the columns exist
         renames = {ra_name: "ra", dec_name: "dec"}
         if redshift_name is not None:
             renames[redshift_name] = "redshift"
@@ -145,34 +154,37 @@
             if n_patches is not None:
                 patch_mode = "creating"
             elif patch_centers is not None:
                 patch_mode = "applying"
             else:
                 raise ValueError(
                     "either of 'patch_name', 'patch_centers', or 'n_patches' "
-                    "must be provided")
+                    "must be provided"
+                )
         if unload:
             if not os.path.exists(cache_directory):
                 raise FileNotFoundError(
-                    f"patch directory does not exist: '{cache_directory}'")
+                    f"patch directory does not exist: '{cache_directory}'"
+                )
             self._logger.debug(f"using cache directory '{cache_directory}'")
 
         # create new patches
         if patch_mode != "dividing":
             position = CoordSky.from_array(
-                np.deg2rad(data[[ra_name, dec_name]].to_numpy()))
+                np.deg2rad(data[[ra_name, dec_name]].to_numpy())
+            )
             if patch_mode == "creating":
                 patch_centers, patch_ids = create_patches(
-                    position=position, n_patches=n_patches)
+                    position=position, n_patches=n_patches
+                )
                 log_msg = f"creating {n_patches} patches"
             else:
                 if isinstance(patch_centers, BaseCatalog):
                     patch_centers = patch_centers.centers.to_3d()
-                patch_ids = assign_patches(
-                    centers=patch_centers, position=position)
+                patch_ids = assign_patches(centers=patch_centers, position=position)
                 n_patches = len(patch_centers)
                 log_msg = f"applying {n_patches} patches from external data"
             patch_name = "patch"  # the default name
             data[patch_name] = patch_ids
             centers = {pid: pos for pid, pos in enumerate(patch_centers)}
         else:
             n_patches = len(data[patch_name].unique())
@@ -188,52 +200,53 @@
             patch_iter = data.groupby(patch_name)
             if progress:
                 patch_iter = job_progress_bar(patch_iter, total=n_patches)
             for patch_id, patch_data in patch_iter:
                 if patch_id < 0:
                     raise ValueError("negative patch IDs are not supported")
                 # drop extra columns
-                patch_data = patch_data.drop(columns=[
-                    col for col in patch_data.columns if col not in renames])
+                patch_data = patch_data.drop(
+                    columns=[col for col in patch_data.columns if col not in renames]
+                )
                 patch_data.rename(columns=renames, inplace=True)
                 patch_data.reset_index(drop=True, inplace=True)
                 # look up the center of the patch if given
                 kwargs = dict(center=centers.get(patch_id))
                 if unload:
                     # data will be written as feather file and loaded on demand
                     kwargs["cachefile"] = os.path.join(
-                        cache_directory, f"patch_{patch_id:.0f}.feather")
+                        cache_directory, f"patch_{patch_id:.0f}.feather"
+                    )
                 patch = PatchCatalog(int(patch_id), patch_data, **kwargs)
                 limits.update(patch.redshifts)
                 if unload:
                     patch.unload()
                 patches[patch.id] = patch
             if progress:  # clean up if any patch was empty and skipped
                 patch_iter.close()
             self._zmin, self._zmax = limits.get()
             self._patches = patches
 
         # also store the patch properties
         if unload:
             centers = self.centers.to_3d()
-            property_df = pd.DataFrame(dict(
-                ids=self.ids,
-                x=centers.x,
-                y=centers.y,
-                z=centers.z,
-                r=self.radii.values))
+            property_df = pd.DataFrame(
+                dict(
+                    ids=self.ids,
+                    x=centers.x,
+                    y=centers.y,
+                    z=centers.z,
+                    r=self.radii.values,
+                )
+            )
             fpath = os.path.join(cache_directory, "properties.feather")
             property_df.to_feather(fpath)
 
     @classmethod
-    def from_cache(
-        cls,
-        cache_directory: str,
-        progress: bool = False
-    ) -> ScipyCatalog:
+    def from_cache(cls, cache_directory: str, progress: bool = False) -> ScipyCatalog:
         super().from_cache(cache_directory)
         new = cls.__new__(cls)
         # load the patch properties
         fpath = os.path.join(cache_directory, "properties.feather")
         property_df = pd.read_feather(fpath)
         # transform data frame to dictionaries
         ids = property_df["ids"]
@@ -252,17 +265,16 @@
             if not path.startswith("patch"):
                 continue
             abspath = os.path.join(cache_directory, path)
             if not os.path.isfile(abspath):
                 continue
             patch_id = patch_id_from_path(path)
             patch = PatchCatalog.from_cached(
-                abspath,
-                center=centers.get(patch_id),
-                radius=radii.get(patch_id))
+                abspath, center=centers.get(patch_id), radius=radii.get(patch_id)
+            )
             limits.update(patch.redshifts)
             patch.unload()
             new._patches[patch.id] = patch
         new._zmin, new._zmax = limits.get()
         return new
 
     def __len__(self) -> int:
@@ -315,16 +327,15 @@
     @property
     def dec(self) -> NDArray[np.float_]:
         return np.concatenate([patch.dec for patch in iter(self)])
 
     @property
     def redshifts(self) -> NDArray[np.float_] | None:
         if self.has_redshifts():
-            return np.concatenate([
-                patch.redshifts for patch in iter(self)])
+            return np.concatenate([patch.redshifts for patch in iter(self)])
         else:
             return None
 
     @property
     def weights(self) -> NDArray[np.float_]:
         weights = []
         for patch in iter(self):
@@ -332,16 +343,15 @@
                 weights.append(patch.weights)
             else:
                 weights.append(np.ones(len(patch)))
         return np.concatenate(weights)
 
     @property
     def patch(self) -> NDArray[np.int_]:
-        return np.concatenate([
-            np.full(len(patch), patch.id) for patch in iter(self)])
+        return np.concatenate([np.full(len(patch), patch.id) for patch in iter(self)])
 
     def get_min_redshift(self) -> float:
         return self._zmin
 
     def get_max_redshift(self) -> float:
         return self._zmax
 
@@ -350,50 +360,51 @@
         return self.get_totals().sum()
 
     def get_totals(self) -> NDArray[np.float_]:
         return np.array([patch.total for patch in self._patches.values()])
 
     @property
     def centers(self) -> CoordSky:
-        return CoordSky.from_coords(
-            [self._patches[pid].center for pid in self.ids])
+        return CoordSky.from_coords([self._patches[pid].center for pid in self.ids])
 
     @property
     def radii(self) -> DistSky:
-        return DistSky.from_dists(
-            [self._patches[pid].radius for pid in self.ids])
+        return DistSky.from_dists([self._patches[pid].radius for pid in self.ids])
 
     def correlate(
         self,
         config: Configuration,
         binned: bool,
         other: ScipyCatalog | None = None,
         linkage: PatchLinkage | None = None,
-        progress: bool = False
+        progress: bool = False,
     ) -> NormalisedCounts | dict[str, NormalisedCounts]:
         super().correlate(config, binned, other, linkage)
 
         auto = other is None
         if not auto and not isinstance(other, ScipyCatalog):
             raise TypeError
 
         if linkage is None:
             cat_for_linkage = self
             if not auto:
                 if len(other) > len(self):
                     cat_for_linkage = other
             linkage = PatchLinkage.from_setup(config, cat_for_linkage)
         patch1_list, patch2_list = linkage.get_patches(
-            self, other, config.backend.crosspatch)
+            self, other, config.backend.crosspatch
+        )
         n_jobs = len(patch1_list)
 
         # prepare job scheduling
         pool = ParallelHelper(
             function=_count_pairs_thread,
-            n_items=n_jobs, num_threads=config.backend.get_threads(n_jobs))
+            n_items=n_jobs,
+            num_threads=config.backend.get_threads(n_jobs),
+        )
         # patch1: PatchCatalog
         pool.add_iterable(patch1_list)
         # patch2: PatchCatalog
         pool.add_iterable(patch2_list)
         # scales: Sequence[Scale]
         pool.add_constant(list(config.scales))
         # cosmology: TypeCosmology
@@ -413,15 +424,16 @@
         n_bins = len(binning)
         n_patches = self.n_patches
         # set up data to repack task results from [ids->scale] to [scale->ids]
         totals1 = np.zeros((n_patches, n_bins))
         totals2 = np.zeros((n_patches, n_bins))
         count_dict = {
             str(scale): PatchedCount.zeros(binning, n_patches, auto=auto)
-            for scale in config.scales}
+            for scale in config.scales
+        }
         # run the scheduled tasks
         result_iter = pool.iter_result(ordered=False)
         # add an optional progress bar
         if progress:
             result_iter = job_progress_bar(result_iter, total=pool.n_jobs())
         for patch_data in result_iter:
             id1, id2 = patch_data.patches
@@ -431,37 +443,36 @@
             # record counts at each scale
             for scale_key, count in patch_data.counts.items():
                 if auto and id1 == id2:
                     count = count * 0.5  # autocorr. pairs are counted twice
                 count_dict[scale_key].set_measurement((id1, id2), count)
 
         total = PatchedTotal(  # not scale-dependent
-            binning=binning,
-            totals1=totals1,
-            totals2=totals2,
-            auto=auto)
+            binning=binning, totals1=totals1, totals2=totals2, auto=auto
+        )
         return pack_results(count_dict, total)
 
     def true_redshifts(
         self,
         config: Configuration,
         sampling_config: ResamplingConfig | None = None,
-        progress: bool = False
+        progress: bool = False,
     ) -> HistData:
         super().true_redshifts(config)
         if sampling_config is None:
             sampling_config = ResamplingConfig()  # default values
 
         if not self.has_redshifts():
             raise ValueError("catalog has no redshifts")
         # compute the reshift histogram in each patch
         pool = ParallelHelper(
             function=_histogram_thread,
             n_items=self.n_patches,
-            num_threads=config.backend.get_threads(self.n_patches))
+            num_threads=config.backend.get_threads(self.n_patches),
+        )
         # patch: PatchCatalog
         pool.add_iterable(self._patches.values())
         # NDArray[np.float_]
         pool.add_constant(config.binning.zbins)
         iterator = pool.iter_result()
         if progress:
             iterator = job_progress_bar(iterator)
@@ -472,8 +483,9 @@
         patch_idx = sampling_config.get_samples(self.n_patches)
         nz_data = hist_counts.sum(axis=0)
         nz_samp = np.sum(hist_counts[patch_idx], axis=1)
         return HistData(
             binning=binning,
             data=nz_data,
             samples=nz_samp,
-            method=sampling_config.method)
+            method=sampling_config.method,
+        )
```

### Comparing `yet_another_wizz-2.5/src/yaw/catalogs/scipy/kdtree.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/kdtree.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from scipy.spatial import cKDTree
 
 from yaw.core.coordinates import Coordinate, DistSky
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import NDArray
 
+__all__ = ["SphericalKDTree"]
+
 
 class InvalidScalesError(Exception):
     pass
 
 
 class SphericalKDTree:
     """Wrapper around :obj:`scipy.spatial.cKDTree` that represents angular
@@ -26,15 +28,15 @@
 
     _total = None
 
     def __init__(
         self,
         position: Coordinate,
         weights: NDArray[np.float_] | None = None,
-        leafsize: int = 16
+        leafsize: int = 16,
     ) -> None:
         """Build a new tree from a set of coordinates.
 
         Args:
             position (:obj:`yaw.coordinates.Coordinate`):
                 A vector of coordinates in either angular or 3D coordiantes, is
                 converted to 3D coordinates if needed.
@@ -45,15 +47,15 @@
                 with no further childs.
         """
         position = np.atleast_2d(position.to_3d().values)
         self.tree = cKDTree(position, leafsize)
         if weights is None:
             self.weights = np.ones(len(position))
         else:
-            assert(len(weights) == len(position))
+            assert len(weights) == len(position)
             self.weights = np.asarray(weights)
 
     def __len__(self) -> int:
         return len(self.weights)
 
     @property
     def total(self) -> float:
@@ -63,15 +65,15 @@
         return self._total
 
     def count(
         self,
         other: SphericalKDTree,
         scales: NDArray[np.float_],
         dist_weight_scale: float | None = None,
-        weight_res: int = 50
+        weight_res: int = 50,
     ) -> NDArray:
         """Count pairs on a set of angular scales.
 
         Pairs are counted with in a range of minimum and maximum angle in
         radian. If multiple scales are provided, the set of scales is converted
         into a list of radial bins. After counting, the binned counts are summed
         to obtain the counts for the (potentially overlapping) input scales.
@@ -97,41 +99,43 @@
                 The number of logarithmic angular bins used to compute the
                 angular weights. Ignored if no power-law index is set.
 
         Returns:
             :obj:`NDArray`:
                 The pair counts for each input scale, with optional inidividual
                 point weights and radial weights applied.
-        
+
         .. Warning::
 
             For autocorrelation measurements, ``other`` must be the same
             tree as the calling instance itself. This will results in pairs
             being counted twice, as they normally would be in the cross-tree
             counting case.
         """
         # unpack query scales
         scales = np.atleast_2d(scales)
         if scales.shape[1] != 2:
-            raise InvalidScalesError(
-                "'scales' must be composed of tuples of length 2")
+            raise InvalidScalesError("'scales' must be composed of tuples of length 2")
         if np.any(scales <= 0.0):
             raise InvalidScalesError("scales must be positive (r > 0)")
         if np.any(scales > np.pi):
             raise InvalidScalesError("scales exceed 180 deg")
         log_scales = np.log10(scales).flatten()
         # construct bins
         rlog_edges = np.linspace(log_scales.min(), log_scales.max(), weight_res)
         rlog_edges = np.array(sorted(set(rlog_edges) | set(log_scales)))
-        r_edges = 10 ** rlog_edges
+        r_edges = 10**rlog_edges
         # count pairs
         try:
             counts = self.tree.count_neighbors(
-                other.tree, DistSky(r_edges).to_3d().values,
-                weights=(self.weights, other.weights), cumulative=False)
+                other.tree,
+                DistSky(r_edges).to_3d().values,
+                weights=(self.weights, other.weights),
+                cumulative=False,
+            )
         except IndexError:
             counts = np.zeros_like(r_edges)
         counts = counts[1:]  # discard counts with 0 < R <= r_min
         # apply the distance weights
         if dist_weight_scale is not None:
             rlog_centers = (rlog_edges[:-1] + rlog_edges[1:]) / 2.0
             counts *= (10**rlog_centers) ** dist_weight_scale
```

### Comparing `yet_another_wizz-2.5/src/yaw/catalogs/scipy/patches.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/patches.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,38 +4,38 @@
 from collections.abc import Iterator
 from typing import TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
 from scipy.cluster import vq
 
-from yaw.core.coordinates import (
-    Coordinate, Coord3D, CoordSky, Distance, DistSky)
-
 from yaw.catalogs.scipy.kdtree import SphericalKDTree
+from yaw.core.coordinates import Coord3D, Coordinate, CoordSky, Distance, DistSky
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import NDArray
     from pandas import DataFrame, Interval
 
+__all__ = ["PatchCatalog"]
+
 
 class NotAPatchFileError(Exception):
     pass
 
 
 class CachingError(Exception):
     pass
 
 
 def patch_id_from_path(fpath: str) -> int:
     """Extract the patch ID from the file name in the cache directory"""
     ext = ".feather"
     if not fpath.endswith(ext):
         raise NotAPatchFileError("input must be a .feather file")
-    prefix, patch_id = fpath[:-len(ext)].rsplit("_", 1)
+    prefix, patch_id = fpath[: -len(ext)].rsplit("_", 1)
     return int(patch_id)
 
 
 class PatchCatalog:
     """Represents a single spatial patch of a :obj:`ScipyCatalog`.
 
     A patch holds the data from single patch of the catalogue and provides
@@ -60,20 +60,20 @@
     def __init__(
         self,
         id: int,
         data: DataFrame,
         cachefile: str | None = None,
         center: Coordinate | None = None,
         radius: Distance | None = None,
-        degrees: bool = True
+        degrees: bool = True,
     ) -> None:
         """Create a new patch from a data frame.
 
         Coordiantes are converted to radian. If a cache path is provided, a
-        cache file is created and the data is dropped from memory.     
+        cache file is created and the data is dropped from memory.
 
         Args:
             id (:obj:`int`):
                 Unique index of the patch.
             data (:obj:`pandas.DataFrame`):
                 Data frame with columns ``ra``, ``dec`` (by default assumed to
                 be in degrees) and optionally ``weights``, ``redshift`` if
@@ -93,30 +93,29 @@
         if "ra" not in data:
             raise KeyError("right ascension column ('ra') is required")
         if "dec" not in data:
             raise KeyError("declination column ('dec') is required")
         if not set(data.columns) <= set(["ra", "dec", "redshift", "weights"]):
             raise KeyError(
                 "'data' contains unidentified columns, optional columns are "
-                "restricted to 'redshift' and 'weights'")
+                "restricted to 'redshift' and 'weights'"
+            )
         # next line is crucial, otherwise lines below modify data inplace
         self._data = data.copy()
         if degrees:
             self._data["ra"] = np.deg2rad(data["ra"])
             self._data["dec"] = np.deg2rad(data["dec"])
         # if there is a file path, store the file
         if cachefile is not None:
             self.cachefile = cachefile
             self._data.to_feather(cachefile)
         self._init(center, radius)
 
     def _init(
-        self,
-        center: Coordinate | None = None,
-        radius: Distance | None = None
+        self, center: Coordinate | None = None, radius: Distance | None = None
     ) -> None:
         self._len = len(self._data)
         self._has_z = "redshift" in self._data
         self._has_weights = "weights" in self._data
         if self.has_weights():
             self._total = float(self.weights.sum())
         else:
@@ -155,15 +154,15 @@
         return self._len
 
     @classmethod
     def from_cached(
         cls,
         cachefile: str,
         center: Coordinate | None = None,
-        radius: Distance | None = None
+        radius: Distance | None = None,
     ) -> PatchCatalog:
         """Restore the patch instance from its cache file.
 
         Optionally, the center and radius of the patch can be provided to avoid
         recomputing these quantities.
 
         Args:
@@ -197,25 +196,24 @@
     def require_loaded(self) -> None:
         """Raise a :obj:`CachingError` if the data is not present in memory."""
         if not self.is_loaded():
             raise CachingError("data is not loaded")
 
     def load(self, use_threads: bool = True) -> None:
         """Load the data from the cache file into memory.
-        
+
         Raises a :obj:`CachingError` if no cache file is sepcified."""
         if not self.is_loaded():
             if self.cachefile is None:
                 raise CachingError("no datapath provided to load the data")
-            self._data = pd.read_feather(
-                self.cachefile, use_threads=use_threads)
+            self._data = pd.read_feather(self.cachefile, use_threads=use_threads)
 
     def unload(self) -> None:
         """Drop the data from memory.
-        
+
         Raises a :obj:`CachingError` if no cache file is sepcified."""
         if self.cachefile is None:
             raise CachingError("no datapath provided to unload the data")
         self._data = None
         gc.collect()
 
     def has_redshifts(self) -> bool:
@@ -232,31 +230,31 @@
         the patch data."""
         self.require_loaded()
         return self._data
 
     @property
     def ra(self) -> NDArray[np.float_]:
         """Get an array of the right ascension values in radians.
-        
+
         Raises a :obj:`CachingError` if data is not loaded."""
         self.require_loaded()
         return self._data["ra"].to_numpy()
 
     @property
     def dec(self) -> NDArray[np.float_]:
         """Get an array of the declination values in radians.
-        
+
         Raises a :obj:`CachingError` if data is not loaded."""
         self.require_loaded()
         return self._data["dec"].to_numpy()
 
     @property
     def pos(self) -> CoordSky:
         """Get a vector of the object sky positions in radians.
-        
+
         Raises a :obj:`CachingError` if data is not loaded.
 
         Returns:
             :obj:`yaw.core.coordinates.CoordSky`
         """
         self.require_loaded()
         return CoordSky(self.ra, self.dec)
@@ -283,44 +281,42 @@
         else:
             return None
 
     @property
     def total(self) -> float:
         """Get the sum of weights or the number of objects if weights are not
         available.
-        
+
         Available even if no data is loaded."""
         return self._total
 
     @property
     def center(self) -> CoordSky:
         """Get the patch centers in radians.
-        
+
         Available even if no data is loaded.
 
         Returns:
             :obj:`yaw.core.coordinates.CoordSky`
         """
         return self._center.to_sky()
 
     @property
     def radius(self) -> DistSky:
         """Get the patch size in radians.
-        
+
         Available even if no data is loaded.
 
         Returns:
             :obj:`yaw.core.coordinates.DistSky`
         """
         return self._radius
 
     def iter_bins(
-        self,
-        z_bins: NDArray[np.float_],
-        allow_no_redshift: bool = False
+        self, z_bins: NDArray[np.float_], allow_no_redshift: bool = False
     ) -> Iterator[tuple[Interval, PatchCatalog]]:
         """Iterate the patch in bins of redshift.
 
         Args:
             z_bins (:obj:`NDArray`):
                 Edges of the redshift bins.
             allow_no_redshift (:obj:`bool`):
@@ -335,82 +331,80 @@
         """
         if not allow_no_redshift and not self.has_redshifts():
             raise ValueError("no redshifts for iteration provdided")
         if allow_no_redshift:
             for intv in pd.IntervalIndex.from_breaks(z_bins, closed="left"):
                 yield intv, self
         else:
-            for intv, bin_data in self._data.groupby(
-                    pd.cut(self.redshifts, z_bins)):
+            for intv, bin_data in self._data.groupby(pd.cut(self.redshifts, z_bins)):
                 yield intv, PatchCatalog(
-                    self.id, bin_data, degrees=False,
-                    center=self._center, radius=self._radius)
+                    self.id,
+                    bin_data,
+                    degrees=False,
+                    center=self._center,
+                    radius=self._radius,
+                )
 
     def get_tree(self, **kwargs) -> SphericalKDTree:
         """Build a :obj:`SphericalKDTree` from the patch data coordiantes."""
         tree = SphericalKDTree(self.pos, self.weights, **kwargs)
         tree._total = self.total  # no need to recompute this
         return tree
 
 
 # Determine patch centers with k-means clustering. The implementation in
 # treecorr is quite good, but might not be available. Implement a fallback using
 # the scipy.cluster module.
 
-def assign_patches(
-    centers: Coordinate,
-    position: Coordinate
-) -> NDArray[np.int_]:
+
+def assign_patches(centers: Coordinate, position: Coordinate) -> NDArray[np.int_]:
     """Assign objects based on their coordinate to a list of points based on
     proximit."""
     patches, dist = vq.vq(position.to_3d().values, centers.to_3d().values)
     return patches
 
 
 try:
     import treecorr
 
     def treecorr_patches(
-        position: Coordinate,
-        n_patches: int,
-        **kwargs
+        position: Coordinate, n_patches: int, **kwargs
     ) -> tuple[Coord3D, NDArray[np.int_]]:
         """Use the *k*-means clustering algorithm of :obj:`treecorr.Catalog` to
         generate spatial patches and assigning objects to those patches.
         """
         position = position.to_sky()
         cat = treecorr.Catalog(
-            ra=position.ra, ra_units="radians",
-            dec=position.dec, dec_units="radians",
-            npatch=n_patches)
+            ra=position.ra,
+            ra_units="radians",
+            dec=position.dec,
+            dec_units="radians",
+            npatch=n_patches,
+        )
         xyz = np.atleast_2d(cat.patch_centers)
         centers = Coord3D.from_array(xyz)
         if n_patches == 1:
             patches = np.zeros(len(position), dtype=np.int_)
         else:
             patches = assign_patches(centers=centers, position=position)
         del cat  # might not be necessary
         return centers, patches
 
     create_patches = treecorr_patches
 
 except ImportError:
 
     def scipy_patches(
-        position: Coordinate,
-        n_patches: int,
-        n_max: int = 500_000
+        position: Coordinate, n_patches: int, n_max: int = 500_000
     ) -> tuple[Coord3D, NDArray[np.int_]]:
         """Use the *k*-means clustering algorithm of :obj:`scipy.cluster` to
         generate spatial patches and assigning objects to those patches.
         """
         position = position.to_3d()
-        subset = np.random.randint(
-            0, len(position), size=min(n_max, len(position)))
+        subset = np.random.randint(0, len(position), size=min(n_max, len(position)))
         # place on unit sphere to avoid coordinate distortions
-        centers, _ = vq.kmeans2(
-            position[subset].values, n_patches, minit="points")
+        centers, _ = vq.kmeans2(position[subset].values, n_patches, minit="points")
         centers = Coord3D.from_array(centers)
         patches = assign_patches(centers=centers, position=position)
         return centers, patches
 
     create_patches = scipy_patches
```

### Comparing `yet_another_wizz-2.5/src/yaw/catalogs/treecorr/catalog.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/treecorr/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,67 +1,75 @@
 from __future__ import annotations
 
 import itertools
 import os
 import sys
 from collections.abc import Iterator
 from typing import TYPE_CHECKING, Dict, NoReturn, Tuple
+
 try:  # pragma: no cover
     from typing import TypeAlias
 except ImportError:  # pragma: no cover
     from typing_extensions import TypeAlias
 
 import numpy as np
 import pandas as pd
 from numpy.typing import NDArray
 from treecorr import Catalog, NNCorrelation
 
 from yaw.catalogs import BaseCatalog
 from yaw.config import Configuration, ResamplingConfig
-from yaw.core.coordinates import Coordinate, Coord3D, CoordSky, DistSky
+from yaw.core.coordinates import Coord3D, Coordinate, CoordSky, DistSky
 from yaw.core.logging import TimedLog
 from yaw.correlation.paircounts import (
-    NormalisedCounts, PatchedCount, PatchedTotal, pack_results)
+    NormalisedCounts,
+    PatchedCount,
+    PatchedTotal,
+    pack_results,
+)
 from yaw.redshifts import HistData
 
 if TYPE_CHECKING:  # pragma: no cover
     from pandas import DataFrame, Interval
+
     from yaw.catalogs import PatchLinkage
 
+__all__ = ["EmptyCatalog", "TreecorrCatalog"]
+
 
 TypeNNResult: TypeAlias = Dict[Tuple[int, int], NNCorrelation]  # supports py3.8
 
 
 def _iter_bin_masks(
-    data: NDArray,
-    bins: NDArray,
-    closed: str = "left"
+    data: NDArray, bins: NDArray, closed: str = "left"
 ) -> Iterator[tuple[Interval, NDArray[np.bool_]]]:
     """Split data into bins and return an iterator that yields the boolean masks
     that select the data of the current bin out of the input data array."""
     if closed not in ("left", "right"):
         raise ValueError("'closed' must be either of 'left', 'right'")
     intervals = pd.IntervalIndex.from_breaks(bins, closed=closed)
-    bin_ids = np.digitize(data, bins, right=(closed=="right"))
+    bin_ids = np.digitize(data, bins, right=(closed == "right"))
     for i, interval in enumerate(intervals, 1):
         yield interval, (bin_ids == i)
 
 
 def take_subset(
-    cat: TreecorrCatalog,
-    items: NDArray[np.bool_] | NDArray[np.int_] | slice
+    cat: TreecorrCatalog, items: NDArray[np.bool_] | NDArray[np.int_] | slice
 ) -> TreecorrCatalog | EmptyCatalog:
     """Construct a new TreecorrCatalog with a subset of its entries."""
     ra = cat.ra[items]
     if len(ra) == 0:
         return EmptyCatalog(n_patches=cat.n_patches)
     kwargs = dict(
-        ra=ra, ra_units="radian",
-        dec=cat.dec[items], dec_units="radian",
-        patch=cat.patch[items])
+        ra=ra,
+        ra_units="radian",
+        dec=cat.dec[items],
+        dec_units="radian",
+        patch=cat.patch[items],
+    )
     if cat.has_redshifts():
         kwargs["r"] = cat.redshifts[items]
     if cat.has_weights():
         kwargs["w"] = cat.weights[items]
     return TreecorrCatalog.from_treecorr(Catalog(**kwargs))
 
 
@@ -82,15 +90,15 @@
 
 
 class TreecorrCatalog(BaseCatalog):
     """An implementation of the :obj:`BaseCatalog` using ``TreeCorr`` for the
     pair counting.
 
     .. Note::
-    
+
         The current implementation is not very efficient, because the internal
         fields of the underlying :obj:`treecorr.Catalog` must be rebuilt every
         time the catalog is iterated in redshift bins for the pair counting.
 
     .. Warning::
 
         Currently this backend does not support restoration from cache and
@@ -106,75 +114,75 @@
         *,
         patch_name: str | None = None,
         patch_centers: BaseCatalog | Coordinate | None = None,
         n_patches: int | None = None,
         redshift_name: str | None = None,
         weight_name: str | None = None,
         cache_directory: str | None = None,
-        progress: bool = False
+        progress: bool = False,
     ) -> None:
         # construct the underlying TreeCorr catalogue
         kwargs = dict()
         if cache_directory is not None:
             kwargs["save_patch_dir"] = cache_directory
             if not os.path.exists(cache_directory):
                 raise FileNotFoundError(
-                    f"patch directory does not exist: '{cache_directory}'")
+                    f"patch directory does not exist: '{cache_directory}'"
+                )
             self._logger.info(f"using cache directory '{cache_directory}'")
 
         if n_patches is not None:
             kwargs["npatch"] = n_patches
             log_msg = f"creating {n_patches} patches"
         elif patch_name is not None:
             kwargs["patch"] = data[patch_name]
-            log_msg = f"splitting data into predefined patches"
+            log_msg = "splitting data into predefined patches"
         elif isinstance(patch_centers, BaseCatalog):
             kwargs["patch_centers"] = patch_centers.centers.to_3d().values
             n_patches = patch_centers.n_patches
             log_msg = f"applying {n_patches} patches from external data"
         elif isinstance(patch_centers, Coordinate):
             centers = patch_centers.to_3d()
             kwargs["patch_centers"] = centers.values
             n_patches = len(centers)
             log_msg = f"applying {n_patches} patches from external data"
         else:
             raise ValueError(
                 "either of 'patch_name', 'patch_centers', or 'n_patches' "
-                "must be provided")
+                "must be provided"
+            )
 
         with TimedLog(self._logger.info, log_msg):
             self._catalog = Catalog(
-                ra=data[ra_name], ra_units="degrees",
-                dec=data[dec_name], dec_units="degrees",
+                ra=data[ra_name],
+                ra_units="degrees",
+                dec=data[dec_name],
+                dec_units="degrees",
                 r=None if redshift_name is None else data[redshift_name],
                 w=None if weight_name is None else data[weight_name],
-                **kwargs)
+                **kwargs,
+            )
             self._make_patches()
 
         if cache_directory is not None:
             self.unload()
 
     @classmethod
-    def from_cache(
-        cls,
-        cache_directory: str,
-        progress: bool = False
-    ) -> NoReturn:
+    def from_cache(cls, cache_directory: str, progress: bool = False) -> NoReturn:
         """
         Raises:
             NotImplementedError
 
         .. Warning::
 
             Currently this backend does not support restoration from cache.
         """
-        #super().from_cache(cache_directory)
-        #self._make_patches()
-        raise NotImplementedError(
-            "restoring from cache is currently not supported")
+        # super().from_cache(cache_directory)
+        # self._make_patches()
+        raise NotImplementedError("restoring from cache is currently not supported")
 
     @classmethod
     def from_treecorr(cls, cat: Catalog) -> TreecorrCatalog:
         """Create a new instace from a :obj:`treecorr.Catalog`."""
         new = cls.__new__(cls)
         new._catalog = cat
         new._make_patches()
@@ -284,17 +292,15 @@
             # compute the angular radius from the maximum separation in 3D
             position = patch.pos.to_3d()
             radius = patch.centers.to_3d().distance(position).max()
             radii.append(radius.to_sky())
         return DistSky.from_dists(radii)
 
     def iter_bins(
-        self,
-        z_bins: NDArray[np.float_],
-        allow_no_redshift: bool = False
+        self, z_bins: NDArray[np.float_], allow_no_redshift: bool = False
     ) -> Iterator[tuple[Interval, TreecorrCatalog | EmptyCatalog]]:
         """Iterate the catalogue in bins of redshift.
 
         Args:
             z_bins (:obj:`NDArray`):
                 Edges of the redshift bins.
             allow_no_redshift (:obj:`bool`):
@@ -318,28 +324,28 @@
 
     def correlate(
         self,
         config: Configuration,
         binned: bool,
         other: TreecorrCatalog = None,
         linkage: PatchLinkage | None = None,
-        progress: bool = False
+        progress: bool = False,
     ) -> NormalisedCounts | dict[str, NormalisedCounts]:
         super().correlate(config, binned, other, linkage)
 
         auto = other is None
         if not auto and not isinstance(other, TreecorrCatalog):
             raise TypeError
         nncorr_config = dict(
             sep_units="radian",
             metric="Arc",
-            nbins=(
-                1 if config.scales.rweight is None else config.scales.rbin_num),
+            nbins=(1 if config.scales.rweight is None else config.scales.rbin_num),
             bin_slop=config.backend.rbin_slop,
-            num_threads=config.backend.get_threads())
+            num_threads=config.backend.get_threads(),
+        )
 
         # bin the catalogues if necessary
         cats1 = self.iter_bins(config.binning.zbins)
         if auto:
             cats2 = itertools.repeat((None, None))
         else:
             if binned:
@@ -351,89 +357,88 @@
         binning = pd.IntervalIndex.from_breaks(config.binning.zbins)
         n_bins = len(binning)
         n_patches = self.n_patches
         totals1 = np.zeros((n_patches, n_bins))
         totals2 = np.zeros((n_patches, n_bins))
         count_dict = {
             str(scale): PatchedCount.zeros(binning, n_patches, auto=auto)
-            for scale in config.scales}
+            for scale in config.scales
+        }
 
         # iterate the bins and compute the correlation
         self._logger.debug(
-            f"running treecorr on {config.backend.get_threads()} threads")
+            f"running treecorr on {config.backend.get_threads()} threads"
+        )
         for i, ((intv, bincat1), (_, bincat2)) in enumerate(zip(cats1, cats2)):
             if progress:
                 _prog_msg = f"processing bin {i+1} / {n_bins}\r"
                 sys.stderr.write(_prog_msg)
                 sys.stderr.flush()
 
             angles = [
-                scale.to_radian(intv.mid, config.cosmology)
-                for scale in config.scales]
+                scale.to_radian(intv.mid, config.cosmology) for scale in config.scales
+            ]
             # extract the total number of objects per patch
             totals1[:, i] = bincat1.get_totals()
             if bincat2 is None:
                 totals2[:, i] = totals1[:, i]
             else:
                 totals2[:, i] = bincat2.get_totals()
 
             # trivial case: no data in redshift interval, no counts to update
-            if (
-                isinstance(bincat1, EmptyCatalog) or
-                isinstance(bincat2, EmptyCatalog)
-            ):
+            if isinstance(bincat1, EmptyCatalog) or isinstance(bincat2, EmptyCatalog):
                 continue
 
             for scale, (ang_min, ang_max) in zip(config.scales, angles):
                 # run the correlation measurement
                 correlation = NNCorrelation(
-                    min_sep=ang_min, max_sep=ang_max, **nncorr_config)
+                    min_sep=ang_min, max_sep=ang_max, **nncorr_config
+                )
                 correlation.process(
                     bincat1.to_treecorr(),
-                    None if bincat2 is None else bincat2.to_treecorr())
+                    None if bincat2 is None else bincat2.to_treecorr(),
+                )
 
                 # extract the pair counts
                 scale_counts = count_dict[str(scale)]
                 result: TypeNNResult = correlation.results
                 for (pid1, pid2), corr_result in result.items():
                     scale_counts.counts[pid1, pid2, i] = corr_result.weight
 
         if progress:
             sys.stderr.write((" " * len(_prog_msg)) + "\r")  # clear line
 
         total = PatchedTotal(  # not scale-dependent
-            binning=binning,
-            totals1=totals1,
-            totals2=totals2,
-            auto=auto)
+            binning=binning, totals1=totals1, totals2=totals2, auto=auto
+        )
         return pack_results(count_dict, total)
 
     def true_redshifts(
         self,
         config: Configuration,
         sampling_config: ResamplingConfig | None = None,
-        progress: bool = False
+        progress: bool = False,
     ) -> HistData:
         if sampling_config is None:
             sampling_config = ResamplingConfig()  # default values
 
         super().true_redshifts(config)
         if not self.has_redshifts():
             raise ValueError("catalog has no redshifts")
         # compute the reshift histogram in each patch
         hist_counts = []
         for patch in iter(self):
-            counts, bins = np.histogram(
-                patch.r, config.binning.zbins, weights=patch.w)
+            counts, bins = np.histogram(patch.r, config.binning.zbins, weights=patch.w)
             hist_counts.append(counts)
         hist_counts = np.array(hist_counts)
 
         # construct the output data samples
         binning = pd.IntervalIndex.from_breaks(config.binning.zbins)
         patch_idx = sampling_config.get_samples(self.n_patches)
         nz_data = hist_counts.sum(axis=0)
         nz_samp = np.sum(hist_counts[patch_idx], axis=1)
         return HistData(
             binning=binning,
             data=nz_data,
             samples=nz_samp,
-            method=sampling_config.method)
+            method=sampling_config.method,
+        )
```

### Comparing `yet_another_wizz-2.5/src/yaw/config/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/config/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,12 +22,25 @@
 ``yaw.config.DEFAULT``), parameters that support a fixed set of options can be
 accessed through :obj:`yaw.config.OPTIONS`, an instance of the
 :obj:`~yaw.config.options.Options` generating class.
 """
 
 from yaw.config import default as DEFAULT
 from yaw.config.options import OPTIONS
+
+# isort: split
 from yaw.config.backend import BackendConfig
 from yaw.config.binning import AutoBinningConfig, ManualBinningConfig
 from yaw.config.config import Configuration
 from yaw.config.resampling import ResamplingConfig
 from yaw.config.scales import ScalesConfig
+
+__all__ = [
+    "DEFAULT",
+    "BackendConfig",
+    "AutoBinningConfig",
+    "ManualBinningConfig",
+    "Configuration",
+    "OPTIONS",
+    "ResamplingConfig",
+    "ScalesConfig",
+]
```

### Comparing `yet_another_wizz-2.5/src/yaw/config/backend.py` & `yet_another_wizz-2.5.post0/src/yaw/config/backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 import os
 from dataclasses import dataclass, field
-from typing import Any
 
+from yaw.config import default as DEFAULT
 from yaw.core.abc import DictRepresentation
 from yaw.core.docs import Parameter
 
-from yaw.config import default as DEFAULT
+__all__ = ["BackendConfig"]
 
 
 @dataclass(frozen=True)
 class BackendConfig(DictRepresentation):
     """Configuration of backends used for correlation measurements.
-    
+
     Args:
         thread_num (:obj:`int`, optional):
             Number of threads to use for parallel processing.
         crosspatch (:obj:`bool`, optional):
             Whether to count pairs across patch boundaries (``scipy`` backend
             only).
         rbin_slop (:obj:`int`, optional):
@@ -26,42 +26,47 @@
 
     # general
     thread_num: int | None = field(
         default=DEFAULT.Backend.thread_num,
         metadata=Parameter(
             type=int,
             help="default number of threads to use",
-            default_text="(default: all)"))
+            default_text="(default: all)",
+        ),
+    )
     """Number of threads to use for parallel processing."""
     # scipy
     crosspatch: bool = field(
         default=DEFAULT.Backend.crosspatch,
         metadata=Parameter(
             type=bool,
-            help="whether to count pairs across patch boundaries (scipy "
-                 "backend only)"))
+            help="whether to count pairs across patch boundaries (scipy backend only)",
+        ),
+    )
     """Whether to count pairs across patch boundaries (``scipy`` backend only).
     """
     # treecorr
     rbin_slop: float = field(
         default=DEFAULT.Backend.rbin_slop,
         metadata=Parameter(
             type=float,
             help="TreeCorr 'rbin_slop' parameter",
             default_text="(default: %(default)s), without 'rweight' this just "
-                         "a single radial bin, otherwise 'rbin_num'"))
+            "a single radial bin, otherwise 'rbin_num'",
+        ),
+    )
     """`TreeCorr` ``rbin_slop`` parameter (``treecorr`` backend only)."""
 
     def __post_init__(self) -> None:
         if self.thread_num is None:
             object.__setattr__(self, "thread_num", os.cpu_count())
 
     def get_threads(self, max=None) -> int:
         """Get the number of threads for parallel processing.
-        
+
         The value is capped at the number of logical cores available.
         """
         if self.thread_num is None:
             thread_num = os.cpu_count()
         else:
             thread_num = self.thread_num
         if max is not None:
```

### Comparing `yet_another_wizz-2.5/src/yaw/config/binning.py` & `yet_another_wizz-2.5.post0/src/yaw/config/binning.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 
 import logging
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any
 
 import numpy as np
 
+from yaw.config import OPTIONS
+from yaw.config import default as DEFAULT
+from yaw.config.utils import ConfigError
 from yaw.core.abc import DictRepresentation
 from yaw.core.cosmology import BinFactory, TypeCosmology
 from yaw.core.docs import Parameter
 from yaw.core.math import array_equal
 
-from yaw.config import default as DEFAULT, OPTIONS
-from yaw.config.utils import ConfigError
-
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import NDArray
 
+__all__ = ["AutoBinningConfig", "ManualBinningConfig", "make_binning_config"]
+
 
 logger = logging.getLogger(__name__)
 
 
 class BaseBinningConfig(DictRepresentation):
     """Base class for redshift binning configuration."""
 
@@ -45,17 +47,20 @@
     Args:
         zbins (:obj:`NDArray`):
             Edges of redshift bins, must increase monotonically.
     """
 
     zbins: NDArray[np.float_] = field(
         metadata=Parameter(
-            type=float, nargs="*",
+            type=float,
+            nargs="*",
             help="list of custom redshift bin edges, if provided, other "
-                 "binning parameters are omitted, method is set to 'manual'"))
+            "binning parameters are omitted, method is set to 'manual'",
+        )
+    )
 
     def __post_init__(self) -> None:
         if len(self.zbins) < 2:
             raise ConfigError("'zbins' must have at least two edges")
         BinFactory.check(self.zbins)
         object.__setattr__(self, "zbins", np.asarray(self.zbins))
 
@@ -81,29 +86,25 @@
 
     @property
     def zbin_num(self) -> int:
         """Number of redshift bins."""
         return len(self.zbins) - 1
 
     @classmethod
-    def from_dict(
-        cls,
-        the_dict: dict[str, Any],
-        **kwargs
-    ) -> ManualBinningConfig:
+    def from_dict(cls, the_dict: dict[str, Any], **kwargs) -> ManualBinningConfig:
         return cls(np.asarray(the_dict["zbins"]))
 
     def to_dict(self) -> dict[str, Any]:
         return dict(method=self.method, zbins=self.zbins.tolist())
 
 
 @dataclass(frozen=True, repr=False)
 class AutoBinningConfig(BaseBinningConfig):
     """Configuration that generates a redshift binning.
-    
+
     To generate a redshift binning use the :meth:`generate` method.
 
     Args:
         zbins (:obj:`NDArray`):
             Edges of redshift bins, must increase monotonically.
         method (:obj:`str`):
             Method used to create redshift binning, either of
@@ -111,55 +112,62 @@
     """
 
     zbins: NDArray[np.float_]
     method: str = field(
         default=DEFAULT.Configuration.binning.method,
         metadata=Parameter(
             choices=OPTIONS.binning,
-            help="redshift binning method, 'logspace' means equal size in "
-                 "log(1+z)",
-            default_text="(default: %(default)s)"))
+            help="redshift binning method, 'logspace' means equal size in log(1+z)",
+            default_text="(default: %(default)s)",
+        ),
+    )
     """Method used to create redshift binning, see
     :obj:`~yaw.config.options.Options.binning`."""
     zmin: float = field(
         init=False,
         metadata=Parameter(
             type=float,
             help="lower redshift limit",
-            default_text="(default: %(default)s)"))
+            default_text="(default: %(default)s)",
+        ),
+    )
     """Lowest redshift bin edge."""
     zmax: float = field(
         init=False,
         metadata=Parameter(
             type=float,
             help="upper redshift limit",
-            default_text="(default: %(default)s)"))
+            default_text="(default: %(default)s)",
+        ),
+    )
     """Highest redshift bin edge."""
     zbin_num: int = field(
         default=DEFAULT.AutoBinning.zbin_num,
         init=False,
         metadata=Parameter(
             type=int,
             help="number of redshift bins",
-            default_text="(default: %(default)s)"))
+            default_text="(default: %(default)s)",
+        ),
+    )
     """Number of redshift bins."""
 
     def __post_init__(self) -> None:
         object.__setattr__(self, "zmin", float(self.zbins[0]))
         object.__setattr__(self, "zmax", float(self.zbins[-1]))
-        object.__setattr__(self, "zbin_num", len(self.zbins)-1)
+        object.__setattr__(self, "zbin_num", len(self.zbins) - 1)
 
     @classmethod
     def generate(
         cls,
         zmin: float,
         zmax: float,
         zbin_num: int = DEFAULT.AutoBinning.zbin_num,
         method: str = DEFAULT.AutoBinning.method,
-        cosmology: TypeCosmology | None = None
+        cosmology: TypeCosmology | None = None,
     ) -> AutoBinningConfig:
         """Generate a new redshift binning configuration.
 
         Generates a specified number of bins between a lower and upper redshift
         limit. The spacing of the bins depends the generation method, the
         default is a linear spacing.
 
@@ -173,15 +181,15 @@
             method (:obj:`str`, optional):
                 Method used to create redshift binning, for a list of valid
                 options and their description see
                 :obj:`~yaw.config.options.Options.binning`.
             cosmology (:obj:`astropy.cosmology.FLRW`, :obj:`~yaw.core.cosmology.CustomCosmology`, optional):
                 Cosmological model used for distance calculations. For a custom
                 model, refer to :mod:`yaw.core.cosmology`.
-        
+
         Returns:
             :obj:`AutoBinningConfig`
         """
         zbins = BinFactory(zmin, zmax, zbin_num, cosmology).get(method)
         return cls(zbins, method)
 
     def __eq__(self, other: ManualBinningConfig) -> bool:
@@ -189,49 +197,42 @@
             return False
         if self.method != other.method:
             return False
         return True
 
     @classmethod
     def from_dict(
-        cls,
-        the_dict: dict[str, Any],
-        cosmology: TypeCosmology | None = None
+        cls, the_dict: dict[str, Any], cosmology: TypeCosmology | None = None
     ) -> AutoBinningConfig:
         """Create a class instance from a dictionary representation of the
         minimally required data.
-        
+
         Args:
             the_dict (:obj:`dict`):
                 Dictionary containing the data.
             cosmology (:obj:`astropy.cosmology.FLRW`, :obj:`~yaw.core.cosmology.CustomCosmology`, optional):
                 Cosmological model used for distance calculations. For a custom
                 model, refer to :mod:`yaw.core.cosmology`.
         """
         return cls.generate(**the_dict, cosmology=cosmology)
 
     def to_dict(self) -> dict[str, Any]:
         return dict(
-            zmin=self.zmin,
-            zmax=self.zmax,
-            zbin_num=self.zbin_num,
-            method=self.method)
+            zmin=self.zmin, zmax=self.zmax, zbin_num=self.zbin_num, method=self.method
+        )
 
 
 def warn_binning_args_ignored(
-    zmin: bool | float | None,
-    zmax: bool | float | None,
-    zbin_num: bool | int | None
+    zmin: bool | float | None, zmax: bool | float | None, zbin_num: bool | int | None
 ) -> None:
     """Issue a warning that values are ignored, if any of the arguments is
     set."""
     # NOTE: NotSet is also False
     if zmin or zmax or zbin_num:
-        logger.warn(
-            "'zmin', 'zmax', 'nbins' are ignored if 'zbins' is provided")
+        logger.warn("'zmin', 'zmax', 'nbins' are ignored if 'zbins' is provided")
 
 
 def make_binning_config(
     cosmology: TypeCosmology | str | None,
     zmin: float | None = None,
     zmax: float | None = None,
     zbin_num: int | None = None,
@@ -244,16 +245,15 @@
     The ``cosmology`` argument is always required. If redshift bins (``zbins``)
     are provided, a :obj:`ManualBinningConfig` is returned, otherwise an
     :obj:`AutoBinningConfig`. Issues a warning if any argument is set but
     ignored by the returned configuration instance.
     """
     auto_args_set = (zmin is not None, zmax is not None, zbin_num is not None)
     if zbins is None and not all(auto_args_set):
-        raise ConfigError(
-            "either 'zbins' or 'zmin', 'zmax', 'zbin_num' are required")
+        raise ConfigError("either 'zbins' or 'zmin', 'zmax', 'zbin_num' are required")
     elif all(auto_args_set):
         return AutoBinningConfig.generate(
-            zmin=zmin, zmax=zmax, zbin_num=zbin_num,
-            method=method, cosmology=cosmology)
+            zmin=zmin, zmax=zmax, zbin_num=zbin_num, method=method, cosmology=cosmology
+        )
     else:
         warn_binning_args_ignored(*auto_args_set)
         return ManualBinningConfig(zbins)
```

### Comparing `yet_another_wizz-2.5/src/yaw/config/config.py` & `yet_another_wizz-2.5.post0/src/yaw/config/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,32 +3,38 @@
 import logging
 from dataclasses import asdict, dataclass, field
 from typing import TYPE_CHECKING, Any, get_args
 
 import numpy as np
 import yaml
 
-from yaw.core.abc import DictRepresentation
-from yaw.core.docs import Parameter
-from yaw.core.cosmology import (
-    TypeCosmology, get_default_cosmology, r_kpc_to_angle)
-
-from yaw.config import default as DEFAULT, OPTIONS, utils
+from yaw.config import OPTIONS
+from yaw.config import default as DEFAULT
+from yaw.config import utils
 from yaw.config.backend import BackendConfig
 from yaw.config.binning import (
-    AutoBinningConfig, ManualBinningConfig, make_binning_config,
-    warn_binning_args_ignored)
+    AutoBinningConfig,
+    ManualBinningConfig,
+    make_binning_config,
+    warn_binning_args_ignored,
+)
 from yaw.config.scales import ScalesConfig
+from yaw.core.abc import DictRepresentation
+from yaw.core.cosmology import TypeCosmology, get_default_cosmology, r_kpc_to_angle
+from yaw.core.docs import Parameter
 
 if TYPE_CHECKING:  # pragma: no cover
     from matplotlib.figure import Figure
     from numpy.typing import ArrayLike, NDArray
+
     from yaw.catalogs import BaseCatalog
     from yaw.core.utils import TypePathStr
 
+__all__ = ["Configuration"]
+
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass(frozen=True)
 class Configuration(DictRepresentation):
     """The central configration for correlation measurements.
@@ -71,29 +77,31 @@
     binning: AutoBinningConfig | ManualBinningConfig
     """The redshift binning configuration."""
     backend: BackendConfig = field(default_factory=BackendConfig)
     """The backend-specific configuration."""
     cosmology: TypeCosmology | str | None = field(
         default=DEFAULT.Configuration.cosmology,
         metadata=Parameter(
-            type=str, choices=OPTIONS.cosmology,
+            type=str,
+            choices=OPTIONS.cosmology,
             help="cosmological model used for distance calculations",
-            default_text="(see astropy.cosmology, default: %(default)s)"))
+            default_text="(see astropy.cosmology, default: %(default)s)",
+        ),
+    )
     """The cosmological model for distance calculations."""
 
     def __post_init__(self) -> None:
         # parse cosmology
         if self.cosmology is None:
             cosmology = get_default_cosmology()
         elif isinstance(self.cosmology, str):
             cosmology = utils.yaml_to_cosmology(self.cosmology)
         elif not isinstance(self.cosmology, get_args(TypeCosmology)):
             which = ", ".join(get_args(TypeCosmology))
-            raise utils.ConfigError(
-                f"'cosmology' must be instance of: {which}")
+            raise utils.ConfigError(f"'cosmology' must be instance of: {which}")
         else:
             cosmology = self.cosmology
         cosmology = utils.parse_cosmology(self.cosmology)
         object.__setattr__(self, "cosmology", cosmology)
 
     @classmethod
     def create(
@@ -110,15 +118,15 @@
         zmax: ArrayLike = None,
         zbin_num: int | None = DEFAULT.Configuration.binning.zbin_num,
         method: str = DEFAULT.Configuration.binning.method,
         zbins: NDArray[np.float_] | None = None,
         # BackendConfig
         thread_num: int | None = DEFAULT.Configuration.backend.thread_num,
         crosspatch: bool = DEFAULT.Configuration.backend.crosspatch,
-        rbin_slop: float = DEFAULT.Configuration.backend.rbin_slop
+        rbin_slop: float = DEFAULT.Configuration.backend.rbin_slop,
     ) -> Configuration:
         """Create a new configuration object.
 
         Except for the ``cosmology`` parameter, all other parameters are passed
         to the constructors of the respective :obj:`ScalesConfig`,
         :obj:`AutoBinningConfig` / :obj:`ManualBinningConfig`,
         :obj:`BackendConfig` classes.
@@ -161,29 +169,32 @@
             thread_num (:obj:`int`, optional):
                 Default number of threads to use.
             crosspatch (:obj:`bool`, optional):
                 whether to count pairs across patch boundaries (scipy backend
                 only)
             rbin_slop (:obj:`float`, optional):
                 TreeCorr 'rbin_slop' parameter
-    
+
         Returns:
             :obj:`Configuration`
         """
         cosmology = utils.parse_cosmology(cosmology)
-        scales = ScalesConfig(
-            rmin=rmin, rmax=rmax, rweight=rweight, rbin_num=rbin_num)
+        scales = ScalesConfig(rmin=rmin, rmax=rmax, rweight=rweight, rbin_num=rbin_num)
         binning = make_binning_config(
-            cosmology=cosmology, zmin=zmin, zmax=zmax, zbin_num=zbin_num,
-            method=method, zbins=zbins)
+            cosmology=cosmology,
+            zmin=zmin,
+            zmax=zmax,
+            zbin_num=zbin_num,
+            method=method,
+            zbins=zbins,
+        )
         backend = BackendConfig(
-            thread_num=thread_num, crosspatch=crosspatch, rbin_slop=rbin_slop)
-        return cls(
-            scales=scales, binning=binning,
-            backend=backend, cosmology=cosmology)
+            thread_num=thread_num, crosspatch=crosspatch, rbin_slop=rbin_slop
+        )
+        return cls(scales=scales, binning=binning, backend=backend, cosmology=cosmology)
 
     def modify(
         self,
         *,
         cosmology: TypeCosmology | str | None = DEFAULT.NotSet,
         # ScalesConfig
         rmin: ArrayLike | None = DEFAULT.NotSet,
@@ -195,15 +206,15 @@
         zmax: float | None = DEFAULT.NotSet,
         zbin_num: int | None = DEFAULT.NotSet,
         method: str | None = DEFAULT.NotSet,
         zbins: NDArray[np.float_] | None = DEFAULT.NotSet,
         # BackendConfig
         thread_num: int | None = DEFAULT.NotSet,
         crosspatch: bool | None = DEFAULT.NotSet,
-        rbin_slop: float | None = DEFAULT.NotSet
+        rbin_slop: float | None = DEFAULT.NotSet,
     ) -> Configuration:
         """Create a copy of the current configuration with updated parameter
         values.
 
         The method arguments are identical to :meth:`create`. Values that should
         not be modified are by default represented by the special value
         :obj:`~yaw.config.default.NotSet`.
@@ -241,118 +252,120 @@
         if crosspatch is not DEFAULT.NotSet:
             config["backend"]["crosspatch"] = crosspatch
         if rbin_slop is not DEFAULT.NotSet:
             config["backend"]["rbin_slop"] = rbin_slop
         return self.__class__.from_dict(config)
 
     def plot_scales(
-        self,
-        catalog: BaseCatalog,
-        log: bool = True,
-        legend: bool = True
+        self, catalog: BaseCatalog, log: bool = True, legend: bool = True
     ) -> Figure:
         """Plot the configured correlation scales at different redshifts in
         comparison to the size of patches in a data catalogue."""
         import matplotlib.pyplot as plt
 
         fig, ax_scale = plt.subplots(1, 1)
         # plot scale of annulus
         for r_min, r_max in self.scales.as_array():
-            ang_min, ang_max = np.transpose([
-                r_kpc_to_angle([r_min, r_max], z, self.cosmology)
-                for z in self.binning.zbins])
+            ang_min, ang_max = np.transpose(
+                [
+                    r_kpc_to_angle([r_min, r_max], z, self.cosmology)
+                    for z in self.binning.zbins
+                ]
+            )
             ax_scale.fill_between(
-                self.binning.zbins, ang_min, ang_max, step="post", alpha=0.3,
-                label=rf"${r_min:.0f} < r \leq {r_max:.0f}$ kpc")
+                self.binning.zbins,
+                ang_min,
+                ang_max,
+                step="post",
+                alpha=0.3,
+                label=rf"${r_min:.0f} < r \leq {r_max:.0f}$ kpc",
+            )
         if legend:
             ax_scale.legend(loc="lower right")
         # plot patch sizes
         ax_patch = ax_scale.twiny()
         bins = np.histogram_bin_edges(catalog.radii)
         if log:
             ax_patch.set_yscale("log")
             bins = np.logspace(
-                np.log10(bins[0]), np.log10(bins[-1]), len(bins), base=10.0)
+                np.log10(bins[0]), np.log10(bins[-1]), len(bins), base=10.0
+            )
         ax_patch.hist(
-            catalog.radii, bins,
-            orientation="horizontal", color="k", alpha=0.5)
+            catalog.radii, bins, orientation="horizontal", color="k", alpha=0.5
+        )
         # decorate
         ax_scale.set_xlim(self.binning.zmin, self.binning.zmax)
         ax_scale.set_ylabel("Radius / rad")
         ax_scale.set_xlabel("Redshift")
         ax_patch.set_xlabel("Patch count")
         return fig
 
     @classmethod
-    def from_dict(
-        cls,
-        the_dict: dict[str, Any],
-        **kwargs
-    ) -> Configuration:
+    def from_dict(cls, the_dict: dict[str, Any], **kwargs) -> Configuration:
         config = {k: v for k, v in the_dict.items()}
-        cosmology = utils.parse_cosmology(config.pop(
-            "cosmology", DEFAULT.Configuration.cosmology))
+        cosmology = utils.parse_cosmology(
+            config.pop("cosmology", DEFAULT.Configuration.cosmology)
+        )
         # parse the required subgroups
         try:
             scales = ScalesConfig.from_dict(config.pop("scales"))
         except (TypeError, KeyError) as e:
             utils.parse_section_error(e, "scales")
         try:
             binning_conf = config.pop("binning")
             if "zbins" in binning_conf:
                 binning = ManualBinningConfig(binning_conf["zbins"])
             else:
                 binning = AutoBinningConfig.generate(
-                    cosmology=cosmology, **binning_conf)
+                    cosmology=cosmology, **binning_conf
+                )
         except (TypeError, KeyError) as e:
             utils.parse_section_error(e, "binning")
         # parse the optional subgroups
         try:
             backend = BackendConfig.from_dict(config.pop("backend"))
         except KeyError:
             backend = BackendConfig()
         except TypeError as e:
             utils.parse_section_error(e, "backend")
         # check that there are no entries left
         if len(config) > 0:
             key = next(iter(config.keys()))
             raise utils.ConfigError(f"encountered unknown section '{key}'")
-        return cls(
-            scales=scales, binning=binning,
-            backend=backend, cosmology=cosmology)
+        return cls(scales=scales, binning=binning, backend=backend, cosmology=cosmology)
 
     def to_dict(self) -> dict[str, Any]:
         values = dict()
         for attr in asdict(self):
             value = getattr(self, attr)  # avoid asdict() recursion
             if attr == "cosmology":
                 values[attr] = utils.cosmology_to_yaml(value)
             else:
                 values[attr] = value.to_dict()
         return values
 
     @classmethod
     def from_yaml(cls, path: TypePathStr) -> Configuration:
         """Create a new instance by loading the configuration from a YAML file.
-        
+
         Args:
             path (:obj:`pathlib.Path`, :obj:`str`):
                 Path to the YAML file containing the configuration.
 
         Returns:
-            :obj:`Configuration`                
+            :obj:`Configuration`
         """
         logger.info(f"reading configuration file '{path}'")
         with open(str(path)) as f:
             config = yaml.safe_load(f.read())
         return cls.from_dict(config)
 
     def to_yaml(self, path: TypePathStr) -> None:
         """Store the configuration as YAML file.
-        
+
         Args:
             path (:obj:`pathlib.Path`, :obj:`str`):
                 Path to which the YAML file is written.
         """
         logger.info(f"writing configuration file '{path}'")
         string = yaml.dump(self.to_dict())
         with open(str(path), "w") as f:
```

### Comparing `yet_another_wizz-2.5/src/yaw/config/default.py` & `yet_another_wizz-2.5.post0/src/yaw/config/default.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 """This module implements the default values for the different configuration
 objects. Each of the ``*Config`` objects has a corresponding class holding just
 the default values, as listed below.
 """
 
-class _NotSet_meta(type):
+__all__ = [
+    "NotSet",
+    "Scales",
+    "AutoBinning",
+    "Backend",
+    "Configuration",
+    "Resampling",
+    "backend",
+]
+
 
+class _NotSet_meta(type):
     def __repr__(self) -> str:
         return "NotSet"  # pragma: no cover
 
     def __bool__(self) -> bool:
         return False
```

### Comparing `yet_another_wizz-2.5/src/yaw/config/options.py` & `yet_another_wizz-2.5.post0/src/yaw/config/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """This module implements a class that generates the value options for certain
 configuration parameters. An instance of this class can be accessed directly as
 :obj:`yaw.config.OPTIONS`.
 """
 
 from __future__ import annotations
 
+__all__ = ["OPTIONS"]
 
-class Options:
 
+class Options:
     @property
     def backend(self) -> tuple[str]:
         """Lists the names of the currently available backends for correlation
         measurements."""
         from yaw.catalogs import BaseCatalog
 
         return tuple(sorted(BaseCatalog._backends.keys()))
@@ -21,41 +22,41 @@
         """Lists the currently implemented methods to generate redshift bins
         with the :obj:`~yaw.config.AutoBinningConfig` class.
 
         .. rubric:: Values
 
         ``comoving``: Generate a binning with equal width in radial comoving
         distance.
-        
+
         ``linear``: Generate a binning with equal width in redshift.
-        
+
         ``logspace``: Generate a binning with equal width in logarithmic
         redshift :math:`\\log(1+z)`.
         """
         return ("comoving", "linear", "logspace")
 
     @property
     def cosmology(self) -> tuple[str]:
         """Lists the availble named cosmologies in :obj:`astropy`.
-        
+
         On top of these comological models, custom cosmologies can be defined by
         subclassing :obj:`yaw.core.cosmology.CustomCosmology`.
         """
         from astropy.cosmology import available
 
         return available
 
     @property
     def kind(self) -> tuple[str]:
         """Lists the currently implemented methods for covariance calculation.
 
         .. rubric:: Values
 
         ``full``: Compute all matrix elements of the covariance.
-        
+
         ``diag``: Compute only the main diagonal and the primary off-diagonals
         of the covariance matrix. This option applies, if the covariance is
         computed from a concatenated set of data samples, which have a
         crosscorrelation of interest. For example if concatenating the samples
         obtained from multiple redshift bins, the primary off-diagonals contain
         the covariance at the same redshift between different bins.
 
@@ -68,15 +69,15 @@
         """Lists the available modes to merge correlation measurements.
 
         .. rubric:: Values
 
         ``patches``: Merge measurements by concatenating spatial patches, i.e.
         extending the area over which measurements are taken. This may miss out
         some correlation signal between the two measurements.
-        
+
         ``redshift``: Merge measurements by concatenating redshift bins, i.e.
         extending the redshift range.
         """
         return ("patches", "redshift")
 
     @property
     def method(self) -> tuple[str]:
@@ -85,15 +86,15 @@
         Resampling uses the spatial patches to get uncertainty estimates for the
         correlation function measurements.
 
         .. rubric:: Values
 
         ``jackknife``: Use jackknife resampling (generate samples and leave out
         one patch at a time).
-        
+
         ``bootstrap``: Use bootstrap resampling (generate samples by randomly
         drawing patches with replacement).
         """
         return ("jackknife", "bootstrap")
 
 
 OPTIONS = Options()
```

### Comparing `yet_another_wizz-2.5/src/yaw/config/resampling.py` & `yet_another_wizz-2.5.post0/src/yaw/config/resampling.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any
 
 import numpy as np
 
-from yaw.core.abc import DictRepresentation
-
-from yaw.config import default as DEFAULT, OPTIONS
+from yaw.config import OPTIONS
+from yaw.config import default as DEFAULT
 from yaw.config.utils import ConfigError
+from yaw.core.abc import DictRepresentation
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import NDArray
 
+__all__ = ["ResamplingConfig"]
+
 
 @dataclass(frozen=True)
 class ResamplingConfig(DictRepresentation):
     """Configuration for error estimation from spatial resampling.
 
     Used for all functions and methods that use spatial patches for error
     estimation. Use the :meth:`get_samples` method to generate samples from the
@@ -46,29 +48,30 @@
     n_boot: int = DEFAULT.Resampling.n_boot
     """Number of samples to generate for the ``bootstrap`` method."""
     global_norm: bool = DEFAULT.Resampling.global_norm
     """Whether to normalise paircounts globally or for each sample."""
     seed: int = DEFAULT.Resampling.seed
     """Random seed to use."""
     _resampling_idx: NDArray[np.int_] | None = field(
-        default=None, init=False, repr=False)
+        default=None, init=False, repr=False
+    )
 
     def __post_init__(self) -> None:
         if self.method not in OPTIONS.method:
             opts = ", ".join(f"'{s}'" for s in OPTIONS.method)
             raise ConfigError(
-                f"invalid resampling method '{self.method}', "
-                f"must either of {opts}")
+                f"invalid resampling method '{self.method}', must either of {opts}"
+            )
 
     @property
     def n_patches(self) -> int | None:
         """The number of spatial patches for which this configuratin is valid.
-        
+
         Available only after generating samples with :meth:`get_samples`.
-        
+
         Returns:
             int if samples have been generated, else None.
         """
         if self._resampling_idx is None:
             return None
         else:
             return self._resampling_idx.shape[1]
@@ -85,16 +88,16 @@
 
     def _generate_jackknife(self, n_patches: int) -> NDArray[np.int_]:
         """Generate samples for the jackknife resampling method.
 
         For N patches, draw N realisations by leaving out one of the N patches.
         """
         N = n_patches
-        idx = np.delete(np.tile(np.arange(0, N), N), np.s_[::N+1])
-        return idx.reshape((N, N-1))
+        idx = np.delete(np.tile(np.arange(0, N), N), np.s_[:: N + 1])
+        return idx.reshape((N, N - 1))
 
     def get_samples(self, n_patches: int) -> NDArray[np.int_]:
         """Generate a list of patch indices that produces samples for the
         selected resampling method.
 
         Args:
             n_patches (:obj:`int`):
@@ -116,15 +119,16 @@
                 idx = self._generate_jackknife(n_patches)
             else:
                 idx = self._generate_bootstrap(n_patches)
             object.__setattr__(self, "_resampling_idx", idx)
         elif n_patches != self.n_patches:
             raise ValueError(
                 f"'n_patches' does not match, expected {self.n_patches}, but "
-                f"got {n_patches}")
+                f"got {n_patches}"
+            )
         return self._resampling_idx
 
     def reset(self) -> None:
         """Reset the internally stored patch indices generated by
         :meth:`get_samples`."""
         object.__setattr__(self, "_resampling_idx", None)
```

### Comparing `yet_another_wizz-2.5/src/yaw/config/scales.py` & `yet_another_wizz-2.5.post0/src/yaw/config/scales.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 from __future__ import annotations
 
 from collections.abc import Iterator, Sequence
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING
 
 import numpy as np
 from deprecated import deprecated
 
+from yaw.config import default as DEFAULT
+from yaw.config.utils import ConfigError
 from yaw.core.abc import DictRepresentation
 from yaw.core.cosmology import Scale
 from yaw.core.docs import Parameter
 from yaw.core.math import array_equal
 
-from yaw.config.utils import ConfigError
-from yaw.config import default as DEFAULT
-
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import NDArray
 
+__all__ = ["ScalesConfig"]
+
 
 @dataclass(frozen=True)
 class ScalesConfig(DictRepresentation):
     """Configuration of scales used for correlation measurements.
 
     Correlation functions are measured on one or many intervals
-    :math:`r_{\\rm min} \leq r < r_{\\rm max}` angular diameter distance in kpc.
-    When measuring correlations, this scale is coverted to angles at the current
-    redshift.
-    
+    :math:`r_{\\rm min} \\leq r < r_{\\rm max}` angular diameter distance in
+    kpc. When measuring correlations, this scale is coverted to angles at the
+    current redshift.
+
     Additionally, pairs can be weighted by their separation
     :math:`r^\\alpha` if a power-law exponent is provided through ``rweight``.
     The weighting is applied logarithmically spaced bins of separation (based
     on the logarithmic bin centers). This is an approximation to actually
     weighting each pair individually and the resolution of this approximation
     can be controlled by setting the number of bins.
 
@@ -47,50 +48,61 @@
         rbin_num (:obj:`int`, optional):
             Number of radial logarithmic bin used to approximate the weighting
             by separation.
     """
 
     rmin: Sequence[float] | float = field(
         metadata=Parameter(
-            type=float, nargs="*", required=True,
-            help="(list of) lower scale limit in kpc (pyhsical)"))
+            type=float,
+            nargs="*",
+            required=True,
+            help="(list of) lower scale limit in kpc (pyhsical)",
+        )
+    )
     """Lower scale limit(s) in kpc (angular diameter distance)."""
     rmax: Sequence[float] | float = field(
         metadata=Parameter(
-            type=float, nargs="*", required=True,
-            help="(list of) upper scale limit in kpc (pyhsical)"))
+            type=float,
+            nargs="*",
+            required=True,
+            help="(list of) upper scale limit in kpc (pyhsical)",
+        )
+    )
     """Upper scale limit(s) in kpc (angular diameter distance)."""
     rweight: float | None = field(
         default=DEFAULT.Scales.rweight,
         metadata=Parameter(
             type=float,
             help="weight galaxy pairs by their separation to power 'rweight'",
-            default_text="(default: no weighting applied)"))
+            default_text="(default: no weighting applied)",
+        ),
+    )
     """Power-law exponent used to weight pairs by their separation."""
     rbin_num: int = field(
         default=DEFAULT.Scales.rbin_num,
         metadata=Parameter(
             type=int,
-            help="number of bins in log r used (i.e. resolution) to compute "
-                 "distance weights",
-            default_text="(default: %(default)s)"))
+            help="number of bins in log r used (i.e. resolution) to compute distance weights",
+            default_text="(default: %(default)s)",
+        ),
+    )
     """Number of radial logarithmic bin used to approximate the weighting by
     separation."""
 
     def __post_init__(self) -> None:
-        msg_scale_error = f"scales violates 'rmin' < 'rmax'"
+        msg_scale_error = "scales violates 'rmin' < 'rmax'"
         # validation, set to basic python types
         scalars = (float, int, np.number)
-        if (
-            isinstance(self.rmin, (Sequence, np.ndarray)) and
-            isinstance(self.rmax, (Sequence, np.ndarray))
+        if isinstance(self.rmin, (Sequence, np.ndarray)) and isinstance(
+            self.rmax, (Sequence, np.ndarray)
         ):
             if len(self.rmin) != len(self.rmax):
                 raise ConfigError(
-                    "number of elements in 'rmin' and 'rmax' do not match")
+                    "number of elements in 'rmin' and 'rmax' do not match"
+                )
             # for clean YAML conversion
             for rmin, rmax in zip(self.rmin, self.rmax):
                 if rmin >= rmax:
                     raise ConfigError(msg_scale_error)
             if len(self.rmin) == 1:
                 rmin = float(self.rmin[0])
                 rmax = float(self.rmax[0])
@@ -102,16 +114,15 @@
         elif isinstance(self.rmin, scalars) and isinstance(self.rmax, scalars):
             # for clean YAML conversion
             object.__setattr__(self, "rmin", float(self.rmin))
             object.__setattr__(self, "rmax", float(self.rmax))
             if self.rmin >= self.rmax:
                 raise ConfigError(msg_scale_error)
         else:
-            raise ConfigError(
-                "'rmin' and 'rmax' must be both sequences or float")
+            raise ConfigError("'rmin' and 'rmax' must be both sequences or float")
 
     def __eq__(self, other: ScalesConfig) -> bool:
         if not array_equal(self.as_array(), other.as_array()):
             return False
         if self.rweight != other.rweight:
             return False
         if self.rbin_num != other.rbin_num:
@@ -126,16 +137,15 @@
         for rmin, rmax in self.as_array():
             yield Scale(rmin=rmin, rmax=rmax)
 
     def as_array(self) -> NDArray[np.float_]:
         """Obtain the scales cuts as array of shape (2, N)"""
         return np.atleast_2d(np.transpose([self.rmin, self.rmax]))
 
-    @deprecated(
-        "use [str(scale) for scale in ScalesConfig] instead", version="2.3.1")
+    @deprecated("use [str(scale) for scale in ScalesConfig] instead", version="2.3.1")
     def dict_keys(self) -> list[str]:
         """Get the scale cuts formatted as a list of strings.
 
         Format is ``kpc[rmin]t[rmax]``, used as keys to pack outputs of
         correlation measurements in a dictionary when measuring with multiple
         scales cuts.
```

### Comparing `yet_another_wizz-2.5/src/yaw/config/utils.py` & `yet_another_wizz-2.5.post0/src/yaw/config/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,63 +1,68 @@
 from __future__ import annotations
+
 from typing import NoReturn, get_args
 
 import astropy.cosmology
 
 from yaw.core.cosmology import TypeCosmology, get_default_cosmology
 
+__all__ = [
+    "cosmology_to_yaml",
+    "yaml_to_cosmology",
+    "parse_cosmology",
+    "parse_section_error",
+]
+
 
 class ConfigError(Exception):
     pass
 
 
 def cosmology_to_yaml(cosmology: TypeCosmology) -> str:
     """Try to represent the cosmological model in a YAML-friendly way.
-    
+
     If it is one of the names :obj:`astropy` cosmologies, returns the name,
     otherwise raises an :exc:`ConfigError`."""
     if not isinstance(cosmology, astropy.cosmology.FLRW):
         raise ConfigError("cannot serialise custom cosmoligies to YAML")
     if cosmology.name not in astropy.cosmology.available:
-        raise ConfigError(
-            "can only serialise predefined astropy cosmologies to YAML")
+        raise ConfigError("can only serialise predefined astropy cosmologies to YAML")
     return cosmology.name
 
 
 def yaml_to_cosmology(cosmo_name: str) -> TypeCosmology:
     """Reinstantiate the cosmological model from its name representation."""
     if cosmo_name not in astropy.cosmology.available:
         raise ConfigError(
             f"unknown cosmology with name '{cosmo_name}', see "
-            "'astropy.cosmology.available'")
+            "'astropy.cosmology.available'"
+        )
     return getattr(astropy.cosmology, cosmo_name)
 
 
 def parse_cosmology(cosmology: TypeCosmology | str | None) -> TypeCosmology:
     """Construct the cosmological model.
-    
+
     Either returns the default model, loads one of the named cosmological
     :obj:`astropy` cosmologies, otherwise returns the input if it is an
     :obj:`astropy` cosmologies or subclass of
     :obj:`yaw.core.cosmology.CustomCosmology`."""
     if cosmology is None:
         cosmology = get_default_cosmology()
     elif isinstance(cosmology, str):
         cosmology = yaml_to_cosmology(cosmology)
     elif not isinstance(cosmology, get_args(TypeCosmology)):
         which = ", ".join(get_args(TypeCosmology))
-        raise ConfigError(
-            f"'cosmology' must be instance of: {which}")
+        raise ConfigError(f"'cosmology' must be instance of: {which}")
     return cosmology
 
 
 def parse_section_error(
-    exception: Exception,
-    section: str,
-    reraise: Exception = ConfigError
+    exception: Exception, section: str, reraise: Exception = ConfigError
 ) -> NoReturn:
     """Reraises are a more descriptive exception from an existing exception when
     parsing a YAML configuration.
 
     Covered cases are undefined key names, missing required key names or
     entirely missing subsection in the configuration.
     """
```

### Comparing `yet_another_wizz-2.5/src/yaw/core/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/core/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,7 +12,9 @@
 * parallelisation with multiprocessing (:mod:`yaw.core.parallel`), and
 
 * a few other convenience functions in various submodules.
 """
 
 from yaw.core.containers import SampledData, SampledValue
 from yaw.core.math import global_covariance
+
+__all__ = ["SampledData", "SampledValue", "global_covariance"]
```

### Comparing `yet_another_wizz-2.5/src/yaw/core/abc.py` & `yet_another_wizz-2.5.post0/src/yaw/core/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,26 @@
 import h5py
 import numpy as np
 import pandas as pd
 from numpy.typing import NDArray
 
 if TYPE_CHECKING:  # pragma: no cover
     from pandas import IntervalIndex
+
     from yaw.core.containers import Indexer
     from yaw.core.utils import TypePathStr
 
+__all__ = [
+    "PatchedQuantity",
+    "BinnedQuantity",
+    "concatenate_bin_edges",
+    "HDFSerializable",
+    "DictRepresentation",
+]
+
 
 _Tpatched = TypeVar("_Tpatched", bound="PatchedQuantity")
 
 
 class PatchedQuantity(ABC):
     """Base class for an object that has data organised in spatial patches."""
 
@@ -60,15 +69,15 @@
             all inputs is identical. Cannot merge cross- with autocorrelation
             containers.
 
         Args:
             *data:
                 Containers of same type that are appended to the patch dimension
                 of this container.
-        
+
         Returns:
             New instance of this container with combined data.
         """
         raise NotImplementedError
 
 
 _Tbinned = TypeVar("_Tbinned", bound="BinnedQuantity")
@@ -133,37 +142,34 @@
             some operations on the returned container may fail.
 
         Returns:
             :obj:`yaw.core.containers.Indexer`
         """
         raise NotImplementedError
 
-    def is_compatible(
-        self: _Tbinned,
-        other: _Tbinned,
-        require: bool = False
-    ) -> bool:
+    def is_compatible(self: _Tbinned, other: _Tbinned, require: bool = False) -> bool:
         """Check whether this instance is compatible with another instance.
-         
+
         Ensures that both objects are instances of the same class and that the
         redshift binning is identical.
 
         Args:
             other (:obj:`BinnedQuantity`):
                 Object instance to compare to.
             require (:obj:`bool`, optional)
                 Raise a ValueError if any of the checks fail.
-        
+
         Returns:
             :obj:`bool`
         """
         if not isinstance(other, self.__class__):
             raise TypeError(
                 f"object of type {type(other)} is not compatible with "
-                f"{self.__class__}")
+                f"{self.__class__}"
+            )
         if self.n_bins != other.n_bins:
             if require:
                 raise ValueError("number of bins do not agree")
             return False
         if np.any(self.get_binning() != other.get_binning()):
             if require:
                 raise ValueError("binning is not identical")
@@ -183,15 +189,15 @@
             non-overlapping. Cannot merge cross- with autocorrelation
             containers.
 
         Args:
             *data:
                 Containers of same type that are appended to the patch dimension
                 of this container.
-        
+
         Returns:
             New instance of this container with combined data.
         """
         raise NotImplementedError
 
 
 def concatenate_bin_edges(*patched: BinnedQuantity) -> IntervalIndex:
@@ -217,18 +223,15 @@
 _Thdf = TypeVar("_Thdf", bound="HDFSerializable")
 
 
 class HDFSerializable(ABC):
     """Base class for an object that can be serialised into a HDF5 file."""
 
     @abstractclassmethod
-    def from_hdf(
-        cls: Type[_Thdf],
-        source: h5py.Group
-    ) -> _Thdf:
+    def from_hdf(cls: Type[_Thdf], source: h5py.Group) -> _Thdf:
         """Create a class instance by deserialising data from a HDF5 group.
 
         Args:
             source (:obj:`h5py.Group`):
                 Group in an opened HDF5 file that contains the serialised data.
 
         Returns:
@@ -277,19 +280,19 @@
 class DictRepresentation(ABC):
     """Base class for an object that can be serialised into a dictionary."""
 
     @classmethod
     def from_dict(
         cls: Type[_Tdict],
         the_dict: dict[str, Any],
-        **kwargs: dict[str, Any]  # passing additional constructor data
+        **kwargs: dict[str, Any],  # passing additional constructor data
     ) -> _Tdict:
         """Create a class instance from a dictionary representation of the
         minimally required data.
-        
+
         Args:
             the_dict (:obj:`dict`):
                 Dictionary containing the data.
             **kwargs: Additional data needed to construct the class instance.
         """
         return cls(**the_dict)
```

### Comparing `yet_another_wizz-2.5/src/yaw/core/containers.py` & `yet_another_wizz-2.5.post0/src/yaw/core/containers.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,24 @@
 from collections.abc import Iterator, Sequence
 from dataclasses import dataclass, field, fields
 from typing import TYPE_CHECKING, Callable, Generic, NamedTuple, TypeVar
 
 import numpy as np
 import pandas as pd
 
+from yaw.config import OPTIONS
 from yaw.core.abc import BinnedQuantity, concatenate_bin_edges
 from yaw.core.math import cov_from_samples
-from yaw.config import OPTIONS
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import NDArray
     from pandas import DataFrame, IntervalIndex, Series
 
+__all__ = ["Indexer", "PatchIDs", "PatchCorrelationData", "SampledValue", "SampledData"]
+
 
 _TK = TypeVar("_TK")
 _TV = TypeVar("_TV")
 
 
 class Indexer(Generic[_TK, _TV], Iterator):
     """Helper class to implemented a class attribute that can be used as
@@ -99,14 +101,15 @@
             Total number of objects after binning by redshift in first patch.
         totals1 (:obj:`NDArray`):
             Total number of objects after binning by redshift in second patch.
         counts (:obj:`dict`):
             Dictionary listing the number of counted pairs after binning by
             redshift. Each item represents results from a different scale.
     """
+
     patches: PatchIDs
     totals1: NDArray
     totals2: NDArray
     counts: dict[str, NDArray]
 
 
 _Tscalar = TypeVar("_Tscalar", bound=np.number)
@@ -119,15 +122,15 @@
 
     Supports comparison of the values and samples with ``==`` and ``!=``.
 
     .. rubric:: Examples
 
     Create a value container with 100 assumed jackknife samples that scatter
     around zero with a standard deviation of 0.1:
-    
+
     >>> from numpy.random import normal
     >>> samples = normal(loc=0.0, scale=0.01, size=101)
     >>> value = yaw.core.SampledValue(0.0, samples, method="jackknife")
     >>> value
     SampledValue(value=0, error=0.963, n_samples=100, method='jackknife')
 
     Args:
@@ -171,17 +174,18 @@
         return f"{self.value:+.3g}+/-{self.error:.3g}"
 
     def __eq__(self, other: object) -> bool:
         if isinstance(other, self.__class__):
             if self.samples.shape != other.samples.shape:
                 return False
             return (
-                self.method == other.method and
-                self.value == other.value and
-                np.all(self.samples == other.samples))
+                self.method == other.method
+                and self.value == other.value
+                and np.all(self.samples == other.samples)
+            )
         else:
             return False
 
     def __ne__(self, other: object) -> bool:
         return not self.__eq__(other)
 
     @property
@@ -223,28 +227,28 @@
     Slicing and indexing follows the same rules as the underlying ``data``
     :obj:`NDArray`. Refer to :obj:`~yaw.correlation.CorrData` for some indexing
     and iteration examples.
 
     .. rubric:: Examples
 
     Create a redshift binning:
-    
+
     >>> import pandas as pd
     >>> bins = pd.IntervalIndex.from_breaks([0.1, 0.2, 0.3])
     >>> bins
     IntervalIndex([(0.1, 0.2], (0.2, 0.3]], dtype='interval[float64, right]')
 
     Create some sample data for the bins with value 1 and five assumed jackknife
     samples normal-distributed around 1.
 
     >>> import numpy as np
     >>> n_bins, n_samples = len(bins), 5
     >>> data = np.ones(n_bins)
     >>> samples = np.random.normal(1.0, size=(n_samples, n_bins))
-    
+
     Create the container:
 
     >>> values = yaw.core.SampledData(bins, data, samples, method="jackknife")
     >>> values
     SampledData(n_bins=2, z='0.100...0.300', n_samples=10, method='jackknife')
 
     Add the container to itself and verify that the values are doubled:
@@ -274,16 +278,15 @@
     covariance: NDArray = field(init=False)
     """Covariance matrix automatically computed from the resampled values."""
 
     def __post_init__(self) -> None:
         if self.data.shape != (self.n_bins,):
             raise ValueError("unexpected shape of 'data' array")
         if not self.samples.shape[1] == self.n_bins:
-            raise ValueError(
-                "number of bins for 'data' and 'samples' do not match")
+            raise ValueError("number of bins for 'data' and 'samples' do not match")
         if self.method not in OPTIONS.method:
             raise ValueError(f"unknown sampling method '{self.method}'")
 
         covmat = cov_from_samples(self.samples, self.method)
         object.__setattr__(self, "covariance", np.atleast_2d(covmat))
 
     def __repr__(self) -> str:
@@ -293,39 +296,42 @@
         return f"{string}, {n_samples=}, {method=})"
 
     def __eq__(self, other: object) -> bool:
         if isinstance(other, self.__class__):
             if self.samples.shape != other.samples.shape:
                 return False
             return (
-                self.method == other.method and
-                np.all(self.data == other.data) and
-                np.all(self.samples == other.samples) and
-                (self.binning == other.binning).all())
+                self.method == other.method
+                and np.all(self.data == other.data)
+                and np.all(self.samples == other.samples)
+                and (self.binning == other.binning).all()
+            )
         else:
             return False
 
     def __ne__(self, other: object) -> bool:
         return not self.__eq__(other)
 
     def __add__(self, other: _Tdata) -> _Tdata:
         self.is_compatible(other, require=True)
         return self.__class__(
             binning=self.get_binning(),
-            data=self.data+other.data,
-            samples=self.samples+other.samples,
-            method=self.method)
+            data=self.data + other.data,
+            samples=self.samples + other.samples,
+            method=self.method,
+        )
 
     def __sub__(self, other: _Tdata) -> _Tdata:
         self.is_compatible(other, require=True)
         return self.__class__(
             binning=self.get_binning(),
-            data=self.data-other.data,
-            samples=self.samples-other.samples,
-            method=self.method)
+            data=self.data - other.data,
+            samples=self.samples - other.samples,
+            method=self.method,
+        )
 
     @property
     def bins(self: _Tdata) -> Indexer[int | slice | Sequence, _Tdata]:
         def builder(inst: _Tdata, item: int | slice | Sequence) -> _Tdata:
             if isinstance(item, int):
                 item = [item]
             # try to take subsets along bin axis
@@ -346,36 +352,36 @@
     def n_samples(self) -> int:
         """Number of samples used for error estimate."""
         return len(self.samples)
 
     @property
     def error(self) -> NDArray:
         """The uncertainty (standard error) of the data.
-        
+
         Returns:
             :obj:`NDArray`
         """
         return np.sqrt(np.diag(self.covariance))
 
     def get_binning(self) -> IntervalIndex:
         return self.binning
 
     def is_compatible(self, other: SampledData, require: bool = False) -> bool:
         """Check whether this instance is compatible with another instance.
-        
+
         Ensures that both objects are instances of the same class, that the
         redshift binning is identical, that the number of samples agree, and
         that the resampling method is identical.
 
         Args:
             other (:obj:`BinnedQuantity`):
                 Object instance to compare to.
             require (:obj:`bool`, optional)
                 Raise a ValueError if any of the checks fail.
-        
+
         Returns:
             :obj:`bool`
         """
         if not super().is_compatible(other, require):
             return False
         if self.n_samples != other.n_samples:
             if require:
@@ -412,37 +418,37 @@
         The columns are labelled numerically and each represent one of the
         samples."""
         return pd.DataFrame(self.samples.T, index=self.binning)
 
     def get_error(self) -> Series:
         """Get value error estimate (diagonal of covariance matrix) as series
         with its corresponding redshift bin intervals as index.
-        
+
         Returns:
             :obj:`pandas.Series`
         """
         return pd.Series(self.error, index=self.binning)
 
     def get_covariance(self) -> DataFrame:
         """Get value covariance matrix as data frame with its corresponding
         redshift bin intervals as index and column labels.
-        
+
         Returns:
             :obj:`pandas.DataFrame`
         """
         return pd.DataFrame(
-            data=self.covariance, index=self.binning, columns=self.binning)
+            data=self.covariance, index=self.binning, columns=self.binning
+        )
 
     def get_correlation(self) -> DataFrame:
         """Get value correlation matrix as data frame with its corresponding
         redshift bin intervals as index and column labels.
-        
+
         Returns:
             :obj:`pandas.DataFrame`
         """
         stdev = np.sqrt(np.diag(self.covariance))
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             corr = self.covariance / np.outer(stdev, stdev)
         corr[self.covariance == 0] = 0
-        return pd.DataFrame(
-            data=corr, index=self.binning, columns=self.binning)
+        return pd.DataFrame(data=corr, index=self.binning, columns=self.binning)
```

### Comparing `yet_another_wizz-2.5/src/yaw/core/coordinates.py` & `yet_another_wizz-2.5.post0/src/yaw/core/coordinates.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,32 +13,36 @@
 import numpy as np
 
 from yaw.core.math import sgn
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import ArrayLike, NDArray
 
+__all__ = ["Coord3D", "CoordSky", "Dist3D", "DistSky"]
+
 
 class Coordinate(ABC):
     """Base class for a vector of coordinates."""
 
     @abstractmethod
-    def __init__(self, coords: dict[str, ArrayLike]) -> None: pass
+    def __init__(self, coords: dict[str, ArrayLike]) -> None:
+        pass
 
     @abstractclassmethod
     def from_array(cls, array) -> Coordinate:
         pass
 
     @abstractclassmethod
     def from_coords(cls, coords: Sequence[Coordinate]) -> Coordinate:
         """Concatenate a sequence of coordinates into a new vector of
         coordates."""
         pass
 
-    def __repr__(self) -> str: pass
+    def __repr__(self) -> str:
+        pass
 
     @abstractproperty
     def dim(self) -> tuple[str]:
         """A list of names of coordinates in the coordinate system."""
         pass
 
     @property
@@ -69,15 +73,16 @@
         .. Warning::
             During conversion, points loose their radial information. After
             back-transformation to :obj:`Coord3D` they lie on the unit sphere.
         """
         pass
 
     @abstractmethod
-    def distance(self, other: Coordinate) -> Distance: pass
+    def distance(self, other: Coordinate) -> Distance:
+        pass
 
 
 class Coord3D(Coordinate):
     """A representation of a vector of 3-dim Euclidean coordiantes (x, y, z)."""
 
     x: NDArray
     """The `x`-coordiante(s)."""
@@ -148,46 +153,45 @@
     def to_3d(self) -> Coord3D:
         return self
 
     def to_sky(self) -> CoordSky:
         x = self.x
         y = self.y
         z = self.z
-        r_d2 = np.sqrt(x*x + y*y)
-        r_d3 = np.sqrt(x*x + y*y + z*z)
+        r_d2 = np.sqrt(x * x + y * y)
+        r_d3 = np.sqrt(x * x + y * y + z * z)
         # transform
-        ra = np.arccos(x / r_d2) * sgn(y) % (2.0*np.pi)
+        ra = np.arccos(x / r_d2) * sgn(y) % (2.0 * np.pi)
         ra[np.isnan(ra)] = 0.0
         dec = np.arcsin(self.z / r_d3)
         return CoordSky(ra, dec)
 
     def distance(self, other: Coordinate) -> Dist3D:
         """Compute the Euclidean distance between two coordinate vectors.
-        
+
         Coordinates are automatically converted before distance calculation.
 
         Args:
             other (:obj:`Coordinate`):
                 Second coordinate vector.
-        
+
         Returns:
             :obj:`Dist3D`:
                 Euclidean distance between points in this and the other vector.
         """
         c1 = self.to_3d()
         c2 = other.to_3d()
-        return Dist3D(np.sqrt(
-            (c1.x - c2.x)**2 +
-            (c1.y - c2.y)**2 +
-            (c1.z - c2.z)**2))
+        return Dist3D(
+            np.sqrt((c1.x - c2.x) ** 2 + (c1.y - c2.y) ** 2 + (c1.z - c2.z) ** 2)
+        )
 
 
 class CoordSky(Coordinate):
     """A representation of a vector of angular coordinates in radian.
-    
+
     Angles follow the astronomical convention of R.A./Dec., i.e. declination
     values are in the range of [:math:`-\\pi`, :math:`\\pi`].
     """
 
     ra: NDArray
     """The right ascension coordinate(s)."""
     dec: NDArray
@@ -247,31 +251,30 @@
 
     def mean(self) -> Coord3D:
         return self.to_3d().mean().to_sky()
 
     def to_3d(self) -> Coord3D:
         cos_dec = np.cos(self.dec)
         return Coord3D(
-            x=np.cos(self.ra) * cos_dec,
-            y=np.sin(self.ra) * cos_dec,
-            z=np.sin(self.dec))
+            x=np.cos(self.ra) * cos_dec, y=np.sin(self.ra) * cos_dec, z=np.sin(self.dec)
+        )
 
     def to_sky(self) -> CoordSky:
         return self
 
     def distance(self, other: Coordinate) -> DistSky:
         """Compute the angular distance in radian between two coordinate
         vectors.
 
         Coordinates are automatically converted before distance calculation.
 
         Args:
             other (:obj:`Coordinate`):
                 Second coordinate vector.
-        
+
         Returns:
             :obj:`DistSky`:
                 Angular distance in radian between points in this and the other
                 vector.
         """
         # lazy shortcut
         self_3D = self.to_3d()
@@ -302,16 +305,15 @@
             Additionally, distances implement element-wise addition and
             subtraction, as well as the comparison operators.
         """
         self._values = np.atleast_1d(distance).astype(np.float_)
 
     @classmethod
     def from_dists(cls: _Tdist, dists: Sequence[_Tdist]) -> _Tdist:
-        """Concatenate a sequence of distances into a new vector of distances.
-        """
+        """Concatenate a sequence of distances into a new vector of distances."""
         return cls(np.concatenate([dist._values for dist in dists], axis=0))
 
     def __len__(self) -> int:
         return len(self._values)
 
     def __getitem__(self, idx: ArrayLike) -> CoordSky:
         return self.__class__(self._values[idx])
@@ -335,18 +337,20 @@
     def __eq__(self, other: Distance) -> ArrayLike[np.bool_]:
         return self.values == other.values
 
     def __lt__(self, other: Distance) -> ArrayLike[np.bool_]:
         return self.values < other.values
 
     @abstractmethod
-    def __add__(self: _Tdist, other: _Tdist) -> _Tdist: pass
+    def __add__(self: _Tdist, other: _Tdist) -> _Tdist:
+        pass
 
     @abstractmethod
-    def __sub__(self:_Tdist, other: _Tdist) -> _Tdist: pass
+    def __sub__(self: _Tdist, other: _Tdist) -> _Tdist:
+        pass
 
     def min(self) -> _Tdist:
         """Compute the minimum value and return it as new `Distance`
         instance."""
         return self.__class__(self.values.min())
 
     def max(self) -> _Tdist:
```

### Comparing `yet_another_wizz-2.5/src/yaw/core/cosmology.py` & `yet_another_wizz-2.5.post0/src/yaw/core/cosmology.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,33 @@
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from collections.abc import Sequence
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Union
+
 try:  # pragma: no cover
     from typing import TypeAlias
 except ImportError:  # pragma: no cover
     from typing_extensions import TypeAlias
 
 import numpy as np
-from astropy.cosmology import FLRW, Planck15, available
+from astropy.cosmology import FLRW, Planck15
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import ArrayLike, NDArray
 
+__all__ = [
+    "get_default_cosmology",
+    "CustomCosmology",
+    "r_kpc_to_angle",
+    "Scale",
+    "BinFactory",
+]
 
 
 def get_default_cosmology() -> FLRW:
     """Get the default cosmology (Planck Collaboration et al. 2015)."""
     return Planck15
 
 
@@ -70,21 +78,19 @@
         NotImplemented
 
 
 TypeCosmology: TypeAlias = Union[FLRW, CustomCosmology]
 
 
 def r_kpc_to_angle(
-    r_kpc: NDArray[np.float_] | Sequence[float],
-    z: float,
-    cosmology: TypeCosmology
+    r_kpc: NDArray[np.float_] | Sequence[float], z: float, cosmology: TypeCosmology
 ) -> NDArray[np.float_]:
     """Convert from a physical separation in kpc to angles in radian at a given
     redshift.
-    
+
     Args:
         r_kpc (:obj:`NDArray`, number):
             Physical separation in kpc.
         z (:obj:`float`):
             Redshift at which conversion happens.
         cosmology (:obj:`astropy.cosmology.FLRW`, :obj:`CustomCosmology`):
             Cosmological model used for calculations.
@@ -96,23 +102,23 @@
     f_K = cosmology.comoving_transverse_distance(z)  # for 1 radian in Mpc
     return np.asarray(r_kpc) / 1000.0 * (1.0 + z) / f_K.value
 
 
 @dataclass(frozen=True)
 class Scale:
     """Class that represents a range of physical scales in kpc.
-    
+
     The range is defined by a lower and an upper scale limit. An instance can be
     converted to a string representation that is used as dictionary key in some
     places of ``yaw``.
 
     .. rubric:: Examples
 
     Get the center points:
-    
+
     >>> scale = Scale(100, 1000)
     >>> scale.mid, scale.mid_log
     (550.0, 316.22776601683796)
 
     String representation:
 
     >>> str(scale)
@@ -140,21 +146,17 @@
         lmax = np.log10(self.rmax)
         lmid = (lmin + lmax) / 2.0
         return 10**lmid
 
     def __str__(self) -> str:
         return f"kpc{self.rmin:.0f}t{self.rmax:.0f}"
 
-    def to_radian(
-        self,
-        z: float,
-        cosmology: TypeCosmology
-    ) -> NDArray[np.float_]:
+    def to_radian(self, z: float, cosmology: TypeCosmology) -> NDArray[np.float_]:
         """Get the separation in radian at a given redshift.
-        
+
         Args:
             z (:obj:`float`):
                 Redshift at which conversion happens.
             cosmology (:obj:`astropy.cosmology.FLRW`, :obj:`CustomCosmology`):
                 Cosmological model used for calculations.
 
         Returns:
@@ -168,15 +170,15 @@
     """Class used to generate redshift bins."""
 
     def __init__(
         self,
         zmin: float,
         zmax: float,
         nbins: int,
-        cosmology: TypeCosmology | None = None
+        cosmology: TypeCosmology | None = None,
     ):
         """Create a new bin generator.
 
         Args:
             zmin (:obj:`float`):
                 Minimum redshift, lowest redshift bin edges.
             zmax (:obj:`float`):
@@ -200,31 +202,33 @@
         return np.linspace(self.zmin, self.zmax, self.nbins + 1)
 
     def comoving(self) -> NDArray[np.float_]:
         """Generate a binning with equal width in radial comoving distance."""
         cbinning = np.linspace(
             self.cosmology.comoving_distance(self.zmin).value,
             self.cosmology.comoving_distance(self.zmax).value,
-            self.nbins + 1)
+            self.nbins + 1,
+        )
         # construct a spline mapping from comoving distance to redshift
         zarray = np.linspace(0, 10.0, 5000)
         carray = self.cosmology.comoving_distance(zarray).value
         return np.interp(cbinning, xp=carray, fp=zarray)  # redshift @ cbinning
 
     def logspace(self) -> NDArray[np.float_]:
         """Generate a binning with equal width in logarithmic redshift
         :math:`\\log(1+z)`."""
         logbinning = np.linspace(
-            np.log(1.0 + self.zmin), np.log(1.0 + self.zmax), self.nbins + 1)
+            np.log(1.0 + self.zmin), np.log(1.0 + self.zmax), self.nbins + 1
+        )
         return np.exp(logbinning) - 1.0
 
     @staticmethod
     def check(zbins: NDArray[np.float_]) -> None:
         """Check if a list of bin edges in monotonicaly increasing.
-        
+
         Raises a :exc:`ValueError` if the condition is not met.
 
         Args:
             zbins (:obj:`NDArray`):
                 Redshift bin edges to check.
         """
         if np.any(np.diff(zbins) <= 0):
```

### Comparing `yet_another_wizz-2.5/src/yaw/core/docs.py` & `yet_another_wizz-2.5.post0/src/yaw/core/docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from typing import TYPE_CHECKING, Any
 
 import yaml
 
 if TYPE_CHECKING:  # pragma: no cover
     from argparse import ArgumentParser
 
+__all__ = ["Parameter", "get_doc_args", "populate_parser"]
+
 
 @dataclass(frozen=True)
 class Parameter(Mapping):
     """Class to implement automatic generation of parameter descriptions.
 
     This class provides the metadata needed to generate a new commandline
     argument for python's :mod:`argparse` module. Each constructor argument
@@ -55,31 +57,32 @@
                 metavar = None
             object.__setattr__(self, "metavar", metavar)
 
     def __len__(self) -> int:
         return 5
 
     def __iter__(self) -> Iterator[str]:
-        for field in fields(self):
-            if field.init:
-                yield f"yaw_{field.name}"
+        for cfield in fields(self):
+            if cfield.init:
+                yield f"yaw_{cfield.name}"
 
     def __getitem__(self, key: str) -> Any:
         return asdict(self)[key[4:]]
 
     @classmethod
     def from_field(cls, field: Field) -> Parameter:
         """Create a new instance from a :obj:`dataclassField`."""
         kwargs = {}
         for key, value in field.metadata.items():
             if key.startswith("yaw_"):
                 kwargs[key[4:]] = value
         if len(kwargs) == 0:
             raise TypeError(
-                f"cannot convert field with name '{field.name}' to Parameter")
+                f"cannot convert field with name '{field.name}' to Parameter"
+            )
         return cls(**kwargs)
 
     def is_flag(self) -> bool:
         """Indicates if argument is a flag with ``action="store_true/false``."""
         return self.type is bool
 
     def get_kwargs(self) -> dict[str, Any]:
@@ -89,36 +92,35 @@
         default = kwargs.pop("default_text")
         if default is not None:
             kwargs["help"] += " " + default
         return kwargs
 
 
 def get_doc_args(
-    dclass: object | type,
-    indicate_opt: bool = True
+    dclass: object | type, indicate_opt: bool = True
 ) -> list[tuple[str, str | None]]:
     """Generate a section with default values for a YAML configuration file.
-    
+
     Entries are added for those dataclass fields that contain a Parameter
     instance in the ``metadata`` field.
     """
     lines = []
     argfields = fields(dclass)
     if len(argfields) > 0:
-        for field in argfields:
+        for cfield in argfields:
             try:  # omit parameter if not shipped with parameter information
-                param = Parameter.from_field(field)
+                param = Parameter.from_field(cfield)
                 # format the value as 'key: value'
-                if field.default is not MISSING:
-                    default = field.default
+                if cfield.default is not MISSING:
+                    default = cfield.default
                     optional = True
                 else:
                     default = None
                     optional = False
-                value = yaml.dump({field.name.strip("_"): default}).strip()
+                value = yaml.dump({cfield.name.strip("_"): default}).strip()
                 # format the optional comment
                 comment = param.help
                 if indicate_opt and optional:
                     comment = "(opt) " + comment
                 if param.choices is not None:
                     comment += f" ({', '.join(param.choices)})"
                 lines.append((value, comment))
@@ -126,41 +128,45 @@
                 pass
     return lines
 
 
 def populate_parser(
     dclass: object | type,
     default_parser: ArgumentParser,
-    extra_parsers: Mapping[str, ArgumentParser] | None = None
+    extra_parsers: Mapping[str, ArgumentParser] | None = None,
 ) -> None:
     """Populate a parser instance or argument group with arguments from a
     dataclass.
-    
+
     Arguments are added for those dataclass fields that contain a Parameter
     instance in the ``metadata`` field.
     """
-    for field in fields(dclass):
+    for cfield in fields(dclass):
         try:
-            parameter = Parameter.from_field(field)
+            parameter = Parameter.from_field(cfield)
         except TypeError:
             continue
-        name = field.name.strip("_").replace("_", "-")
+        name = cfield.name.strip("_").replace("_", "-")
 
         if parameter.parser_id == "default":
             parser = default_parser
         else:
             parser = extra_parsers[parameter.parser_id]
-        
+
         if parameter.is_flag():
-            if field.default == True:
+            if cfield.default is True:
                 parser.add_argument(
-                    f"--no-{name}", dest=field.name,
-                    action="store_false", help=parameter.help)
+                    f"--no-{name}",
+                    dest=cfield.name,
+                    action="store_false",
+                    help=parameter.help,
+                )
             else:
                 parser.add_argument(
-                    f"--{name}", action="store_true", help=parameter.help)
+                    f"--{name}", action="store_true", help=parameter.help
+                )
 
         else:
             kwargs = parameter.get_kwargs()
-            if field.default is not MISSING:
-                kwargs["default"] = field.default
+            if cfield.default is not MISSING:
+                kwargs["default"] = cfield.default
             parser.add_argument(f"--{name}", **kwargs)
```

### Comparing `yet_another_wizz-2.5/src/yaw/core/logging.py` & `yet_another_wizz-2.5.post0/src/yaw/core/logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 
 import logging
 import warnings
 from datetime import timedelta
 from timeit import default_timer
 from typing import Callable
 
+__all__ = ["LogCustomWarning", "TimedLog"]
+
 
 class LogCustomWarning:
     """Context wrapper that temporarily redirects warnings to a logger."""
 
     def __init__(
         self,
         logger: logging.Logger,
         alt_message: str | None = None,
-        ignore: bool = True
+        ignore: bool = True,
     ):
         """Instead of showing the warning through the :func:`warnings.warn`
         machinery, write the message as warning to the provided logger.
 
         Args:
             logger (:obj:`logging.Logger`):
                 The logger instance to which the warning is redirected.
@@ -51,29 +53,25 @@
     def __exit__(self, exc_type, exc_value, exc_traceback) -> None:
         warnings.showwarning = self._old_showwarning
 
 
 class TimedLog:
     """Context wrapper that measures the elapsed time and emits a log message on
     exit.
-    
+
     Emits a log in the format ``{message} - done {elapsed time}``.
 
     Args:
         logging_callback (Callable):
             Function that processes the log message on context wrapper exit.
         msg (:obj:`str`, optional):
             The log message body.
     """
 
-    def __init__(
-        self,
-        logging_callback: Callable,
-        msg: str | None = None
-    ) -> None:
+    def __init__(self, logging_callback: Callable, msg: str | None = None) -> None:
         self.callback = logging_callback
         self.msg = msg
 
     def __enter__(self) -> TimedLog:
         self.t = default_timer()
         return self
```

### Comparing `yet_another_wizz-2.5/src/yaw/core/math.c` & `yet_another_wizz-2.5.post0/src/yaw/core/math.c`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
             // check for full or partial overlap
             contains = (zmin_n >= zmin_o) && (zmax_n < zmax_o);
             overlaps_min = (zmin_n <= zmin_o) && (zmax_n > zmin_o);
             overlaps_max = (zmin_n <= zmax_o) && (zmax_n > zmax_o);
 
             if (contains || overlaps_min || overlaps_max) {
-                // compute fractional bin overlap 
+                // compute fractional bin overlap
                 zmin_overlap = MAX(zmin_o, zmin_n);
                 zmax_overlap = MIN(zmax_o, zmax_n);
                 fraction = (zmax_overlap - zmin_overlap) / (zmax_o - zmin_o);
 
                 // assume uniform distribution of data in bin and increment
                 // counts by the bin count weighted by the overlap fraction
                 counts_new[i_new] += count * fraction;
```

### Comparing `yet_another_wizz-2.5/src/yaw/core/math.py` & `yet_another_wizz-2.5.post0/src/yaw/core/math.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,42 +9,53 @@
 import numpy as np
 from numpy.typing import NDArray
 
 from ._math import _rebin
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import ArrayLike
+
     from yaw.core.containers import SampledData
 
+__all__ = [
+    "array_equal",
+    "outer_triu_sum",
+    "apply_bool_mask_ndim",
+    "apply_slice_ndim",
+    "sgn",
+    "cov_from_samples",
+    "global_covariance",
+    "corr_from_cov",
+    "rebin",
+    "shift_histogram",
+]
+
 
 _Tarr = TypeVar("_Tarr", bound=NDArray)
 
 
 def array_equal(arr1: NDArray, arr2: NDArray) -> bool:
     """Check if the shape and array elements of two numpy array are equal."""
     return (
-        isinstance(arr1, np.ndarray) and
-        isinstance(arr2, np.ndarray) and
-        arr1.shape == arr2.shape and
-        (arr1 == arr2).all())
+        isinstance(arr1, np.ndarray)
+        and isinstance(arr2, np.ndarray)
+        and arr1.shape == arr2.shape
+        and (arr1 == arr2).all()
+    )
 
 
 def outer_triu_sum(
-    a: ArrayLike,
-    b: ArrayLike,
-    *,
-    k: int = 0,
-    axis: int | None = None
+    a: ArrayLike, b: ArrayLike, *, k: int = 0, axis: int | None = None
 ) -> NDArray:
     """Compute the sum over the upper triangle of the outer product.
 
     Shapes of input array must be identical. Equivalent to
-    
+
     >>> np.triu(np.outer(a, b), k).sum(axis)
-    
+
     but supports extra dimensions in a and b and does not construct the full
     outer product matrix in memory.
 
     Args:
         a (:obj:`NDArray`):
             First input array.
         b (:obj:`NDArray`):
@@ -63,54 +74,51 @@
         raise IndexError("shape of 'a' and 'b' does not match")
     # allocate output array
     dtype = (a[0] * b[0]).dtype  # correct dtype for product
     N = len(a)
     # sum all elements
     if axis is None:
         result = np.zeros_like(a[0], dtype=dtype)
-        for i in range(min(N, N-k)):
-            result += (a[i] * b[max(0, i+k):]).sum(axis=0)
+        for i in range(min(N, N - k)):
+            result += (a[i] * b[max(0, i + k) :]).sum(axis=0)
     # sum row-wise
     elif axis == 1:
         result = np.zeros_like(b, dtype=dtype)
-        for i in range(min(N, N-k)):
-            result[i] = (a[i] * b[max(0, i+k):]).sum(axis=0)
+        for i in range(min(N, N - k)):
+            result[i] = (a[i] * b[max(0, i + k) :]).sum(axis=0)
     # sum column-wise
     elif axis == 0:
         result = np.zeros_like(a, dtype=dtype)
         for i in range(max(0, k), N):
-            result[i] = (a[:min(N, max(0, i-k+1))] * b[i]).sum(axis=0)
+            result[i] = (a[: min(N, max(0, i - k + 1))] * b[i]).sum(axis=0)
     return result[()]
 
 
 def apply_bool_mask_ndim(
-    array: _Tarr,
-    mask: NDArray[np.bool_],
-    axis: int | Sequence[int] | None = None
+    array: _Tarr, mask: NDArray[np.bool_], axis: int | Sequence[int] | None = None
 ) -> _Tarr:
     """Apply a boolean mask (``mask``) to one or many axes of a numpy array."""
     if axis is None:
         axis = list(range(array.ndim))
     elif isinstance(axis, int):
         axis = [axis]
     result = array
     for ax in axis:
         if result.shape[ax] != len(mask):
             raise IndexError(
                 f"boolean index did not match indexed array along dimension "
                 f"{ax}; dimension is {result.shape[ax]} but corresponding "
-                f"boolean dimension is {len(mask)}")
+                f"boolean dimension is {len(mask)}"
+            )
         result = np.compress(mask, result, axis=ax)
     return result
 
 
 def apply_slice_ndim(
-    array: _Tarr,
-    item: int | slice | Sequence,
-    axis: int | Sequence[int] | None = None
+    array: _Tarr, item: int | slice | Sequence, axis: int | Sequence[int] | None = None
 ) -> _Tarr:
     """Apply an integer subset or slice (``item``) to one or many axes of a
     numpy array."""
     if axis is None:
         axis = list(range(array.ndim))
     elif isinstance(axis, int):
         axis = [axis]
@@ -135,18 +143,18 @@
     return np.where(val == 0, 1.0, np.sign(val))
 
 
 def cov_from_samples(
     samples: NDArray | Sequence[NDArray],
     method: str,
     rowvar: bool = False,
-    kind: str = "full"  # full, diag, var
+    kind: str = "full",  # full, diag, var
 ) -> NDArray:
     """Compute a joint covariance from a sequence of data samples.
-    
+
     These samples can be jackknife or bootstrap samples (etc.). If more than one
     set of samples is provided, the samples are concatenated along the second
     axis (default) or along the first axis if ``rowvar=True``.
 
     Args:
         samples (:obj`:NDArray`, :obj:`Sequence[NDArray]`):
             One or many sets of data samples. The number of samples must be
@@ -203,17 +211,15 @@
         covmat = np.diag(np.diag(covmat, k=0), k=0)
     else:
         raise ValueError(f"invalid covariance kind '{kind}'")
     return covmat
 
 
 def global_covariance(
-    data: Sequence[SampledData],
-    method: str | None = None,
-    kind: str = "full"
+    data: Sequence[SampledData], method: str | None = None, kind: str = "full"
 ) -> NDArray:
     """Compute a joint covariance from a set of resampled data.
 
     Typically applied to a set of :obj:`CorrData`,
     :obj:`~yaw.redshifts.RedshiftData`, or :obj:`~yaw.redshifts.HistData`
     containers. The joint covariance is computed by concatenating the samples
     along the redshift binning axis.
@@ -253,49 +259,46 @@
     outer_v = np.outer(v, v)
     return covariance / outer_v
 
 
 def rebin(
     bins_new: NDArray[np.float_],
     bins_old: NDArray[np.float_],
-    counts_old: NDArray[np.float_]
+    counts_old: NDArray[np.float_],
 ) -> NDArray[np.float_]:
     """Recompute compute histogram counts for a new binning.
 
     The new counts are computed by summing the fractional contribution of the
     counts from the original binning to the binning. The new binning may exceed
     or just partially cover the range of the original binning.
 
     Args:
         bins_new (:obj:`NDArray`):
             The new bin edges on which the counts are reevaluated.
         bins_old (:obj:`NDArray`):
             The bin edges from which the original counts were computed.
         counts_old (:obj:`NDArray`):
             The original histogram counts.
- 
+
     Returns:
         :obj:`NDArray`:
-            The histogram counts for the new binning.            
+            The histogram counts for the new binning.
 
     .. Note::
         Implemented as C extension.
     """
     return _rebin(
         bins_new.astype(np.float_),
         bins_old.astype(np.float_),
-        counts_old.astype(np.float_))
+        counts_old.astype(np.float_),
+    )
 
 
 def shift_histogram(
-    bins: NDArray,
-    counts: NDArray,
-    *,
-    A: float = 1.0,
-    dx: float = 0.0
+    bins: NDArray, counts: NDArray, *, A: float = 1.0, dx: float = 0.0
 ) -> NDArray:
     """Shift a histogram by a fixed value.
 
     The histogram values are recomputed for new bin edges that are shifted by
     the desired amount using :func:`rebin`. The normalisation of the histogram
     may change if the shifted binning does not cover the full range of the data.
 
@@ -306,15 +309,15 @@
             The histogram counts.
 
     Keyword args:
         A (:obj:`float`, optional):
             Scalar amplitude used to rescale the new histgram counts.
         dx (:obj:`float`, optional):
             Amount by which the histogram (i.e. the bin edges) are shifted.
- 
+
     Returns:
         :obj:`NDArray`:
-            The shifted histogram counts.            
+            The shifted histogram counts.
     """
     bins_old = bins.astype(np.float_)
     bins_new = bins_old + dx
     return A * _rebin(bins_new, bins_old, counts.astype(np.float_))
```

### Comparing `yet_another_wizz-2.5/src/yaw/core/parallel.py` & `yet_another_wizz-2.5.post0/src/yaw/core/parallel.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from typing import TYPE_CHECKING, Any, Generic, TypeVar
 
 import numpy as np
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import DTypeLike, NDArray
 
+__all__ = ["SharedArray", "ParallelHelper"]
+
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass(frozen=True)
 class SharedArray:
     """Container for shared array that can be easily shared with other
@@ -45,19 +47,25 @@
     dtype: DTypeLike
     """Numpy-style data type of the array."""
 
     @staticmethod
     def _get_mp_type(dtype: DTypeLike | str) -> str:
         type_map = {
             "|b1": "b",  # no bool correspondance, but same number of bytes
-            "i1": "h", "u1": "H",
-            "i2": "i", "u2": "I",
-            "i4": "l", "u4": "L",
-            "i8": "q", "u8": "Q",
-            "f4": "f", "f8": "d"}
+            "i1": "h",
+            "u1": "H",
+            "i2": "i",
+            "u2": "I",
+            "i4": "l",
+            "u4": "L",
+            "i8": "q",
+            "u8": "Q",
+            "f4": "f",
+            "f8": "d",
+        }
         if isinstance(dtype, str):
             dtype = np.dtype(dtype)
         try:
             return type_map[dtype.str.strip("<>")]
         except KeyError as e:
             raise NotImplementedError(
                 f"cannot convert numpy dtype '{dtype.str}' to RawArray"
@@ -66,67 +74,63 @@
     def __len__(self) -> int:
         return self.shape[0]
 
     def __del__(self) -> None:
         object.__delattr__(self, "array")
 
     @classmethod
-    def empty(
-        cls,
-        shape: tuple[int],
-        dtype: DTypeLike | str
-    ) -> SharedArray:
+    def empty(cls, shape: tuple[int], dtype: DTypeLike | str) -> SharedArray:
         """Create an new class instance with uninitialised memory.
-        
+
         Args:
             shape (:obj:`tuple[int]`):
                 Shape of the array.
             dtype (:obj:`DTypeLike`):
                 Numpy-style data type of the array.
 
         Returns:
-            :obj:`SharedArray`                
+            :obj:`SharedArray`
         """
         mtype = cls._get_mp_type(dtype)
         size = int(np.prod(shape))
         new = cls(
-            multiprocessing.RawArray(mtype, size),
-            shape=shape, dtype=np.dtype(dtype))
+            multiprocessing.RawArray(mtype, size), shape=shape, dtype=np.dtype(dtype)
+        )
         return new
 
     @classmethod
     def from_numpy(cls, array: NDArray) -> SharedArray:
         """Create an new class instance from a numpy array.
 
         Args:
             array (:obj:`NDArray`):
                 Input array, used to initialise the shared memory.
 
         Returns:
-            :obj:`SharedArray`                
+            :obj:`SharedArray`
         """
         new = cls.empty(array.shape, array.dtype)
         try:
             buffer = new.to_numpy()
             np.copyto(buffer, array)
+            return new
         except Exception:
             del new
             raise
-        return new
 
     def to_numpy(self, copy: bool = False) -> NDArray:
         """Reconstruct the original numpy array from shared memory.
-        
+
         Args:
             copy (:obj:`bool`):
                 Whether to copy the array values instead of wrapping the shared
                 memory (zero-copy).
 
         Returns:
-            :obj:`NDArray`                
+            :obj:`NDArray`
         """
         arr = np.frombuffer(self.array, dtype=self.dtype).reshape(self.shape)
         if copy:
             return np.copy(arr)
         else:
             return arr
 
@@ -135,15 +139,15 @@
 """Global dictionary used to share :obj:`SharedArray` instances with other
 processes."""
 
 
 def _threadinit(
     shares_dict: dict[str, SharedArray],
     initializer: Callable | None = None,
-    initargs: Iterable | None = None
+    initargs: Iterable | None = None,
 ) -> None:
     """Initialiser function used to send shared arrays to processes."""
     POOL_SHARE.update(shares_dict)
     # call the usual initializer function provided by the user
     if initializer is not None:
         initializer(*initargs)
 
@@ -175,18 +179,15 @@
     .. Tip::
         After completion, call the :meth:`free` method to free the memory of all
         shared array, or use this class as a context wrapper, which will
         automate this process on exit.
     """
 
     def __init__(
-        self,
-        function: Callable[..., _T],
-        n_items: int,
-        num_threads: int | None = None
+        self, function: Callable[..., _T], n_items: int, num_threads: int | None = None
     ) -> None:
         """Create a new instane.
 
         Args:
             function (Callable):
                 Function which accepts an arbitray number of positional
                 arguments.
@@ -228,19 +229,19 @@
 
     def n_threads(self):
         """The total number of threads to use for processing."""
         return self._num_threads
 
     def add_shared_array(self, key: str, array: NDArray | SharedArray) -> None:
         """Add a new shared array as function argument.
-        
+
         .. Note::
             The array will be treated as constant, i.e. the same array is
             applied at each function call.
-        
+
         Args:
             key (:obj:`str`):
                 Identifier name at which the array is registered in the new
                 processes namespace.
             array (:obj:`NDArray`, :obj:`SharedArray`):
                 Array, if numpy array, converted automatically to shared array.
         """
@@ -254,84 +255,76 @@
         """Add the next function argument which will be repeated at each
         function call."""
         self.args.append([value] * self._n_items)
 
     def add_iterable(self, iterable: Collection) -> None:
         """Add the next function argument which will be iterated at each
         function call.
-        
+
         Must be an iterable with :meth:`n_jobs` items.
         """
         if len(iterable) != self._n_items:
-            raise ValueError(
-                f"length of iterable argument must be {self._n_items}")
+            raise ValueError(f"length of iterable argument must be {self._n_items}")
         self.args.append(iterable)
 
     def _init_pool(
-        self,
-        initializer: Callable | None = None,
-        initargs: Iterable | None = None
+        self, initializer: Callable | None = None, initargs: Iterable | None = None
     ) -> multiprocessing.Pool:
-        """Initialises the worker processes for the :obj:`multiprocessing.Pool`.
-        """
+        """Initialises the worker processes for the :obj:`multiprocessing.Pool`."""
         all_initargs = [self.shares]
         if initializer is not None:
             all_initargs.append(initializer)
             if isinstance(initargs, Iterable):
                 all_initargs.append(initargs)
             elif initargs is None:
                 all_initargs.append(None)
             else:
                 raise TypeError("'initargs' must be an iterable")
-        logger.debug(
-            f"running {self.n_jobs()} jobs on {self.n_threads()} threads")
+        logger.debug(f"running {self.n_jobs()} jobs on {self.n_threads()} threads")
         return multiprocessing.Pool(
-            initializer=_threadinit,
-            initargs=all_initargs,
-            processes=self._num_threads)
+            initializer=_threadinit, initargs=all_initargs, processes=self._num_threads
+        )
 
     def result(
-        self,
-        initializer: Callable | None = None,
-        initargs: Iterable | None = None
+        self, initializer: Callable | None = None, initargs: Iterable | None = None
     ) -> list[_T]:
         """Apply the accumulated arguments to a function in a pool of processes.
 
         The call is blocking until all results are received.
 
         Args:
             initializer (Callable, optional):
                 Custom initialiser function to call when creating the pool.
             initargs (Iterable, optional):
                 Arguments applied to the initialiser function.
-        
+
         Returns:
             :obj:`list`:
                 List containing the return values from all function calls.
         """
         with self._init_pool(initializer, initargs) as pool:
             results = pool.starmap(self.function, zip(*self.args))
         return results
 
     def iter_result(
         self,
         initializer: Callable | None = None,
         initargs: Iterable | None = None,
-        ordered: bool = True
+        ordered: bool = True,
     ) -> Iterator[_T]:
         """Apply the accumulated arguments to a function in a pool of processes.
 
         Returns an iterator over the available thread results.
 
         Args:
             initializer (Callable, optional):
                 Custom initialiser function to call when creating the pool.
             initargs (Iterable, optional):
                 Arguments applied to the initialiser function.
-        
+
         Yields:
             :obj:`list`:
                 Iterator over the return values.
         """
         function = functools.partial(_threadwrapper, function=self.function)
         with self._init_pool(initializer, initargs) as pool:
             imap_args = (function, zip(*self.args))
```

### Comparing `yet_another_wizz-2.5/src/yaw/core/utils.py` & `yet_another_wizz-2.5.post0/src/yaw/core/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,28 +8,29 @@
 from pathlib import Path
 from typing import TypeVar, Union
 
 import numpy as np
 import tqdm
 from numpy.typing import NDArray
 
-
-try:
-    from itertools import pairwise as iter_pairwise
-except ImportError:
-    from more_itertools import pairwise as iter_pairwise
+__all__ = [
+    "job_progress_bar",
+    "LimitTracker",
+    "long_num_format",
+    "bytes_format",
+    "format_float_fixed_width",
+]
 
 
 TypePathStr = Union[Path, str]
 Tjob = TypeVar("Tjob")
 
 
 def job_progress_bar(
-    iterable: Iterable[Tjob],
-    total: int | None = None
+    iterable: Iterable[Tjob], total: int | None = None
 ) -> Iterable[Tjob]:
     """Configure and return a tqdm progress bar with custom format."""
     config = dict(delay=0.5, leave=False, smoothing=0.1, unit="jobs")
     return tqdm.tqdm(iterable, total=total, **config)
 
 
 class LimitTracker:
```

### Comparing `yet_another_wizz-2.5/src/yaw/correlation/corrfuncs.py` & `yet_another_wizz-2.5.post0/src/yaw/correlation/corrfuncs.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,34 +12,41 @@
 
 import h5py
 import numpy as np
 import pandas as pd
 from deprecated import deprecated
 
 from yaw.catalogs import PatchLinkage
-from yaw.config import ResamplingConfig, OPTIONS
+from yaw.config import OPTIONS, ResamplingConfig
 from yaw.core.abc import BinnedQuantity, HDFSerializable, PatchedQuantity
 from yaw.core.containers import Indexer, SampledData
 from yaw.core.logging import LogCustomWarning, TimedLog
-from yaw.core.utils import TypePathStr, format_float_fixed_width as fmt_num
+from yaw.core.utils import TypePathStr
+from yaw.core.utils import format_float_fixed_width as fmt_num
 from yaw.correlation.estimators import (
-    CorrelationEstimator, CtsMix, cts_from_code, EstimatorError)
+    CorrelationEstimator,
+    CtsMix,
+    EstimatorError,
+    cts_from_code,
+)
 from yaw.correlation.paircounts import NormalisedCounts, TypeIndex
 
 if TYPE_CHECKING:  # pragma: no cover
     from matplotlib.axis import Axis
     from numpy.typing import NDArray
     from pandas import IntervalIndex
+
     from yaw.catalogs import BaseCatalog
     from yaw.config import Configuration
     from yaw.correlation.estimators import Cts
 
+__all__ = ["CorrData", "CorrFunc", "add_corrfuncs", "autocorrelate", "crosscorrelate"]
 
-logger = logging.getLogger(__name__)
 
+logger = logging.getLogger(__name__)
 
 _Tdata = TypeVar("_Tdata", bound="CorrData")
 
 
 @dataclass(frozen=True, repr=False, eq=False)
 class CorrData(SampledData):
     """Container class for sampled correlation function data.
@@ -106,35 +113,34 @@
 
     @classmethod
     def from_files(cls: Type[_Tdata], path_prefix: TypePathStr) -> _Tdata:
         """Create a new instance by loading the data from ASCII files.
 
         The data is restored from a set of three input files produced by
         :meth:`to_files`.
-        
+
         .. Note::
             These file have the same names but different file extension,
             therefore only provide the base name without any extension to
             specifiy the input files.
 
         Args:
             path_prefix (:obj:`str`):
                 The base name of the input files without any file extension.
-        
+
         Returns:
             :obj:`CorrData`
         """
         name = cls.__name__.lower()[:-4]
         logger.debug(f"reading {name} data from '{path_prefix}.*'")
         # load data and errors
         ext = "dat"
         data_error = np.loadtxt(f"{path_prefix}.{ext}")
         # restore index
-        binning = pd.IntervalIndex.from_arrays(
-            data_error[:, 0], data_error[:, 1])
+        binning = pd.IntervalIndex.from_arrays(data_error[:, 0], data_error[:, 1])
         # load samples
         ext = "smp"
         samples = np.loadtxt(f"{path_prefix}.{ext}")
         # load header
         info = None
         with open(f"{path_prefix}.{ext}") as f:
             for line in f.readlines():
@@ -156,52 +162,55 @@
         else:
             raise ValueError(f"invalid sampling method key '{method_key}'")
         return cls(
             binning=binning,
             data=data_error[:, 2],  # take data column
             samples=samples.T[2:],  # remove redshift bin columns
             method=method,
-            info=info)
+            info=info,
+        )
 
     @property
     def _dat_desc(self) -> str:
         """Description included in the data file."""
         return (
             "# correlation function estimate with symmetric 68% percentile "
-            "confidence")
+            "confidence"
+        )
 
     @property
     def _smp_desc(self) -> str:
         """Description included in the samples file."""
         return f"# {self.n_samples} {self.method} correlation function samples"
 
     @property
     def _cov_desc(self) -> str:
         """Description included in the covariance file."""
         return (
             f"# correlation function estimate covariance matrix "
-            f"({self.n_bins}x{self.n_bins})")
+            f"({self.n_bins}x{self.n_bins})"
+        )
 
     def to_files(self, path_prefix: TypePathStr) -> None:
         """Store the data in a set of ASCII files on disk.
 
         These files can be loaded with the :meth:`from_files` method. There are
         three files with the same name but different file extension.
 
         .. rubric:: Files
 
         ``[path_prefix].dat``: Contains the redshift bin edges, the data values
         and their standard error. Additionally there is information about the
         error estimate and the :obj:`info` attribute.
-        
+
         ``[path_prefix].smp``: Contains one row for each redshift bin. The first
         two columns list the lower and upper edge of the redshift bin, the
         remaining columns list the values of the samples, i.e. there are ``N+2``
         columns. Additionally contains the :obj:`info` attribute.
-        
+
         ``[path_prefix].cov``: Contains the covariance matrix and additionally
         the :obj:`info` attribute.
 
         Args:
             path_prefix (:obj:`str`):
                 The base name of the output files without any file extension.
         """
@@ -222,26 +231,23 @@
 
         # write data and errors
         ext = "dat"
         header = ["z_low", "z_high", "nz", "nz_err"]
         with open(f"{path_prefix}.{ext}", "w") as f:
             write_head(f, comment(self._dat_desc), header, delim=DELIM)
             for zlow, zhigh, nz, nz_err in zip(
-                self.edges[:-1], self.edges[1:],
-                self.data, self.error
+                self.edges[:-1], self.edges[1:], self.data, self.error
             ):
-                values = [
-                    fmt_num(val, PREC) for val in (zlow, zhigh, nz, nz_err)]
+                values = [fmt_num(val, PREC) for val in (zlow, zhigh, nz, nz_err)]
                 f.write(DELIM.join(values) + "\n")
 
         # write samples
         ext = "smp"
         header = ["z_low", "z_high"]
-        header.extend(
-            f"{self.method[:4]}_{i}" for i in range(self.n_samples))
+        header.extend(f"{self.method[:4]}_{i}" for i in range(self.n_samples))
         with open(f"{path_prefix}.{ext}", "w") as f:
             write_head(f, comment(self._smp_desc), header, delim=DELIM)
             for zlow, zhigh, samples in zip(
                 self.edges[:-1], self.edges[1:], self.samples.T
             ):
                 values = [fmt_num(zlow, PREC), fmt_num(zhigh, PREC)]
                 values.extend(fmt_num(val, PREC) for val in samples)
@@ -249,15 +255,15 @@
 
         # write covariance (just for convenience)
         ext = "cov"
         fmt_str = DELIM.join("{: .{prec}e}" for _ in range(self.n_bins)) + "\n"
         with open(f"{path_prefix}.{ext}", "w") as f:
             f.write(f"{comment(self._cov_desc)}\n")
             for values in self.covariance:
-                f.write(fmt_str.format(*values, prec=PREC-3))
+                f.write(fmt_str.format(*values, prec=PREC - 3))
 
     def _make_plot(
         self,
         x: NDArray[np.float_],
         y: NDArray[np.float_],
         yerr: NDArray[np.float_],
         *,
@@ -265,14 +271,15 @@
         label: str | None = None,
         error_bars: bool = True,
         ax: Axis | None = None,
         plot_kwargs: dict[str, Any] | None = None,
         zero_line: bool = False,
     ) -> Axis:
         from matplotlib import pyplot as plt
+
         # configure plot
         if ax is None:
             ax = plt.gca()
         if plot_kwargs is None:
             plot_kwargs = {}
         plot_kwargs.update(dict(color=color, label=label))
         ebar_kwargs = dict(fmt=".", ls="none")
@@ -297,15 +304,15 @@
         color: str | NDArray | None = None,
         label: str | None = None,
         error_bars: bool = True,
         ax: Axis | None = None,
         xoffset: float = 0.0,
         plot_kwargs: dict[str, Any] | None = None,
         zero_line: bool = False,
-        scale_by_dz: bool = False
+        scale_by_dz: bool = False,
     ) -> Axis:  # pragma: no cover
         """Create a plot of the correlation data as a function of redshift.
 
         Create a new axis or plot to an existing one, add x-axis offsets, if
         plotting multiple instances, or specify if the values should be
         represented as points with errorbars (default) or as line plot with
         shaded area to represent uncertainties.
@@ -335,24 +342,27 @@
         x = self.mids + xoffset
         y = self.data
         yerr = self.error
         if scale_by_dz:
             y *= self.dz
             yerr *= self.dz
         return self._make_plot(
-            x, y, yerr,
-            color=color, label=label, error_bars=error_bars, ax=ax,
-            plot_kwargs=plot_kwargs, zero_line=zero_line)
+            x,
+            y,
+            yerr,
+            color=color,
+            label=label,
+            error_bars=error_bars,
+            ax=ax,
+            plot_kwargs=plot_kwargs,
+            zero_line=zero_line,
+        )
 
     def plot_corr(
-        self,
-        *,
-        redshift: bool = False,
-        cmap: str = "RdBu_r",
-        ax: Axis | None = None
+        self, *, redshift: bool = False, cmap: str = "RdBu_r", ax: Axis | None = None
     ) -> Axis:
         """Plot the correlation matrix of the data.
 
         Create a new axis or plot to an existing one.
 
         Args:
             redshift (:obj:`bool`, optional):
@@ -441,15 +451,15 @@
 
     Sample the correlation function
 
     >>> corr.sample()  # uses the default ResamplingConfig
     CorrData(n_bins=30, z='0.070...1.420', n_samples=64, method='jackknife')
 
     Note how the indicated shape changes when a patch subset is selected:
-    
+
     >>> corr.patches[:10]
     CorrFunc(n_bins=30, z='0.070...1.420', dd=True, dr=True, rd=False, rr=False, n_patches=10)
 
     Note how the indicated redshift range and shape change when a bin subset is
     selected:
 
     >>> corr.bins[:3]
@@ -484,146 +494,134 @@
             pairs: NormalisedCounts | None = getattr(self, kind)
             if pairs is None:
                 continue
             try:
                 self.dd.is_compatible(pairs, require=True)
             except ValueError as e:
                 raise ValueError(
-                    f"pair counts '{kind}' and 'dd' are not compatible") from e
+                    f"pair counts '{kind}' and 'dd' are not compatible"
+                ) from e
 
     def __repr__(self) -> str:
         string = super().__repr__()[:-1]
         pairs = f"dd=True, dr={self.dr is not None}, "
         pairs += f"rd={self.rd is not None}, rr={self.rr is not None}"
         other = f"n_patches={self.n_patches}"
         return f"{string}, {pairs}, {other})"
 
     def __eq__(self, other) -> bool:
         if not isinstance(other, self.__class__):
             return False
-        for field in fields(self):
-            kind = field.name
+        for cfield in fields(self):
+            kind = cfield.name
             if getattr(self, kind) != getattr(other, kind):
                 return False
         return True
 
     def __neq__(self, other) -> bool:
         return not self == other
 
     def __add__(self, other: CorrFunc) -> CorrFunc:
         # check that the pair counts are set consistently
         kinds = []
-        for field in fields(self):
-            kind = field.name
+        for cfield in fields(self):
+            kind = cfield.name
             self_set = getattr(self, kind) is not None
             other_set = getattr(other, kind) is not None
             if (self_set and not other_set) or (not self_set and other_set):
-                raise ValueError(
-                    f"pair counts for '{kind}' not set for both operands")
+                raise ValueError(f"pair counts for '{kind}' not set for both operands")
             elif self_set and other_set:
                 kinds.append(kind)
 
-        kwargs = {
-            kind: getattr(self, kind) + getattr(other, kind) for kind in kinds}
+        kwargs = {kind: getattr(self, kind) + getattr(other, kind) for kind in kinds}
         return self.__class__(**kwargs)
 
-    def __radd__(
-        self,
-        other: CorrFunc | int | float
-    ) -> CorrFunc:
+    def __radd__(self, other: CorrFunc | int | float) -> CorrFunc:
         if other == 0:
             return self
         else:
             return self.__add__(other)
 
     def __mul__(self, other: np.number) -> CorrFunc:
         # check that the pair counts are set consistently
         kwargs = {}
-        for field in fields(self):
-            kind = field.name
+        for cfield in fields(self):
+            kind = cfield.name
             counts = getattr(self, kind)
             if counts is not None:
                 kwargs[kind] = counts * other
         return self.__class__(**kwargs)
 
     @property
     def auto(self) -> bool:
         """Whether the stored data are from an autocorrelation measurement."""
         return self.dd.auto
 
     @property
     def bins(self) -> Indexer[TypeIndex, CorrFunc]:
-        def builder(
-            inst: CorrFunc, item: TypeIndex
-        ) -> CorrFunc:
+        def builder(inst: CorrFunc, item: TypeIndex) -> CorrFunc:
             if isinstance(item, int):
                 item = [item]
             kwargs = {}
-            for field in fields(inst):
-                pairs: NormalisedCounts | None = getattr(inst, field.name)
+            for cfield in fields(inst):
+                pairs: NormalisedCounts | None = getattr(inst, cfield.name)
                 if pairs is None:
-                    kwargs[field.name] = None
+                    kwargs[cfield.name] = None
                 else:
-                    kwargs[field.name] = pairs.bins[item]
+                    kwargs[cfield.name] = pairs.bins[item]
             return CorrFunc(**kwargs)
 
         return Indexer(self, builder)
 
     @property
     def patches(self) -> Indexer[TypeIndex, CorrFunc]:
-        def builder(
-            inst: CorrFunc, item: TypeIndex
-        ) -> CorrFunc:
+        def builder(inst: CorrFunc, item: TypeIndex) -> CorrFunc:
             kwargs = {}
-            for field in fields(inst):
-                counts: NormalisedCounts | None = getattr(inst, field.name)
+            for cfield in fields(inst):
+                counts: NormalisedCounts | None = getattr(inst, cfield.name)
                 if counts is not None:
                     counts = counts.patches[item]
-                kwargs[field.name] = counts
+                kwargs[cfield.name] = counts
             return CorrFunc(**kwargs)
 
         return Indexer(self, builder)
 
     def get_binning(self) -> IntervalIndex:
         return self.dd.get_binning()
 
     @property
     def n_patches(self) -> int:
         return self.dd.n_patches
 
-    def is_compatible(
-        self,
-        other: CorrFunc,
-        require: bool = True
-    ) -> bool:
+    def is_compatible(self, other: CorrFunc, require: bool = True) -> bool:
         """Check whether this instance is compatible with another instance.
-         
+
         Ensures that the redshift binning and the number of patches are
         identical.
-        
+
         Args:
             other (:obj:`BinnedQuantity`):
                 Object instance to compare to.
             require (:obj:`bool`)
                 Raise a ValueError if any of the checks fail.
-        
+
         Returns:
             :obj:`bool`
         """
         if self.dd.n_patches != other.dd.n_patches:
             if require:
                 raise ValueError("number of patches does not agree")
             return False
         return self.dd.is_compatible(other.dd, require)
 
     @property
     def estimators(self) -> dict[str, CorrelationEstimator]:
         """Get a listing of correlation estimators implemented, depending on
         which pair counts are available.
-        
+
         Returns:
             :obj:`dict`: Mapping from correlation estimator name abbreviation to
             correlation function class.
         """
         # figure out which of dd, dr, ... are not None
         available = set()
         # iterate all dataclass attributes that are in __init__
@@ -636,29 +634,28 @@
         estimators = {}
         for estimator in CorrelationEstimator.variants:  # registered estimators
             if set(estimator.requires) <= available:
                 estimators[estimator.short] = estimator
         return estimators
 
     def _check_and_select_estimator(
-        self,
-        estimator: str | None
+        self, estimator: str | None
     ) -> type[CorrelationEstimator]:
         options = self.estimators
         if estimator is None:
             for shortname in ["LS", "DP", "PH"]:  # preferred hierarchy
                 if shortname in options:
                     estimator = shortname
                     break
         estimator = estimator.upper()
         if estimator not in options:
             try:
-                index = [
-                    e.short for e in CorrelationEstimator.variants
-                ].index(estimator)
+                index = [e.short for e in CorrelationEstimator.variants].index(
+                    estimator
+                )
                 est_class = CorrelationEstimator.variants[index]
             except ValueError as e:
                 raise ValueError(f"invalid estimator '{estimator}'") from e
             # determine which pair counts are missing
             for attr in fields(self):
                 name = attr.name
                 if not attr.init:
@@ -667,16 +664,16 @@
                 if getattr(self, name) is None and cts in est_class.requires:
                     raise EstimatorError(f"estimator requires {name}")
             else:
                 raise RuntimeError()
         # select the correct estimator
         cls = options[estimator]
         logger.debug(
-            f"selecting estimator '{cls.short}' from "
-            f"{'/'.join(self.estimators)}")
+            f"selecting estimator '{cls.short}' from {'/'.join(self.estimators)}"
+        )
         return cls
 
     def _getattr_from_cts(self, cts: Cts) -> NormalisedCounts | None:
         if isinstance(cts, CtsMix):
             for code in str(cts).split("_"):
                 value = getattr(self, code)
                 if value is not None:
@@ -694,23 +691,23 @@
         return self.sample(*args, **kwargs)
 
     def sample(
         self,
         config: ResamplingConfig | None = None,
         *,
         estimator: str | None = None,
-        info: str | None = None
+        info: str | None = None,
     ) -> CorrData:
         """Compute the correlation function from the stored pair counts,
         including an error estimate from spatial resampling of patches.
 
         Args:
             config (:obj:`~yaw.ResamplingConfig`):
                 Specify the resampling method and its configuration.
-        
+
         Keyword Args:
             estimator (:obj:`str`, optional):
                 The name abbreviation for the correlation estimator to use.
                 Defaults to Landy-Szalay if RR is available, otherwise to
                 Davis-Peebles.
             info (:obj:`str`, optional):
                 Descriptive text passed on to the output :obj:`CorrData`
@@ -751,15 +748,16 @@
         data = est_fun.eval(**required_data, **optional_data)
         samples = est_fun.eval(**required_samples, **optional_samples)
         return CorrData(
             binning=self.get_binning(),
             data=data,
             samples=samples,
             method=config.method,
-            info=info)
+            info=info,
+        )
 
     @classmethod
     def from_hdf(cls, source: h5py.File | h5py.Group) -> CorrFunc:
         def _try_load(root: h5py.Group, name: str) -> NormalisedCounts | None:
             try:
                 return NormalisedCounts.from_hdf(root[name])
             except KeyError:
@@ -770,16 +768,15 @@
         rd = _try_load(source, "random_data")
         rr = _try_load(source, "random_random")
         return cls(dd=dd, dr=dr, rd=rd, rr=rr)
 
     def to_hdf(self, dest: h5py.File | h5py.Group) -> None:
         group = dest.create_group("data_data")
         self.dd.to_hdf(group)
-        group_names = dict(
-            dr="data_random", rd="random_data", rr="random_random")
+        group_names = dict(dr="data_random", rd="random_data", rr="random_random")
         for kind, name in group_names.items():
             data: NormalisedCounts | None = getattr(self, kind)
             if data is not None:
                 group = dest.create_group(name)
                 data.to_hdf(group)
         dest.create_dataset("n_patches", data=self.n_patches)
 
@@ -790,68 +787,59 @@
             return cls.from_hdf(f)
 
     def to_file(self, path: TypePathStr) -> None:
         logger.info(f"writing pair counts to '{path}'")
         with h5py.File(str(path), mode="w") as f:
             self.to_hdf(f)
 
-    def concatenate_patches(
-        self,
-        *cfs: CorrFunc
-    ) -> CorrFunc:
+    def concatenate_patches(self, *cfs: CorrFunc) -> CorrFunc:
         check_mergable([self, *cfs])
         merged = {}
         for kind in ("dd", "dr", "rd", "rr"):
             self_pcounts = getattr(self, kind)
             if self_pcounts is not None:
                 other_pcounts = [getattr(cf, kind) for cf in cfs]
                 merged[kind] = self_pcounts.concatenate_patches(*other_pcounts)
         return self.__class__(**merged)
 
-    def concatenate_bins(
-        self,
-        *cfs: CorrFunc
-    ) -> CorrFunc:
+    def concatenate_bins(self, *cfs: CorrFunc) -> CorrFunc:
         check_mergable([self, *cfs])
         merged = {}
         for kind in ("dd", "dr", "rd", "rr"):
             self_pcounts = getattr(self, kind)
             if self_pcounts is not None:
                 other_pcounts = [getattr(cf, kind) for cf in cfs]
                 merged[kind] = self_pcounts.concatenate_bins(*other_pcounts)
         return self.__class__(**merged)
 
 
-def _create_dummy_counts(
-    counts: Any | dict[str, Any]
-) -> dict[str, None]:
+def _create_dummy_counts(counts: Any | dict[str, Any]) -> dict[str, None]:
     """Duplicate a the return values of
     :meth:`yaw.catalogs.BaseCatalog.correlate`, but replace the :obj:`CorrFunc`
     instances by :obj:`None`."""
     if isinstance(counts, dict):
         dummy = {scale_key: None for scale_key in counts}
     else:
         dummy = None
     return dummy
 
 
 def add_corrfuncs(
-    corrfuncs: Sequence[CorrFunc],
-    weights: Sequence[np.number] | None = None
+    corrfuncs: Sequence[CorrFunc], weights: Sequence[np.number] | None = None
 ) -> CorrFunc:
     """Add correlation functions that are measured at different scales.
-    
+
     The correlation functions are added by summing together their pair counts.
     They can be weighted prior to summation by effectively scaling their pair
     counts with a set of scalar weights, one for each input correlation
     function.
-    
+
     .. Note::
         The actual scales are not checked, but the number of patches and the
-        redshift binning of the inputs must be identical. 
+        redshift binning of the inputs must be identical.
 
     This operation is effectively equivalent to:
 
     >>> corrfunc1 * weight1 + corrfunc2 * weight2  # + ...
 
     Args:
         corrfuncs (sequence of :obj:`CorrFunc`):
@@ -864,15 +852,16 @@
             The combined correlation function after summing the pairs.
     """
     if weights is None:
         weights = [1.0] * len(corrfuncs)
     else:
         if len(corrfuncs) != len(weights):
             raise ValueError(
-                "number of weights must match number of correlation functions")
+                "number of weights must match number of correlation functions"
+            )
     # run summation, rescaling by weights
     combined = 0.0
     for corrfunc, weight in zip(corrfuncs, weights):
         combined = combined + (corrfunc * weight)
     return combined
 
 
@@ -897,15 +886,15 @@
 def autocorrelate(
     config: Configuration,
     data: BaseCatalog,
     random: BaseCatalog,
     *,
     linkage: PatchLinkage | None = None,
     compute_rr: bool = True,
-    progress: bool = False
+    progress: bool = False,
 ) -> CorrFunc | dict[str, CorrFunc]:
     """Compute an angular autocorrelation function in bins of redshift.
 
     The correlation is measured on fixed physical scales that are converted to
     angles for each redshift bin. All parameters (binning, scales, etc.) are
     bundled in the input configuration, see :mod:`yaw.config`.
 
@@ -939,47 +928,48 @@
             ``kpcXXtXX`` pattern, where ``XX`` are the lower and upper scale
             limit as integers, in kpc (see :obj:`yaw.core.cosmology.Scale`).
     """
     _check_patch_centers([data, random])
     scales = config.scales.as_array()
     logger.info(
         f"running autocorrelation ({len(scales)} scales, "
-        f"{scales.min():.0f}<r<={scales.max():.0f}kpc)")
+        f"{scales.min():.0f}<r<={scales.max():.0f}kpc)"
+    )
     if linkage is None:
         linkage = PatchLinkage.from_setup(config, random)
     kwargs = dict(linkage=linkage, progress=progress)
     logger.debug("scheduling DD, DR" + (", RR" if compute_rr else ""))
-    with TimedLog(logger.info, f"counting data-data pairs"):
+    with TimedLog(logger.info, "counting data-data pairs"):
         DD = data.correlate(config, binned=True, **kwargs)
-    with TimedLog(logger.info, f"counting data-rand pairs"):
+    with TimedLog(logger.info, "counting data-rand pairs"):
         DR = data.correlate(config, binned=True, other=random, **kwargs)
     if compute_rr:
-        with TimedLog(logger.info, f"counting rand-rand pairs"):
+        with TimedLog(logger.info, "counting rand-rand pairs"):
             RR = random.correlate(config, binned=True, **kwargs)
     else:
         RR = _create_dummy_counts(DD)
 
     if isinstance(DD, dict):
         result = {
-            scale: CorrFunc(dd=DD[scale], dr=DR[scale], rr=RR[scale])
-            for scale in DD}
+            scale: CorrFunc(dd=DD[scale], dr=DR[scale], rr=RR[scale]) for scale in DD
+        }
     else:
         result = CorrFunc(dd=DD, dr=DR, rr=RR)
     return result
 
 
 def crosscorrelate(
     config: Configuration,
     reference: BaseCatalog,
     unknown: BaseCatalog,
     *,
     ref_rand: BaseCatalog | None = None,
     unk_rand: BaseCatalog | None = None,
     linkage: PatchLinkage | None = None,
-    progress: bool = False
+    progress: bool = False,
 ) -> CorrFunc | dict[str, CorrFunc]:
     """Compute an angular crosscorrelation function in bins of redshift.
 
     The correlation is measured on fixed physical scales that are converted to
     angles for each redshift bin. All parameters (binning, scales, etc.) are
     bundled in the input configuration, see :mod:`yaw.config`.
 
@@ -1033,44 +1023,44 @@
     if compute_rd:
         all_cats.append(ref_rand)
     _check_patch_centers(all_cats)
 
     scales = config.scales.as_array()
     logger.info(
         f"running crosscorrelation ({len(scales)} scales, "
-        f"{scales.min():.0f}<r<={scales.max():.0f}kpc)")
+        f"{scales.min():.0f}<r<={scales.max():.0f}kpc)"
+    )
     if linkage is None:
         linkage = PatchLinkage.from_setup(config, unknown)
     logger.debug(
-        "scheduling DD" + (", DR" if compute_dr else "") +
-        (", RD" if compute_rd else "") + (", RR" if compute_rr else ""))
+        "scheduling DD"
+        + (", DR" if compute_dr else "")
+        + (", RD" if compute_rd else "")
+        + (", RR" if compute_rr else "")
+    )
     kwargs = dict(linkage=linkage, progress=progress)
-    with TimedLog(logger.info, f"counting data-data pairs"):
-        DD = reference.correlate(
-            config, binned=False, other=unknown, **kwargs)
+    with TimedLog(logger.info, "counting data-data pairs"):
+        DD = reference.correlate(config, binned=False, other=unknown, **kwargs)
     if compute_dr:
-        with TimedLog(logger.info, f"counting data-rand pairs"):
-            DR = reference.correlate(
-                config, binned=False, other=unk_rand, **kwargs)
+        with TimedLog(logger.info, "counting data-rand pairs"):
+            DR = reference.correlate(config, binned=False, other=unk_rand, **kwargs)
     else:
         DR = _create_dummy_counts(DD)
     if compute_rd:
-        with TimedLog(logger.info, f"counting rand-data pairs"):
-            RD = ref_rand.correlate(
-                config, binned=False, other=unknown, **kwargs)
+        with TimedLog(logger.info, "counting rand-data pairs"):
+            RD = ref_rand.correlate(config, binned=False, other=unknown, **kwargs)
     else:
         RD = _create_dummy_counts(DD)
     if compute_rr:
-        with TimedLog(logger.info, f"counting rand-rand pairs"):
-            RR = ref_rand.correlate(
-                config, binned=False, other=unk_rand, **kwargs)
+        with TimedLog(logger.info, "counting rand-rand pairs"):
+            RR = ref_rand.correlate(config, binned=False, other=unk_rand, **kwargs)
     else:
         RR = _create_dummy_counts(DD)
 
     if isinstance(DD, dict):
         result = {
-            scale: CorrFunc(
-                dd=DD[scale], dr=DR[scale], rd=RD[scale], rr=RR[scale])
-            for scale in DD}
+            scale: CorrFunc(dd=DD[scale], dr=DR[scale], rd=RD[scale], rr=RR[scale])
+            for scale in DD
+        }
     else:
         result = CorrFunc(dd=DD, dr=DR, rd=RD, rr=RR)
     return result
```

### Comparing `yet_another_wizz-2.5/src/yaw/correlation/estimators.py` & `yet_another_wizz-2.5.post0/src/yaw/correlation/estimators.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,35 +27,44 @@
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import NDArray
 
+__all__ = [
+    "CorrelationEstimator",
+    "PeeblesHauser",
+    "DavisPeebles",
+    "Hamilton",
+    "LandySzalay",
+]
+
 
 logger = logging.getLogger(__name__)
 
 
 class EstimatorError(Exception):
     pass
 
 
 class Cts(ABC):
     """Base class to symbolically represent pair counts."""
 
     @abstractproperty
-    def _hash(self) -> int: 
+    def _hash(self) -> int:
         """Used for comparison.
-        
+
         Equivalent pair counts types should have the same hash value, see
         :obj:`CtsMix`."""
         pass
 
     @abstractproperty
-    def _str(self) -> str: pass
+    def _str(self) -> str:
+        pass
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__}>"
 
     def __str__(self) -> str:
         return self._str
 
@@ -68,64 +77,68 @@
         var1 = set(self._str.split("_"))
         var2 = set(other._str.split("_"))
         return not var1.isdisjoint(var2)
 
 
 class CtsDD(Cts):
     """Symbolic representation of data-data paircounts."""
+
     _str = "dd"
     _hash = 1
 
 
 class CtsDR(Cts):
     """Symbolic representation of data-random paircounts."""
+
     _str = "dr"
     _hash = 2
 
 
 class CtsRD(Cts):
     """Symbolic representation of random-data paircounts."""
+
     _str = "rd"
     _hash = 2
 
 
 class CtsMix(Cts):
     """Symbolic representation of either data-random or random-data paircounts.
-    
+
     >>> CtsDR() == CtsMix()
     True
     >>> CtsRD() == CtsMix()
     True
     """
+
     _str = "dr_rd"
     _hash = 2
 
 
 class CtsRR(Cts):
     """Symbolic representation of random-random paircounts."""
+
     _str = "rr"
     _hash = 3
 
 
 def cts_from_code(code: str) -> Cts:
     """Instantiate the correct :obj:`Cts` subclass from a string.
-    
+
     Valid options are ``dd``, ``dr``, ``rd``, ``rr``, e.g.:
 
     >>> cts_from_code("dr")
-    <CtsDR>    
+    <CtsDR>
     """
     codes = dict(dd=CtsDD, dr=CtsDR, rd=CtsRD, rr=CtsRR)
     if code not in codes:
         raise ValueError(f"unknown pair counts '{code}'")
     return codes[code]()
 
 
 class CorrelationEstimator(ABC):
-
     name: str
     """Full name of the estimator."""
     short: str
     """Get a short form representation of the estimator name."""
     requires: list[Cts]
     """Get a symbolic list of pair counts required to evaluate the estimator.
     """
@@ -142,50 +155,39 @@
         super().__init_subclass__(**kwargs)
         cls.variants.append(cls)
 
     @classmethod
     def _warn_enum_zero(cls, counts: NDArray):
         """Raise a warning if any value in the expression enumerator is zero"""
         if np.any(counts == 0.0):
-            logger.warn(
-                f"estimator {cls.short} encontered zeros in enumerator")
+            logger.warn(f"estimator {cls.short} encontered zeros in enumerator")
 
     @abstractclassmethod
     def eval(
-        cls,
-        *,
-        dd: NDArray,
-        dr: NDArray,
-        rr: NDArray,
-        rd: NDArray | None = None
+        cls, *, dd: NDArray, dr: NDArray, rr: NDArray, rd: NDArray | None = None
     ) -> NDArray:
         """Method that implements the estimator.
-        
+
         Should call :meth:`_warn_enum_zero` to raise warnings on zero-division.
         """
         NotImplemented
 
 
 class PeeblesHauser(CorrelationEstimator):
     """Implementation of the Peebles-Hauser correlation estimator
     :math:`\\frac{DD}{RR} - 1`.
     """
+
     name = "PeeblesHauser"
     short = "PH"
     requires = [CtsDD(), CtsRR()]
     optional = []
 
     @classmethod
-    def eval(
-        cls,
-        *,
-        dd: NDArray,
-        rr: NDArray,
-        **kwargs
-    ) -> NDArray:
+    def eval(cls, *, dd: NDArray, rr: NDArray, **kwargs) -> NDArray:
         """Evaluate the estimator with the given pair counts.
 
         Args:
             dd (:obj:`NDArray`):
                 Data-data pair counts (normalised).
             rr (:obj:`NDArray`):
                 Random-random pair counts (normalised).
@@ -200,27 +202,22 @@
 class DavisPeebles(CorrelationEstimator):
     """Implementation of the Davis-Peebles correlation estimator
     :math:`\\frac{DD}{DR} - 1`.
 
     .. Note::
         Accepts both :math:`DR` and :math:`RD` for the denominator.
     """
+
     name = "DavisPeebles"
     short = "DP"
     requires = [CtsDD(), CtsMix()]
     optional = []
 
     @classmethod
-    def eval(
-        cls,
-        *,
-        dd: NDArray,
-        dr_rd: NDArray,
-        **kwargs
-    ) -> NDArray:
+    def eval(cls, *, dd: NDArray, dr_rd: NDArray, **kwargs) -> NDArray:
         """Evaluate the estimator with the given pair counts.
 
         Args:
             dd (:obj:`NDArray`):
                 Data-data pair counts (normalised).
             dr_rd (:obj:`NDArray`):
                 Either data-random or random-data pair counts (normalised).
@@ -232,27 +229,23 @@
         return dd / dr_rd - 1.0
 
 
 class Hamilton(CorrelationEstimator):
     """Implementation of the Hamilton correlation estimator
     :math:`\\frac{DD \\times RR}{DR \\times RD} - 1`.
     """
+
     name = "Hamilton"
     short = "HM"
     requires = [CtsDD(), CtsDR(), CtsRR()]
     optional = [CtsRD()]
 
     @classmethod
     def eval(
-        cls,
-        *,
-        dd: NDArray,
-        dr: NDArray,
-        rr: NDArray,
-        rd: NDArray | None = None
+        cls, *, dd: NDArray, dr: NDArray, rr: NDArray, rd: NDArray | None = None
     ) -> NDArray:
         """Evaluate the estimator with the given pair counts.
 
         Args:
             dd (:obj:`NDArray`):
                 Data-data pair counts (normalised).
             dr (:obj:`NDArray`):
@@ -272,27 +265,23 @@
         return (dd * rr) / enum - 1.0
 
 
 class LandySzalay(CorrelationEstimator):
     """Implementation of the Landy-Szalay correlation estimator
     :math:`\\frac{DD - (DR + RD)}{RR} + 1`.
     """
+
     name = "LandySzalay"
     short = "LS"
     requires = [CtsDD(), CtsDR(), CtsRR()]
     optional = [CtsRD()]
 
     @classmethod
     def eval(
-        cls,
-        *,
-        dd: NDArray,
-        dr: NDArray,
-        rr: NDArray,
-        rd: NDArray | None = None
+        cls, *, dd: NDArray, dr: NDArray, rr: NDArray, rd: NDArray | None = None
     ) -> NDArray:
         """Evaluate the estimator with the given pair counts.
 
         Args:
             dd (:obj:`NDArray`):
                 Data-data pair counts (normalised).
             dr (:obj:`NDArray`):
```

### Comparing `yet_another_wizz-2.5/src/yaw/correlation/paircounts.py` & `yet_another_wizz-2.5.post0/src/yaw/correlation/paircounts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,116 +1,119 @@
 """This module implements containers for storing pair counts
 (:obj:`PatchedCount`) and the total number of objects (:obj:`PatchedTotal`) for
 pair count normalisation. The data is stored per spatial patch and in bins of
 redshift. The containers implement methods to compute total value (summing over
 all patches) and samples needed for error estimations after evaluating the
 correlation estimator (e.g. jackknife or bootstrap resampling).
 
-Finally, :obj:`NormalisedCounts` implements normalised pair counts and holds both
-a :obj:`PatchedCount` and :obj:`PatchedTotal` container. Its
+Finally, :obj:`NormalisedCounts` implements normalised pair counts and holds
+both a :obj:`PatchedCount` and :obj:`PatchedTotal` container. Its
 :meth:`NormalisedCounts.sample` method computes the ratio of
 counts-to-total-objects and samples thereof.
 """
 
 from __future__ import annotations
 
 import logging
 from abc import abstractmethod
 from collections.abc import Iterable, Sequence
 from dataclasses import dataclass
 from itertools import accumulate
 from typing import TYPE_CHECKING, NoReturn, Union
+
 try:  # pragma: no cover
     from typing import TypeAlias
 except ImportError:  # pragma: no cover
     from typing_extensions import TypeAlias
 
 import h5py
 import numpy as np
 import pandas as pd
 from deprecated import deprecated
 
 from yaw.config import ResamplingConfig
 from yaw.core.abc import (
-    BinnedQuantity, HDFSerializable, PatchedQuantity, concatenate_bin_edges)
+    BinnedQuantity,
+    HDFSerializable,
+    PatchedQuantity,
+    concatenate_bin_edges,
+)
 from yaw.core.containers import Indexer, PatchIDs, SampledData
 from yaw.core.logging import LogCustomWarning
 from yaw.core.math import apply_slice_ndim, outer_triu_sum
 
 if TYPE_CHECKING:  # pragma: no cover
-    from numpy.typing import NDArray, DTypeLike
+    from numpy.typing import DTypeLike, NDArray
     from pandas import IntervalIndex
 
+__all__ = ["PatchedTotal", "PatchedCount", "NormalisedCounts"]
 
-logger = logging.getLogger(__name__)
 
+logger = logging.getLogger(__name__)
 
 _compression = dict(fletcher32=True, compression="gzip", shuffle=True)
 """default compression settings for :obj:`h5py.Dataset`."""
 
 
 TypeSlice: TypeAlias = Union[slice, int, None]
 TypeIndex: TypeAlias = Union[int, slice, Sequence]
 
 
-def check_mergable(
-    patched_arrays: Sequence[PatchedArray],
-    *,
-    patches: bool
-) -> None:
+def check_mergable(patched_arrays: Sequence[PatchedArray], *, patches: bool) -> None:
     """Check if two instaces of PatchedArray can be merged along the patch
     or binning axis.
-    
+
     Args:
         patched_arrays (:obj:`Sequence[PatchedArray]`):
             Instances to merge
-    
+
     Keyword args:
         patches (:obj:`bool`):
             Whether to check for merging patches or binning.
     """
     reference = patched_arrays[0]
     for patched in patched_arrays[1:]:
         if reference.auto != patched.auto:
             raise ValueError("cannot merge mixed cross- and autocorrelations")
         if patches:
             reference.is_compatible(patched, require=True)
         else:
             if reference.auto != patched.auto:
-                raise ValueError(
-                    "cannot merge mixed cross- and autocorrelations")
+                raise ValueError("cannot merge mixed cross- and autocorrelations")
             if reference.n_patches != patched.n_patches:
                 raise ValueError("cannot merge, patch numbers do not match")
 
 
 def binning_from_hdf(source: h5py.Group) -> IntervalIndex:
     """Construct a :obj:`pandas.IntervalIndex` from a group in an HDF5 file."""
     dset = source["binning"]
     left, right = dset[:].T
     closed = dset.attrs["closed"]
     return pd.IntervalIndex.from_arrays(left, right, closed=closed)
 
 
 def binning_to_hdf(binning: IntervalIndex, dest: h5py.Group) -> None:
     """Serialise a :obj:`pandas.IntervalIndex` into a group of an HDF5 file.
-    
+
     Stores the left and right edges for each interval, as well as on which side
     the intervals are closed as group attribute.
     """
     edges = np.column_stack([binning.left, binning.right])
     dset = dest.create_dataset("binning", data=edges, **_compression)
     dset.attrs["closed"] = binning.closed
 
 
 def patch_idx_offset(patched: Iterable[PatchedArray]) -> NDArray[np.int_]:
     """Compute the offsets for patch indices of a set of :obj:`PatchedArray` if
     they were merged into one large :obj:`PatchedArray`."""
     idx_offset = np.fromiter(
         accumulate((p.n_patches for p in patched), initial=0),
-        dtype=np.int_, count=len(patched))
+        dtype=np.int_,
+        count=len(patched),
+    )
     return idx_offset
 
 
 class PatchedArray(BinnedQuantity, PatchedQuantity, HDFSerializable):
     """Base class that implements the interface for classes that store results
     from pair count measurements.
     """
@@ -156,45 +159,35 @@
     def size(self) -> int:
         """The number of items in the underlying data if viewed as array."""
         return np.prod(self.shape)
 
     @abstractmethod
     def as_array(self) -> NDArray:
         """Get the underlying data as contiguous array.
-        
+
         The array 3-dimensional with shape (N, N, K), where N is the number of
         spatial patches, and K is the number of redshift bins."""
         raise NotImplementedError
 
     @abstractmethod
-    def _sum(
-        self,
-        config: ResamplingConfig
-    ) -> NDArray:
+    def _sum(self, config: ResamplingConfig) -> NDArray:
         """Method that implements the sum over all patches."""
         raise NotImplementedError
 
     @abstractmethod
-    def _jackknife(
-        self,
-        config: ResamplingConfig,
-        signal: NDArray
-    ) -> NDArray:
+    def _jackknife(self, config: ResamplingConfig, signal: NDArray) -> NDArray:
         """Method that implements generating jackknife samples of the sum over
         all patches.
 
-        For N patches, draw N realisations by leaving out one of the N patches. 
+        For N patches, draw N realisations by leaving out one of the N patches.
         """
         raise NotImplementedError
 
     @abstractmethod
-    def _bootstrap(
-        self,
-        config: ResamplingConfig
-    ) -> NDArray:
+    def _bootstrap(self, config: ResamplingConfig) -> NDArray:
         """Method that implements generating bootstrap samples of the sum over
         all patches.
 
         For N patches, draw M realisations each containing N randomly chosen
         patches.
         """
         raise NotImplementedError
@@ -229,18 +222,16 @@
             if config.method == "bootstrap":
                 samples = self._bootstrap(config)
             else:
                 samples = self._jackknife(config, signal=data)
         else:
             samples = np.atleast_2d(data)
         return SampledData(
-            binning=self.get_binning(),
-            data=data,
-            samples=samples,
-            method=config.method)
+            binning=self.get_binning(), data=data, samples=samples, method=config.method
+        )
 
 
 class PatchedTotal(PatchedArray):
     """Container class for the product of the total number of objects of two
     samples.
 
     The data in this container, the product of the total number of objects from
@@ -263,15 +254,15 @@
     Select a subset of all redshift bins or all spatial patches:
 
     >>> from yaw.examples import patched_total
     >>> patched_total
     PatchedTotal(n_bins=30, z='0.070...1.420', shape=(64, 64, 30))
 
     Note how the indicated shape changes when a patch subset is selected:
-    
+
     >>> patched_total.patches[:10]
     PatchedTotal(n_bins=30, z='0.070...1.420', shape=(10, 10, 30))
 
     Note how the indicated redshift range and shape change when a bin subset is
     selected:
 
     >>> patched_total.bins[:3]
@@ -285,33 +276,28 @@
     ...     break  # just show the first item
     PatchedTotal(n_bins=1, z='0.070...0.115', shape=(64, 64, 1))
     """
 
     totals1: NDArray
     """The total number of objects from the first data catalogue per patch and
     redshift bin.
-    
+
     The array is of shape (N, K), where N is the number of spatial patches, and
     K is the number of redshift bins.
     """
     totals2: NDArray
     """The total number of objects from the second data catalogue per patch and
     redshift bin.
-    
+
     The array is of shape (N, K), where N is the number of spatial patches, and
     K is the number of redshift bins.
     """
 
     def __init__(
-        self,
-        binning: IntervalIndex,
-        totals1: NDArray,
-        totals2: NDArray,
-        *,
-        auto: bool
+        self, binning: IntervalIndex, totals1: NDArray, totals2: NDArray, *, auto: bool
     ) -> None:
         """Construct a new instance from the total number of objects in the
         first and second catalog.
 
         Args:
             binning (:obj:`pandas.IntervalIndex`):
                 The redshift binning applied to the data.
@@ -324,61 +310,70 @@
                 The total number of objects from the second data catalogue per
                 patch and redshift bin. The array must be of shape (N, K), where
                 N is the number of spatial patches, and K is the number of
                 redshift bins.
 
         Keyword Args:
             auto (:obj:`bool`):
-                Whether the data originates from an autocorrelation measurement.                
+                Whether the data originates from an autocorrelation measurement.
         """
         self._binning = binning
         for i, totals in enumerate((totals1, totals2), 1):
             if totals.ndim != 2:
                 raise ValueError(f"'totals{i}' must be two dimensional")
             if totals.shape[1] != self.n_bins:
                 raise ValueError(
-                    f"number of bins for 'totals{i}' does not match 'binning'")
+                    f"number of bins for 'totals{i}' does not match 'binning'"
+                )
         if totals1.shape != totals2.shape:
             raise ValueError(
                 f"number of patches and bins do not match: "
-                f"{totals1.shape} != {totals2.shape}")
+                f"{totals1.shape} != {totals2.shape}"
+            )
         self.totals1 = totals1
         self.totals2 = totals2
         self.auto = auto
 
     def __eq__(self, other) -> bool:
         if not super().__eq__(other):
             return False  # checks type
         return (
-            np.all(self.totals1 == other.totals1) and
-            np.all(self.totals2 == other.totals2) and
-            self.auto == other.auto)
+            np.all(self.totals1 == other.totals1)
+            and np.all(self.totals2 == other.totals2)
+            and self.auto == other.auto
+        )
 
     def as_array(self) -> NDArray:
         return np.einsum("i...,j...->ij...", self.totals1, self.totals2)
 
     @property
     def bins(self) -> Indexer[TypeIndex, PatchedTotal]:
         def builder(inst: PatchedTotal, item: TypeIndex) -> PatchedTotal:
             if isinstance(item, int):
                 item = [item]
             return PatchedTotal(
-                binning=inst._binning[item], totals1=inst.totals1[:, item],
-                totals2=inst.totals2[:, item], auto=inst.auto)
+                binning=inst._binning[item],
+                totals1=inst.totals1[:, item],
+                totals2=inst.totals2[:, item],
+                auto=inst.auto,
+            )
 
         return Indexer(self, builder)
 
     @property
     def patches(self) -> Indexer[TypeIndex, PatchedTotal]:
         def builder(inst: PatchedTotal, item: TypeIndex) -> PatchedTotal:
             if isinstance(item, int):
                 item = [item]
             return PatchedTotal(
-                binning=inst._binning, totals1=inst.totals1[item],
-                totals2=inst.totals2[item], auto=inst.auto)
+                binning=inst._binning,
+                totals1=inst.totals1[item],
+                totals2=inst.totals2[item],
+                auto=inst.auto,
+            )
 
         return Indexer(self, builder)
 
     def get_binning(self) -> IntervalIndex:
         return self._binning
 
     @property
@@ -389,19 +384,15 @@
     def from_hdf(cls, source: h5py.Group) -> PatchedTotal:
         # reconstruct the binning
         binning = binning_from_hdf(source)
         # load the data
         totals1 = source["totals1"][:]
         totals2 = source["totals2"][:]
         auto = source["auto"][()]
-        return cls(
-            binning=binning,
-            totals1=totals1,
-            totals2=totals2,
-            auto=auto)
+        return cls(binning=binning, totals1=totals1, totals2=totals2, auto=auto)
 
     def to_hdf(self, dest: h5py.Group) -> None:
         # store the binning
         binning_to_hdf(self.get_binning(), dest)
         # store the data
         dest.create_dataset("totals1", data=self.totals1, **_compression)
         dest.create_dataset("totals2", data=self.totals2, **_compression)
@@ -410,39 +401,41 @@
     def concatenate_patches(self, *data: PatchedTotal) -> PatchedTotal:
         all_totals: list[PatchedTotal] = [self, *data]
         check_mergable(all_totals, patches=True)
         return self.__class__(
             binning=self.get_binning().copy(),
             totals1=np.concatenate([t.totals1 for t in all_totals], axis=0),
             totals2=np.concatenate([t.totals2 for t in all_totals], axis=0),
-            auto=self.auto)
+            auto=self.auto,
+        )
 
     def concatenate_bins(self, *data: PatchedTotal) -> PatchedTotal:
         all_totals: list[PatchedTotal] = [self, *data]
         check_mergable(all_totals, patches=False)
         binning = concatenate_bin_edges(*all_totals)
         return self.__class__(
             binning=binning,
             totals1=np.concatenate([t.totals1 for t in all_totals], axis=1),
             totals2=np.concatenate([t.totals2 for t in all_totals], axis=1),
-            auto=self.auto)
+            auto=self.auto,
+        )
 
     # methods implementing the signal
 
     def _sum_cross(self) -> NDArray:
         """Implements the sum over all patches for crosscorrelation data.
-        
+
         Effectively computes the sum of the outer product of :obj:`totals1` and
         :obj:`totals2` along the redshift bin axis.
         """
         return np.einsum("i...,j...->...", self.totals1, self.totals2)
 
     def _sum_auto(self) -> NDArray:
         """Implements the sum over all patches for autocorrelation data.
-        
+
         The same as :meth:`_sum_cross`, but only computes the upper triangle of
         the outer product and weights the diagonal with 1/2 to account for the
         fact that the diagonal elements are true autocorrelations.
         """
         sum_upper = outer_triu_sum(self.totals1, self.totals2, k=1)
         sum_diag = np.einsum("i...,i...->...", self.totals1, self.totals2)
         return sum_upper + 0.5 * sum_diag
@@ -454,50 +447,50 @@
             return self._sum_cross()
 
     # methods implementing jackknife samples
 
     def _jackknife_cross(self, signal: NDArray) -> NDArray:
         """Implements jackknife samples of the sum over all patches for
         crosscorrelation data.
-        
+
         The same as :meth:`_sum_cross`, but adds an additional dimension as
         first axis which lists the samples. For the i-th sample, subtract all
         data containing :obj:`totals1` or :obj:`totals2` from the i-th patch.
         """
         diag = np.einsum("i...,i...->i...", self.totals1, self.totals2)
         rows = np.einsum("i...,j...->i...", self.totals1, self.totals2)
         cols = np.einsum("i...,j...->j...", self.totals1, self.totals2)
         return signal - rows - cols + diag  # subtracted diag twice
 
     def _jackknife_auto(self, signal: NDArray) -> NDArray:
         """Implements jackknife samples of the sum over all patches for
         autocorrelation data.
-        
+
         The same as :meth:`_jackknife_cross`, but only computes the upper
         triangle of the outer product for each sample and weights the diagonal
         with 1/2 to account for the fact that the diagonal elements are true
         autocorrelations.
         """
         diag = np.einsum("i...,i...->i...", self.totals1, self.totals2)
         # sum along axes of upper triangle (without diagonal) of outer product
         rows = outer_triu_sum(self.totals1, self.totals2, k=1, axis=1)
         cols = outer_triu_sum(self.totals1, self.totals2, k=1, axis=0)
-        return signal - rows - cols - 0.5*diag  # diag not in rows or cols
+        return signal - rows - cols - 0.5 * diag  # diag not in rows or cols
 
     def _jackknife(self, config: ResamplingConfig, signal: NDArray) -> NDArray:
         if self.auto:
             return self._jackknife_auto(signal)
         else:
             return self._jackknife_cross(signal)
 
     # methods implementing bootstrap samples
 
     def _bootstrap(self, config: ResamplingConfig, **kwargs) -> NoReturn:
         """Bootstrap resampling currently not implemented.
-        
+
         Raises:
             :exc:`NotImplementedError`
         """
         raise NotImplementedError
 
 
 class PatchedCount(PatchedArray):
@@ -560,15 +553,15 @@
     Select a subset of all redshift bins or all spatial patches:
 
     >>> from yaw.examples import patched_count
     >>> patched_count
     PatchedCount(n_bins=30, z='0.070...1.420', shape=(64, 64, 30))
 
     Note how the indicated shape changes when a patch subset is selected:
-    
+
     >>> patched_count.patches[:10]
     PatchedCount(n_bins=30, z='0.070...1.420', shape=(10, 10, 30))
 
     Note how the indicated redshift range and shape change when a bin subset is
     selected:
 
     >>> patched_count.bins[:3]
@@ -582,15 +575,15 @@
     ...     break  # just show the first item
     PatchedCount(n_bins=1, z='0.070...0.115', shape=(64, 64, 1))
     """
 
     counts: NDArray
     """Internal data array containing the pair counts between spatial patches in
     bins of redshift.
-    
+
     The array is 3-dimensional with shape (N, N, K), where N is the number of
     spatial patches, and K is the number of redshift bins. Same as
     :meth:`as_array`.
     """
 
     def __init__(
         self,
@@ -608,46 +601,44 @@
                 Internal data array containing the pair counts between spatial
                 patches in bins of redshift. The array must be 3-dimensional
                 with shape (N, N, K), where N is the number of spatial patches,
                 and K is the number of redshift bins. Same as :meth:`as_array`.
 
         Keyword Args:
             auto (:obj:`bool`):
-                Whether the data originates from an autocorrelation measurement.                
+                Whether the data originates from an autocorrelation measurement.
         """
         if counts.ndim != 3 or counts.shape[0] != counts.shape[1]:
-            raise IndexError(
-                "counts must be of shape (n_patches, n_patches, n_bins)")
+            raise IndexError("counts must be of shape (n_patches, n_patches, n_bins)")
         if counts.shape[2] != len(binning):
-            raise ValueError(
-                "length of 'binning' and 'counts' dimension do not match")
+            raise ValueError("length of 'binning' and 'counts' dimension do not match")
         self._binning = binning
         self.counts = counts
         self.auto = auto
 
     @classmethod
     def zeros(
         cls,
         binning: IntervalIndex,
         n_patches: int,
         *,
         auto: bool,
-        dtype: DTypeLike = np.float_
+        dtype: DTypeLike = np.float_,
     ) -> PatchedCount:
         """Create a new instance where all elements of the counts array are
         initialised to zero.
-        
+
         Args:
             binning (:obj:`pandas.IntervalIndex`):
                 Redshift binning for the container, determines size of last data
                 array dimension.
             n_patches (:obj:`int`):
                 Number of spatial patches, determines the size of the first two
                 data array dimensions.
-        
+
         Keyword Args:
             auto (:obj:`bool`):
                 Whether the data originates from an autocorrelation measurement.
             dtype (:obj:`DTypeLike`, optional):
                 Data type to use for the internal data array.
 
         """
@@ -660,25 +651,25 @@
         return np.all(self.counts == other.counts) and (self.auto == other.auto)
 
     def __add__(self, other: PatchedCount) -> PatchedCount:
         self.is_compatible(other, require=True)
         if self.n_patches != other.n_patches:
             raise ValueError("number of patches does not agree")
         return self.__class__(
-            self.get_binning(), self.counts + other.counts, auto=self.auto)
+            self.get_binning(), self.counts + other.counts, auto=self.auto
+        )
 
     def __radd__(self, other: PatchedCount | int | float) -> PatchedCount:
         if other == 0:
             return self
         else:
             return self.__add__(other)
 
     def __mul__(self, other: np.number) -> PatchedCount:
-        return self.__class__(
-            self.get_binning(), self.counts * other, auto=self.auto)
+        return self.__class__(self.get_binning(), self.counts * other, auto=self.auto)
 
     def set_measurement(self, key: PatchIDs | tuple[int, int], item: NDArray):
         """Set the counts value in all redshift bins for a pair of patch
         indices.
 
         Args:
             key (:obj:`yaw.core.containers.PatchIDs`, tuple):
@@ -689,29 +680,29 @@
         """
         # check the key
         if not isinstance(key, tuple):
             raise TypeError(f"slice must be of type {tuple}")
         elif len(key) != 2:
             raise IndexError(
                 f"too many indices for array assignment: index must be "
-                f"2-dimensional, but {len(key)} where indexed")
+                f"2-dimensional, but {len(key)} where indexed"
+            )
         # check the item
         item = np.asarray(item)
         if item.shape != (self.n_bins,):
-            raise ValueError(
-                f"can only set items with length n_bins={self.n_bins}")
+            raise ValueError(f"can only set items with length n_bins={self.n_bins}")
         # insert values
         self.counts[key] = item
 
     def as_array(self) -> NDArray:
         return self.counts
 
     def sum(self, axis: int | tuple[int] | None = None, **kwargs) -> NDArray:
         """Shorthand for :meth:`PatchedCount.counts.sum`
-        
+
         Args:
             axis (:obj:`tuple`, :obj:`int`, optional):
                 Axis over which the internal 3-dimensional data array is summed.
             **kwargs:
                 Keyword arguments passed to :meth:`numpy.ndarry.sum`.
         """
         return self.counts.sum(axis=axis, **kwargs)
@@ -720,25 +711,27 @@
     def bins(self) -> Indexer[TypeIndex, PatchedCount]:
         def builder(inst: PatchedCount, item: TypeIndex) -> PatchedCount:
             if isinstance(item, int):
                 item = [item]
             return PatchedCount(
                 binning=inst._binning[item],
                 counts=apply_slice_ndim(inst.counts, item, axis=2),
-                auto=inst.auto)
+                auto=inst.auto,
+            )
 
         return Indexer(self, builder)
 
     @property
     def patches(self) -> Indexer[TypeIndex, PatchedCount]:
         def builder(inst: PatchedCount, item: TypeIndex) -> PatchedCount:
             return PatchedCount(
                 binning=inst._binning,
                 counts=apply_slice_ndim(inst.counts, item, axis=(0, 1)),
-                auto=inst.auto)
+                auto=inst.auto,
+            )
 
         return Indexer(self, builder)
 
     def get_binning(self) -> IntervalIndex:
         return self._binning
 
     @property
@@ -747,26 +740,26 @@
 
     @property
     def n_bins(self) -> int:
         return len(self.get_binning())
 
     def keys(self) -> NDArray:
         """Array of patch index pairs with non-zero pair counts.
-        
+
         The index pairs are ordered by first, then second index. The returned
         array is of shape (N, 2), where N is the number patches that contain
         non-zero entries in any of the redshift bins.
         """
         has_data = np.any(self.counts, axis=2)
         indices = np.nonzero(has_data)
         return np.column_stack(indices)
 
     def values(self) -> NDArray:
         """Array of non-zero pair count values.
-        
+
         The values are ordered in the same way as the indices returned by
         :meth:`keys`.
         """
         keys = self.keys()  # shape (n_nonzero, 2)
         i1, i2 = keys.T
         return self.counts[i1, i2, :]  # shape (n_nonzero, n_bins)
 
@@ -776,22 +769,18 @@
         binning = binning_from_hdf(source)
         # load the sparse data representation
         keys = [tuple(key) for key in source["keys"][:]]
         data = source["data"][:]
         n_patches = source["n_patches"][()]
         auto = source["auto"][()]
         # build dense counts matrix
-        counts = np.zeros(
-            (n_patches, n_patches, len(binning)), dtype=data.dtype)
+        counts = np.zeros((n_patches, n_patches, len(binning)), dtype=data.dtype)
         for key, values in zip(keys, data):
             counts[key] = values
-        return cls(
-            binning=binning,
-            counts=counts,
-            auto=auto)
+        return cls(binning=binning, counts=counts, auto=auto)
 
     def to_hdf(self, dest: h5py.Group) -> None:
         # store the binning
         binning_to_hdf(self.get_binning(), dest)
         # store the data
         dest.create_dataset("keys", data=self.keys(), **_compression)
         dest.create_dataset("data", data=self.values(), **_compression)
@@ -801,41 +790,39 @@
     def concatenate_patches(self, *data: PatchedCount) -> PatchedCount:
         all_counts: list[PatchedCount] = [self, *data]
         check_mergable(all_counts, patches=True)
         offsets = patch_idx_offset(all_counts)
         merged = self.__class__.zeros(
             binning=self.get_binning(),
             n_patches=sum(count.n_patches for count in all_counts),
-            auto=self.auto)
+            auto=self.auto,
+        )
         # insert the blocks of counts into the merged counts array
         loc = 0
         for count, offset in zip(all_counts, offsets):
-            merged.counts[loc:loc+offset, loc:loc+offset] = count.counts
+            merged.counts[loc : loc + offset, loc : loc + offset] = count.counts
             loc += offset
         return merged
 
     def concatenate_bins(self, *data: PatchedCount) -> PatchedCount:
         all_counts: list[PatchedCount] = [self, *data]
         check_mergable(all_counts, patches=False)
         binning = concatenate_bin_edges(*all_counts)
         merged = self.__class__.zeros(
-            binning=binning,
-            n_patches=self.n_patches,
-            auto=self.auto,
-            dtype=self.dtype)
-        merged.counts = np.concatenate(
-            [count.counts for count in all_counts], axis=2)
+            binning=binning, n_patches=self.n_patches, auto=self.auto, dtype=self.dtype
+        )
+        merged.counts = np.concatenate([count.counts for count in all_counts], axis=2)
         return merged
 
     # methods implementing the signal
 
     def _bin_sum_diag(self, data: NDArray) -> np.number:
         """Implements the sum over the autocorrelation patches in a single
         redshift bin.
-        
+
         The autocorrelation patches are stored in the diagonal of the first two
         dimension of the pair count data array.
 
         .. Note::
             This method is valid for both cross- and autocorrelation data.
         """
         return np.diagonal(data).sum()
@@ -867,56 +854,44 @@
                     out[i] = self._bin_sum_cross(data)
             else:
                 out[i] = self._bin_sum_diag(data)
         return out
 
     # methods implementing jackknife samples
 
-    def _bin_jackknife_diag(
-        self,
-        data: NDArray,
-        signal: NDArray
-    ) -> NDArray:
+    def _bin_jackknife_diag(self, data: NDArray, signal: NDArray) -> NDArray:
         """Implements jackknife samples of the sum over the autocorrelation
         patches in a single redshift bin.
 
         The autocorrelation patches are stored in the diagonal of the first two
         dimension of the pair count data array. Samples are computed by leaving
         out the i-th patch in the i-th sample.
 
         .. Note::
             This method is valid for both cross- and autocorrelation data.
         """
         return signal - np.diagonal(data)  # broadcast to (n_patches,)
 
-    def _bin_jackknife_cross(
-        self,
-        data: NDArray,
-        signal: NDArray
-    ) -> NDArray:
+    def _bin_jackknife_cross(self, data: NDArray, signal: NDArray) -> NDArray:
         """Implements jackknife samples of the sum over all patches for
         crosscorrelation data in a single redshift bin.
-        
+
         The same as :meth:`_bin_sum_cross`, but adds an additional dimension as
         first axis which lists the samples. For the i-th sample, subtract all
         data containing counts with objects of the i-th patch.
         """
         diag = np.diagonal(data)
         rows = data.sum(axis=1)
         cols = data.sum(axis=0)
         return signal - rows - cols + diag  # broadcast to (n_patches,)
 
-    def _bin_jackknife_auto(
-        self,
-        data: NDArray,
-        signal: NDArray
-    ) -> NDArray:
+    def _bin_jackknife_auto(self, data: NDArray, signal: NDArray) -> NDArray:
         """Implements jackknife samples of the sum over all patches for
         autocorrelation data in a single redshift bin.
-        
+
         The same as :meth:`_bin_jackknife_cross`, but only sums elements on the
         main diagonal and upper triangle of the pair count array.
         """
         diag = np.diagonal(data)
         # sum along axes of upper triangle (without diagonal) of outer product
         tri_upper = np.triu(data, k=1)
         rows = tri_upper.sum(axis=1).flatten()
@@ -937,15 +912,15 @@
                 out[:, i] = self._bin_jackknife_diag(data, bin_signal)
         return out
 
     # methods implementing bootstrap samples
 
     def _bootstrap(self, config: ResamplingConfig, **kwargs) -> NoReturn:
         """Bootstrap resampling currently not implemented.
-        
+
         Raises:
             :exc:`NotImplementedError`
         """
         raise NotImplementedError
 
 
 @dataclass(frozen=True)
@@ -969,50 +944,43 @@
     count: PatchedCount
     """The pair count container."""
     total: PatchedTotal
     """The container for the total number of objects from the samples."""
 
     def __post_init__(self) -> None:
         if self.count.n_patches != self.total.n_patches:
-            raise ValueError(
-                "number of patches of 'count' and total' do not match")
+            raise ValueError("number of patches of 'count' and total' do not match")
         if self.count.n_bins != self.total.n_bins:
-            raise ValueError(
-                "number of bins of 'count' and total' do not match")
+            raise ValueError("number of bins of 'count' and total' do not match")
 
     def __repr__(self) -> str:
         string = super().__repr__()[:-1]
         n_patches = self.n_patches
         return f"{string}, {n_patches=})"
 
     def __eq__(self, other) -> bool:
         if isinstance(other, self.__class__):
-            return (
-                np.all(self.count == other.count) and
-                np.all(self.total == other.total))
+            return np.all(self.count == other.count) and np.all(
+                self.total == other.total
+            )
         else:
             return False
 
     def __neq__(self, other) -> bool:
         return not self == other
 
     def __add__(self, other: NormalisedCounts) -> NormalisedCounts:
         count = self.count + other.count
-        if (
-            np.any(self.total.totals1 != other.total.totals1) or
-            np.any(self.total.totals2 != other.total.totals2)
+        if np.any(self.total.totals1 != other.total.totals1) or np.any(
+            self.total.totals2 != other.total.totals2
         ):
-            raise ValueError(
-                "total number of objects do not agree for operands")
+            raise ValueError("total number of objects do not agree for operands")
         return self.__class__(count, self.total)
 
-    def __radd__(
-        self,
-        other: NormalisedCounts | int | float
-    ) -> NormalisedCounts:
+    def __radd__(self, other: NormalisedCounts | int | float) -> NormalisedCounts:
         if other == 0:
             return self
         else:
             return self.__add__(other)
 
     def __mul__(self, other: np.number) -> NormalisedCounts:
         return self.__class__(self.count * other, self.total)
@@ -1020,34 +988,29 @@
     @property
     def auto(self) -> bool:
         """Whether the stored data are from an autocorrelation measurement."""
         return self.count.auto
 
     @property
     def bins(self) -> Indexer[TypeIndex, NormalisedCounts]:
-        def builder(
-            inst: NormalisedCounts,
-            item: TypeIndex
-        ) -> NormalisedCounts:
+        def builder(inst: NormalisedCounts, item: TypeIndex) -> NormalisedCounts:
             if isinstance(item, int):
                 item = [item]
             return NormalisedCounts(
-                count=inst.count.bins[item], total=inst.total.bins[item])
+                count=inst.count.bins[item], total=inst.total.bins[item]
+            )
 
         return Indexer(self, builder)
 
     @property
     def patches(self) -> Indexer[TypeIndex, NormalisedCounts]:
-        def builder(
-            inst: NormalisedCounts,
-            item: TypeIndex
-        ) -> NormalisedCounts:
+        def builder(inst: NormalisedCounts, item: TypeIndex) -> NormalisedCounts:
             return NormalisedCounts(
-                count=inst.count.patches[item],
-                total=inst.total.patches[item])
+                count=inst.count.patches[item], total=inst.total.patches[item]
+            )
 
         return Indexer(self, builder)
 
     def get_binning(self) -> IntervalIndex:
         return self.total.get_binning()
 
     @property
@@ -1078,55 +1041,52 @@
         with LogCustomWarning(
             logger, "some patches contain no data after binning by redshift"
         ):
             samples = SampledData(
                 binning=self.get_binning(),
                 data=(counts.data / totals.data),
                 samples=(counts.samples / totals.samples),
-                method=config.method)
+                method=config.method,
+            )
         return samples
 
     @classmethod
     def from_hdf(cls, source: h5py.Group) -> NormalisedCounts:
         count = PatchedCount.from_hdf(source["count"])
         total = PatchedTotal.from_hdf(source["total"])
         return cls(count=count, total=total)
 
     def to_hdf(self, dest: h5py.Group) -> None:
         group = dest.create_group("count")
         self.count.to_hdf(group)
         group = dest.create_group("total")
         self.total.to_hdf(group)
 
-    def concatenate_patches(
-        self, *pcounts: NormalisedCounts
-    ) -> NormalisedCounts:
+    def concatenate_patches(self, *pcounts: NormalisedCounts) -> NormalisedCounts:
         counts = [pc.count for pc in pcounts]
         totals = [pc.total for pc in pcounts]
         return self.__class__(
             count=self.count.concatenate_patches(*counts),
-            total=self.total.concatenate_patches(*totals))
+            total=self.total.concatenate_patches(*totals),
+        )
 
-    def concatenate_bins(
-        self, 
-        *pcounts: NormalisedCounts
-    ) -> NormalisedCounts:
+    def concatenate_bins(self, *pcounts: NormalisedCounts) -> NormalisedCounts:
         counts = [pc.count for pc in pcounts]
         totals = [pc.total for pc in pcounts]
         return self.__class__(
             count=self.count.concatenate_bins(*counts),
-            total=self.total.concatenate_bins(*totals))
+            total=self.total.concatenate_bins(*totals),
+        )
 
 
 def pack_results(
-    count_dict: dict[str, PatchedCount],
-    total: PatchedTotal
+    count_dict: dict[str, PatchedCount], total: PatchedTotal
 ) -> NormalisedCounts | dict[str, NormalisedCounts]:
     """Pack pair counts and the total number of objects.
-     
+
     If measured for multiple scales, the counts should be a dictionary of with
     the scale name as key. In this case, the function returns a dictionary of
     :obj:`NormalisedCounts` with the same keys.
     """
     # drop the dictionary if there is only one scale
     if len(count_dict) == 1:
         count = tuple(count_dict.values())[0]
```

### Comparing `yet_another_wizz-2.5/src/yaw/deprecated.py` & `yet_another_wizz-2.5.post0/src/yaw/deprecated.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,44 +2,52 @@
 
 from deprecated import deprecated
 
 from yaw.correlation import CorrData, CorrFunc
 from yaw.correlation.paircounts import NormalisedCounts
 from yaw.redshifts import HistData
 
+__all__ = ["CorrelationData", "CorrelationFunction", "HistogramData", "PairCountResult"]
+
 
 @deprecated(reason="renamed to yaw.CorrData", action="module", version="2.3.2")
 class CorrelationData(CorrData):
     """
     .. deprecated:: 2.3.2
         Renamed to :meth:`yaw.CorrData`.
     """
+
     pass
 
 
 @deprecated(reason="renamed to yaw.CorrFunc", action="module", version="2.3.2")
 class CorrelationFunction(CorrFunc):
     """
     .. deprecated:: 2.3.2
         Renamed to :meth:`yaw.CorrFunc`.
     """
+
     pass
 
 
 @deprecated(reason="renamed to yaw.HistData", action="module", version="2.3.2")
 class HistogramData(HistData):
     """
     .. deprecated:: 2.3.2
         Renamed to :meth:`yaw.HistData`.
     """
+
     pass
 
 
 @deprecated(
     reason="renamed to yaw.correlation.paircounts.NormalisedCounts",
-    action="module", version="2.3.2")
+    action="module",
+    version="2.3.2",
+)
 class PairCountResult(NormalisedCounts):
     """
     .. deprecated:: 2.3.2
         Renamed to :obj:`yaw.correlation.paircounts.NormalisedCounts`.
     """
+
     pass
```

### Comparing `yet_another_wizz-2.5/src/yaw/examples/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/examples/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,23 @@
 CorrFunc(n_bins=30, z='0.070...1.420', dd=True, dr=True, rd=False, rr=False, n_patches=64)
 """
 
 from pathlib import Path
 
 import yaw
 
+__all__ = [
+    "w_sp",
+    "w_ss",
+    "w_pp",
+    "normalised_counts",
+    "patched_count",
+    "patched_total",
+]
+
 
 _path = Path(__file__).parent
 
 w_sp = yaw.CorrFunc.from_file(_path / "cross_1.hdf")
 """Example data from a crosscorrelation measurement
 (:obj:`~yaw.correlation.CorrFunc` instance)."""
```

### Comparing `yet_another_wizz-2.5/src/yaw/examples/auto_reference.hdf` & `yet_another_wizz-2.5.post0/src/yaw/examples/auto_reference.hdf`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5/src/yaw/examples/auto_unknown_1.hdf` & `yet_another_wizz-2.5.post0/src/yaw/examples/auto_unknown_1.hdf`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5/src/yaw/examples/cross_1.hdf` & `yet_another_wizz-2.5.post0/src/yaw/examples/cross_1.hdf`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5/src/yaw/randoms.py` & `yet_another_wizz-2.5.post0/src/yaw/randoms.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,23 +6,26 @@
 
 import logging
 from typing import TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
 
-from yaw.core.parallel import POOL_SHARE, ParallelHelper, SharedArray
 from yaw.core.logging import TimedLog
+from yaw.core.parallel import POOL_SHARE, ParallelHelper, SharedArray
 from yaw.core.utils import long_num_format
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import NDArray
     from pandas import DataFrame
+
     from yaw.catalogs import BaseCatalog
 
+__all__ = ["UniformRandoms"]
+
 
 logger = logging.getLogger(__name__)
 
 
 class UniformRandoms:
     """Generator for uniform randoms on a rectangular footprint.
 
@@ -39,15 +42,15 @@
 
     def __init__(
         self,
         ra_min: float,
         ra_max: float,
         dec_min: float,
         dec_max: float,
-        seed: int = 12345
+        seed: int = 12345,
     ) -> None:
         """Create a new generator for a the given footprint.
 
         Args:
             ra_min (:obj:`float`):
                 Minimum right ascenion to generate, in degrees.
             ra_max (:obj:`float`):
@@ -60,19 +63,15 @@
                 Seed to use for the random generator.
         """
         self.x_min, self.y_min = self.sky2cylinder(ra_min, dec_min)
         self.x_max, self.y_max = self.sky2cylinder(ra_max, dec_max)
         self.rng = np.random.SeedSequence(seed)
 
     @classmethod
-    def from_catalog(
-        cls,
-        cat: BaseCatalog,
-        seed: int = 12345
-    ) -> UniformRandoms:
+    def from_catalog(cls, cat: BaseCatalog, seed: int = 12345) -> UniformRandoms:
         """Create a new generator with a rectangular footprint obtained from the
         coordinate range of a given data catalogue.
 
         Args:
             cat (:obj:`yaw.catalogs.BaseCatalog`):
                 Catalog instance from which the right ascension and declination
                 range is computed.
@@ -80,65 +79,64 @@
                 Seed to use for the random generator.
         """
         return cls(
             np.rad2deg(cat.ra.min()),
             np.rad2deg(cat.ra.max()),
             np.rad2deg(cat.dec.min()),
             np.rad2deg(cat.dec.max()),
-            seed=seed)
+            seed=seed,
+        )
 
     @staticmethod
     def sky2cylinder(
-        ra: float | NDArray[np.float_],
-        dec: float | NDArray[np.float_]
+        ra: float | NDArray[np.float_], dec: float | NDArray[np.float_]
     ) -> NDArray:
         """Conversion from spherical to cylindrical coordinates.
 
         Args:
             ra (:obj:`float`, :obj:`NDArray`):
                 Right ascension(s) to convert to cylindrical coordinates.
             dec (:obj:`float`, :obj:`NDArray`):
                 Right ascension(s) to convert to cylindrical coordinates.
-        
+
         Returns:
             :obj:`NDArray`:
                 Array with of points in cylindrical coordinates of shape
                 `(N, 2)`.
         """
         x = np.deg2rad(ra)
         y = np.sin(np.deg2rad(dec))
         return np.transpose([x, y])
- 
+
     @staticmethod
     def cylinder2sky(
-        x: float | NDArray[np.float_],
-        y: float | NDArray[np.float_]
+        x: float | NDArray[np.float_], y: float | NDArray[np.float_]
     ) -> float | NDArray[np.float_]:
         """Conversion from cylindrical to spherical coordinates.
 
         Args:
             x (:obj:`float`, :obj:`NDArray`):
                 `x`-coordinate(s) to convert to spherical coordinates.
             y (:obj:`float`, :obj:`NDArray`):
                 `y`-coordinate(s) to convert to spherical coordinates.
-        
+
         Returns:
             :obj:`NDArray`:
                 Array with of points in spherical coordinates of shape `(N, 2)`.
         """
         ra = np.rad2deg(x)
         dec = np.rad2deg(np.arcsin(y))
         return np.transpose([ra, dec])
 
     def generate(
         self,
         size: int,
         names: list[str, str] | None = None,
         draw_from: dict[str, NDArray] | None = None,
-        n_threads: int = 1
+        n_threads: int = 1,
     ) -> DataFrame:
         """Generate new random points.
 
         Generate a specified number of points, additionally draw extra data
         features form a list of input values. Results are returned in a data
         frame.
 
@@ -152,73 +150,74 @@
                 Dictionary of data arrays. If provided, a random sample (with
                 repetition) is drawn from these arrays and assigned to the
                 output data frame. The dictionary keys are used to name the
                 columns in the output.
             n_threads (:obj:`int`, optional):
                 Generate data in parallel using subprocesses, default is
                 parallel processing disabled.
-                
+
                 .. deprecated:: 2.3.2
                     No performance gain observed. May be removed in a future
                     version.
-        
+
         Returns:
             :obj:`pandas.DataFrame`:
                 Data frame with uniform random coordinates and optionally
                 additional features draw from input data.
         """
         # seeds for threads
         if size <= 100 * n_threads:  # there is some kind of floor
             n_threads = 1
         seeds = self.rng.spawn(n_threads)
         # distribute load
-        idx_break = np.linspace(0, size, n_threads+1).astype(np.int_)
+        idx_break = np.linspace(0, size, n_threads + 1).astype(np.int_)
         start = idx_break[:-1]
         end = idx_break[1:]
 
         # create output arrays
         shares = dict(
-            ra=SharedArray.empty((size,), "f8"),
-            dec=SharedArray.empty((size,), "f8"))
+            ra=SharedArray.empty((size,), "f8"), dec=SharedArray.empty((size,), "f8")
+        )
         if draw_from is not None:
             shares["in"] = {
-                key: SharedArray.from_numpy(array)
-                for key, array in draw_from.items()}
+                key: SharedArray.from_numpy(array) for key, array in draw_from.items()
+            }
             shares["out"] = {
                 key: SharedArray.empty((size,), array.dtype)
-                for key, array in draw_from.items()}
+                for key, array in draw_from.items()
+            }
         if names is None:
             names = ["ra", "dec"]
 
         # process
         msg = f"generate ({long_num_format(size)} uniform randoms)"
         with TimedLog(logger.info, msg):
             with ParallelHelper(_generate_uniform_randoms, n_threads) as pool:
                 pool.shares = shares  # assign in bulk
                 pool.add_constant(self)
                 pool.add_iterable(seeds)
                 pool.add_iterable(start)
                 pool.add_iterable(end)
                 pool.result()  # output direclty pasted into shared arrays
                 # convert to dataframe
-                rand = pd.DataFrame({
-                    names[0]: pool.shares["ra"].to_numpy(copy=True),
-                    names[1]: pool.shares["dec"].to_numpy(copy=True)})
+                rand = pd.DataFrame(
+                    {
+                        names[0]: pool.shares["ra"].to_numpy(copy=True),
+                        names[1]: pool.shares["dec"].to_numpy(copy=True),
+                    }
+                )
                 if draw_from is not None:
                     for col, data in pool.shares["out"].items():
                         rand[col] = data.to_numpy(copy=True)
                 # will delete shared arrays after this
         return rand
 
 
 def _generate_uniform_randoms(
-    inst: UniformRandoms,
-    seed: np.random.SeedSequence,
-    start: int,
-    end: int
+    inst: UniformRandoms, seed: np.random.SeedSequence, start: int, end: int
 ) -> int:
     rng = np.random.default_rng(seed)
     size = end - start
     ra = POOL_SHARE["ra"].to_numpy()
     dec = POOL_SHARE["dec"].to_numpy()
     # generate positions
     x = rng.uniform(inst.x_min, inst.x_max, size)
@@ -232,15 +231,14 @@
         for col, data in POOL_SHARE["in"].items():
             if N is None:
                 if len(data.shape) > 1:
                     raise ValueError("data to draw from must be 1-dimensional")
                 N = len(data)
             else:
                 if len(data) != N:
-                    raise ValueError(
-                        "length of columns to draw from does not match")
+                    raise ValueError("length of columns to draw from does not match")
         draw_idx = rng.integers(0, N, size=size)
         # draw and insert data
         for col, data in POOL_SHARE["in"].items():
             rand = POOL_SHARE["out"][col].to_numpy()
             rand[start:end] = data.to_numpy()[draw_idx]
     return size
```

### Comparing `yet_another_wizz-2.5/src/yaw/redshifts.py` & `yet_another_wizz-2.5.post0/src/yaw/redshifts.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,22 +25,25 @@
 import pandas as pd
 import scipy.optimize
 from deprecated import deprecated
 
 from yaw.config import ResamplingConfig
 from yaw.core.containers import SampledValue
 from yaw.core.logging import LogCustomWarning, TimedLog
-from yaw.core.math import shift_histogram, rebin
+from yaw.core.math import rebin, shift_histogram
 from yaw.core.utils import TypePathStr
 from yaw.correlation import CorrData
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import NDArray
+
     from yaw.correlation import CorrFunc
 
+__all__ = ["RedshiftData", "HistData"]
+
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass(frozen=True, repr=False, eq=False)
 class RedshiftData(CorrData):
     """Container class object for redshift estimates.
@@ -48,15 +51,15 @@
     Contains the redshift binning, estimated fraction of galaxies at the given
     redshift (**not** a density), and resampled fractions (e.g. from jackknife
     or bootstrap). The resampled values are used to compute error estimates and
     covariance/correlation matrices. Provides some plotting methods for
     convenience.
 
     This container holds data in the form of
-    :math:`\\frac{w_\\rm{sp}(z)}{\\sqrt{\\Delta z \, w_\\rm{ss}(z) \, w_\\rm{pp}(z)}}`,
+    :math:`\\frac{w_\\rm{sp}(z)}{\\sqrt{\\Delta z \\, w_\\rm{ss}(z) \\, w_\\rm{pp}(z)}}`,
     where :math:`w_\\rm{sp}` is the crosscorrelation function, and
     :math:`w_\\rm{ss}` and :math:`w_\\rm{pp}` are autocorrelation functions that
     account for the evolving galaxy bias. If no autocorrelation is provided, the
     data is still scaled by :math:`1/\\Delta z` compared to the crosscorrelation
     data in :obj:`~yaw.correlation.CorrData`.
 
     .. Note::
@@ -69,15 +72,15 @@
     from :obj:`~yaw.core.containers.SampledData`, check the examples there.
 
     .. rubric:: Examples
 
     Create a redshift estimate from a crosscorrelation function and correct for
     the evolving bias of the reference sample using its autocorrelation
     function:
-    
+
     >>> from yaw.examples import w_sp  # crosscorrelation
     >>> from yaw.examples import w_ss  # reference sample autocorrelation
     >>> nz = yaw.yaw.RedshiftData.from_corrfuncs(w_sp, ref_corr=w_ss)
     RedshiftData(n_bins=30, z='0.070...1.420', n_samples=64, method='jackknife')
 
     Use a different estimator when sampling the autocorrelation function, e.g.
     the Peebles-Hauser estimator:
@@ -125,30 +128,29 @@
             available options.
         info (:obj:`str`, optional):
             Descriptive text included in the headers of output files produced
             by :func:`CorrData.to_files`.
     """
 
     @classmethod
-    @deprecated(
-        reason="renamed to RedshiftData.from_corrdata", version="2.3.2")
+    @deprecated(reason="renamed to RedshiftData.from_corrdata", version="2.3.2")
     def from_correlation_data(cls, *args, **kwargs):
         """
         .. deprecated:: 2.3.2
             Renamed to :meth:`from_corrdata`.
         """
         return cls.from_corrdata(*args, **kwargs)
 
     @classmethod
     def from_corrdata(
         cls,
         cross_data: CorrData,
         ref_data: CorrData | None = None,
         unk_data: CorrData | None = None,
-        info: str | None = None
+        info: str | None = None,
     ) -> RedshiftData:
         """Compute redshift estimate from readily sampled function data.
 
         The required argument is a crosscorrelation measurement, additional
         parameters can specify sample autocorrelation measurements that are used
         to mitigate the evolving galaxy bias.
 
@@ -159,46 +161,45 @@
                 Data from the sampled reference sample autocorrelation function.
                 Used to mitigate reference bias evolution.
             unk_corr (:obj:`CorrData`, optional):
                 Data from the sampled unknown sample autocorrelation function.
                 Used to mitigate unknown bias evolution.
 
         Returns:
-            :obj:`RedshiftData`                
+            :obj:`RedshiftData`
         """
-        logger.debug(
-            "computing clustering redshifts from correlation function samples")
+        logger.debug("computing clustering redshifts from correlation function samples")
         w_sp_data = cross_data.data
         w_sp_samp = cross_data.samples
         mitigate = []
 
         if ref_data is None:
             w_ss_data = np.float64(1.0)
             w_ss_samp = np.float64(1.0)
         else:
             try:
                 ref_data.is_compatible(cross_data, require=True)
             except ValueError as e:
                 raise ValueError(
-                    "'ref_corr' correlation data is not compatible with "
-                    "'cross_data'") from e
+                    "'ref_corr' correlation data is not compatible with 'cross_data'"
+                ) from e
             w_ss_data = ref_data.data
             w_ss_samp = ref_data.samples
             mitigate.append("reference")
 
         if unk_data is None:
             w_pp_data = np.float64(1.0)
             w_pp_samp = np.float64(1.0)
         else:
             try:
                 unk_data.is_compatible(cross_data, require=True)
             except ValueError as e:
                 raise ValueError(
-                    "'unk_data' correlation data is not compatible with "
-                    "'cross_data'") from e
+                    "'unk_data' correlation data is not compatible with " "'cross_data'"
+                ) from e
             w_pp_data = unk_data.data
             w_pp_samp = unk_data.samples
             mitigate.append("unknown")
 
         if len(mitigate) > 0:
             logger.debug(f"mitigating {' and '.join(mitigate)} sample bias")
         N = cross_data.n_samples
@@ -212,19 +213,19 @@
             warnings.simplefilter("ignore")
             nz_samp = w_sp_samp / np.sqrt(dzsq_samp * w_ss_samp * w_pp_samp)
         return cls(
             binning=cross_data.binning,
             data=nz_data,
             samples=nz_samp,
             method=cross_data.method,
-            info=info)
+            info=info,
+        )
 
     @classmethod
-    @deprecated(
-        reason="renamed to RedshiftData.from_corrfuncs", version="2.3.2")
+    @deprecated(reason="renamed to RedshiftData.from_corrfuncs", version="2.3.2")
     def from_correlation_functions(cls, *args, **kwargs):
         """
         .. deprecated:: 2.3.2
             Renamed to :meth:`from_corrfuncs`.
         """
         return cls.from_corrfuncs(*args, **kwargs)
 
@@ -235,15 +236,15 @@
         ref_corr: CorrFunc | None = None,
         unk_corr: CorrFunc | None = None,
         *,
         cross_est: str | None = None,
         ref_est: str | None = None,
         unk_est: str | None = None,
         config: ResamplingConfig | None = None,
-        info: str | None = None
+        info: str | None = None,
     ) -> RedshiftData:
         """Sample correlation functions to compute a redshift estimate.
 
         The required argument is a crosscorrelation measurement, additional
         parameters can specify sample autocorrelation measurements that are used
         to mitigate the evolving galaxy bias.
 
@@ -260,46 +261,46 @@
         Returns:
             :obj:`RedshiftData`
         """
         if config is None:
             config = ResamplingConfig()
         with TimedLog(
             logger.debug,
-            f"estimating clustering redshifts with method '{config.method}'"
+            f"estimating clustering redshifts with method '{config.method}'",
         ):
             # check compatibilty before sampling anything
             if ref_corr is not None:
                 try:
                     cross_corr.is_compatible(ref_corr, require=True)
                 except ValueError as e:
                     raise ValueError(
                         "'ref_corr' correlation function is not compatible "
-                        "with 'cross_corr'") from e
+                        "with 'cross_corr'"
+                    ) from e
             if unk_corr is not None:
                 try:
                     cross_corr.is_compatible(unk_corr, require=True)
                 except ValueError as e:
                     raise ValueError(
                         "'unk_corr' correlation function is not compatible "
-                        "with 'cross_corr'") from e
+                        "with 'cross_corr'"
+                    ) from e
             # sample pair counts and evaluate estimator
             cross_data = cross_corr.sample(config, estimator=cross_est)
             if ref_corr is not None:
                 ref_data = ref_corr.sample(config, estimator=ref_est)
             else:
                 ref_data = None
             if unk_corr is not None:
                 unk_data = unk_corr.sample(config, estimator=unk_est)
             else:
                 unk_data = None
             return cls.from_correlation_data(
-                cross_data=cross_data,
-                ref_data=ref_data,
-                unk_data=unk_data,
-                info=info)
+                cross_data=cross_data, ref_data=ref_data, unk_data=unk_data, info=info
+            )
 
     @property
     def _dat_desc(self) -> str:
         return "# n(z) estimate with symmetric 68% percentile confidence"
 
     @property
     def _smp_desc(self) -> str:
@@ -320,38 +321,42 @@
             The fit does not use the uncertainties but weights the data points
             inversely to their amplitude.
 
         Args:
             to (:obj:`CorrData`, optional):
                 Reference data to which the stored values are normalised by
                 fitting.
-        
+
         Returns:
             :obj:`RedshiftData`
         """
         if to is None:
             norm = np.nansum(self.dz * self.data)
         else:
             y_from = self.data
             y_to = to.data
             mask = np.isfinite(y_from) & np.isfinite(y_to) & (y_to > 0.0)
             norm = scipy.optimize.curve_fit(
                 lambda x, norm: y_from[mask] / norm,  # x is a dummy variable
-                xdata=to.mids[mask], ydata=y_to[mask],
-                p0=[1.0], sigma=1/y_to[mask])[0][0]
+                xdata=to.mids[mask],
+                ydata=y_to[mask],
+                p0=[1.0],
+                sigma=1 / y_to[mask],
+            )[0][0]
         return self.__class__(
             binning=self.get_binning(),
             data=self.data / norm,
             samples=self.samples / norm,
             method=self.method,
-            info=self.info)
+            info=self.info,
+        )
 
     def mean(self):
         """Attempts to compute a mean redshift.
-        
+
         .. Warning::
             This should be just considered an estimate since the redshift
             estimate is not a true probability density, due to residual negative
             correlation amplitudes.
 
         Returns:
             :obj:`~yaw.core.SampledValue`:
@@ -370,39 +375,37 @@
             The result may be inaccurate since the redshift estimate is not a
             true probability density, due to residual negative correlation
             amplitudes.
 
         Args:
             bins (:obj:`NDArray`):
                 Edges of the new redshift bins. May exceed or cover just a
-                fraction of the original redshift range.            
+                fraction of the original redshift range.
 
         Returns:
             :obj:`RedshiftData`:
         """
         old_bins = self.edges
         # shift main values
         data = rebin(bins, old_bins, self.data)
         # shift the value samples
-        samples = np.empty([self.n_samples, len(bins)-1], data.dtype)
+        samples = np.empty([self.n_samples, len(bins) - 1], data.dtype)
         for i, sample in enumerate(self.samples):
             samples[i] = rebin(bins, old_bins, sample)
 
         return self.__class__(
             binning=pd.IntervalIndex.from_breaks(bins),
             data=data,
             samples=samples,
             method=self.method,
-            info=self.info)
+            info=self.info,
+        )
 
     def shift(
-        self,
-        dz: float | SampledValue = 0.0,
-        *,
-        amplitude: float | SampledValue = 1.0
+        self, dz: float | SampledValue = 0.0, *, amplitude: float | SampledValue = 1.0
     ) -> RedshiftData:
         """Attempts shift the data along the redshift axis.
 
         The shifting is performed by recomputing the redshift estimate with its
         original redshift bins which are shifted by some amount.
 
         .. Warning::
@@ -443,21 +446,22 @@
             samples[i] = shift_histogram(bins, sample, A=amplitude, dx=dz)
 
         return self.__class__(
             binning=self.get_binning(),
             data=data,
             samples=samples,
             method=self.method,
-            info=self.info)
+            info=self.info,
+        )
 
 
 @dataclass(frozen=True, repr=False, eq=False)
 class HistData(RedshiftData):
     """Container for histogram data.
-    
+
     Contains the redshift binning, histogram counts, and resampled counts (e.g.
     from jackknife or bootstrap). The resampled values are used to compute error
     estimates and covariance/correlation matrices. Provides some plotting
     methods for convenience.
 
     Args:
         binning (:obj:`pandas.IntervalIndex`):
@@ -488,37 +492,36 @@
     def _smp_desc(self) -> str:
         n = "normalised " if self.density else " "
         return f"# {self.n_samples} {self.method} n(z) {n}histogram samples"
 
     @property
     def _cov_desc(self) -> str:
         n = "normalised " if self.density else " "
-        return (
-            f"# n(z) {n}histogram covariance matrix "
-            f"({self.n_bins}x{self.n_bins})")
+        return f"# n(z) {n}histogram covariance matrix ({self.n_bins}x{self.n_bins})"
 
     @classmethod
     def from_files(cls, path_prefix: TypePathStr) -> HistData:
         new = super().from_files(path_prefix)
         with open(f"{path_prefix}.dat") as f:
             line = f.readline()
             density = "normalised" in line
         return cls(
             binning=new.get_binning(),
             data=new.data,
             samples=new.samples,
             method=new.method,
-            density=density)
+            density=density,
+        )
 
     def normalised(self, *args, **kwargs) -> HistData:
         """Obtain a normalised copy of the data.
 
         Normalises the data by integration along the redshift axis. This sets
         the containers :obj:`density` flag to ``True``.
-        
+
         Returns:
             :obj:`HistData`
         """
         if self.density:  # guard from repeatedly altering the data
             return self
         zmin, zmax = self.edges[[0, -1]]
         width_correction = (zmax - zmin) / (self.n_bins * self.dz)
@@ -527,15 +530,16 @@
         norm = np.nansum(self.dz * data)
         return self.__class__(
             binning=self.get_binning(),
             data=data / norm,
             samples=samples / norm,
             method=self.method,
             info=self.info,
-            density=True)
+            density=True,
+        )
 
     def mean(self) -> SampledValue:
         """Compute the mean redshift.
 
         Returns:
             :obj:`~yaw.core.SampledValue`:
                 Mean redshift for the redshift data and its samples in a data
@@ -553,28 +557,25 @@
         .. Warning::
             The result may be inaccurate since the result is interpolated
             step-wise.
 
         Args:
             bins (:obj:`NDArray`):
                 Edges of the new redshift bins. May exceed or cover just a
-                fraction of the original redshift range.            
+                fraction of the original redshift range.
 
         Returns:
             :obj:`HistData`:
         """
         result = super().rebin(bins)
         object.__setattr__(self, "density", self.density)
         return result
 
     def shift(
-        self,
-        dz: float | SampledValue = 0.0,
-        *,
-        amplitude: float | SampledValue = 1.0
+        self, dz: float | SampledValue = 0.0, *, amplitude: float | SampledValue = 1.0
     ) -> HistData:
         """Shifts the data along the redshift axis.
 
         The shifting is performed by recomputing the histogram with its original
         redshift bins which are shifted by some amount.
 
         .. Warning::
```

### Comparing `yet_another_wizz-2.5/src/yaw_cli/commandline/main.py` & `yet_another_wizz-2.5.post0/src/yaw_cli/commandline/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,45 +2,46 @@
 
 import argparse
 from collections.abc import Sequence
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 from yaw import __version__
-
+from yaw_cli.commandline import utils
 from yaw_cli.pipeline.data import BinnedInput, Input
 from yaw_cli.pipeline.logger import Colors, init_logger, print_yaw_message
 
-from yaw_cli.commandline import utils
-
 if TYPE_CHECKING:  # pragma: no cover
     from yaw_cli.commandline.subcommands import SubCommand
 
 
 class _Commandline:
-
     def __init__(self) -> None:
         self._subcommands: dict[str, SubCommand] = {}
         # add parser
         self.parser = argparse.ArgumentParser(
             prog="yaw_cli",
             description="yet_another_wizz: modular clustering redshift pipeline.",
-            epilog="Thank you for using yet_another_wizz. Please consider citing 'A&A 642, A200 (2020)' when publishing results obtained with this code.")
+            epilog="Thank you for using yet_another_wizz. Please consider citing 'A&A 642, A200 (2020)' when publishing results obtained with this code.",
+        )
         self.parser.add_argument(
-            "--version", action="version", version=f"yet_another_wizz v{__version__}")
+            "--version", action="version", version=f"yet_another_wizz v{__version__}"
+        )
         self.subparsers = self.parser.add_subparsers(
             title="modules",
             description="The pipeline is split into modules which perform specifc tasks as listed below. Each module has its own dedicated --help command.",
-            dest="task")
+            dest="task",
+        )
 
     def register_subcommand(self, command: SubCommand) -> None:
         name = command.get_name()
         if name in self._subcommands:
             raise utils.CommandlineInitError(
-                f"subcommand with name '{name}' already exists")
+                f"subcommand with name '{name}' already exists"
+            )
         self._subcommands[name] = command
         command.add_parser()
 
     def parse_args(self, args: Sequence[str] | None = None) -> argparse.Namespace:
         return self.parser.parse_args(args)
 
     def print_usage(self) -> None:
@@ -49,136 +50,184 @@
     def create_subparser(
         self,
         name: str,
         help: str,
         description: str,
         wdir: bool = True,
         threads: bool = False,
-        progress: bool = False
+        progress: bool = False,
     ) -> argparse.ArgumentParser:
         parser = self.subparsers.add_parser(
-            name=name, help=help, description=description)
+            name=name, help=help, description=description
+        )
         parser.add_argument(
-            "-v", "--verbose", action="count", default=0,
-            help="show additional information in terminal, repeat to show debug messages")
+            "-v",
+            "--verbose",
+            action="count",
+            default=0,
+            help="show additional information in terminal, repeat to show debug messages",
+        )
         if wdir:
             parser.add_argument(
-                "wdir", metavar="<directory>", type=utils.Directory_exists,
-                help="project directory, must exist")
+                "wdir",
+                metavar="<directory>",
+                type=utils.Directory_exists,
+                help="project directory, must exist",
+            )
         if threads:
             parser.add_argument(
-                "--threads", type=int, metavar="<int>",
-                help="number of threads to use (default: from configuration)")
+                "--threads",
+                type=int,
+                metavar="<int>",
+                help="number of threads to use (default: from configuration)",
+            )
         if progress:
             parser.add_argument(
-                "--progress", action="store_true",
-                help="show a progress bar if the backend supports it")
+                "--progress",
+                action="store_true",
+                help="show a progress bar if the backend supports it",
+            )
         return parser
 
     @staticmethod
     def add_input_parser(
         parser: argparse.ArgumentParser,
         title: str,
         prefix: str,
         required: bool = False,
         binned: bool = False,
-        require_z: bool = False
+        require_z: bool = False,
     ):
         # create an argument group for the parser
         opt = "" if required else " (optional)"
         group = parser.add_argument_group(
-            title=title, description=f"specify the {title} input file{opt}")
+            title=title, description=f"specify the {title} input file{opt}"
+        )
         if binned:
             group.add_argument(
-                f"--{prefix}-path", required=required, nargs="+", type=utils.Path_exists, metavar="<file>",
-                help="(list of) input file paths (e.g. if the data sample is binned tomographically)")
+                f"--{prefix}-path",
+                required=required,
+                nargs="+",
+                type=utils.Path_exists,
+                metavar="<file>",
+                help="(list of) input file paths (e.g. if the data sample is binned tomographically)",
+            )
         else:
             group.add_argument(
-                f"--{prefix}-path", required=required, type=utils.Path_exists, metavar="<file>",
-                help="input file path")
-        group.add_argument(
-            f"--{prefix}-ra", required=required, metavar="<str>",
-            help="column name of right ascension")
-        group.add_argument(
-            f"--{prefix}-dec", required=required, metavar="<str>",
-            help="column name of declination")
-        group.add_argument(
-            f"--{prefix}-z", metavar="<str>", required=(required and require_z),
-            help="column name of redshift")
-        group.add_argument(
-            f"--{prefix}-w", metavar="<str>",
-            help="column name of object weight")
-        group.add_argument(
-            f"--{prefix}-patch", metavar="<str>",
-            help="column name of patch assignment index")
+                f"--{prefix}-path",
+                required=required,
+                type=utils.Path_exists,
+                metavar="<file>",
+                help="input file path",
+            )
+        group.add_argument(
+            f"--{prefix}-ra",
+            required=required,
+            metavar="<str>",
+            help="column name of right ascension",
+        )
+        group.add_argument(
+            f"--{prefix}-dec",
+            required=required,
+            metavar="<str>",
+            help="column name of declination",
+        )
+        group.add_argument(
+            f"--{prefix}-z",
+            metavar="<str>",
+            required=(required and require_z),
+            help="column name of redshift",
+        )
+        group.add_argument(
+            f"--{prefix}-w", metavar="<str>", help="column name of object weight"
+        )
+        group.add_argument(
+            f"--{prefix}-patch",
+            metavar="<str>",
+            help="column name of patch assignment index",
+        )
         if binned:
             group.add_argument(
-                f"--{prefix}-idx", type=int, metavar="<int>", nargs="+",
-                help=f"integer index to identify the input files (or bins) provided with [--{prefix}-path] (default: 0, 1, ...)")
-        group.add_argument(
-            f"--{prefix}-cache", action="store_true",
-            help="cache the data in the project's cache directory")
+                f"--{prefix}-idx",
+                type=int,
+                metavar="<int>",
+                nargs="+",
+                help=f"integer index to identify the input files (or bins) provided with [--{prefix}-path] (default: 0, 1, ...)",
+            )
+        group.add_argument(
+            f"--{prefix}-cache",
+            action="store_true",
+            help="cache the data in the project's cache directory",
+        )
 
     @staticmethod
     def get_input_from_args(
-        args: argparse.Namespace,
-        prefix: str,
-        require_z: bool = False
+        args: argparse.Namespace, prefix: str, require_z: bool = False
     ) -> BinnedInput | Input | None:
         # mapping of parser argument name suffix to in Input class argument
         suffix_to_kwarg = dict(
-            path="filepath", ra="ra", dec="dec", z="redshift",
-            w="weight", patch="patches", cache="cache", idx="index")
+            path="filepath",
+            ra="ra",
+            dec="dec",
+            z="redshift",
+            w="weight",
+            patch="patches",
+            cache="cache",
+            idx="index",
+        )
         # get all entries in args that match the given prefix
         args_subset = {}
         for arg, value in vars(args).items():
             if arg.startswith(f"{prefix}_") and value is not None:
-                suffix = arg[len(prefix)+1:]
+                suffix = arg[len(prefix) + 1 :]
                 args_subset[suffix] = value
 
         # the argument group can be optional
         if args_subset.get("path") is None:
             # check that there are no other arguments provided in the group
             if not all(
-                isinstance(value, (bool, type(None)))
-                for value in args_subset.values()
+                isinstance(value, (bool, type(None))) for value in args_subset.values()
             ):  # argparse flags have False as default value instead of None
                 raise argparse.ArgumentError(
                     f"the following arguments are required if any other "
-                    f"--{prefix}-* is provided: --{prefix}-path")
+                    f"--{prefix}-* is provided: --{prefix}-path"
+                )
             return None
 
         else:
-            binned = (not isinstance(args_subset["path"], (Path, str)))
+            binned = not isinstance(args_subset["path"], (Path, str))
             # check for optionally required arguments not known to the parser
             required = ["ra", "dec"]
             if require_z:
                 required.append("z")
             for suffix in required:
                 if suffix not in args_subset:
                     arg = f"--{prefix}-{suffix}"
                     raise argparse.ArgumentError(
-                        f"the following arguments are required: {arg}")
+                        f"the following arguments are required: {arg}"
+                    )
             # return the (Binned)Input instance
             kwargs = {}
             for suffix, value in args_subset.items():
                 kw_name = suffix_to_kwarg[suffix]
                 kwargs[kw_name] = value
             idx = kwargs.pop("index", None)
             if binned:
                 # check the --*-idx argument
                 paths = args_subset["path"]
                 if idx is not None:
                     if len(idx) != len(paths):
                         raise argparse.ArgumentError(
                             f"number of file paths [--{prefix}-path] and "
-                            f"indices [--{prefix}-idx] do not match")
+                            f"indices [--{prefix}-idx] do not match"
+                        )
                     if len(idx) != len(set(idx)):
                         raise argparse.ArgumentError(
-                            f"indices [--{prefix}-idx] not unique")
+                            f"indices [--{prefix}-idx] not unique"
+                        )
                 else:
                     idx = range(1, len(paths) + 1)
                 # update the key word arguments with a dict: idx -> path
                 kwargs["filepath"] = {i: path for i, path in zip(idx, paths)}
                 return BinnedInput.from_dict(kwargs)
             else:
                 return Input.from_dict(kwargs)
```

### Comparing `yet_another_wizz-2.5/src/yaw_cli/commandline/subcommands.py` & `yet_another_wizz-2.5.post0/src/yaw_cli/commandline/subcommands.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from __future__ import annotations
 
 import argparse
 import logging
 import sys
 from abc import ABC, abstractclassmethod
 
-from yaw import __version__
 from yaw import config as yaw_config
-from yaw.config import Configuration, DEFAULT, OPTIONS
+from yaw.config import DEFAULT, OPTIONS, Configuration
 from yaw.core.docs import populate_parser
-
+from yaw_cli.commandline import utils
+from yaw_cli.commandline.main import Commandline
 from yaw_cli.pipeline import tasks as yaw_tasks
 from yaw_cli.pipeline.merge import MergedDirectory, open_yaw_directory
 from yaw_cli.pipeline.project import (
-    ProjectDirectory, load_config_from_setup, load_setup_as_dict)
-
-from yaw_cli.commandline import utils
-from yaw_cli.commandline.main import Commandline
-
+    ProjectDirectory,
+    load_config_from_setup,
+    load_setup_as_dict,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class SubCommand(ABC):
-
     def __init_subclass__(cls, **kwargs) -> None:
         super().__init_subclass__(**kwargs)
         Commandline.register_subcommand(cls)
 
     @abstractclassmethod
     def get_name(cls) -> str:
         return "command"
@@ -38,92 +36,111 @@
 
     @abstractclassmethod
     def run(cls, args: argparse.Namespace) -> None:
         pass
 
 
 class CommandInit(SubCommand):
-
     @classmethod
     def get_name(cls) -> str:
         return "init"
 
     @classmethod
     def add_parser(cls) -> None:
         parser = Commandline.create_subparser(
             name=cls.get_name(),
             help="initialise and configure a new a project directory",
-            description="Initialise and create a project directory with a "
-                        "configuration. Specify the reference sample data and "
-                        "optionally randoms.",
+            description="Initialise and create a project directory with a configuration"
+            ". Specify the reference sample data and optionally randoms.",
             wdir=False,
             threads=False,
-            progress=False)
+            progress=False,
+        )
         parser.add_argument(  # manual since special help text
-            "wdir", metavar="<path>", type=utils.Path_absolute,
-            help="project directory, must not exist")
+            "wdir",
+            metavar="<path>",
+            type=utils.Path_absolute,
+            help="project directory, must not exist",
+        )
         parser.add_argument(
-            "-s", "--setup", type=utils.Path_exists, metavar="<file>",
+            "-s",
+            "--setup",
+            type=utils.Path_exists,
+            metavar="<file>",
             help="optionl setup YAML file (e.g. from 'yaw_cli run -d') with "
-                 "base configuration that is overwritten by arguments below")
+            "base configuration that is overwritten by arguments below",
+        )
 
-        group_other = parser.add_argument_group(
-            title="additional arguments")
+        group_other = parser.add_argument_group(title="additional arguments")
         group_other.add_argument(
-            "--backend", choices=OPTIONS.backend, default=DEFAULT.backend,
-            help="backend used for pair counting (default: %(default)s)")
+            "--backend",
+            choices=OPTIONS.backend,
+            default=DEFAULT.backend,
+            help="backend used for pair counting (default: %(default)s)",
+        )
         group_other.add_argument(
-            "--cache-path", metavar="<path>", type=utils.Path_absolute,
+            "--cache-path",
+            metavar="<path>",
+            type=utils.Path_absolute,
             help="non-standard location for the cache directory (e.g. on "
-                 "faster storage, default: [project directory]/cache)")
+            "faster storage, default: [project directory]/cache)",
+        )
         group_other.add_argument(
-            "--n-patches", type=int, metavar="<int>",
+            "--n-patches",
+            type=int,
+            metavar="<int>",
             help="split all input data into this number of spatial patches for "
-                 "covariance estimation (default: patch index for catalogs)")
+            "covariance estimation (default: patch index for catalogs)",
+        )
         populate_parser(yaw_config.Configuration, group_other)
 
         Commandline.add_input_parser(
-            parser, "reference (data)", prefix="ref",
-            required=True, require_z=True)
+            parser, "reference (data)", prefix="ref", required=True, require_z=True
+        )
 
         Commandline.add_input_parser(
-            parser, "reference (random)", prefix="rand",
-            required=False, require_z=True)
+            parser, "reference (random)", prefix="rand", required=False, require_z=True
+        )
 
         group_scales = parser.add_argument_group(
             title="measurement scales",
-            description="sets the physical scales for the correlation "
-                        "measurements")
+            description="sets the physical scales for the correlation measurements",
+        )
         populate_parser(yaw_config.ScalesConfig, group_scales)
 
         group_bins = parser.add_argument_group(
             title="redshift binning",
-            description="sets the redshift binning for the clustering "
-                        "redshifts")
+            description="sets the redshift binning for the clustering redshifts",
+        )
         populate_parser(yaw_config.AutoBinningConfig, group_bins)
         populate_parser(yaw_config.ManualBinningConfig, group_bins)
 
         group_backend = parser.add_argument_group(
             title="backend specific",
-            description="parameters that are specific to pair counting "
-                        "backends")
+            description="parameters that are specific to pair counting backends",
+        )
         populate_parser(yaw_config.BackendConfig, group_backend)
 
     @classmethod
     def run(cls, args: argparse.Namespace) -> None:
         # parser arguments for Configuration
         config_args = dict(
             cosmology=args.cosmology,
-            rmin=args.rmin, rmax=args.rmax,
-            rweight=args.rweight, rbin_num=args.rbin_num,
-            zmin=args.zmin, zmax=args.zmax,
-            zbin_num=args.zbin_num, method=args.method,
+            rmin=args.rmin,
+            rmax=args.rmax,
+            rweight=args.rweight,
+            rbin_num=args.rbin_num,
+            zmin=args.zmin,
+            zmax=args.zmax,
+            zbin_num=args.zbin_num,
+            method=args.method,
             thread_num=args.thread_num,
             crosspatch=args.crosspatch,
-            rbin_slop=args.rbin_slop)
+            rbin_slop=args.rbin_slop,
+        )
         renames = dict(threads="thread_num", no_crosspatch="crosspatch")
 
         # load base configuration from setup file and update from command line
         if args.setup is not None:
             base_config = load_config_from_setup(args.setup)
             # optional arguments have default values which may overshadow values
             # in the base configuration
@@ -142,291 +159,315 @@
 
         # parse the configuration as given
         else:
             config = Configuration.create(**config_args)
 
         # create the project directory
         with ProjectDirectory.create(
-            args.wdir, config, n_patches=args.n_patches,
-            cachepath=args.cache_path, backend=args.backend
+            args.wdir,
+            config,
+            n_patches=args.n_patches,
+            cachepath=args.cache_path,
+            backend=args.backend,
         ) as project:
             # get the data catalog and the optional random catalog
-            input_ref = Commandline.get_input_from_args(
-                args, "ref", require_z=True)
-            input_rand = Commandline.get_input_from_args(
-                args, "rand", require_z=True)
+            input_ref = Commandline.get_input_from_args(args, "ref", require_z=True)
+            input_rand = Commandline.get_input_from_args(args, "rand", require_z=True)
             project.set_reference(data=input_ref, rand=input_rand)
 
 
 class CommandCrosscorr(SubCommand):
-
     @classmethod
     def get_name(cls) -> str:
         return "cross"
 
     @classmethod
     def add_parser(cls) -> None:
         parser = Commandline.create_subparser(
             name=cls.get_name(),
             help="measure angular cross-correlation functions",
-            description="Specify the unknown data sample(s) and optionally "
-                        "randoms. Measure the angular cross-correlation "
-                        "function amplitude with the reference sample in bins "
-                        "of redshift.",
+            description="Specify the unknown data sample(s) and optionally randoms. "
+            "Measure the angular cross-correlation function amplitude with the reference "
+            "sample in bins of redshift.",
             progress=True,
-            threads=True)
+            threads=True,
+        )
         populate_parser(yaw_tasks.TaskCrosscorr, parser)
 
         Commandline.add_input_parser(
-            parser, "unknown (data)", prefix="unk",
-            required=True, binned=True)
+            parser, "unknown (data)", prefix="unk", required=True, binned=True
+        )
 
         Commandline.add_input_parser(
-            parser, "unknown (random)", prefix="rand",
-            required=False, binned=True)
+            parser, "unknown (random)", prefix="rand", required=False, binned=True
+        )
 
     @classmethod
     def run(cls, args: argparse.Namespace) -> None:
         with ProjectDirectory(args.wdir) as project:
             # get the data catalog and the optional random catalog
-            input_unk = Commandline.get_input_from_args(
-                args, "unk", require_z=False)
-            input_rand = Commandline.get_input_from_args(
-                args, "rand", require_z=False)
+            input_unk = Commandline.get_input_from_args(args, "unk", require_z=False)
+            input_rand = Commandline.get_input_from_args(args, "rand", require_z=False)
             if input_unk.get_bin_indices() != input_rand.get_bin_indices():
-                raise ValueError(
-                    "bin indices for data and randoms do not match")
+                raise ValueError("bin indices for data and randoms do not match")
             for idx in input_unk.get_bin_indices():
                 project.add_unknown(
-                    idx, data=input_unk.get(idx), rand=input_rand.get(idx))
+                    idx, data=input_unk.get(idx), rand=input_rand.get(idx)
+                )
 
             task = yaw_tasks.TaskCrosscorr.from_argparse(args)
-            project.tasks.run(
-                task, progress=args.progress, threads=args.threads)
+            project.tasks.run(task, progress=args.progress, threads=args.threads)
 
 
 class CommandAutocorr(SubCommand):
-
     @classmethod
     def get_name(cls) -> str:
         return "auto"
 
     @classmethod
     def add_parser(cls) -> None:
         parser = Commandline.create_subparser(
             name=cls.get_name(),
             help="measure angular autocorrelation functions",
-            description="Measure the angular autocorrelation function "
-                        "amplitude of the reference sample. Can be applied to "
-                        "the unknown sample if redshift point-estimates are "
-                        "available.",
+            description="Measure the angular autocorrelation function amplitude of the "
+            "reference sample. Can be applied to the unknown sample if redshift point-"
+            "estimates are available.",
             progress=True,
-            threads=True)
+            threads=True,
+        )
         parser.add_argument(
-            "--which", choices=("ref", "unk"), default="ref",
+            "--which",
+            choices=("ref", "unk"),
+            default="ref",
             help="for which sample the autocorrelation should be computed "
-                 "(default: %(default)s, requires redshifts [--*-z] for data "
-                 "and random sample)")
+            "(default: %(default)s, requires redshifts [--*-z] for data "
+            "and random sample)",
+        )
         populate_parser(yaw_tasks.TaskAutocorr, parser)
 
     @classmethod
     def run(cls, args: argparse.Namespace) -> None:
         with ProjectDirectory(args.wdir) as project:
             if args.which == "ref":
                 task = yaw_tasks.TaskAutocorrReference.from_argparse(args)
             else:
                 task = yaw_tasks.TaskAutocorrUnknown.from_argparse(args)
-            project.tasks.run(
-                task, progress=args.progress, threads=args.threads)
+            project.tasks.run(task, progress=args.progress, threads=args.threads)
 
 
 class CommandTrueRedshifts(SubCommand):
-
     @classmethod
     def get_name(cls) -> str:
         return "ztrue"
 
     @classmethod
     def add_parser(cls) -> None:
         parser = Commandline.create_subparser(
             name=cls.get_name(),
             help=yaw_tasks.TaskTrueRedshifts.get_help(),
-            description="Compute the redshift distributions of the unknown "
-                        "data sample(s), which requires providing point-"
-                        "estimate redshifts for the catalog.",
+            description="Compute the redshift distributions of the unknown data sample(s), "
+            "which requires providing point-estimate redshifts for the catalog.",
             progress=True,
-            threads=True)
+            threads=True,
+        )
         populate_parser(yaw_tasks.TaskTrueRedshifts, parser)
 
     @classmethod
     def run(cls, args: argparse.Namespace) -> None:
         with ProjectDirectory(args.wdir) as project:
             task = yaw_tasks.TaskTrueRedshifts.from_argparse(args)
-            project.tasks.run(
-                task, progress=args.progress, threads=args.threads)
+            project.tasks.run(task, progress=args.progress, threads=args.threads)
 
 
 class CommandCache(SubCommand):
-
     @classmethod
     def get_name(cls) -> str:
         return "cache"
 
     @classmethod
     def add_parser(cls) -> None:
         parser = Commandline.create_subparser(
             name=cls.get_name(),
             help="mange or clean up cache directories",
             description="Get a summary of the project's cache directory "
-                        "(location, size, etc.) or remove entries with --drop.")
+            "(location, size, etc.) or remove entries with --drop.",
+        )
         parser.add_argument(
-            "--drop", action="store_true",
-            help="drop all cache entries")
+            "--drop", action="store_true", help="drop all cache entries"
+        )
 
     @classmethod
     def run(cls, args: argparse.Namespace) -> None:
         with ProjectDirectory(args.wdir) as project:
             if args.drop:
                 task = yaw_tasks.TaskDropCache.from_argparse(args)
                 project.tasks.run(task)
             else:
                 cachedir = project.inputs.get_cache()
                 cachedir.print_contents()
 
 
 class CommandMerge(SubCommand):
-
     @classmethod
     def get_name(cls) -> str:
         return "merge"
 
     @classmethod
     def add_parser(cls) -> None:
         parser = Commandline.create_subparser(
             name=cls.get_name(),
             help="merge correlation measurements from different sources",
-            description="Combine pair count data from different project "
-                        "directories with compatible configuration. Supported "
-                        "cases are: concatenating patches with the same "
-                        "redshift binning and concatenating redshift "
-                        "bins with same patches (not verified).",
-            wdir=False)
+            description="Combine pair count data from different project directories with "
+            "compatible configuration. Supported cases are: concatenating patches with "
+            "the same redshift binning and concatenating redshift bins with same patches "
+            "(not verified).",
+            wdir=False,
+        )
         parser.add_argument(  # manual since special help text
-            "wdir", metavar="<path>", type=utils.Path_absolute,
-            help="directory where data is merged, must not exist")
+            "wdir",
+            metavar="<path>",
+            type=utils.Path_absolute,
+            help="directory where data is merged, must not exist",
+        )
         parser.add_argument(
-            "--mode", choices=OPTIONS.merge, required=True,
-            help="specify whether merging is performed on tomographic bins, "
-                 "extending spatially from patches, or by concatenating along "
-                 "the redshift axis")
+            "--mode",
+            choices=OPTIONS.merge,
+            required=True,
+            help="specify whether merging is performed on tomographic bins, extending "
+            "spatially from patches, or by concatenating along the redshift axis",
+        )
         parser.add_argument(
-            "-p", "--projects", nargs="+", required=True,
-            help="list of project directory paths to merge")
+            "-p",
+            "--projects",
+            nargs="+",
+            required=True,
+            help="list of project directory paths to merge",
+        )
 
     @classmethod
     def run(cls, args: argparse.Namespace) -> None:
         MergedDirectory.from_projects(args.wdir, args.projects, mode=args.mode)
 
 
 class CommandEstimateCorr(SubCommand):
-
     @classmethod
     def get_name(cls) -> str:
         return "zcc"
 
     @classmethod
     def add_parser(cls) -> None:
         parser = Commandline.create_subparser(
             name=cls.get_name(),
             help=yaw_tasks.TaskEstimateCorr.get_help(),
-            description="Compute clustering redshift estimates for the unknown "
-                        "data sample(s), optionally mitigating galaxy bias "
-                        "estimated from any measured autocorrelation function.")
+            description="Compute clustering redshift estimates for the unknown data "
+            "sample(s), optionally mitigating galaxy bias estimated from any measured "
+            "autocorrelation function.",
+        )
 
         group_est = parser.add_argument_group(
             title="correlation estimators",
             description="configure estimators for the different types of "
-                        "correlation functions")
+            "correlation functions",
+        )
 
         group_samp = parser.add_argument_group(
             title="resampling",
-            description="configure the resampling used for covariance "
-                        "estimates")
+            description="configure the resampling used for covariance " "estimates",
+        )
 
-        populate_parser(yaw_tasks.TaskEstimateCorr, parser, extra_parsers=dict(
-            estimators=group_est, sampling=group_samp))
+        populate_parser(
+            yaw_tasks.TaskEstimateCorr,
+            parser,
+            extra_parsers=dict(estimators=group_est, sampling=group_samp),
+        )
 
     @classmethod
     def run(cls, args: argparse.Namespace) -> None:
         with open_yaw_directory(args.wdir) as project:
             task = yaw_tasks.TaskEstimateCorr.from_argparse(args)
             project.tasks.run(task)
 
 
 class CommandPlot(SubCommand):
-
     @classmethod
     def get_name(cls) -> str:
         return "plot"
 
     @classmethod
     def add_parser(cls) -> None:
         parser = Commandline.create_subparser(
             name=cls.get_name(),
             help=yaw_tasks.TaskPlot.get_help(),
             description="Plot the autocorrelations and redshift estimates into "
-                        "the 'estimate' directory.")
+            "the 'estimate' directory.",
+        )
         populate_parser(yaw_tasks.TaskPlot, parser)
 
     @classmethod
     def run(cls, args: argparse.Namespace) -> None:
         with open_yaw_directory(args.wdir) as project:
             task = yaw_tasks.TaskPlot.from_argparse(args)
             project.tasks.run(task)
 
 
 class CommandRun(SubCommand):
-
     @classmethod
     def get_name(cls) -> str:
         return "run"
 
     @classmethod
     def add_parser(cls) -> None:
         parser = Commandline.create_subparser(
             name=cls.get_name(),
             help="perform tasks specified in a setup file",
-            description="Read a task list and configuration from a setup file "
-                        "(e.g. as generated by 'init'). Apply the tasks to the "
-                        "specified data samples.",
+            description="Read a task list and configuration from a setup file (e.g. as "
+            "generated by 'init'). Apply the tasks to the specified data samples.",
             wdir=False,
             threads=True,
-            progress=True)
+            progress=True,
+        )
         parser.add_argument(  # manual since special help text
-            "wdir", metavar="<path>", type=utils.Path_absolute,
-            help="project directory, must not exist")
+            "wdir",
+            metavar="<path>",
+            type=utils.Path_absolute,
+            help="project directory, must not exist",
+        )
 
         group_setup = parser.add_argument_group(
             title="setup configuration",
-            description="select a setup file to run with optional modifcations")
+            description="select a setup file to run with optional modifcations",
+        )
         group_setup.add_argument(
-            "-d", "--dump", action=utils.DumpConfigAction,
-            const="default", nargs=0,
-            help="dump an empty setup file with default values to the terminal")
+            "-d",
+            "--dump",
+            action=utils.DumpConfigAction,
+            const="default",
+            nargs=0,
+            help="dump an empty setup file with default values to the terminal",
+        )
         group_setup.add_argument(
-            "-s", "--setup", required=True,
-            type=utils.Path_exists, metavar="<file>",
-            help="setup YAML file with configuration, input files and "
-                 "task list")
+            "-s",
+            "--setup",
+            required=True,
+            type=utils.Path_exists,
+            metavar="<file>",
+            help="setup YAML file with configuration, input files and task list",
+        )
         group_setup.add_argument(
-            "--config-from", type=utils.Path_exists, metavar="<file>",
-            help="load the 'configuration' section from this setup file")
+            "--config-from",
+            type=utils.Path_exists,
+            metavar="<file>",
+            help="load the 'configuration' section from this setup file",
+        )
         group_setup.add_argument(
-            "--cache-path", metavar="<path>", type=utils.Path_absolute,
-            help="replace the 'data.cachepath' value in the setup file")
+            "--cache-path",
+            metavar="<path>",
+            type=utils.Path_absolute,
+            help="replace the 'data.cachepath' value in the setup file",
+        )
 
     @classmethod
     def run(cls, args: argparse.Namespace) -> None:
         # get the configuration from an external file
         setup = load_setup_as_dict(args.setup)
         if args.config_from is not None:
             config = load_config_from_setup(args.config_from)
```

### Comparing `yet_another_wizz-2.5/src/yaw_cli/commandline/utils.py` & `yet_another_wizz-2.5.post0/src/yaw_cli/commandline/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,28 @@
 
 class CommandlineInitError(Exception):
     pass
 
 
 class DumpConfigAction(Action):
     def __init__(
-        self, option_strings, dest, nargs=0, const="default",
-        required=False, help=None
+        self, option_strings, dest, nargs=0, const="default", required=False, help=None
     ) -> None:
         super().__init__(
-            option_strings=option_strings, dest=dest, nargs=0,
-            const=const, required=required, help=help)
+            option_strings=option_strings,
+            dest=dest,
+            nargs=0,
+            const=const,
+            required=required,
+            help=help,
+        )
 
     def __call__(self, parser, namespace, values, option_string):
         from yaw_cli.pipeline.default_setup import setup_default
+
         print(setup_default)
         parser.exit()
 
 
 def Path_absolute(path: str) -> Path:
     return Path(path).expanduser().absolute()
```

### Comparing `yet_another_wizz-2.5/src/yaw_cli/pipeline/data.py` & `yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 import numpy as np
 
 from yaw.catalogs import NewCatalog
 from yaw.config import default as DEFAULT
 from yaw.core.abc import DictRepresentation
 from yaw.core.coordinates import Coordinate, CoordSky
-from yaw.core.utils import TypePathStr, format_float_fixed_width as fmt_num
-
+from yaw.core.utils import TypePathStr
+from yaw.core.utils import format_float_fixed_width as fmt_num
 from yaw_cli.pipeline.directories import CacheDirectory
 
 if TYPE_CHECKING:
     from yaw.catalogs import BaseCatalog
 
 
 logger = logging.getLogger(__name__)
@@ -33,15 +33,14 @@
 
 class MissingCatalogError(InputError):
     pass
 
 
 @dataclass(frozen=True)
 class Input(DictRepresentation):
-
     filepath: TypePathStr
     ra: str
     dec: str
     redshift: str | None = field(default=None)
     weight: str | None = field(default=None)
     patches: str | None = field(default=None)
     cache: bool | None = field(default=False)
@@ -51,32 +50,30 @@
 
     @staticmethod
     def _check_filepath_type(filepath) -> None:
         if not isinstance(filepath, (str, Path)):
             raise TypeError(f"'filepath' must be of type {str} or {Path}")
 
     @classmethod
-    def from_dict(
-        cls,
-        the_dict: dict[str, str | None],
-        **kwargs
-    ) -> Input:
+    def from_dict(cls, the_dict: dict[str, str | None], **kwargs) -> Input:
         key_names = set(the_dict.keys())
         try:  # check for extra keys
             all_names = set(field.name for field in fields(cls))
             item = (key_names - all_names).pop()
-            raise  InputConfigError(f"encountered unknown argument '{item}'")
+            raise InputConfigError(f"encountered unknown argument '{item}'")
         except KeyError:
             pass
         try:  # check for missing keys
             pos_names = set(
-                field.name for field in fields(cls)
-                if isinstance(field.default, _MISSING_TYPE))
+                field.name
+                for field in fields(cls)
+                if isinstance(field.default, _MISSING_TYPE)
+            )
             item = (pos_names - key_names).pop()
-            raise  InputConfigError(f"missing argument '{item}'")
+            raise InputConfigError(f"missing argument '{item}'")
         except KeyError:
             pass
         cls._check_filepath_type(the_dict["filepath"])
         return cls(**the_dict)
 
     def _filepath_to_dict(self) -> str:
         return str(self.filepath)
@@ -90,20 +87,20 @@
                 result[key] = self._filepath_to_dict()
             else:
                 result[key] = value
         return result
 
 
 class BinnedInput(Input):
-
     filepath: dict[int, TypePathStr]
 
     def __post_init__(self):
         object.__setattr__(
-            self, "filepath", {i: Path(fp) for i, fp in self.filepath.items()})
+            self, "filepath", {i: Path(fp) for i, fp in self.filepath.items()}
+        )
 
     def get_bin_indices(self) -> set[int]:
         return set(self.filepath.keys())
 
     @property
     def n_bins(self) -> int:
         return len(self.filepath)
@@ -144,36 +141,30 @@
 
     @staticmethod
     def _check_filepath_type(filepath) -> None:
         if not isinstance(filepath, dict):
             raise TypeError(f"'filepath' must be of type {dict}")
 
     @classmethod
-    def from_dict(
-        cls,
-        filedata: dict[str, dict | str | None],
-        **kwargs
-    ) -> BinnedInput:
+    def from_dict(cls, filedata: dict[str, dict | str | None], **kwargs) -> BinnedInput:
         return super().from_dict(filedata)
 
     def _filepath_to_dict(self) -> str:
         return {bin_idx: str(fp) for bin_idx, fp in self.filepath.items()}
 
 
 def load_input(cat_dict: dict[str, Any]) -> BinnedInput:
     try:
         return Input.from_dict(cat_dict)
     except TypeError:
         return BinnedInput.from_dict(cat_dict)
 
 
 def _parse_catalog_dict(
-    inputs_dict: dict[str, dict],
-    section: str,
-    binned: bool
+    inputs_dict: dict[str, dict], section: str, binned: bool
 ) -> dict[str, Input | BinnedInput]:
     _inputs_dict = {k: v for k, v in inputs_dict.items()}
     # read in the optionally existing inputs
     parsed = dict()
     for kind in ("data", "rand"):
         cat_dict = _inputs_dict.pop(kind, None)
         if cat_dict is None:
@@ -196,33 +187,34 @@
             parsed[kind] = input
 
     # check for additional or misnamed inputs
     if len(_inputs_dict) > 0:
         key = next(iter(_inputs_dict.keys()))
         raise InputConfigError(
             f"encountered unknown catalog type '{key}', in section '{section}',"
-            " must be 'data' or 'rand'")
+            " must be 'data' or 'rand'"
+        )
 
     # extra care: make sure that the bin indices match
     if binned and parsed["data"] is not None and parsed["rand"] is not None:
         if parsed["data"].get_bin_indices() != parsed["rand"].get_bin_indices():
             raise InputConfigError(
                 f"bin indices in '{section}:data:filepath' and "
-                f" '{section}:rand:filepath' do not match")
+                f" '{section}:rand:filepath' do not match"
+            )
     return parsed
 
 
 class InputManager(DictRepresentation):
-
     def __init__(
         self,
         cachepath: TypePathStr,
         n_patches: int | None = None,
         patch_centers: Coordinate | None = None,
-        backend: str = DEFAULT.backend
+        backend: str = DEFAULT.backend,
     ) -> None:
         if not isinstance(cachepath, (str, Path)):
             raise TypeError("'cachepath' must be 'str' or 'Path'")
         self._cachepath = cachepath
         self.cache_dir.mkdir(parents=True, exist_ok=True)
         # set up patch centers
         self._raise_n_patch_mismatch(patch_centers, n_patches)
@@ -231,71 +223,76 @@
         # create file backend
         self.catalog_factory = NewCatalog(backend)
         self._reference: dict[str, Input | None] = dict(data=None, rand=None)
         self._unknown: dict[str, BinnedInput | None] = dict(data=None, rand=None)
 
     @staticmethod
     def _raise_n_patch_mismatch(
-        centers: Sequence |  None,
-        n_patches: int | None
+        centers: Sequence | None, n_patches: int | None
     ) -> None:
         if centers is not None and n_patches is not None:
             if len(centers) != n_patches:
                 raise InputConfigError(
-                    f"got {len(centers)} patch centers but {n_patches=}")
+                    f"got {len(centers)} patch centers but {n_patches=}"
+                )
 
     @classmethod
     def from_dict(
-        cls,
-        the_dict: dict[str, dict],
-        patch_centers: Coordinate | None = None
+        cls, the_dict: dict[str, dict], patch_centers: Coordinate | None = None
     ) -> InputManager:
         inputs = {k: v for k, v in the_dict.items()}
         # parse optional parameters
         new = cls(
             cachepath=inputs.pop("cachepath"),
             patch_centers=patch_centers,
             n_patches=inputs.pop("n_patches", None),
-            backend=inputs.pop("backend", DEFAULT.backend))
+            backend=inputs.pop("backend", DEFAULT.backend),
+        )
         # parse reference
         new._reference = _parse_catalog_dict(
-            inputs.pop("reference", dict()),
-            section="reference", binned=False)
+            inputs.pop("reference", dict()), section="reference", binned=False
+        )
         for kind, data in new._reference.items():
             if isinstance(data, BinnedInput):
                 raise InputConfigError(
                     "binned reference cataloge not permitted, in "
-                    f"'reference:{kind}:filepath'")
+                    f"'reference:{kind}:filepath'"
+                )
         # parse unknown
         new._unknown = _parse_catalog_dict(
-            inputs.pop("unknown", dict()),
-            section="unknown", binned=True)
+            inputs.pop("unknown", dict()), section="unknown", binned=True
+        )
         # check that there are no extra sections
         if len(inputs) > 0:
             key = next(iter(inputs.keys()))
             raise InputConfigError(
                 f"encountered unknown section '{key}', "
-                "must be 'reference' or 'unknown'")
+                "must be 'reference' or 'unknown'"
+            )
         return new
 
     def to_dict(self) -> dict[str, Any]:
         inputs = dict()
         if self.n_patches is not None:
             inputs["n_patches"] = self.n_patches
         inputs["cachepath"] = str(self._cachepath)
         inputs["backend"] = self.catalog_factory.backend_name
         # parse the input files, omit empty sections
         ref = {
             kind: inp.to_dict()
-            for kind, inp in self._reference.items() if inp is not None}
+            for kind, inp in self._reference.items()
+            if inp is not None
+        }
         if len(ref) > 0:
             inputs["reference"] = ref
         unk = {
             kind: inp.to_dict()
-            for kind, inp in self._unknown.items() if inp is not None}
+            for kind, inp in self._unknown.items()
+            if inp is not None
+        }
         if len(unk) > 0:
             inputs["unknown"] = unk
         return inputs
 
     def centers_from_file(self, fpath: TypePathStr) -> None:
         logger.debug("restoring patch centers")
         centers = np.loadtxt(str(fpath))
@@ -312,16 +309,18 @@
             line = delim.join(f"{h:>{PREC}s}" for h in header)
             f.write(f"# {line[2:]}\n")
 
         if self._centers is None:
             raise InputConfigError("patch centers undetermined")
         with open(str(fpath), "w") as f:
             write_head(
-                f, f"# {len(self._centers)} patch centers in sky coordinates",
-                ["ra", "dec"])
+                f,
+                f"# {len(self._centers)} patch centers in sky coordinates",
+                ["ra", "dec"],
+            )
             for coord in self.patch_centers:
                 ra, dec = coord.ra[0], coord.dec[0]
                 f.write(f"{fmt_num(ra, PREC)}{DELIM}{fmt_num(dec, PREC)}\n")
 
     @property
     def n_patches(self) -> int | None:
         return self._n_patches
@@ -358,52 +357,46 @@
             if hasattr(cat, "n_bins"):
                 n_bins.append(cat.n_bins)
         return max(n_bins)
 
     def _check_patch_definition(self, catalog: Input) -> None:
         if catalog.patches is None and self.external_patches:
             raise InputConfigError(
-                "'n_patches' not set and no patch index column provided")
+                "'n_patches' not set and no patch index column provided"
+            )
         elif catalog.patches is not None and not self.external_patches:
             raise InputConfigError(
-                "'n_patches' and catalog 'patches' are mutually exclusive")
+                "'n_patches' and catalog 'patches' are mutually exclusive"
+            )
 
-    def set_reference(
-        self,
-        data: Input,
-        rand: Input | None = None
-    ) -> None:
+    def set_reference(self, data: Input, rand: Input | None = None) -> None:
         logger.debug(f"registering reference data catalog '{data.filepath}'")
         self._check_patch_definition(data)
         self._reference["data"] = data
         if rand is not None:
             self._check_patch_definition(rand)
             self._reference["rand"] = rand
-    
-    def add_unknown(
-        self,
-        bin_idx: int,
-        data: Input,
-        rand: Input | None = None
-    ) -> None:
+
+    def add_unknown(self, bin_idx: int, data: Input, rand: Input | None = None) -> None:
         logger.debug(
-            f"registering unknown bin {bin_idx} data catalog "
-            f"'{data.filepath}'")
+            f"registering unknown bin {bin_idx} data catalog '{data.filepath}'"
+        )
         # make sure the bin indices will remain aligned
         if self._unknown["rand"] is not None and rand is None:
             raise ValueError(
-                "unknown randoms exist but no randoms for current bin provided")
+                "unknown randoms exist but no randoms for current bin provided"
+            )
         elif (
-            self._unknown["data"] is not None and
-            self._unknown["rand"] is None and
-            rand is not None
+            self._unknown["data"] is not None
+            and self._unknown["rand"] is None
+            and rand is not None
         ):
             raise ValueError(
-                "no previous randoms configured, cannot add randoms for "
-                "current bin")
+                "no previous randoms configured, cannot add randoms for current bin"
+            )
         # set the data
         for key, value in zip(["data", "rand"], [data, rand]):
             if value is None:
                 continue
             self._check_patch_definition(value)
             if self._unknown[key] is None:
                 self._unknown[key] = BinnedInput.from_inputs({bin_idx: value})
@@ -434,19 +427,15 @@
     def get_bin_indices(self) -> set[int]:
         for inputs in self._unknown.values():
             if inputs is not None:
                 return inputs.get_bin_indices()
         return set()
 
     def _load_catalog(
-        self,
-        sample: str,
-        kind: str,
-        bin_idx: int | None = None,
-        progress: bool = False
+        self, sample: str, kind: str, bin_idx: int | None = None, progress: bool = False
     ) -> BaseCatalog:
         # get the correct sample type
         if sample == "reference":
             inputs = self.get_reference()
         elif sample == "unknown":
             if bin_idx is None:
                 raise ValueError("no 'bin_idx' provided")
@@ -458,16 +447,15 @@
             input = inputs[kind]
         except KeyError as e:
             raise ValueError("'kind' must be either of 'data'/'rand'") from e
         if input is None:
             if kind == "rand":
                 kind = "random"
             bin_info = f" bin {bin_idx} " if bin_idx is not None else " "
-            raise MissingCatalogError(
-                f"no {sample} {kind}{bin_info}catalog specified")
+            raise MissingCatalogError(f"no {sample} {kind}{bin_info}catalog specified")
 
         # determine the correct cache path to use
         if sample == "reference":
             cachepath = self.get_cache().get_reference()[kind]
         else:
             cachepath = self.get_cache().get_unknown(bin_idx)[kind]
 
@@ -495,26 +483,19 @@
             catalog = self.catalog_factory.from_file(**load_kwargs)
             # store patch centers for consecutive loads
             if self._centers is None:
                 self._centers = catalog.centers
 
         return catalog
 
-    def load_reference(
-            self,
-        kind: str,
-        progress: bool = False
-    ) -> BaseCatalog:
-        logger.info(
-            f"loading reference {'random' if kind == 'rand' else kind} catalog")
+    def load_reference(self, kind: str, progress: bool = False) -> BaseCatalog:
+        logger.info(f"loading reference {'random' if kind == 'rand' else kind} catalog")
         return self._load_catalog("reference", kind, progress=progress)
 
     def load_unknown(
-        self,
-        kind: str,
-        bin_idx: int,
-        progress: bool = False
+        self, kind: str, bin_idx: int, progress: bool = False
     ) -> BaseCatalog:
         logger.info(
             f"loading unknown bin {bin_idx} "
-            f"{'random' if kind == 'rand' else kind} catalog")
+            f"{'random' if kind == 'rand' else kind} catalog"
+        )
         return self._load_catalog("unknown", kind, bin_idx, progress=progress)
```

### Comparing `yet_another_wizz-2.5/src/yaw_cli/pipeline/default_setup.py` & `yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/default_setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,128 +1,212 @@
 from __future__ import annotations
 
 import textwrap
 
 from yaw import config
 from yaw.core.docs import get_doc_args
-
 from yaw_cli.pipeline import tasks
 
-
 WIDTH = 100
 TAB = "    "
 DASH = "  - "
 COMM_PAD = 24
 COMM_SEP = "# "
 
 
 def wrap_comment(text, indents=0, initial="", subsequent=""):
     if isinstance(indents, str):
-        indent = indents +  COMM_SEP
+        indent = indents + COMM_SEP
     else:
         indent = (TAB * indents) + COMM_SEP
-    return "\n".join(textwrap.wrap(
-        text, width=int(0.7*WIDTH),
-        initial_indent=indent+initial, subsequent_indent=indent+subsequent)
-    ) + "\n"
+    return (
+        "\n".join(
+            textwrap.wrap(
+                text,
+                width=int(0.7 * WIDTH),
+                initial_indent=indent + initial,
+                subsequent_indent=indent + subsequent,
+            )
+        )
+        + "\n"
+    )
 
 
 def format_line(text, comment, indents=0):
     if isinstance(indents, str):
         indent = indents
     else:
-        indent = (TAB * indents)
+        indent = TAB * indents
     initial = indent + f"{text:{COMM_PAD}s}" + COMM_SEP
-    subsequent = (" " *len(indent)) + (" " * COMM_PAD) + COMM_SEP
-    return "\n".join(textwrap.wrap(
-        comment, width=WIDTH,
-        initial_indent=initial, subsequent_indent=subsequent)
-    ) + "\n"
+    subsequent = (" " * len(indent)) + (" " * COMM_PAD) + COMM_SEP
+    return (
+        "\n".join(
+            textwrap.wrap(
+                comment,
+                width=WIDTH,
+                initial_indent=initial,
+                subsequent_indent=subsequent,
+            )
+        )
+        + "\n"
+    )
 
 
 def make_doc(dclass: object | type, indent=1, indicate_opt: bool = True) -> str:
     doc = ""
     for value, comment in get_doc_args(dclass, indicate_opt):
         string = TAB * indent
         string += f"{value:{COMM_PAD}s}"
         if comment is not None:
             lines = textwrap.wrap(
-                comment, width=WIDTH,
-                initial_indent=string+COMM_SEP,
-                subsequent_indent=" "*len(string)+COMM_SEP)
+                comment,
+                width=WIDTH,
+                initial_indent=string + COMM_SEP,
+                subsequent_indent=" " * len(string) + COMM_SEP,
+            )
             string = "\n".join(lines)
         doc += string + "\n"
     return doc
 
 
 setup_default = wrap_comment("yet_another_wizz setup configuration")
 setup_default += "\n"
-setup_default += wrap_comment("NOTE: (opt) in commment indicates entries that may be omitted.")
+setup_default += wrap_comment(
+    "NOTE: (opt) in commment indicates entries that may be omitted."
+)
 
 # configuration
 setup_default += "\n"
-setup_default += wrap_comment("This section configures the correlation measurements and redshift binning of the clustering redshift estimates.")
+setup_default += wrap_comment(
+    "This section configures the correlation measurements and redshift binning of the clustering redshift estimates."
+)
 setup_default += "configuration:\n"
 
 setup_default += format_line("backend:", "(opt) backend specific parameters", indents=1)
 setup_default += make_doc(config.BackendConfig, indent=2)
 
-setup_default += format_line("binning:", "specify the redshift binning for the clustering redshifts", indents=1)
+setup_default += format_line(
+    "binning:", "specify the redshift binning for the clustering redshifts", indents=1
+)
 setup_default += make_doc(config.AutoBinningConfig, indent=2)
 setup_default += make_doc(config.ManualBinningConfig, indent=2)
 
-setup_default += format_line("scales:", "specify the correlation measurement scales", indents=1)
+setup_default += format_line(
+    "scales:", "specify the correlation measurement scales", indents=1
+)
 setup_default += make_doc(config.ScalesConfig, indent=2)
 
 setup_default += make_doc(config.Configuration, indent=1)
 
 # data
 setup_default += "\n"
-setup_default += wrap_comment("This section defines the input data products and their meta data. These can be FITS, PARQUET, CSV or FEATHER files.")
+setup_default += wrap_comment(
+    "This section defines the input data products and their meta data. These can be FITS, PARQUET, CSV or FEATHER files."
+)
 setup_default += "data:\n"
 
-setup_default += format_line("backend: scipy", f"(opt) name of the data catalog backend ({', '.join(config.OPTIONS.backend)})", indents=1)
-setup_default += format_line("cachepath: null", "(opt) cache directory path, e.g. on fast storage device (recommended for 'backend=scipy', default is within project directory)", indents=1)
-setup_default += format_line("n_patches: null", "(opt) number of automatic spatial patches to use for input catalogs below, provide only if no 'data/rand.patches' provided", indents=1)
+setup_default += format_line(
+    "backend: scipy",
+    f"(opt) name of the data catalog backend ({', '.join(config.OPTIONS.backend)})",
+    indents=1,
+)
+setup_default += format_line(
+    "cachepath: null",
+    "(opt) cache directory path, e.g. on fast storage device (recommended for 'backend=scipy', default is within project directory)",
+    indents=1,
+)
+setup_default += format_line(
+    "n_patches: null",
+    "(opt) number of automatic spatial patches to use for input catalogs below, provide only if no 'data/rand.patches' provided",
+    indents=1,
+)
 
 level = 1
-setup_default += format_line("reference:", "(opt) reference data sample with know redshifts", indents=level)
+setup_default += format_line(
+    "reference:", "(opt) reference data sample with know redshifts", indents=level
+)
 level += 1
-setup_default += format_line("data:" , "data catalog file and column names", indents=level)
+setup_default += format_line(
+    "data:", "data catalog file and column names", indents=level
+)
 level += 1
 setup_default += format_line("filepath: ...", "input file path", indents=level)
 setup_default += format_line("ra: ra", "right ascension in degrees", indents=level)
 setup_default += format_line("dec: dec", "declination in degrees", indents=level)
-setup_default += format_line("redshift: z", "redshift of objects (required)", indents=level)
-setup_default += format_line("patches: patch", "(opt) integer index for patch assignment, couting from 0...N-1", indents=level)
+setup_default += format_line(
+    "redshift: z", "redshift of objects (required)", indents=level
+)
+setup_default += format_line(
+    "patches: patch",
+    "(opt) integer index for patch assignment, couting from 0...N-1",
+    indents=level,
+)
 setup_default += format_line("weight: weight", "(opt) object weight", indents=level)
-setup_default += format_line("cache: false", "(opt) whether to cache the file in the cache directory", indents=level)
+setup_default += format_line(
+    "cache: false",
+    "(opt) whether to cache the file in the cache directory",
+    indents=level,
+)
 level -= 1
-setup_default += format_line("rand: null", "random catalog for data sample, omit or repeat arguments from 'data' above", indents=level)
+setup_default += format_line(
+    "rand: null",
+    "random catalog for data sample, omit or repeat arguments from 'data' above",
+    indents=level,
+)
 
 level = 1
-setup_default += format_line("unknown:", "(opt) unknown data sample for which clustering redshifts are estimated, typically in tomographic redshift bins, see below", indents=level)
+setup_default += format_line(
+    "unknown:",
+    "(opt) unknown data sample for which clustering redshifts are estimated, typically in tomographic redshift bins, see below",
+    indents=level,
+)
 level += 1
-setup_default += format_line("data:", "data catalog file and column names", indents=level)
+setup_default += format_line(
+    "data:", "data catalog file and column names", indents=level
+)
 level += 1
-setup_default += format_line("filepath:", "either a single file path (no tomographic bins) or a mapping of integer bin index to file path (as shown below)", indents=2)
-setup_default += format_line("1: ...", "bin 1", indents=level+1)
-setup_default += format_line("2: ...", "bin 2", indents=level+1)
+setup_default += format_line(
+    "filepath:",
+    "either a single file path (no tomographic bins) or a mapping of integer bin index to file path (as shown below)",
+    indents=2,
+)
+setup_default += format_line("1: ...", "bin 1", indents=level + 1)
+setup_default += format_line("2: ...", "bin 2", indents=level + 1)
 setup_default += format_line("ra: ra", "right ascension in degrees", indents=level)
 setup_default += format_line("dec: dec", "declination in degrees", indents=level)
-setup_default += format_line("redshift: z", "(opt) redshift of objects, if provided, enables computing the autocorrelation of the unknown sample", indents=level)
-setup_default += format_line("patches: patch", "(opt) integer index for patch assignment, couting from 0...N-1", indents=level)
+setup_default += format_line(
+    "redshift: z",
+    "(opt) redshift of objects, if provided, enables computing the autocorrelation of the unknown sample",
+    indents=level,
+)
+setup_default += format_line(
+    "patches: patch",
+    "(opt) integer index for patch assignment, couting from 0...N-1",
+    indents=level,
+)
 setup_default += format_line("weight: weight", "(opt) object weight", indents=level)
-setup_default += format_line("cache: false", "(opt) whether to cache the file in the cache directory", indents=level)
+setup_default += format_line(
+    "cache: false",
+    "(opt) whether to cache the file in the cache directory",
+    indents=level,
+)
 level -= 1
-setup_default += format_line("rand: null", "random catalog for data sample, omit or repeat arguments from 'data' above ('filepath' format must must match 'data' above)", indents=level)
+setup_default += format_line(
+    "rand: null",
+    "random catalog for data sample, omit or repeat arguments from 'data' above ('filepath' format must must match 'data' above)",
+    indents=level,
+)
 
 # tasks
 setup_default += "\n"
-setup_default += wrap_comment("The section below is entirely optional and used to specify tasks to execute when using the 'yaw_cli run' command. The list is generated and updated automatically when running 'yaw_cli' subcommands. Tasks can be provided as single list entry, e.g.")
+setup_default += wrap_comment(
+    "The section below is entirely optional and used to specify tasks to execute when using the 'yaw_cli run' command. The list is generated and updated automatically when running 'yaw_cli' subcommands. Tasks can be provided as single list entry, e.g."
+)
 setup_default += f"{COMM_SEP}  - cross\n{COMM_SEP}  - zcc\n"
-setup_default += wrap_comment("to get a basic cluster redshift estimate or with the optional parameters listed below (all values optional, defaults listed).")
+setup_default += wrap_comment(
+    "to get a basic cluster redshift estimate or with the optional parameters listed below (all values optional, defaults listed)."
+)
 setup_default += "tasks:\n"
 for task in tasks.Task.all_tasks():
     setup_default += format_line(task.get_name(), task.get_help(), indents=DASH)
     setup_default += make_doc(task, indent=2, indicate_opt=False)
 setup_default = setup_default.strip("\n")
```

### Comparing `yet_another_wizz-2.5/src/yaw_cli/pipeline/directories.py` & `yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/directories.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,71 +7,70 @@
 from abc import ABC, abstractmethod, abstractproperty
 from collections.abc import Iterator
 from pathlib import Path, _posix_flavour, _windows_flavour
 from typing import Any
 
 from yaw.core.utils import bytes_format
 
-
 logger = logging.getLogger(__name__)
 
 
 def _get_numeric_suffix(path: Path) -> int:
     base = path.with_suffix(suffix="").name
     _, num = base.rsplit("_", 1)
     return int(num)
 
 
 class Directory(Path):
-
     # seems to be the easiest way to subclass pathlib.Path
-    _flavour = _windows_flavour if os.name == 'nt' else _posix_flavour
+    _flavour = _windows_flavour if os.name == "nt" else _posix_flavour
 
     def print_contents(self) -> None:
         sizes = dict()
         for path in self.iterdir():
             if path.is_dir():
-                sizes[path.name] = ("d", sum(
-                    file.stat().st_size for file in path.rglob("*")))
+                sizes[path.name] = (
+                    "d",
+                    sum(file.stat().st_size for file in path.rglob("*")),
+                )
             else:
                 sizes[path.name] = ("f", path.stat().st_size)
         print(f"cache path: {self}")
         if len(sizes) == 0:
             width = 10
             total = bytes_format(0)
         else:
             width = min(30, max(len(name) for name in sizes))
             for i, name in enumerate(sorted(sizes), 1):
-                print_name = textwrap.shorten(
-                    name, width=width, placeholder="...")
+                print_name = textwrap.shorten(name, width=width, placeholder="...")
                 kind, bytes = sizes[name]
                 bytes_fmt = bytes_format(bytes)
                 print(f"{kind}> {print_name:{width}s}{bytes_fmt:>10s}")
             total = bytes_format(sum(b for _, b in sizes.values()))
         print("-" * (width + 13))
         print(f"{'total':{width+3}s}{total:>10s}")
 
 
 class CacheDirectory(Directory):
-
     def _generate_filenames(self, base: str) -> dict[str, Path]:
         tags = ("data", "rand")
         return {tag: Path(self.joinpath(f"{base}.{tag}")) for tag in tags}
 
     def get_reference(self) -> dict[str, Path]:
         return self._generate_filenames("reference")
 
     def get_unknown(self, bin_idx: int) -> dict[str, Path]:
         return self._generate_filenames(f"unknown_{bin_idx}")
 
     def get_bin_indices(self) -> set[int]:
         return set(
             _get_numeric_suffix(path)
             for path in self.iterdir()
-            if path.name.startswith("unknown"))
+            if path.name.startswith("unknown")
+        )
 
     def drop(self, name: str) -> None:
         logger.debug(f"dropping cache '{name}'")
         path = self.joinpath(name)
         if path.is_dir():
             shutil.rmtree(str(path))
         else:
@@ -80,68 +79,75 @@
     def drop_all(self) -> None:
         logger.info("dropping cached data")
         for path in self.iterdir():
             self.drop(path.name)
 
 
 class DataDirectory(Directory, ABC):
-
     @abstractproperty
-    def _auto_reference_prefix(self) -> str: pass
+    def _auto_reference_prefix(self) -> str:
+        pass
 
     @abstractproperty
-    def _cross_prefix(self) -> str: pass
+    def _cross_prefix(self) -> str:
+        pass
 
     @abstractproperty
-    def _auto_prefix(self) -> str: pass
+    def _auto_prefix(self) -> str:
+        pass
 
     @abstractmethod
-    def get_auto_reference(self) -> Path: pass
+    def get_auto_reference(self) -> Path:
+        pass
 
     @property
     def has_auto_reference(self) -> bool:
         try:
             next(self.glob(self._auto_reference_prefix + "*"))
             return True
         except StopIteration:
             return False
 
     @abstractmethod
-    def get_auto(self, bin_idx: int) -> Path: pass
+    def get_auto(self, bin_idx: int) -> Path:
+        pass
 
     @property
     def has_auto(self) -> bool:
         try:
             next(self.glob(self._auto_prefix + "*"))
             return True
         except StopIteration:
             return False
 
     @abstractmethod
-    def get_cross(self, bin_idx: int) -> Path: pass
+    def get_cross(self, bin_idx: int) -> Path:
+        pass
 
     @property
     def has_cross(self) -> bool:
         try:
             next(self.glob(self._cross_prefix + "*"))
             return True
         except StopIteration:
             return False
 
     def get_cross_indices(self) -> set[int]:
         return set(
             _get_numeric_suffix(path)
             for path in self.iterdir()
-            if path.name.startswith(self._cross_prefix))
+            if path.name.startswith(self._cross_prefix)
+        )
 
     def get_auto_indices(self) -> set[int]:
         return set(
             _get_numeric_suffix(path)
             for path in self.iterdir()
-            if path.name.startswith(self._auto_prefix))
+            if path.name.startswith(self._auto_prefix)
+        )
 
     def iter_cross(self) -> Iterator[tuple[int, Any]]:
         for idx in sorted(self.get_cross_indices()):
             yield idx, self.get_cross(idx)
 
     def iter_auto(self) -> Iterator[tuple[int, Any]]:
         for idx in sorted(self.get_auto_indices()):
@@ -149,15 +155,14 @@
 
     def iter_bins(self) -> Iterator[tuple[int, tuple[Any, Any]]]:
         for idx in sorted(self.get_cross_indices() | self.get_auto_indices()):
             yield idx, self.get_cross(idx), self.get_auto(idx)
 
 
 class CountsDirectory(DataDirectory):
-
     _auto_reference_prefix = "auto_reference"
     _cross_prefix = "cross"
     _auto_prefix = "auto_unknown"
 
     def get_auto_reference(self) -> Path:
         return Path(self.joinpath(f"{self._auto_reference_prefix}.hdf"))
 
@@ -165,15 +170,14 @@
         return Path(self.joinpath(f"{self._auto_prefix}_{bin_idx}.hdf"))
 
     def get_cross(self, bin_idx: int) -> Path:
         return Path(self.joinpath(f"{self._cross_prefix}_{bin_idx}.hdf"))
 
 
 class EstimateDirectory(DataDirectory):
-
     _auto_reference_prefix = "auto_reference"
     _cross_prefix = "nz_cc"
     _auto_prefix = "auto_unknown"
 
     def get_auto_reference(self) -> Path:
         return Path(self.joinpath(self._auto_reference_prefix))
 
@@ -181,15 +185,14 @@
         return Path(self.joinpath(f"{self._auto_prefix}_{bin_idx}"))
 
     def get_cross(self, bin_idx: int) -> Path:
         return Path(self.joinpath(f"{self._cross_prefix}_{bin_idx}"))
 
 
 class TrueDirectory(Directory):
-
     _auto_reference_prefix = "nz_reference"
     _true_prefix = "nz_true"
 
     @property
     def has_reference(self) -> bool:
         try:
             next(self.glob(self._auto_reference_prefix + "*"))
@@ -211,12 +214,13 @@
     def get_unknown(self, bin_idx: int) -> Path:
         return Path(self.joinpath(f"{self._true_prefix}_{bin_idx}"))
 
     def get_bin_indices(self) -> set[int]:
         return set(
             _get_numeric_suffix(path)
             for path in self.iterdir()
-            if path.name.startswith(self._true_prefix))
+            if path.name.startswith(self._true_prefix)
+        )
 
     def iter_bins(self) -> Iterator[tuple[int, Path]]:
         for idx in sorted(self.get_bin_indices()):
             yield idx, self.get_unknown(idx)
```

### Comparing `yet_another_wizz-2.5/src/yaw_cli/pipeline/logger.py` & `yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,32 +3,33 @@
 import logging
 import os
 import sys
 
 
 def term_supports_color() -> bool:
     plat = sys.platform
-    supported = (
-        plat != "Pocket PC" and
-        (plat != "win32" or "ANSICON" in os.environ))
+    supported = plat != "Pocket PC" and (plat != "win32" or "ANSICON" in os.environ)
     isatty = hasattr(sys.stdout, "isatty") and sys.stdout.isatty()
     return supported and isatty
 
 
 if term_supports_color():
+
     class Colors:
         sep = "|"
         gry = "\033[2m"
         bld = "\033[1m"
         blu = "\033[1;34m"
         grn = "\033[1;32m"
         ylw = "\033[1;33m"
         red = "\033[1;31m"
         rst = "\033[0m"
+
 else:
+
     class Colors:
         sep = "|"
         gry = ""
         bld = ""
         blu = ""
         grn = ""
         ylw = ""
@@ -40,41 +41,39 @@
     def filter(self, record):
         record.exc_info = None
         record.exc_text = None
         return "yaw" in record.name
 
 
 class CustomFormatter(logging.Formatter):
-
     level = "%(levelname).3s"
     msg = "%(message)s"
     FORMATS = {
         logging.DEBUG: f"{Colors.gry}DBG {Colors.sep} {msg}{Colors.rst}",
         logging.INFO: f"INF {Colors.sep} {msg}",
         logging.WARNING: f"{Colors.ylw}WRN {Colors.sep} {msg}{Colors.rst}",
         logging.ERROR: f"{Colors.red}ERR {Colors.sep} {msg}{Colors.rst}",
-        logging.CRITICAL: f"{Colors.red}CRT {Colors.sep} {msg}{Colors.rst}"}
+        logging.CRITICAL: f"{Colors.red}CRT {Colors.sep} {msg}{Colors.rst}",
+    }
 
     def format(self, record):
         log_fmt = self.FORMATS.get(record.levelno, self.FORMATS[logging.INFO])
         formatter = logging.Formatter(log_fmt)
         return formatter.format(record)
 
 
 def print_yaw_message(msg: str, color: str = Colors.blu) -> None:
     print(f"{color}YAW {Colors.sep} {msg}{Colors.rst}")
 
+
 def get_logger() -> logging.Logger:
     return logging.getLogger("yaw")
 
 
-def init_logger(
-    level: str = "info",
-    plain: bool = True
-) -> logging.Logger:
+def init_logger(level: str = "info", plain: bool = True) -> logging.Logger:
     level = getattr(logging, level.upper())
     handler = logging.StreamHandler(sys.stdout)
     if plain:
         handler.setFormatter(CustomFormatter())
     else:
         format = "%(levelname)s:%(name)s:%(message)s"
         handler.setFormatter(logging.Formatter(format))
```

### Comparing `yet_another_wizz-2.5/src/yaw_cli/pipeline/merge.py` & `yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/merge.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 from __future__ import annotations
 
 import logging
-from collections.abc import Iterable
+from collections.abc import Iterable, Sequence
 from itertools import groupby
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 import numpy as np
 import pandas as pd
 
-from collections.abc import Sequence
-
-from yaw.config import (
-    Configuration, ManualBinningConfig, ScalesConfig,
-    default as DEFAULT, OPTIONS)
+from yaw.config import OPTIONS, Configuration, ManualBinningConfig, ScalesConfig
+from yaw.config import default as DEFAULT
 from yaw.core.utils import TypePathStr
 from yaw.correlation import CorrFunc
 from yaw.redshifts import HistData
-
 from yaw_cli.pipeline.project import (
-    ProjectDirectory, ProjectState, YawDirectory, compress_config)
+    ProjectDirectory,
+    ProjectState,
+    YawDirectory,
+    compress_config,
+)
 from yaw_cli.pipeline.tasks import MergedTask, Task, TaskError, TaskManager
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import NDArray
-    from yaw_cli.pipeline.project import YawDirectory
 
 
 logger = logging.getLogger(__name__)
 
 
 class MergeError(Exception):
     pass
@@ -36,16 +35,15 @@
 
 def all_equal(iterable: Iterable) -> bool:
     g = groupby(iterable)
     return next(g, True) and not next(g, False)
 
 
 def merge_config(
-    projects: Sequence[YawDirectory],
-    merge_binning: bool = True
+    projects: Sequence[YawDirectory], merge_binning: bool = True
 ) -> Configuration:
     if len(projects) == 0:
         raise ValueError("'projects' is an empty sequence")
 
     # check configurations match
     if not all_equal(p.config.cosmology for p in projects):
         raise MergeError("cosmological models do not match")
@@ -88,38 +86,37 @@
         bin_config = config.binning  # all identical
 
     config = Configuration(
         scales=ScalesConfig(
             rmin=[r for r, _ in common],
             rmax=[r for _, r in common],
             rweight=config.scales.rweight,
-            rbin_num=config.scales.rbin_num),
+            rbin_num=config.scales.rbin_num,
+        ),
         binning=bin_config,
-        cosmology=config.cosmology)
+        cosmology=config.cosmology,
+    )
     return config
 
 
 def get_common_bins(projects: Sequence[YawDirectory]) -> set[int]:
     bin_sets = []
     for project in projects:
         bin_sets.append(project.get_bin_indices())
     common = set.intersection(*bin_sets)
     if len(common) == 0:
         MergeError("found no common bins")
     extra = set.union(*bin_sets) - common
     if len(extra) > 0:
-        logger.warn(
-            f"ignoring uncommon bins: {', '.join(str(b) for b in extra)}")
+        logger.warn(f"ignoring uncommon bins: {', '.join(str(b) for b in extra)}")
     return common
 
 
 def merge_state_attr(
-    states: Iterable[ProjectState],
-    attr: str,
-    require: bool = False
+    states: Iterable[ProjectState], attr: str, require: bool = False
 ) -> bool:
     attr_states = [getattr(state, attr) for state in states]
     attr_state = all(attr_states)
     if require and not attr_state and any(attr_states):
         raise MergeError(f"state attribute '{attr}' differs for some cases")
     return attr_state
 
@@ -148,96 +145,88 @@
         logger.warn("ignoring uncommon true redshift distributions")
     try:
         has_nz_ref = merge_state_attr(states, "has_nz_ref", require=True)
     except MergeError:
         has_nz_ref = False
         logger.warn("ignoring uncommon reference sample redshift distributions")
     return ProjectState(
-        has_w_ss=has_w_ss, has_w_pp=has_w_pp, has_w_sp=has_w_sp,
-        has_nz_true=has_nz_true, has_nz_ref=has_nz_ref)
+        has_w_ss=has_w_ss,
+        has_w_pp=has_w_pp,
+        has_w_sp=has_w_sp,
+        has_nz_true=has_nz_true,
+        has_nz_ref=has_nz_ref,
+    )
 
 
-def merge_cfs(
-    mode: str,
-    cfs: Sequence[CorrFunc]
-) -> CorrFunc:
+def merge_cfs(mode: str, cfs: Sequence[CorrFunc]) -> CorrFunc:
     cfs_ordered = sorted(cfs, key=lambda cf: cf.edges[0])
     if mode == "redshift":
         return cfs_ordered[0].concatenate_bins(*cfs_ordered[1:])
     else:
         return cfs_ordered[0].concatenate_patches(*cfs_ordered[1:])
 
 
 def merge_hists(
-    mode: str,
-    bin_edges: NDArray[np.float_],
-    hists: Sequence[HistData]
+    mode: str, bin_edges: NDArray[np.float_], hists: Sequence[HistData]
 ) -> HistData:
     methods = [hist.method for hist in hists]
     if all_equal(methods):
         method = methods[0]
     else:
-        raise MergeError(
-            "cannot merge histograms with different resampling methods")
+        raise MergeError("cannot merge histograms with different resampling methods")
 
     densities = [hist.density for hist in hists]
     if any(densities):
         raise MergeError("cannot merge normalised histograms with")
 
     hists_ordered = sorted(hists, key=lambda hist: hist.edges[0])
     if mode == "redshift":
         return HistData(
             binning=pd.IntervalIndex.from_breaks(bin_edges),
             data=np.concatenate([hist.data for hist in hists_ordered]),
-            samples=np.concatenate([
-                hist.samples for hist in hists_ordered], axis=1),
-            method=method)
+            samples=np.concatenate([hist.samples for hist in hists_ordered], axis=1),
+            method=method,
+        )
     else:
         return HistData(
             binning=pd.IntervalIndex.from_breaks(bin_edges),
             data=np.sum([hist.data for hist in hists], axis=0),
             samples=np.sum([hist.samples for hist in hists], axis=1),
-            method=method)
+            method=method,
+        )
 
 
 def open_yaw_directory(path: TypePathStr) -> ProjectDirectory | MergedDirectory:
     if Path(path).joinpath("merged.yaml").exists():
         return MergedDirectory(path)
     else:
         return ProjectDirectory(path)
 
 
 class MergedManager(TaskManager):
-
     def _insert_task(self, task: MergedTask, task_list: list[Task]) -> None:
         if not isinstance(task, MergedTask):
             raise TaskError(
-                f"task '{task.get_name()}' cannot be executed after merging")
+                f"task '{task.get_name()}' cannot be executed after merging"
+            )
         return super()._insert_task(task, task_list)
 
     def schedule(self, task: MergedTask) -> None:
         return super().schedule(task)
 
     def run(
-        self,
-        task: MergedTask,
-        progress: bool = False,
-        threads: int | None = None
+        self, task: MergedTask, progress: bool = False, threads: int | None = None
     ) -> None:
         return super().run(task, progress, threads)
 
 
 class MergedDirectory(YawDirectory):
-
     @classmethod
     def from_projects(
-        cls,
-        path: TypePathStr,
-        inputs: Sequence[TypePathStr],
-        mode: str
+        cls, path: TypePathStr, inputs: Sequence[TypePathStr], mode: str
     ) -> MergedDirectory:
         logger.info(f"merging {len(inputs)} project directories")
         projects: list[YawDirectory] = []
         for project in inputs:
             projects.append(open_yaw_directory(project))
 
         # check and merge configurations
@@ -250,63 +239,85 @@
         merged_state = get_merged_state(projects)
         bins = get_common_bins(projects)
 
         # create output
         setup = dict(
             configuration=config.to_dict(),
             sources=[str(path) for path in inputs],
-            tasks=[])
+            tasks=[],
+        )
         merged = cls.from_dict(setup, path)
 
         # merge and write the pair counts files
         for scale, counts_dir in merged.iter_counts(create=True):
             logmsg = f"merging {{:}} for scale '{scale}'"
-            project_counts_dir = [
-                    project.get_counts_dir(scale) for project in projects]
+            project_counts_dir = [project.get_counts_dir(scale) for project in projects]
             if merged_state.has_w_ss:
                 logger.info(logmsg.format("reference autocorrelation function"))
-                cf = merge_cfs(mode, [
-                    CorrFunc.from_file(cdir.get_auto_reference())
-                    for cdir in project_counts_dir])
+                cf = merge_cfs(
+                    mode,
+                    [
+                        CorrFunc.from_file(cdir.get_auto_reference())
+                        for cdir in project_counts_dir
+                    ],
+                )
                 cf.to_file(counts_dir.get_auto_reference())
             if merged_state.has_w_sp:
                 logger.info(logmsg.format("unknown autocorrelation functions"))
                 for bin_idx in bins:
-                    cf = merge_cfs(mode, [
-                        CorrFunc.from_file(cdir.get_cross(bin_idx))
-                        for cdir in project_counts_dir])
+                    cf = merge_cfs(
+                        mode,
+                        [
+                            CorrFunc.from_file(cdir.get_cross(bin_idx))
+                            for cdir in project_counts_dir
+                        ],
+                    )
                     cf.to_file(counts_dir.get_cross(bin_idx))
             if merged_state.has_w_pp:
                 logger.info(logmsg.format("crosscorrelation functions"))
                 for bin_idx in bins:
-                    cf = merge_cfs(mode, [
-                        CorrFunc.from_file(cdir.get_auto(bin_idx))
-                        for cdir in project_counts_dir])
+                    cf = merge_cfs(
+                        mode,
+                        [
+                            CorrFunc.from_file(cdir.get_auto(bin_idx))
+                            for cdir in project_counts_dir
+                        ],
+                    )
                     cf.to_file(counts_dir.get_auto(bin_idx))
 
         # merge the reference sample redshift distribution
         true_dir = merged.get_true_dir()
         project_true_dir = [project.get_true_dir() for project in projects]
         if merged_state.has_nz_ref:
             logger.info("merging reference sample redshift distribution")
             try:
-                hist = merge_hists(mode, config.binning.zbins, [
-                    HistData.from_files(tdir.get_reference())
-                    for tdir in project_true_dir])
+                hist = merge_hists(
+                    mode,
+                    config.binning.zbins,
+                    [
+                        HistData.from_files(tdir.get_reference())
+                        for tdir in project_true_dir
+                    ],
+                )
             except MergeError as e:
                 logger.error(e.args[0] + ", skipping")
             else:
                 hist.to_files(true_dir.get_reference())
         if merged_state.has_nz_true:
             for bin_idx in bins:
                 logger.info("merging true redshift distributions")
                 try:
-                    hist = merge_hists(mode, config.binning.zbins, [
-                        HistData.from_files(tdir.get_unknown(bin_idx))
-                        for tdir in project_true_dir])
+                    hist = merge_hists(
+                        mode,
+                        config.binning.zbins,
+                        [
+                            HistData.from_files(tdir.get_unknown(bin_idx))
+                            for tdir in project_true_dir
+                        ],
+                    )
                 except MergeError as e:
                     logger.error(e.args[0] + ", skipping")
                 else:
                     hist.to_files(true_dir.get_unknown(bin_idx))
 
         return merged
 
@@ -324,19 +335,21 @@
     @property
     def sources(self) -> tuple[Path]:
         return self._sources
 
     def to_dict(self) -> dict[str, Any]:
         # strip default values from config
         configuration = compress_config(
-            self._config.to_dict(), DEFAULT.Configuration.__dict__)
+            self._config.to_dict(), DEFAULT.Configuration.__dict__
+        )
         setup = dict(
             configuration=configuration,
             sources=[str(fpath) for fpath in self._sources],
-            tasks=self._tasks.history_to_list())
+            tasks=self._tasks.history_to_list(),
+        )
         return setup
 
     def get_bin_indices(self) -> set[int]:
         for scale in self.iter_scales():
             counts = self.get_counts_dir(scale)
             return counts.get_cross_indices() | counts.get_auto_indices()
```

### Comparing `yet_another_wizz-2.5/src/yaw_cli/pipeline/plot.py` & `yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/plot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,66 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
-import numpy as np
 import matplotlib
-matplotlib.use("agg")
 import matplotlib.pyplot as plt
+import numpy as np
 
 from yaw.correlation import CorrData
 from yaw.redshifts import RedshiftData
-
 from yaw_cli.pipeline.project import ProjectDirectory
 
 if TYPE_CHECKING:  # pragma: no cover
-    from numpy.typing import NDArray
-    from matplotlib.figure import Figure
     from matplotlib.axis import Axis
+    from matplotlib.figure import Figure
+    from numpy.typing import NDArray
 
 
+matplotlib.pyplot.switch_backend("Agg")
+
 logger = logging.getLogger(__name__)
 
 
 def despine(ax: Axis) -> None:
     ax.spines["right"].set_visible(False)
     ax.spines["top"].set_visible(False)
 
 
 def scale_key_to_math(scale: str) -> str:
     rmin, rmax = scale[3:].split("t")
     return rf"${rmin} < r \leq {rmax}$ kpc"
 
 
 class Plotter:
-
     def __init__(
-        self,
-        project: ProjectDirectory,
-        dpi: int = 100,
-        scale: float = 1.0
+        self, project: ProjectDirectory, dpi: int = 100, scale: float = 1.0
     ) -> None:
         self.project = project
         self.dpi = dpi
         self.scale = scale
 
     def figsize(self, n_col: int, n_row: int) -> tuple[float, float]:
-        return (0.5 + 3.5*n_col*self.scale, 0.3 + 3*n_row*self.scale)
+        return (0.5 + 3.5 * n_col * self.scale, 0.3 + 3 * n_row * self.scale)
 
-    def mkfig(
-        self,
-        n_plots: int,
-        n_col: int = 3
-    ) -> tuple[Figure, Axis | NDArray]:
+    def mkfig(self, n_plots: int, n_col: int = 3) -> tuple[Figure, Axis | NDArray]:
         n_row, rest = divmod(n_plots, n_col)
         if n_row == 0:
             n_row, n_col = 1, rest
         elif rest > 0:
             n_row += 1
         fig, axis = plt.subplots(
-            n_row, n_col, figsize=self.figsize(n_col=n_col, n_row=n_row),
-            dpi=self.dpi, sharex=True, sharey=True)
+            n_row,
+            n_col,
+            figsize=self.figsize(n_col=n_col, n_row=n_row),
+            dpi=self.dpi,
+            sharex=True,
+            sharey=True,
+        )
         if n_plots == 1:
             return fig, axis
         axes = np.atleast_2d(axis)
         for i, ax in enumerate(axes.flatten()):
             if i >= n_plots:
                 ax.remove()
         return fig, axes
@@ -80,34 +77,29 @@
             despine(ax)
         for ax in axes[-1]:
             self._decorate_xaxis(ax)
         for ax in axes[:, 0]:
             ax.set_ylabel(ylabel, fontsize=self.label_fontsize)
 
     def _track_lim(
-        self,
-        lims: tuple[float, float],
-        data: NDArray
+        self, lims: tuple[float, float], data: NDArray
     ) -> tuple[float, float]:
         y_min = np.nanmin(data)
         y_max = np.nanmax(data)
         return min(lims[0], y_min), max(lims[1], y_max)
 
     def _ylim_with_lim(
-        self,
-        ax: Axis,
-        lims: tuple[float, float] | None,
-        margin: float = 0.15
+        self, ax: Axis, lims: tuple[float, float] | None, margin: float = 0.15
     ) -> None:
         if lims is not None:
             axlims = ax.get_ylim()
             ymin = max(axlims[0], lims[0])
             ymax = min(axlims[1], lims[1])
             dy = ymax - ymin
-            ax.set_ylim(ymin - margin*dy, ymax + margin*dy)
+            ax.set_ylim(ymin - margin * dy, ymax + margin * dy)
 
     def auto_reference(self, title: str | None = None) -> Figure | None:
         if not self.project.get_state().has_w_ss_cf:
             logger.debug("skipping reference autocorrelation")
             return
 
         fig, ax = self.mkfig(1)
@@ -167,15 +159,15 @@
                             ylims = np.inf, -np.inf
                         nzt = RedshiftData.from_files(true_path).normalised()
                         ylims = self._track_lim(ylims, nzt.data)
                         nzt.plot(error_bars=False, color="k", ax=ax)
                     else:
                         nzt = None
                     nz_ts[bin] = nzt
-                # plot optional 
+                # plot optional
                 nz = RedshiftData.from_files(path).normalised(to=nzt)
                 label = f"{scale_key_to_math(scale)} / {tag=}"
                 nz.plot(zero_line=True, label=label, ax=ax)
                 ax.legend(title=f"{bin=}", prop=dict(size=8))
 
             self._decorate_subplots(axes, r"$n_{\sf cc}$")
             if title is not None:
```

### Comparing `yet_another_wizz-2.5/src/yaw_cli/pipeline/processing.py` & `yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 
 import yaw
 from yaw.catalogs import BaseCatalog, PatchLinkage
 from yaw.config import ResamplingConfig
 from yaw.core.utils import format_float_fixed_width as fmt_num
 from yaw.correlation import CorrData, CorrFunc
 from yaw.redshifts import RedshiftData
-
 from yaw_cli.pipeline.data import MissingCatalogError
 
-if TYPE_CHECKING: ## pragma: no cover
+if TYPE_CHECKING:  # pragma: no cover
     from yaw.config import Configuration
     from yaw_cli.pipeline.project import ProjectDirectory, ProjectState
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -26,29 +25,22 @@
 
 
 _Tbc = tuple[BaseCatalog, Union[BaseCatalog, None]]
 _Tcf = dict[str, CorrFunc]
 _Tcd = dict[str, CorrData]
 
 
-def _cf_as_dict(
-    config: Configuration,
-    cfs: CorrFunc | _Tcf
-) -> _Tcf:
+def _cf_as_dict(config: Configuration, cfs: CorrFunc | _Tcf) -> _Tcf:
     if not isinstance(cfs, dict):
         cfs = {str(config.scales[0]): cfs}
     return cfs
 
 
 class PostProcessor:
-
-    def __init__(
-        self,
-        project: ProjectDirectory
-    ) -> None:
+    def __init__(self, project: ProjectDirectory) -> None:
         self.project = project
         self.set_run_context()
         self._bin_idx = None
         # warning state flags
         self._warned_patches = False
         self._warned_linkage = False
         # create place holder attributes
@@ -56,17 +48,15 @@
         self._w_ss: _Tcf | None = None
         self._w_pp: _Tcf | None = None
         self._w_sp_data: _Tcd | None = None
         self._w_ss_data: _Tcd | None = None
         self._w_pp_data: _Tcd | None = None
 
     def set_run_context(
-        self,
-        progress: bool = False,
-        threads: int | None = None
+        self, progress: bool = False, threads: int | None = None
     ) -> None:
         self.progress = progress
         if threads is None:
             self.config = self.project.config
         else:
             self.config = self.project.config.modify(thread_num=threads)
 
@@ -133,77 +123,59 @@
 
     def _sample_corrfunc(
         self,
         cfs_kind: str,
         *,
         tag: str,
         config: ResamplingConfig,
-        estimator: str | None = None
+        estimator: str | None = None,
     ) -> _Tcd:
         cfs: _Tcf = getattr(self, f"_{cfs_kind}")
         data = getattr(self, f"_{cfs_kind}_data")
         if data is None:
             data = {}
         for scale, cf in cfs.items():
             logger.debug(f"processing pair counts for {tag=} / {scale=}")
-            data[(scale, tag)] = cf.sample(
-                config, estimator=estimator, info=cfs_kind)
+            data[(scale, tag)] = cf.sample(config, estimator=estimator, info=cfs_kind)
         setattr(self, f"_{cfs_kind}_data", data)
         return data
 
     def sample_auto_ref(
-        self,
-        *,
-        tag: str,
-        config: ResamplingConfig,
-        estimator: str | None = None
+        self, *, tag: str, config: ResamplingConfig, estimator: str | None = None
     ) -> _Tcd:
         return self._sample_corrfunc(
-            "w_ss", tag=tag, config=config, estimator=estimator)
+            "w_ss", tag=tag, config=config, estimator=estimator
+        )
 
     def sample_auto_unk(
-        self,
-        *,
-        tag: str,
-        config: ResamplingConfig,
-        estimator: str | None = None
+        self, *, tag: str, config: ResamplingConfig, estimator: str | None = None
     ) -> _Tcd:
         return self._sample_corrfunc(
-            "w_pp", tag=tag, config=config, estimator=estimator)
+            "w_pp", tag=tag, config=config, estimator=estimator
+        )
 
     def sample_cross(
-        self,
-        *,
-        tag: str,
-        config: ResamplingConfig,
-        estimator: str | None = None
+        self, *, tag: str, config: ResamplingConfig, estimator: str | None = None
     ) -> _Tcd:
         return self._sample_corrfunc(
-            "w_sp", tag=tag, config=config, estimator=estimator)
+            "w_sp", tag=tag, config=config, estimator=estimator
+        )
 
     def write_auto_ref(self, tag: str) -> None:
-        for scale_tag, est_dir in self.project.iter_estimate(
-            create=True, tag=tag
-        ):
+        for scale_tag, est_dir in self.project.iter_estimate(create=True, tag=tag):
             path = est_dir.get_auto_reference()
             self._w_ss_data[scale_tag].to_files(path)
 
     def write_auto_unk(self, tag: str) -> None:
-        for scale_tag, est_dir in self.project.iter_estimate(
-            create=True, tag=tag
-        ):
+        for scale_tag, est_dir in self.project.iter_estimate(create=True, tag=tag):
             path = est_dir.get_auto(self.get_bin_idx())
             self._w_pp_data[scale_tag].to_files(path)
 
     def write_nz_cc(
-        self,
-        tag: str,
-        *,
-        bias_ref: bool = True,
-        bias_unk: bool = True
+        self, tag: str, *, bias_ref: bool = True, bias_unk: bool = True
     ) -> None:
         def get_info(w_ii_data: dict[str, CorrData | None]) -> str:
             if len(w_ii_data) == 0:
                 return None
             cd = next(iter(w_ii_data.values()))
             return cd.info
 
@@ -222,24 +194,26 @@
 
         info = f"{get_info(cross_data)} / sqrt({' '.join(denom_info)})"
         for scale in self.project.iter_scales():
             key = (scale, tag)
             est_dir = self.project.get_estimate_dir(scale, tag, create=True)
             path = est_dir.get_cross(self.get_bin_idx())
             nz_data = RedshiftData.from_correlation_data(
-                cross_data[key], ref_data[key], unk_data[key], info=info)
+                cross_data[key], ref_data[key], unk_data[key], info=info
+            )
             nz_data.to_files(path)
 
     def plot(self):
         plot_dir = self.project.estimate_path
         try:
             import matplotlib.pyplot as plt
+
             from yaw_cli.pipeline.plot import Plotter
-            logger.info(
-                f"creating check-plots in '{plot_dir}'")
+
+            logger.info(f"creating check-plots in '{plot_dir}'")
         except ImportError:
             logger.error("could not import matplotlib, plotting disabled")
             return
 
         def plot_wrapper(method, title, name):
             fig = method(title)
             if fig is not None:
@@ -251,48 +225,44 @@
             return False
 
         plotter = Plotter(self.project)
         plotted = False
         plotted |= plot_wrapper(
             method=plotter.auto_reference,
             title="Reference autocorrelation",
-            name="auto_reference.png")
+            name="auto_reference.png",
+        )
         plotted |= plot_wrapper(
             method=plotter.auto_unknown,
             title="Unknown autocorrelation",
-            name="auto_unknown.png")
+            name="auto_unknown.png",
+        )
         plotted |= plot_wrapper(
-            method=plotter.nz,
-            title="Redshift estimate",
-            name="nz_estimate.png")
+            method=plotter.nz, title="Redshift estimate", name="nz_estimate.png"
+        )
         if not plotted:
             logger.warn("there was no data to plot")
 
 
 class DataProcessor(PostProcessor):
-
-    def __init__(
-        self,
-        project: ProjectDirectory
-    ) -> None:
+    def __init__(self, project: ProjectDirectory) -> None:
         super().__init__(project)
         # warning state flags
         self._warned_patches = False
         self._warned_linkage = False
         # create place holder attributes
         self._ref_data: BaseCatalog | None = None
         self._ref_rand: BaseCatalog | None = None
         self._unk_data: BaseCatalog | None = None
         self._unk_rand: BaseCatalog | None = None
         self._linkage: PatchLinkage | None = None
 
     def load_reference(self, skip_rand: bool = False) -> _Tbc:
         def load(kind):
-            cat = self.project.inputs.load_reference(
-                kind=kind, progress=self.progress)
+            cat = self.project.inputs.load_reference(kind=kind, progress=self.progress)
             patch_file = self.project.patch_file
             if not patch_file.exists():
                 self.project.inputs.centers_to_file(patch_file)
             return cat
 
         # load randoms first since preferrable for optional patch creation
         try:
@@ -307,15 +277,16 @@
         self._ref_data = load("data")
         self._warn_patches()
         return self._ref_data, self._ref_rand
 
     def load_unknown(self, skip_rand: bool = False) -> _Tbc:
         def load(kind, idx):
             cat = self.project.inputs.load_unknown(
-                kind=kind, bin_idx=idx, progress=self.progress)
+                kind=kind, bin_idx=idx, progress=self.progress
+            )
             patch_file = self.project.patch_file
             if not patch_file.exists():
                 self.project.inputs.centers_to_file(patch_file)
             return cat
 
         idx = self.get_bin_idx()
         # load randoms first since preferrable for optional patch creation
@@ -330,80 +301,97 @@
             self._unk_rand = None
         self._unk_data = load("data", idx)
         self._warn_patches()
         return self._unk_data, self._unk_rand
 
     def compute_linkage(self) -> None:
         if self._linkage is None:
-            cats = (self._unk_rand, self._unk_data,
-                    self._ref_rand, self._ref_data)
+            cats = (self._unk_rand, self._unk_data, self._ref_rand, self._ref_data)
             for cat in cats:
                 if cat is not None:
                     break
             else:
                 raise MissingCatalogError("no catalogs loaded")
             self._linkage = PatchLinkage.from_setup(self.config, cat)
             if self._linkage.density > 0.3 and not self._warned_linkage:
                 logger.warn(
                     "linkage density > 0.3, either patches overlap "
-                    "significantly or are small compared to scales")
+                    "significantly or are small compared to scales"
+                )
                 self._warned_linkage = True
 
     def run_auto_ref(self, *, compute_rr: bool) -> _Tcf:
         if self._ref_rand is None:
             raise MissingCatalogError(
-                "reference autocorrelation requires reference randoms")
+                "reference autocorrelation requires reference randoms"
+            )
         cfs = yaw.autocorrelate(
-            self.config, self._ref_data, self._ref_rand,
-            linkage=self._linkage, compute_rr=compute_rr,
-            progress=self.progress)
+            self.config,
+            self._ref_data,
+            self._ref_rand,
+            linkage=self._linkage,
+            compute_rr=compute_rr,
+            progress=self.progress,
+        )
         cfs = _cf_as_dict(self.config, cfs)
         for scale, counts_dir in self.project.iter_counts(create=True):
             cfs[scale].to_file(counts_dir.get_auto_reference())
         self._w_ss = cfs
         return cfs
 
     def run_auto_unk(self, *, compute_rr: bool) -> _Tcf:
         idx = self.get_bin_idx()
         if self._unk_rand is None:
             raise MissingCatalogError(
-                "unknown autocorrelation requires unknown randoms")
+                "unknown autocorrelation requires unknown randoms"
+            )
         cfs = yaw.autocorrelate(
-            self.config, self._unk_data, self._unk_rand,
-            linkage=self._linkage, compute_rr=compute_rr,
-            progress=self.progress)
+            self.config,
+            self._unk_data,
+            self._unk_rand,
+            linkage=self._linkage,
+            compute_rr=compute_rr,
+            progress=self.progress,
+        )
         cfs = _cf_as_dict(self.config, cfs)
         for scale, counts_dir in self.project.iter_counts(create=True):
             cfs[scale].to_file(counts_dir.get_auto(idx))
         self._w_pp = cfs
         return cfs
 
     def run_cross(self, *, compute_rr: bool) -> _Tcf:
         idx = self.get_bin_idx()
         if compute_rr:
             if self._ref_rand is None:
                 raise MissingCatalogError(
-                    "crosscorrelation with RR requires reference randoms")
+                    "crosscorrelation with RR requires reference randoms"
+                )
             if self._unk_rand is None:
                 raise MissingCatalogError(
-                    "crosscorrelation with RR requires unknown randoms")
+                    "crosscorrelation with RR requires unknown randoms"
+                )
             randoms = dict(ref_rand=self._ref_rand, unk_rand=self._unk_rand)
         else:
             # prefer using DR over RD if both are possible
             if self._unk_rand is not None:
                 randoms = dict(unk_rand=self._unk_rand)
             elif self._ref_rand is not None:
                 randoms = dict(ref_rand=self._ref_rand)
             else:
                 raise MissingCatalogError(
-                    "crosscorrelation requires either reference or "
-                    "unknown randoms")
+                    "crosscorrelation requires either reference or unknown randoms"
+                )
         cfs = yaw.crosscorrelate(
-            self.config, self._ref_data, self._unk_data,
-            **randoms, linkage=self._linkage, progress=self.progress)
+            self.config,
+            self._ref_data,
+            self._unk_data,
+            **randoms,
+            linkage=self._linkage,
+            progress=self.progress,
+        )
         cfs = _cf_as_dict(self.config, cfs)
         for scale, counts_dir in self.project.iter_counts(create=True):
             cfs[scale].to_file(counts_dir.get_cross(idx))
         self._w_sp = cfs
         return cfs
 
     def write_nz_ref(self) -> None:
```

### Comparing `yet_another_wizz-2.5/src/yaw_cli/pipeline/project.py` & `yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,22 +9,26 @@
 from itertools import zip_longest
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 import yaml
 
 from yaw import __version__
-from yaw.config import Configuration, default as DEFAULT
-from yaw.config.utils import parse_section_error 
+from yaw.config import Configuration
+from yaw.config import default as DEFAULT
+from yaw.config.utils import parse_section_error
 from yaw.core.abc import DictRepresentation
 from yaw.core.utils import TypePathStr
-
 from yaw_cli.pipeline.data import InputManager
 from yaw_cli.pipeline.directories import (
-    CacheDirectory, CountsDirectory, EstimateDirectory, TrueDirectory)
+    CacheDirectory,
+    CountsDirectory,
+    EstimateDirectory,
+    TrueDirectory,
+)
 from yaw_cli.pipeline.logger import get_logger
 from yaw_cli.pipeline.processing import DataProcessor, PostProcessor
 from yaw_cli.pipeline.tasks import TaskManager
 
 if TYPE_CHECKING:  # pragma: no cover
     from yaw_cli.pipeline.data import Input
 
@@ -43,18 +47,15 @@
     this = [int(s) for s in __version__.split(".")][:2]
     other = [int(s) for s in version.split(".")][:2]
     for t, o in zip_longest(this, other, fillvalue=0):
         if t != o:
             raise SetupError(msg)
 
 
-def compress_config(
-    config: dict[str, Any],
-    default: dict[str, Any]
-) -> dict[str, Any]:
+def compress_config(config: dict[str, Any], default: dict[str, Any]) -> dict[str, Any]:
     compressed = dict(**config)
     for key, value in config.items():
         if key in default:
             refval = default[key]
             if isinstance(value, dict) and hasattr(refval, "__dict__"):
                 new = compress_config(value, refval.__dict__)
                 if len(new) == 0:
@@ -62,18 +63,15 @@
                 else:
                     compressed[key] = new
             elif value == refval:
                 compressed.pop(key)
     return compressed
 
 
-def write_setup_file(
-    path: TypePathStr,
-    setup_dict: dict[str, Any]
-) -> None:
+def write_setup_file(path: TypePathStr, setup_dict: dict[str, Any]) -> None:
     logger.debug("writing setup file")
     setup_dict = {k: v for k, v in setup_dict.items()}
     setup_dict["_version"] = __version__
     lines = yaml.dump(setup_dict).split("\n")
     # some postprocessing for better readibility
     indent = " " * 4
     string = "# yet_another_wizz setup configuration (auto generated)\n"
@@ -104,30 +102,30 @@
 
 
 def load_setup_as_dict(setup_file: TypePathStr) -> dict[str, Any]:
     with open(setup_file) as f:
         try:
             return yaml.safe_load(f.read())
         except Exception as e:
-            raise SetupError(
-                f"parsing the setup file '{setup_file}' failed") from e
+            raise SetupError(f"parsing the setup file '{setup_file}' failed") from e
 
 
 def load_config_from_setup(setup_file: TypePathStr) -> Configuration:
     logger.info(f"importing configuration from '{setup_file}'")
     setup_dict = load_setup_as_dict(setup_file)
     return parse_config_from_setup(setup_dict)
 
 
 def parse_config_from_setup(setup_dict: dict[str, Any]) -> Configuration:
     try:
         return Configuration.from_dict(setup_dict["configuration"])
     except KeyError as e:
         parse_section_error(e, "configuration", SetupError)
 
+
 @dataclass(frozen=True)
 class ProjectState:
     has_reference: bool = False
     has_unknown: bool = False
     has_w_ss: bool = False
     has_w_sp: bool = False
     has_w_pp: bool = False
@@ -135,26 +133,25 @@
     has_w_pp_cf: bool = False
     has_nz_cc: bool = False
     has_nz_ref: bool = False
     has_nz_true: bool = False
 
 
 class YawDirectory(DictRepresentation):
-
     _tasks: TaskManager
 
     def __init__(self, path: TypePathStr) -> None:
         self._path = Path(path).expanduser()
         if not self.path.exists():
-            raise FileNotFoundError(
-                f"project directory '{self.path}' does not exist")
+            raise FileNotFoundError(f"project directory '{self.path}' does not exist")
         if not self.setup_file.exists():
             raise FileNotFoundError(
                 f"not a {self.__class__.__name__}, setup file "
-                f"'{self.setup_file}' does not exist")
+                f"'{self.setup_file}' does not exist"
+            )
         if not self.log_file.exists():
             logger.info(f"setting up log file '{self.log_file}'")
         else:
             logger.info(f"resuming project at '{self._path}'")
         self._add_log_file_handle()
         with open(self.setup_file) as f:
             setup = yaml.safe_load(f.read())
@@ -167,28 +164,30 @@
 
     def _add_log_file_handle(self):
         # create the file logger
         logger = get_logger()
         fh = logging.FileHandler(self.log_file, mode="a")
         fh.setLevel(logging.DEBUG)
         formatter = logging.Formatter(
-            "%(asctime)s - %(name)s - %(levelname)s - %(message)s")
+            "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+        )
         fh.setFormatter(formatter)
         logger.addHandler(fh)
 
     def __enter__(self) -> ProjectDirectory:
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         # TODO: this is sometimes executed even if an exception was raised
         if exc_type is None:
             self.setup_write()
 
     @abstractproperty
-    def setup_file(self) -> Path: pass
+    def setup_file(self) -> Path:
+        pass
 
     def setup_write(self) -> None:
         write_setup_file(self.setup_file, self.to_dict())
 
     @abstractmethod
     def setup_reload(self, setup: dict) -> None:
         check_version(setup.pop("_version", __version__))
@@ -251,15 +250,16 @@
             has_w_ss=has_w_ss,
             has_w_sp=has_w_sp,
             has_w_pp=has_w_pp,
             has_w_ss_cf=has_w_ss_cf,
             has_w_pp_cf=has_w_pp_cf,
             has_nz_cc=has_nz_cc,
             has_nz_ref=true_dir.has_reference,
-            has_nz_true=true_dir.has_unknown)
+            has_nz_true=true_dir.has_unknown,
+        )
 
     @property
     def processor(self) -> PostProcessor:
         return self._tasks._engine
 
     @property
     def path(self) -> Path:
@@ -277,41 +277,33 @@
     def bin_weight_file(self) -> Path:
         return self._path.joinpath("bin_weights.dat")
 
     @property
     def counts_path(self) -> Path:
         return self.path.joinpath("paircounts")
 
-    def get_counts_dir(
-        self,
-        scale_key: str,
-        create: bool = False
-    ) -> CountsDirectory:
+    def get_counts_dir(self, scale_key: str, create: bool = False) -> CountsDirectory:
         path = self.counts_path.joinpath(scale_key)
         if create:
             path.mkdir(exist_ok=True)
         return CountsDirectory(path)
 
     def iter_counts(
-        self,
-        create: bool = False
+        self, create: bool = False
     ) -> Iterator[tuple[str, CountsDirectory]]:
         for scale in self.iter_scales():
             counts = self.get_counts_dir(scale, create=create)
             yield scale, counts
 
     @property
     def estimate_path(self) -> Path:
         return self.path.joinpath("estimate")
 
     def get_estimate_dir(
-        self,
-        scale_key: str,
-        tag: str = "fid",
-        create: bool = False
+        self, scale_key: str, tag: str = "fid", create: bool = False
     ) -> EstimateDirectory:
         path = self.estimate_path.joinpath(scale_key, tag)
         if create:
             path.mkdir(exist_ok=True, parents=True)
         return EstimateDirectory(path)
 
     def iter_tags(self) -> Iterator[str]:
@@ -322,78 +314,67 @@
                 for tag_path in path.iterdir():
                     if tag_path.is_dir():
                         tags.add(tag_path.name)
         for tag in sorted(tags):
             yield tag
 
     def iter_estimate(
-        self,
-        create: bool = False,
-        tag: str = DEFAULT.NotSet
+        self, create: bool = False, tag: str = DEFAULT.NotSet
     ) -> Iterator[tuple[tuple[str, str], EstimateDirectory]]:
         if tag is DEFAULT.NotSet:
             tag_iter = self.iter_tags()
         else:
             tag_iter = (tag,)
         for tag in tag_iter:
             for scale in self.iter_scales():
                 est = self.get_estimate_dir(scale, tag, create=create)
                 yield (scale, tag), est
 
-    def get_true_dir(
-        self,
-        create: bool = False
-    ) -> TrueDirectory:
+    def get_true_dir(self, create: bool = False) -> TrueDirectory:
         path = self.path.joinpath("true")
         if create:
             path.mkdir(exist_ok=True)
         return TrueDirectory(path)
 
     @property
     def tasks(self) -> TaskManager:
         return self._tasks
 
     @abstractmethod
-    def get_bin_indices(self) -> set[int]: pass
+    def get_bin_indices(self) -> set[int]:
+        pass
 
     @abstractproperty
-    def n_bins(self) -> int: pass
+    def n_bins(self) -> int:
+        pass
 
 
 class ProjectDirectory(YawDirectory):
-
     @classmethod
     def create(
         cls,
         path: TypePathStr,
         config: Configuration,
         n_patches: int | None = None,
         cachepath: TypePathStr | None = None,
-        backend: str = DEFAULT.backend
+        backend: str = DEFAULT.backend,
     ) -> ProjectDirectory:
         logger.info(f"creating new project at '{path}'")
         data = dict()
         if n_patches is not None:
             data["n_patches"] = n_patches
         if cachepath is not None:
             data["cachepath"] = cachepath
         if backend != DEFAULT.backend:
             data["backend"] = backend
-        setup_dict = dict(
-            configuration=config.to_dict(),
-            data=data,
-            tasks=[])
+        setup_dict = dict(configuration=config.to_dict(), data=data, tasks=[])
         return cls.from_dict(setup_dict, path=path)
 
     @classmethod
-    def from_setup(
-        cls,
-        path: TypePathStr,
-        setup_file: TypePathStr
-    ) -> ProjectDirectory:
+    def from_setup(cls, path: TypePathStr, setup_file: TypePathStr) -> ProjectDirectory:
         new = cls.__new__(cls)  # access to path attributes
         new._path = Path(path).expanduser()
         new._path.mkdir(parents=True, exist_ok=False)
         # copy setup file
         shutil.copy(str(setup_file), str(new.setup_file))
         return cls(path)
 
@@ -420,19 +401,21 @@
         # try loading existsing patch centers
         if self.patch_file.exists():
             self._inputs.centers_from_file(self.patch_file)
 
     def to_dict(self) -> dict[str, Any]:
         # strip default values from config
         configuration = compress_config(
-            self._config.to_dict(), DEFAULT.Configuration.__dict__)
+            self._config.to_dict(), DEFAULT.Configuration.__dict__
+        )
         setup = dict(
             configuration=configuration,
             data=self._inputs.to_dict(),
-            tasks=self._tasks.history_to_list())
+            tasks=self._tasks.history_to_list(),
+        )
         # cache: if default location set to None. Reason: if cloning setup,
         # original cache would be used (unless manually overridden)
         if setup["data"]["cachepath"] == str(self.default_cache_path):
             setup["data"].pop("cachepath")
         return setup
 
     @property
@@ -446,34 +429,25 @@
     @property
     def default_cache_path(self) -> Path:
         return self._path.joinpath("cache")
 
     def get_cache_dir(self) -> CacheDirectory:
         return self.inputs.get_cache()
 
-    def set_reference(
-        self,
-        data: Input,
-        rand: Input | None = None
-    ) -> None:
+    def set_reference(self, data: Input, rand: Input | None = None) -> None:
         if rand is not None:
-            logger.debug(
-                f"registering reference random catalog '{rand.filepath}'")
+            logger.debug(f"registering reference random catalog '{rand.filepath}'")
         self._inputs.set_reference(data, rand)
-    
-    def add_unknown(
-        self,
-        bin_idx: int,
-        data: Input,
-        rand: Input | None = None
-    ) -> None:
+
+    def add_unknown(self, bin_idx: int, data: Input, rand: Input | None = None) -> None:
         if rand is not None:
             logger.debug(
                 f"registering unknown bin {bin_idx} random catalog "
-                f"'{rand.filepath}'")
+                f"'{rand.filepath}'"
+            )
         self._inputs.add_unknown(bin_idx, data, rand)
 
     def get_bin_indices(self) -> set[int]:
         return self._inputs.get_bin_indices()
 
     @property
     def n_bins(self) -> int:
```

### Comparing `yet_another_wizz-2.5/src/yaw_cli/pipeline/tasks.py` & `yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,49 +2,48 @@
 
 import bisect
 import functools
 import logging
 from abc import abstractclassmethod, abstractmethod
 from collections import deque
 from collections.abc import Iterator, Sequence
-from dataclasses import dataclass, field, fields, asdict, MISSING
+from dataclasses import MISSING, asdict, dataclass, field, fields
 from typing import TYPE_CHECKING, Any
 
-from yaw.config import ResamplingConfig, default as DEFAULT, OPTIONS
+from yaw.config import OPTIONS, ResamplingConfig
+from yaw.config import default as DEFAULT
 from yaw.core.abc import DictRepresentation
 from yaw.core.docs import Parameter
 from yaw.correlation.estimators import CorrelationEstimator
-
-from yaw_cli.pipeline.processing import DataProcessor
 from yaw_cli.pipeline.logger import print_yaw_message
+from yaw_cli.pipeline.processing import DataProcessor
 
 if TYPE_CHECKING:  # pragma: no cover
     from argparse import Namespace
+
     from yaw_cli.pipeline.project import ProjectDirectory
 
 
 logger = logging.getLogger(__name__)
 
 ESTIMATORS = [est.short for est in CorrelationEstimator.variants]
 
 
 class TaskError(Exception):
     pass
 
 
 class UndefinedTaskError(TaskError):
-
     def __init__(self, task: str) -> None:
         msg = f"got undefined task with name '{task}', options are: "
         msg += ", ".join(f"'{name}'" for name in Task._tasks)
         super().__init__(msg)
 
 
 class TaskArgumentError(TaskError):
-
     def __init__(self, argument, taskname, options=None) -> None:
         msg = f"encountered unknown argument '{argument}' in task '{taskname}'"
         msg += ", options are:"
         if options is not None:
             if len(options) == 0:
                 msg += " no arguments"
             else:
@@ -121,17 +120,17 @@
 
 
 class MergedTask(Task):
     pass
 
 
 class RepeatableTask(Task):
-
     @abstractmethod
-    def get_identifier(self) -> Any: raise NotImplementedError
+    def get_identifier(self) -> Any:
+        raise NotImplementedError
 
     def __eq__(self, other: Task) -> bool:
         if super().__eq__(other) and hasattr(other, "get_identifier"):
             # additionally compare on the argument level
             return self.get_identifier() == other.get_identifier()
         return False
 
@@ -141,225 +140,239 @@
         return Task._tasks[name]
     except KeyError as e:
         raise UndefinedTaskError(name) from e
 
 
 @dataclass(frozen=True)
 class TaskCrosscorr(Task):
-
     rr: bool = field(
         default=False,
         metadata=Parameter(
             type=bool,
-            help="compute random-random pair counts, even if both randoms are "
-                "available"))
+            help="compute random-random pair counts, even if both randoms are available",
+        ),
+    )
 
     @classmethod
     def get_name(cls) -> str:
         return "cross"
 
     @classmethod
     def get_help(cls) -> str:
         return "compute the crosscorrelation"
 
 
 @dataclass(frozen=True)
 class TaskAutocorr(Task):
-
     rr: bool = field(
         default=True,
-        metadata=Parameter(
-            type=bool,
-            help="do not compute random-random pair counts"))
+        metadata=Parameter(type=bool, help="do not compute random-random pair counts"),
+    )
 
 
 @dataclass(frozen=True)
 class TaskAutocorrReference(TaskAutocorr):
-
     @classmethod
     def get_name(cls) -> str:
         return "auto_ref"
 
     @classmethod
     def get_help(cls) -> str:
-        return (
-            "compute the reference sample autocorrelation for bias mitigation")
+        return "compute the reference sample autocorrelation for bias mitigation"
 
 
 @dataclass(frozen=True)
 class TaskAutocorrUnknown(TaskAutocorr):
-
     @classmethod
     def get_name(cls) -> str:
         return "auto_unk"
 
     @classmethod
     def get_help(cls) -> str:
         return "compute the unknown sample autocorrelation for bias mitigation"
 
 
 @dataclass(frozen=True)
 class TaskTrueRedshifts(Task):
-
     @classmethod
     def get_name(cls) -> str:
         return "ztrue"
 
     @classmethod
     def get_help(cls) -> str:
         return (
             "compute true redshift distributions for unknown data (requires "
-            "point estimate)")
+            "point estimate)"
+        )
 
     def __call__(self, project: ProjectDirectory) -> Any:
         super().__call__(project)
         project.engine.run(ztrue=self)
 
 
 @dataclass(frozen=True)
 class TaskDropCache(Task):
-
     @classmethod
     def get_name(cls) -> str:
         return "drop_cache"
 
     @classmethod
     def get_help(cls) -> str:
         return "delete temporary data in cache directory, has no arguments"
 
 
 @dataclass(frozen=True)
 class TaskEstimateCorr(MergedTask, RepeatableTask):
-
     tag: str = field(
         default="fid",
         metadata=Parameter(
             type=str,
             help="unique identifier for different configurations",
-            default_text="(default: %(default)s)"))
+            default_text="(default: %(default)s)",
+        ),
+    )
     bias_ref: bool = field(
         default=True,
         metadata=Parameter(
             type=bool,
             help="whether to mitigate the reference sample bias using its "
-                 "autocorrelation function (if available)"))
+            "autocorrelation function (if available)",
+        ),
+    )
     bias_unk: bool = field(
         default=True,
         metadata=Parameter(
             type=bool,
             help="whether to mitigate the unknown sample bias using its "
-                 "autocorrelation functions (if available)"))
+            "autocorrelation functions (if available)",
+        ),
+    )
 
     est_cross: str | None = field(
         default=None,
         metadata=Parameter(
-            type=str, choices=ESTIMATORS,
+            type=str,
+            choices=ESTIMATORS,
             help="correlation estimator for crosscorrelations",
             default_text="(default: LS or DP)",
-            parser_id="estimators"))
+            parser_id="estimators",
+        ),
+    )
     est_auto: str | None = field(
         default=None,
         metadata=Parameter(
-            type=str, choices=ESTIMATORS,
+            type=str,
+            choices=ESTIMATORS,
             help="correlation estimator for autocorrelations",
             default_text="(default: LS or DP)",
-            parser_id="estimators"))
+            parser_id="estimators",
+        ),
+    )
 
     method: str = field(
         default=DEFAULT.Resampling.method,
         metadata=Parameter(
-            type=str, choices=OPTIONS.method,
+            type=str,
+            choices=OPTIONS.method,
             help="resampling method for covariance estimates",
             default_text="(default: %(default)s)",
-            parser_id="sampling"))
+            parser_id="sampling",
+        ),
+    )
     crosspatch: bool = field(
         default=DEFAULT.Resampling.crosspatch,
         metadata=Parameter(
             type=bool,
             help="whether to include cross-patch pair counts when resampling",
-            parser_id="sampling"))
+            parser_id="sampling",
+        ),
+    )
     n_boot: int = field(
         default=DEFAULT.Resampling.n_boot,
         metadata=Parameter(
             type=int,
             help="number of bootstrap samples",
             default_text="(default: %(default)s)",
-            parser_id="sampling"))
+            parser_id="sampling",
+        ),
+    )
     global_norm: bool = field(
         default=DEFAULT.Resampling.global_norm,
         metadata=Parameter(
             type=bool,
             help="normalise pair counts globally instead of patch-wise",
-            parser_id="sampling"))
+            parser_id="sampling",
+        ),
+    )
     seed: int = field(
         default=DEFAULT.Resampling.seed,
         metadata=Parameter(
             type=int,
             help="random seed for bootstrap sample generation",
             default_text="(default: %(default)s)",
-            parser_id="sampling"))
+            parser_id="sampling",
+        ),
+    )
 
     @classmethod
     def get_name(cls) -> str:
         return "zcc"
 
     @classmethod
     def get_help(cls) -> str:
         return (
             "compute clustering redshift estimates for the unknown data, task "
-            "can be added repeatedly if different a 'tag' is used")
+            "can be added repeatedly if different a 'tag' is used"
+        )
 
     def get_identifier(self) -> str:
         return self.tag
 
     @property
     def config(self) -> ResamplingConfig:
         return ResamplingConfig(
             method=self.method,
             crosspatch=self.crosspatch,
             n_boot=self.n_boot,
             global_norm=self.global_norm,
-            seed=self.seed)
+            seed=self.seed,
+        )
 
 
 @dataclass(frozen=True)
 class TaskPlot(MergedTask, Task):
-
     @classmethod
     def get_name(cls) -> str:
         return "plot"
 
     @classmethod
     def get_help(cls) -> str:
         return "generate automatic check plots"
 
 
 class TaskManager(Sequence):
-
     def __init__(self, project: ProjectDirectory) -> None:
         self._engine = DataProcessor(project)
         self._history: list[Task] = []
         self._queue: deque[Task] = deque([])
 
     @classmethod
     def from_history_list(
-        cls,
-        task_list: Sequence[dict[str, Any] | str],
-        project: ProjectDirectory
+        cls, task_list: Sequence[dict[str, Any] | str], project: ProjectDirectory
     ) -> TaskManager:
         new = cls(project)
         for task in task_list:
             if isinstance(task, str):
                 name, arg_dict = task, {}
             elif isinstance(task, dict):
                 name, arg_dict = task.popitem()
             else:
                 raise TaskError(
-                    "serialisation format must be 'str(name)' or "
-                    "{str(name): dict(**args)}'")
+                    "serialisation format must be 'str(name)' or {str(name): dict(**args)}'"
+                )
             task_inst = get_task(name).from_dict(arg_dict)
             new._insert_task(task_inst, new._history)
         return new
 
     def history_to_list(self) -> list[dict[str, Any] | str]:
         task_list = []
         for task in self._history:
@@ -405,25 +418,23 @@
         return tuple(t for t in self._queue)
 
     def get_history(self) -> tuple[Task]:
         return tuple(t for t in self._history)
 
     def _insert_task(self, task: Task, task_list: list[Task]) -> None:
         if not isinstance(task, Task):
-            raise TypeError(
-                f"'task' must be of type {Task}, got {type(task)}")
+            raise TypeError(f"'task' must be of type {Task}, got {type(task)}")
         try:
             task_list.remove(task)
         except ValueError:
             pass
         bisect.insort(task_list, task)
 
     def schedule(self, task: Task) -> None:
-        t_args = ", ".join(
-            f"{k}={repr(v)}" for k, v in asdict(task).items())
+        t_args = ", ".join(f"{k}={repr(v)}" for k, v in asdict(task).items())
         if len(t_args) == 0:
             t_args = "---"
         logger.debug(f"'{task.get_name()}' arguments: {t_args}")
         self._insert_task(task, self._queue)
 
     def reschedule_history(self) -> None:
         for task in self.get_history():
@@ -432,35 +443,28 @@
     def drop(self, task: Task) -> Task:
         self._queue.remove(task)
         return task
 
     def clear(self) -> None:
         self._queue.clear()
 
-    def process(
-        self,
-        progress: bool = False,
-        threads: int | None = None
-    ) -> None:
+    def process(self, progress: bool = False, threads: int | None = None) -> None:
         kwargs = self._get_run_args(self._queue)
         try:
             self._engine.set_run_context(progress=progress, threads=threads)
             self._run(**kwargs)
         finally:
             self._engine.reset_run_context()
         # move tasks to history
         while len(self._queue) > 0:
             task = self._queue.pop()
             self._insert_task(task, self._history)
 
     def run(
-        self,
-        task: Task,
-        progress: bool = False,
-        threads: int | None = None
+        self, task: Task, progress: bool = False, threads: int | None = None
     ) -> None:
         # log task
         logger.info(f"running task '{task.get_name()}'")
         args = ", ".join(f"{k}={repr(v)}" for k, v in asdict(task).items())
         if len(args) == 0:
             args = "---"
         logger.debug(f"arguments: {args}")
@@ -470,16 +474,15 @@
             self._queue = deque([])
             self._insert_task(task, self._queue)
             self.process(progress=progress, threads=threads)
         finally:
             self._queue = queue
 
     def _get_run_args(
-        self,
-        task_list: list[Task]
+        self, task_list: list[Task]
     ) -> dict[str, Task | list[RepeatableTask]]:
         tasks = {}
         for task in task_list:
             name = task.get_name()
             # handle repeatable task
             if name in tasks:
                 if isinstance(tasks[name], RepeatableTask):
@@ -530,16 +533,18 @@
             engine.compute_linkage()
             engine.run_auto_ref(compute_rr=auto_ref.rr)
         elif do_zcc and has_w_ss:
             engine.load_auto_ref()
         if do_zcc and engine._w_ss is not None:
             for zcc_task in zcc:
                 engine.sample_auto_ref(
-                    tag=zcc_task.tag, config=zcc_task.config,
-                    estimator=zcc_task.est_auto)
+                    tag=zcc_task.tag,
+                    config=zcc_task.config,
+                    estimator=zcc_task.est_auto,
+                )
                 engine.write_auto_ref(zcc_task.tag)
                 zcc_processed = True
 
         if do_w_sp or do_w_pp or (do_zcc and (has_w_sp or has_w_pp)) or do_true:
             for i, idx in enumerate(engine.iter_bins(), 1):
                 message = "processing unknown "
                 if engine.project.n_bins == 1:
@@ -568,33 +573,36 @@
 
                 if do_zcc:
                     for zcc_task in zcc:
                         if engine._w_pp is not None:
                             engine.sample_auto_unk(
                                 tag=zcc_task.tag,
                                 config=zcc_task.config,
-                                estimator=zcc_task.est_auto)
+                                estimator=zcc_task.est_auto,
+                            )
                             engine.write_auto_unk(tag=zcc_task.tag)
                             zcc_processed = True
                         if engine._w_sp is not None:
                             engine.sample_cross(
                                 tag=zcc_task.tag,
                                 config=zcc_task.config,
-                                estimator=zcc_task.est_cross)
+                                estimator=zcc_task.est_cross,
+                            )
                             engine.write_nz_cc(
                                 tag=zcc_task.tag,
                                 bias_ref=zcc_task.bias_ref,
-                                bias_unk=zcc_task.bias_unk)
+                                bias_unk=zcc_task.bias_unk,
+                            )
                             zcc_processed = True
 
                 if do_true:
                     engine.write_nz_true()
 
         if do_zcc and not zcc_processed:
             logger.warn("task 'zcc': there were no pair counts to process")
 
         if drop_cache:
             engine.drop_cache()
-        
+
         if plot:
             print_yaw_message("plotting data")
             engine.plot()
```

### Comparing `yet_another_wizz-2.5/src/yet_another_wizz.egg-info/PKG-INFO` & `yet_another_wizz-2.5.post0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,43 @@
 Metadata-Version: 2.1
-Name: yet-another-wizz
-Version: 2.5
+Name: yet_another_wizz
+Version: 2.5.post0
 Summary: Implementation of the Schmidt et al. (2013) clustering redshift method and wrapper scripts to produce cross-correlation (CC) redshifts.
 Home-page: https://github.com/jlvdb/yet_another_wizz.git
 Author-email: Jan Luca van den Busch <jlvdb@astro.ruhr-uni-bochum.de>
 License: GPL-3.0-or-later
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: plot
 Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: style
 Provides-Extra: dev
 License-File: LICENSE
 
 yet_another_wizz
 ================
 
+.. image:: https://badge.fury.io/py/yet-another-wizz.svg
+    :target: https://badge.fury.io/py/yet-another-wizz
+.. image:: https://readthedocs.org/projects/yet-another-wizz/badge/?version=latest
+    :target: https://yet-another-wizz.readthedocs.io/en/latest/?badge=latest
+.. image:: https://github.com/jlvdb/yet_another_wizz/actions/workflows/run-tests.yml/badge.svg
+    :target: https://github.com/jlvdb/yet_another_wizz/actions/workflows/run-tests.yml
+.. image:: https://codecov.io/gh/jlvdb/yet_another_wizz/branch/main/graph/badge.svg?token=PC41ME2AR8
+    :target: https://codecov.io/gh/jlvdb/yet_another_wizz
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+    :target: https://pycqa.github.io/isort/
+
 
 *yet_another_wizz* is a python package to efficiently compute cross-correlation
 redshifts, also know as clustering redshifts and is hosted on github:
 
 - code: https://github.com/jlvdb/yet_another_wizz.git
 - docs: https://yet-another-wizz.readthedocs.io/
 - PyPI: https://pypi.org/project/yet_another_wizz/
@@ -67,15 +82,15 @@
 Reporting bugs and requesting features
 --------------------------------------
 
 For bug reports or requesting new features, please use the github issue page:
 
 https://github.com/jlvdb/yet_another_wizz/issues
 
-    
+
 **Maintainers:**
 
 - Jan Luca van den Busch
   (*author*, Ruhr-Universität Bochum, Astronomisches Institut)
 
 
 Acknowledgements
```

### Comparing `yet_another_wizz-2.5/src/yet_another_wizz.egg-info/SOURCES.txt` & `yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 src/yaw/correlation/estimators.py
 src/yaw/correlation/paircounts.py
 src/yaw/examples/__init__.py
 src/yaw/examples/auto_reference.hdf
 src/yaw/examples/auto_unknown_1.hdf
 src/yaw/examples/cross_1.hdf
 src/yaw_cli/__init__.py
-src/yaw_cli/__main__.py
 src/yaw_cli/commandline/__init__.py
 src/yaw_cli/commandline/main.py
 src/yaw_cli/commandline/subcommands.py
 src/yaw_cli/commandline/utils.py
 src/yaw_cli/pipeline/__init__.py
 src/yaw_cli/pipeline/data.py
 src/yaw_cli/pipeline/default_setup.py
```

