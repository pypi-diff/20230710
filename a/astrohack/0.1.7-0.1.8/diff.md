# Comparing `tmp/astrohack-0.1.7.tar.gz` & `tmp/astrohack-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrohack-0.1.7.tar", last modified: Fri Jul  7 19:34:11 2023, max compression
+gzip compressed data, was "astrohack-0.1.8.tar", last modified: Mon Jul 10 18:41:42 2023, max compression
```

## Comparing `astrohack-0.1.7.tar` & `astrohack-0.1.8.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.470522 astrohack-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 19:33:55.000000 astrohack-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 19:33:55.000000 astrohack-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-07 19:34:11.470522 astrohack-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-07 19:33:55.000000 astrohack-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:33:55.000000 astrohack-0.1.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-07 19:33:55.000000 astrohack-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 19:34:11.470522 astrohack-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.462522 astrohack-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.462522 astrohack-0.1.7/src/astrohack/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.466522 astrohack-0.1.7/src/astrohack/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_dask_graph_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.466522 astrohack-0.1.7/src/astrohack/_utils/_dask_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_dask_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19864 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    22554 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)    12086 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_extract_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_gaussfitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    22951 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_imaging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.466522 astrohack-0.1.7/src/astrohack/_utils/_logger/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5462 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_logger/_astrohack_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.466522 astrohack-0.1.7/src/astrohack/_utils/_panel_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    36145 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_panel_classes/antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_panel_classes/base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_panel_classes/polygon_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_panel_classes/ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_panel_classes/telescope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.466522 astrohack-0.1.7/src/astrohack/_utils/_parm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_parm_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2156 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_parm_utils/_check_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)    27855 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_phase_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/astrohack_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.462522 astrohack-0.1.7/src/astrohack/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.470522 astrohack-0.1.7/src/astrohack/data/.file_meta_data/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.470522 astrohack-0.1.7/src/astrohack/data/telescopes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.470522 astrohack-0.1.7/src/astrohack/data/telescopes/aca_7m.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.470522 astrohack-0.1.7/src/astrohack/data/telescopes/alma_da.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.470522 astrohack-0.1.7/src/astrohack/data/telescopes/alma_dv.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.470522 astrohack-0.1.7/src/astrohack/data/telescopes/alma_tp.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.470522 astrohack-0.1.7/src/astrohack/data/telescopes/vla.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/vla.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/vla.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/vla.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.470522 astrohack-0.1.7/src/astrohack/data/telescopes/vlba.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/vlba.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/vlba.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    33264 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/gdown_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/holog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/locit.py
--rw-r--r--   0 runner    (1001) docker     (123)    42606 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/mds.py
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.470522 astrohack-0.1.7/src/astrohack/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/visualization/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.466522 astrohack-0.1.7/src/astrohack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-07 19:34:11.000000 astrohack-0.1.7/src/astrohack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-07 19:34:11.000000 astrohack-0.1.7/src/astrohack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:34:11.000000 astrohack-0.1.7/src/astrohack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-07 19:34:11.000000 astrohack-0.1.7/src/astrohack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 19:34:11.000000 astrohack-0.1.7/src/astrohack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.006725 astrohack-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 18:41:23.000000 astrohack-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:41:23.000000 astrohack-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-10 18:41:42.006725 astrohack-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-10 18:41:23.000000 astrohack-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:23.000000 astrohack-0.1.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-10 18:41:23.000000 astrohack-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:41:42.006725 astrohack-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:41.986724 astrohack-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:41.990724 astrohack-0.1.8/src/astrohack/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:41.998725 astrohack-0.1.8/src/astrohack/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_dask_graph_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:41.998725 astrohack-0.1.8/src/astrohack/_utils/_dask_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_dask_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19864 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22554 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12086 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_extract_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_gaussfitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22951 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_imaging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:41.998725 astrohack-0.1.8/src/astrohack/_utils/_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5462 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_logger/_astrohack_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:41.998725 astrohack-0.1.8/src/astrohack/_utils/_panel_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    36145 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_panel_classes/antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_panel_classes/base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_panel_classes/polygon_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_panel_classes/ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_panel_classes/telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.002725 astrohack-0.1.8/src/astrohack/_utils/_parm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_parm_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2156 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_parm_utils/_check_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27855 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_phase_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/_utils/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/astrohack_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:41.986724 astrohack-0.1.8/src/astrohack/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.002725 astrohack-0.1.8/src/astrohack/data/.file_meta_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.002725 astrohack-0.1.8/src/astrohack/data/telescopes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.002725 astrohack-0.1.8/src/astrohack/data/telescopes/aca_7m.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.002725 astrohack-0.1.8/src/astrohack/data/telescopes/alma_da.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.002725 astrohack-0.1.8/src/astrohack/data/telescopes/alma_dv.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.006725 astrohack-0.1.8/src/astrohack/data/telescopes/alma_tp.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.006725 astrohack-0.1.8/src/astrohack/data/telescopes/vla.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/vla.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/vla.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/vla.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.006725 astrohack-0.1.8/src/astrohack/data/telescopes/vlba.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/vlba.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/vlba.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33264 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/gdown_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/locit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42606 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/mds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:42.006725 astrohack-0.1.8/src/astrohack/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-10 18:41:23.000000 astrohack-0.1.8/src/astrohack/visualization/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:41:41.994724 astrohack-0.1.8/src/astrohack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-10 18:41:41.000000 astrohack-0.1.8/src/astrohack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-10 18:41:41.000000 astrohack-0.1.8/src/astrohack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:41:41.000000 astrohack-0.1.8/src/astrohack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-10 18:41:41.000000 astrohack-0.1.8/src/astrohack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 18:41:41.000000 astrohack-0.1.8/src/astrohack.egg-info/top_level.txt
```

### Comparing `astrohack-0.1.7/LICENSE` & `astrohack-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/PKG-INFO` & `astrohack-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.1.7
+Version: 0.1.8
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `astrohack-0.1.7/README.md` & `astrohack-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/pyproject.toml` & `astrohack-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "astrohack"
-version = "0.1.7"
+version = "0.1.8"
 description = "Holography Antenna Commissioning Kit"
 authors = [
     {name = "Jan-Willem Steeb", email="jsteeb@nrao.edu"},
     {name = "Joshua Hoskins", email="jhoskins@nrao.edu"}, 
     {name = "Victor de Souza Magalhaes", email="vdesouza@nrao.edu"}
 ]
 license = {file = "LICENSE.txt"}
```

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_algorithms.py` & `astrohack-0.1.8/src/astrohack/_utils/_algorithms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_combine.py` & `astrohack-0.1.8/src/astrohack/_utils/_combine.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_constants.py` & `astrohack-0.1.8/src/astrohack/_utils/_constants.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_conversion.py` & `astrohack-0.1.8/src/astrohack/_utils/_conversion.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_dask_graph_tools.py` & `astrohack-0.1.8/src/astrohack/_utils/_dask_graph_tools.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py` & `astrohack-0.1.8/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py` & `astrohack-0.1.8/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_diagnostics.py` & `astrohack-0.1.8/src/astrohack/_utils/_diagnostics.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_dio.py` & `astrohack-0.1.8/src/astrohack/_utils/_dio.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_extract_holog.py` & `astrohack-0.1.8/src/astrohack/_utils/_extract_holog.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_extract_point.py` & `astrohack-0.1.8/src/astrohack/_utils/_extract_point.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_gaussfitter.py` & `astrohack-0.1.8/src/astrohack/_utils/_gaussfitter.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_holog.py` & `astrohack-0.1.8/src/astrohack/_utils/_holog.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_imaging.py` & `astrohack-0.1.8/src/astrohack/_utils/_imaging.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_logger/_astrohack_logger.py` & `astrohack-0.1.8/src/astrohack/_utils/_logger/_astrohack_logger.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_panel.py` & `astrohack-0.1.8/src/astrohack/_utils/_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_panel_classes/antenna_surface.py` & `astrohack-0.1.8/src/astrohack/_utils/_panel_classes/antenna_surface.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_panel_classes/base_panel.py` & `astrohack-0.1.8/src/astrohack/_utils/_panel_classes/base_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_panel_classes/polygon_panel.py` & `astrohack-0.1.8/src/astrohack/_utils/_panel_classes/polygon_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_panel_classes/ring_panel.py` & `astrohack-0.1.8/src/astrohack/_utils/_panel_classes/ring_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_panel_classes/telescope.py` & `astrohack-0.1.8/src/astrohack/_utils/_panel_classes/telescope.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_parm_utils/_check_logger_parms.py` & `astrohack-0.1.8/src/astrohack/_utils/_parm_utils/_check_logger_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_parm_utils/_check_parms.py` & `astrohack-0.1.8/src/astrohack/_utils/_parm_utils/_check_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_phase_fitting.py` & `astrohack-0.1.8/src/astrohack/_utils/_phase_fitting.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/_utils/_tools.py` & `astrohack-0.1.8/src/astrohack/_utils/_tools.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/astrohack_client.py` & `astrohack-0.1.8/src/astrohack/astrohack_client.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/combine.py` & `astrohack-0.1.8/src/astrohack/combine.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json` & `astrohack-0.1.8/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json` & `astrohack-0.1.8/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json` & `astrohack-0.1.8/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs` & `astrohack-0.1.8/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata` & `astrohack-0.1.8/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/data/telescopes/alma_da.zarr/.zattrs` & `astrohack-0.1.8/src/astrohack/data/telescopes/alma_da.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata` & `astrohack-0.1.8/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs` & `astrohack-0.1.8/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata` & `astrohack-0.1.8/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs` & `astrohack-0.1.8/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata` & `astrohack-0.1.8/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/data/telescopes/vla.zarr/.zattrs` & `astrohack-0.1.8/src/astrohack/data/telescopes/vla.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/data/telescopes/vla.zarr/.zmetadata` & `astrohack-0.1.8/src/astrohack/data/telescopes/vla.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/data/telescopes/vlba.zarr/.zattrs` & `astrohack-0.1.8/src/astrohack/data/telescopes/vlba.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/data/telescopes/vlba.zarr/.zmetadata` & `astrohack-0.1.8/src/astrohack/data/telescopes/vlba.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/dio.py` & `astrohack-0.1.8/src/astrohack/dio.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/extract_holog.py` & `astrohack-0.1.8/src/astrohack/extract_holog.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/gdown_utils.py` & `astrohack-0.1.8/src/astrohack/gdown_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import re
 import gdown
 import shutil
 import json
 
 from prettytable import PrettyTable
-from prettytable import DOUBLE_BORDER
 
 gdown_ids = {
     'ea25_cal_small_before_fixed.split.ms':'1oydlR7kA7F4n0i9KF9HgRc2jq1ziUslt',
     'ea25_cal_small_after_fixed.split.ms':'1TATMxKTFYIEO-l9L3jdYj62lZ8TZex4T',
     'J1924-2914.ms.calibrated.split.SPW3': '1OSDjWM1IskPOlC0w1wVBqsTp8JAbNGzL',
     'extract_holog_verification.json':'1Wd79KCl-wxlUwBRxYFUnofG8mN0Xfzga',
     'holog_numerical_verification.json':'16kl_DMHWVb0TwxuHq1dRr1TbIor_IU-a',
@@ -125,8 +124,8 @@
         DEC: {ms_info['dec']}
         EPOCH: {ms_info['epoch']}
         Notes: {ms_info['notes']}
         """
 
         table.add_row([str(key), description_string])
         
-    print(table)
+    print(table)
```

### Comparing `astrohack-0.1.7/src/astrohack/holog.py` & `astrohack-0.1.8/src/astrohack/holog.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/mds.py` & `astrohack-0.1.8/src/astrohack/mds.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/panel.py` & `astrohack-0.1.8/src/astrohack/panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/profiling.py` & `astrohack-0.1.8/src/astrohack/profiling.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack/visualization/viewer.py` & `astrohack-0.1.8/src/astrohack/visualization/viewer.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.7/src/astrohack.egg-info/PKG-INFO` & `astrohack-0.1.8/src/astrohack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.1.7
+Version: 0.1.8
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `astrohack-0.1.7/src/astrohack.egg-info/SOURCES.txt` & `astrohack-0.1.8/src/astrohack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

