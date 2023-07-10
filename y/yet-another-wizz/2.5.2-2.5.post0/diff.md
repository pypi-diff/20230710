# Comparing `tmp/yet_another_wizz-2.5.2.tar.gz` & `tmp/yet_another_wizz-2.5.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yet_another_wizz-2.5.2.tar", last modified: Mon Jul 10 19:20:44 2023, max compression
+gzip compressed data, was "yet_another_wizz-2.5.post0.tar", last modified: Mon Jul 10 08:18:48 2023, max compression
```

## Comparing `yet_another_wizz-2.5.2.tar` & `yet_another_wizz-2.5.post0.tar`

### file list

```diff
@@ -1,64 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:20:44.603727 yet_another_wizz-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-10 19:20:44.603727 yet_another_wizz-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 19:20:44.603727 yet_another_wizz-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:20:44.595727 yet_another_wizz-2.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:20:44.599727 yet_another_wizz-2.5.2/src/yaw/
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:20:44.599727 yet_another_wizz-2.5.2/src/yaw/catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/catalogs/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/catalogs/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/catalogs/linkage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:20:44.599727 yet_another_wizz-2.5.2/src/yaw/catalogs/scipy/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/catalogs/scipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/catalogs/scipy/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/catalogs/scipy/kdtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/catalogs/scipy/patches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:20:44.599727 yet_another_wizz-2.5.2/src/yaw/catalogs/treecorr/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/catalogs/treecorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15092 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/catalogs/treecorr/catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:20:44.599727 yet_another_wizz-2.5.2/src/yaw/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/config/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/config/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)    14643 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/config/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/config/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/config/resampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/config/scales.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:20:44.603727 yet_another_wizz-2.5.2/src/yaw/core/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9967 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/core/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16139 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/core/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/core/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/core/cosmology.py
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/core/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/core/math.c
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/core/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/core/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:20:44.603727 yet_another_wizz-2.5.2/src/yaw/correlation/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/correlation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40475 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/correlation/corrfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/correlation/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)    41424 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/correlation/paircounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/deprecated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:20:44.603727 yet_another_wizz-2.5.2/src/yaw/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   129479 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/examples/auto_reference.hdf
--rw-r--r--   0 runner    (1001) docker     (123)   123032 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/examples/auto_unknown_1.hdf
--rw-r--r--   0 runner    (1001) docker     (123)   100475 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/examples/cross_1.hdf
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)    22405 2023-07-10 19:19:10.000000 yet_another_wizz-2.5.2/src/yaw/redshifts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:20:44.603727 yet_another_wizz-2.5.2/src/yet_another_wizz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-10 19:20:44.000000 yet_another_wizz-2.5.2/src/yet_another_wizz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-10 19:20:44.000000 yet_another_wizz-2.5.2/src/yet_another_wizz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:20:44.000000 yet_another_wizz-2.5.2/src/yet_another_wizz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-10 19:20:44.000000 yet_another_wizz-2.5.2/src/yet_another_wizz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 19:20:44.000000 yet_another_wizz-2.5.2/src/yet_another_wizz.egg-info/top_level.txt
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

### Comparing `yet_another_wizz-2.5.2/LICENSE` & `yet_another_wizz-2.5.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/PKG-INFO` & `yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
-Name: yet_another_wizz
-Version: 2.5.2
+Name: yet-another-wizz
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
-Provides-Extra: cli
 Provides-Extra: plot
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: style
 Provides-Extra: dev
 License-File: LICENSE
 
@@ -58,33 +57,29 @@
 Installation
 ------------
 
 The yet_another_wizz package can be installed directly with pip::
 
     pip install yet_another_wizz
 
-This will install the python library ``yaw``. There also exists a separate
-command line tool called *yet_another_wizz_cli* (``yaw_cli``) that is available
-at PyPI and `github <https://github.com/jlvdb/yet_another_wizz_cli>`_. To
-install it alongside the python library, type::
-
-    pip install yet_another_wizz[cli]
+This will install the python package ``yaw``, as well as the ``yaw_cli``
+executable command line tool.
 
 
 Usage
 -----
 
 There are two main ways to use yet_another_wizz,
 
-- the python library ``yaw`` itself and
-- the (separate) ``yaw_cli`` commmand line tool.
+- the ``yaw_cli`` commmand line tool and
+- the python package ``yaw`` directly.
 
 Most people will probably get started with the command line tool, which should
 cover all necessary tasks for a standard clustering redshift calibration. For
-custom solutions, use the python library. A basic example as well as the API
+custom solutions, use the python package. A basic example as well as the API
 reference can be found in the official documentation.
 
 
 Reporting bugs and requesting features
 --------------------------------------
 
 For bug reports or requesting new features, please use the github issue page:
```

### Comparing `yet_another_wizz-2.5.2/README.rst` & `yet_another_wizz-2.5.post0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -37,33 +37,29 @@
 Installation
 ------------
 
 The yet_another_wizz package can be installed directly with pip::
 
     pip install yet_another_wizz
 
-This will install the python library ``yaw``. There also exists a separate
-command line tool called *yet_another_wizz_cli* (``yaw_cli``) that is available
-at PyPI and `github <https://github.com/jlvdb/yet_another_wizz_cli>`_. To
-install it alongside the python library, type::
-
-    pip install yet_another_wizz[cli]
+This will install the python package ``yaw``, as well as the ``yaw_cli``
+executable command line tool.
 
 
 Usage
 -----
 
 There are two main ways to use yet_another_wizz,
 
-- the python library ``yaw`` itself and
-- the (separate) ``yaw_cli`` commmand line tool.
+- the ``yaw_cli`` commmand line tool and
+- the python package ``yaw`` directly.
 
 Most people will probably get started with the command line tool, which should
 cover all necessary tasks for a standard clustering redshift calibration. For
-custom solutions, use the python library. A basic example as well as the API
+custom solutions, use the python package. A basic example as well as the API
 reference can be found in the official documentation.
 
 
 Reporting bugs and requesting features
 --------------------------------------
 
 For bug reports or requesting new features, please use the github issue page:
```

### Comparing `yet_another_wizz-2.5.2/pyproject.toml` & `yet_another_wizz-2.5.post0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -18,37 +18,37 @@
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)"
 ]
 requires-python = ">=3.8"
 dependencies = [
     "typing_extensions;python_version<'3.10'",
     "more_itertools;python_version<'3.10'",
     "deprecated",
-    "tqdm",
     "numpy",
+    "pyarrow",
+    "tqdm",
+    "h5py",
     "pandas",
     "astropandas>=1.2.1",
     "scipy",
     "astropy",
-    "pyarrow",
-    "h5py",
-    "pyyaml",
     "treecorr>=4.3",
+    "emcee",
     "matplotlib",
 ]
 
+[project.scripts]
+yaw_cli = "yaw_cli:Commandline.main"
+
 [project.optional-dependencies]
-cli = ["yet_another_wizz_cli>=1.2.1"]
 plot = ["matplotlib"]
-# note that yaw_cli is currently necessary to generate the joint docs
 docs = [
     "sphinx",
     "sphinx-design",
     "sphinx-copybutton",
     "pydata-sphinx-theme",
-    "yet_another_wizz[cli]",
 ]
 test = [
     "typing_extensions",
     "more_itertools",
     "coverage",
     "pytest",
     "pytest-cov",
@@ -77,21 +77,17 @@
     "examples/*.hdf",
     "examples/*.dat",
     "examples/*.cov",
     "examples/*.smp",
 ]
 
 [tool.pytest.ini_options]
-testpaths = [
-    "tests",
-]
-addopts = [
-    "--cov=yaw",
-    "--cov-report=xml",
-]
+minversion = "6.0"
+addopts = "-ra -q"
+testpaths = ["tests"]
 
 [tool.isort]
 profile = "black"
 
 [tool.black]
 include = ".pyi?$"
 exclude = """
```

### Comparing `yet_another_wizz-2.5.2/src/yaw/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     CorrelationFunction,
     HistogramData,
     PairCountResult,
 )
 from yaw.randoms import UniformRandoms
 from yaw.redshifts import HistData, RedshiftData
 
-__version__ = "2.5.2"
+__version__ = "2.5.post0"
 
 __all__ = [
     "NewCatalog",
     "Configuration",
     "ResamplingConfig",
     "Scale",
     "global_covariance",
```

### Comparing `yet_another_wizz-2.5.2/src/yaw/catalogs/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/catalogs/catalog.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/catalog.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/catalogs/factory.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/factory.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/catalogs/linkage.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/linkage.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/catalogs/scipy/catalog.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/catalog.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/catalogs/scipy/kdtree.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/kdtree.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/catalogs/scipy/patches.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/patches.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/catalogs/treecorr/catalog.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/treecorr/catalog.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/config/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/config/backend.py` & `yet_another_wizz-2.5.post0/src/yaw/config/backend.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/config/binning.py` & `yet_another_wizz-2.5.post0/src/yaw/config/binning.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
 def warn_binning_args_ignored(
     zmin: bool | float | None, zmax: bool | float | None, zbin_num: bool | int | None
 ) -> None:
     """Issue a warning that values are ignored, if any of the arguments is
     set."""
     # NOTE: NotSet is also False
     if zmin or zmax or zbin_num:
-        logger.warning("'zmin', 'zmax', 'nbins' are ignored if 'zbins' is provided")
+        logger.warn("'zmin', 'zmax', 'nbins' are ignored if 'zbins' is provided")
 
 
 def make_binning_config(
     cosmology: TypeCosmology | str | None,
     zmin: float | None = None,
     zmax: float | None = None,
     zbin_num: int | None = None,
```

### Comparing `yet_another_wizz-2.5.2/src/yaw/config/config.py` & `yet_another_wizz-2.5.post0/src/yaw/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,15 +308,20 @@
         # parse the required subgroups
         try:
             scales = ScalesConfig.from_dict(config.pop("scales"))
         except (TypeError, KeyError) as e:
             utils.parse_section_error(e, "scales")
         try:
             binning_conf = config.pop("binning")
-            binning = make_binning_config(cosmology, **binning_conf)
+            if "zbins" in binning_conf:
+                binning = ManualBinningConfig(binning_conf["zbins"])
+            else:
+                binning = AutoBinningConfig.generate(
+                    cosmology=cosmology, **binning_conf
+                )
         except (TypeError, KeyError) as e:
             utils.parse_section_error(e, "binning")
         # parse the optional subgroups
         try:
             backend = BackendConfig.from_dict(config.pop("backend"))
         except KeyError:
             backend = BackendConfig()
```

### Comparing `yet_another_wizz-2.5.2/src/yaw/config/default.py` & `yet_another_wizz-2.5.post0/src/yaw/config/default.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/config/options.py` & `yet_another_wizz-2.5.post0/src/yaw/config/options.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/config/resampling.py` & `yet_another_wizz-2.5.post0/src/yaw/config/resampling.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/config/scales.py` & `yet_another_wizz-2.5.post0/src/yaw/config/scales.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/config/utils.py` & `yet_another_wizz-2.5.post0/src/yaw/config/utils.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/core/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/core/abc.py` & `yet_another_wizz-2.5.post0/src/yaw/core/abc.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/core/containers.py` & `yet_another_wizz-2.5.post0/src/yaw/core/containers.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/core/coordinates.py` & `yet_another_wizz-2.5.post0/src/yaw/core/coordinates.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/core/cosmology.py` & `yet_another_wizz-2.5.post0/src/yaw/core/cosmology.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/core/docs.py` & `yet_another_wizz-2.5.post0/src/yaw/core/docs.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/core/logging.py` & `yet_another_wizz-2.5.post0/src/yaw/core/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,37 +17,37 @@
 
     def __init__(
         self,
         logger: logging.Logger,
         alt_message: str | None = None,
         ignore: bool = True,
     ):
-        """Instead of showing the warning through the :func:`warnings.warning`
+        """Instead of showing the warning through the :func:`warnings.warn`
         machinery, write the message as warning to the provided logger.
 
         Args:
             logger (:obj:`logging.Logger`):
                 The logger instance to which the warning is redirected.
             alt_message (:obj:`str`, optional):
                 Replace the original message text with this value instead.
             ignore (:obj:`bool`, optional):
-                Do not show warning with :func:`warnings.warning` (the default).
+                Do not show warning with :func:`warnings.warn` (the default).
         """
         self._logger = logger
         self._message = alt_message
         self._ignore = ignore
 
     def _process_warning(self, message, category, filename, lineno, *args):
         if not self._ignore:
             self._old_showwarning(message, category, filename, lineno, *args)
         if self._message is not None:
             message = self._message
         else:
             message = f"{category.__name__}: {message}"
-        self._logger.warning(message)
+        self._logger.warn(message)
 
     def __enter__(self) -> TimedLog:
         self._old_showwarning = warnings.showwarning
         warnings.showwarning = self._process_warning
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback) -> None:
```

### Comparing `yet_another_wizz-2.5.2/src/yaw/core/math.c` & `yet_another_wizz-2.5.post0/src/yaw/core/math.c`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/core/math.py` & `yet_another_wizz-2.5.post0/src/yaw/core/math.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/core/parallel.py` & `yet_another_wizz-2.5.post0/src/yaw/core/parallel.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/core/utils.py` & `yet_another_wizz-2.5.post0/src/yaw/core/utils.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/correlation/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/correlation/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/correlation/corrfuncs.py` & `yet_another_wizz-2.5.post0/src/yaw/correlation/corrfuncs.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/correlation/estimators.py` & `yet_another_wizz-2.5.post0/src/yaw/correlation/estimators.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         super().__init_subclass__(**kwargs)
         cls.variants.append(cls)
 
     @classmethod
     def _warn_enum_zero(cls, counts: NDArray):
         """Raise a warning if any value in the expression enumerator is zero"""
         if np.any(counts == 0.0):
-            logger.warning(f"estimator {cls.short} encontered zeros in enumerator")
+            logger.warn(f"estimator {cls.short} encontered zeros in enumerator")
 
     @abstractclassmethod
     def eval(
         cls, *, dd: NDArray, dr: NDArray, rr: NDArray, rd: NDArray | None = None
     ) -> NDArray:
         """Method that implements the estimator.
```

### Comparing `yet_another_wizz-2.5.2/src/yaw/correlation/paircounts.py` & `yet_another_wizz-2.5.post0/src/yaw/correlation/paircounts.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/deprecated.py` & `yet_another_wizz-2.5.post0/src/yaw/deprecated.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/examples/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/examples/auto_reference.hdf` & `yet_another_wizz-2.5.post0/src/yaw/examples/auto_reference.hdf`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/examples/auto_unknown_1.hdf` & `yet_another_wizz-2.5.post0/src/yaw/examples/auto_unknown_1.hdf`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/examples/cross_1.hdf` & `yet_another_wizz-2.5.post0/src/yaw/examples/cross_1.hdf`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/randoms.py` & `yet_another_wizz-2.5.post0/src/yaw/randoms.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.2/src/yaw/redshifts.py` & `yet_another_wizz-2.5.post0/src/yaw/redshifts.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
                 ref_data = ref_corr.sample(config, estimator=ref_est)
             else:
                 ref_data = None
             if unk_corr is not None:
                 unk_data = unk_corr.sample(config, estimator=unk_est)
             else:
                 unk_data = None
-            return cls.from_corrdata(
+            return cls.from_correlation_data(
                 cross_data=cross_data, ref_data=ref_data, unk_data=unk_data, info=info
             )
 
     @property
     def _dat_desc(self) -> str:
         return "# n(z) estimate with symmetric 68% percentile confidence"
```

### Comparing `yet_another_wizz-2.5.2/src/yet_another_wizz.egg-info/PKG-INFO` & `yet_another_wizz-2.5.post0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
-Name: yet-another-wizz
-Version: 2.5.2
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
-Provides-Extra: cli
 Provides-Extra: plot
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: style
 Provides-Extra: dev
 License-File: LICENSE
 
@@ -58,33 +57,29 @@
 Installation
 ------------
 
 The yet_another_wizz package can be installed directly with pip::
 
     pip install yet_another_wizz
 
-This will install the python library ``yaw``. There also exists a separate
-command line tool called *yet_another_wizz_cli* (``yaw_cli``) that is available
-at PyPI and `github <https://github.com/jlvdb/yet_another_wizz_cli>`_. To
-install it alongside the python library, type::
-
-    pip install yet_another_wizz[cli]
+This will install the python package ``yaw``, as well as the ``yaw_cli``
+executable command line tool.
 
 
 Usage
 -----
 
 There are two main ways to use yet_another_wizz,
 
-- the python library ``yaw`` itself and
-- the (separate) ``yaw_cli`` commmand line tool.
+- the ``yaw_cli`` commmand line tool and
+- the python package ``yaw`` directly.
 
 Most people will probably get started with the command line tool, which should
 cover all necessary tasks for a standard clustering redshift calibration. For
-custom solutions, use the python library. A basic example as well as the API
+custom solutions, use the python package. A basic example as well as the API
 reference can be found in the official documentation.
 
 
 Reporting bugs and requesting features
 --------------------------------------
 
 For bug reports or requesting new features, please use the github issue page:
```

