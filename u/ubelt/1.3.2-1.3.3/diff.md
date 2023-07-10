# Comparing `tmp/ubelt-1.3.2.tar.gz` & `tmp/ubelt-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubelt-1.3.2.tar", last modified: Thu Jun 22 22:39:39 2023, max compression
+gzip compressed data, was "ubelt-1.3.3.tar", last modified: Mon Jul 10 21:06:22 2023, max compression
```

## Comparing `ubelt-1.3.2.tar` & `ubelt-1.3.3.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:39.954758 ubelt-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-22 22:39:34.000000 ubelt-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    59674 2023-06-22 22:39:39.954758 ubelt-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    58336 2023-06-22 22:39:34.000000 ubelt-1.3.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-22 22:39:34.000000 ubelt-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 22:39:39.954758 ubelt-1.3.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     7952 2023-06-22 22:39:34.000000 ubelt-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:39.954758 ubelt-1.3.2/ubelt/
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/__main__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/_win32_links.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/_win32_links.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16069 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/orderedset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/orderedset.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    36626 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/progiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/progiter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_arg.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_arg.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    52100 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_cache.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    32162 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_cmd.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_colors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_const.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_const.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_deprecate.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_deprecate.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    74794 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_dict.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_download.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_download_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_download_manager.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_format.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_func.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20133 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_futures.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    50076 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_hash.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    38458 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_import.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_indexable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_indexable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10328 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_io.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13011 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_links.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_links.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    32834 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_list.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_memoize.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_mixins.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    59662 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_path.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14734 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_platform.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    42633 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_repr.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_str.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_stream.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22732 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_time.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_zip.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:39.954758 ubelt-1.3.2/ubelt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    59674 2023-06-22 22:39:39.000000 ubelt-1.3.2/ubelt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-22 22:39:39.000000 ubelt-1.3.2/ubelt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 22:39:39.000000 ubelt-1.3.2/ubelt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-06-22 22:39:39.000000 ubelt-1.3.2/ubelt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 22:39:39.000000 ubelt-1.3.2/ubelt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:06:22.348130 ubelt-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-10 21:06:10.000000 ubelt-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    59674 2023-07-10 21:06:22.348130 ubelt-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    58336 2023-07-10 21:06:10.000000 ubelt-1.3.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-10 21:06:10.000000 ubelt-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 21:06:22.348130 ubelt-1.3.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7952 2023-07-10 21:06:10.000000 ubelt-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:06:22.344130 ubelt-1.3.3/ubelt/
+-rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/__main__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/_win32_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/_win32_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16913 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/orderedset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/orderedset.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    36626 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/progiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/progiter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_arg.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    52733 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    32174 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_cmd.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_colors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_const.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_deprecate.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    75546 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_dict.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_download.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_download_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_download_manager.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_func.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20683 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_futures.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    50095 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_hash.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    38649 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_import.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_indexable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_indexable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10328 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_io.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13011 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    33087 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_memoize.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    59778 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_path.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14734 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_platform.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    42963 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_repr.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_str.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_stream.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22732 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_time.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-10 21:06:10.000000 ubelt-1.3.3/ubelt/util_zip.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:06:22.348130 ubelt-1.3.3/ubelt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    59674 2023-07-10 21:06:22.000000 ubelt-1.3.3/ubelt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-10 21:06:22.000000 ubelt-1.3.3/ubelt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 21:06:22.000000 ubelt-1.3.3/ubelt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-07-10 21:06:22.000000 ubelt-1.3.3/ubelt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 21:06:22.000000 ubelt-1.3.3/ubelt.egg-info/top_level.txt
```

### Comparing `ubelt-1.3.2/LICENSE` & `ubelt-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/PKG-INFO` & `ubelt-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubelt
-Version: 1.3.2
+Version: 1.3.3
 Summary: A Python utility belt containing simple tools, a stdlib like feel, and extra batteries.
 Home-page: https://github.com/Erotemic/ubelt
 Author: Jon Crall
 Author-email: erotemic@gmail.com
 License: Apache 2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ubelt-1.3.2/README.rst` & `ubelt-1.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/pyproject.toml` & `ubelt-1.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/setup.py` & `ubelt-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/__init__.py` & `ubelt-1.3.3/ubelt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     mkinit ubelt -w  # todo: get sphinx to ignore this
     # TODO: Lazy imports with mkinit (requires python 3.7)
 
 Testing:
     xdoctest ubelt
 """
 
-__version__ = '1.3.2'
+__version__ = '1.3.3'
 
 # Deprecated functions
 from ubelt.util_platform import (
     ensure_app_cache_dir, ensure_app_config_dir,
     ensure_app_data_dir, get_app_cache_dir, get_app_config_dir,
     get_app_data_dir,
 )
@@ -152,53 +152,54 @@
 from ubelt.util_hash import (hash_data, hash_file,)
 from ubelt.util_import import (import_module_from_name,
                                import_module_from_path, modname_to_modpath,
                                modpath_to_modname, split_modpath,)
 from ubelt.util_indexable import (IndexableWalker, indexable_allclose,)
 from ubelt.util_memoize import (memoize, memoize_method, memoize_property,)
 from ubelt.util_mixins import (NiceRepr,)
-from ubelt.util_path import (Path, TempDir, augpath, ensuredir, expandpath,
-                             shrinkuser, userhome,)
+from ubelt.util_path import (ChDir, Path, TempDir, augpath, ensuredir,
+                             expandpath, shrinkuser, userhome,)
 from ubelt.util_platform import (DARWIN, LINUX, POSIX, WIN32, find_exe,
                                  find_path, platform_cache_dir,
                                  platform_config_dir, platform_data_dir,)
 from ubelt.util_str import (codeblock, hzcat, indent, paragraph,)
 from ubelt.util_stream import (CaptureStdout, CaptureStream, TeeStringIO,)
 from ubelt.util_time import (Timer, timeparse, timestamp,)
 from ubelt.util_zip import (split_archive, zopen,)
 from ubelt.orderedset import (OrderedSet, oset,)
 from ubelt.progiter import (ProgIter,)
 
 __all__ = ['AutoDict', 'AutoOrderedDict', 'CacheStamp', 'Cacher',
-           'CaptureStdout', 'CaptureStream', 'DARWIN', 'DownloadManager',
-           'Executor', 'FormatterExtensions', 'IndexableWalker', 'JobPool',
-           'LINUX', 'NO_COLOR', 'NiceRepr', 'NoParam', 'OrderedSet', 'POSIX',
-           'Path', 'ProgIter', 'ReprExtensions', 'SetDict', 'TeeStringIO',
-           'TempDir', 'Timer', 'UDict', 'WIN32', 'allsame', 'argflag',
-           'argmax', 'argmin', 'argsort', 'argunique', 'argval', 'augpath',
-           'boolmask', 'chunks', 'cmd', 'codeblock', 'color_text',
-           'compatible', 'compress', 'ddict', 'delete', 'dict_diff',
-           'dict_hist', 'dict_isect', 'dict_subset', 'dict_union', 'download',
-           'dzip', 'ensure_app_cache_dir', 'ensure_app_config_dir',
-           'ensure_app_data_dir', 'ensure_unicode', 'ensuredir', 'expandpath',
-           'find_duplicates', 'find_exe', 'find_path', 'flatten',
-           'get_app_cache_dir', 'get_app_config_dir', 'get_app_data_dir',
-           'grabdata', 'group_items', 'hash_data', 'hash_file',
-           'highlight_code', 'hzcat', 'identity', 'import_module_from_name',
-           'import_module_from_path', 'indent', 'indexable_allclose',
-           'inject_method', 'invert_dict', 'iter_window', 'iterable',
-           'map_keys', 'map_vals', 'map_values', 'memoize', 'memoize_method',
-           'memoize_property', 'modname_to_modpath', 'modpath_to_modname',
-           'named_product', 'odict', 'orderedset', 'oset', 'paragraph', 'peek',
-           'platform_cache_dir', 'platform_config_dir', 'platform_data_dir',
-           'progiter', 'readfrom', 'repr2', 'schedule_deprecation', 'sdict',
-           'shrinkuser', 'sorted_keys', 'sorted_vals', 'sorted_values',
-           'split_archive', 'split_modpath', 'symlink', 'take', 'timeparse',
-           'timestamp', 'touch', 'udict', 'unique', 'unique_flags', 'urepr',
-           'userhome', 'util_arg', 'util_cache', 'util_cmd', 'util_colors',
-           'util_const', 'util_deprecate', 'util_dict', 'util_download',
+           'CaptureStdout', 'CaptureStream', 'ChDir', 'DARWIN',
+           'DownloadManager', 'Executor', 'FormatterExtensions',
+           'IndexableWalker', 'JobPool', 'LINUX', 'NO_COLOR', 'NiceRepr',
+           'NoParam', 'OrderedSet', 'POSIX', 'Path', 'ProgIter',
+           'ReprExtensions', 'SetDict', 'TeeStringIO', 'TempDir', 'Timer',
+           'UDict', 'WIN32', 'allsame', 'argflag', 'argmax', 'argmin',
+           'argsort', 'argunique', 'argval', 'augpath', 'boolmask', 'chunks',
+           'cmd', 'codeblock', 'color_text', 'compatible', 'compress', 'ddict',
+           'delete', 'dict_diff', 'dict_hist', 'dict_isect', 'dict_subset',
+           'dict_union', 'download', 'dzip', 'ensure_app_cache_dir',
+           'ensure_app_config_dir', 'ensure_app_data_dir', 'ensure_unicode',
+           'ensuredir', 'expandpath', 'find_duplicates', 'find_exe',
+           'find_path', 'flatten', 'get_app_cache_dir', 'get_app_config_dir',
+           'get_app_data_dir', 'grabdata', 'group_items', 'hash_data',
+           'hash_file', 'highlight_code', 'hzcat', 'identity',
+           'import_module_from_name', 'import_module_from_path', 'indent',
+           'indexable_allclose', 'inject_method', 'invert_dict', 'iter_window',
+           'iterable', 'map_keys', 'map_vals', 'map_values', 'memoize',
+           'memoize_method', 'memoize_property', 'modname_to_modpath',
+           'modpath_to_modname', 'named_product', 'odict', 'orderedset',
+           'oset', 'paragraph', 'peek', 'platform_cache_dir',
+           'platform_config_dir', 'platform_data_dir', 'progiter', 'readfrom',
+           'repr2', 'schedule_deprecation', 'sdict', 'shrinkuser',
+           'sorted_keys', 'sorted_vals', 'sorted_values', 'split_archive',
+           'split_modpath', 'symlink', 'take', 'timeparse', 'timestamp',
+           'touch', 'udict', 'unique', 'unique_flags', 'urepr', 'userhome',
+           'util_arg', 'util_cache', 'util_cmd', 'util_colors', 'util_const',
+           'util_deprecate', 'util_dict', 'util_download',
            'util_download_manager', 'util_format', 'util_func', 'util_futures',
            'util_hash', 'util_import', 'util_indexable', 'util_io',
            'util_links', 'util_list', 'util_memoize', 'util_mixins',
            'util_path', 'util_platform', 'util_repr', 'util_str',
            'util_stream', 'util_time', 'util_zip', 'varied_values', 'writeto',
            'zopen']
```

### Comparing `ubelt-1.3.2/ubelt/_win32_links.py` & `ubelt-1.3.3/ubelt/_win32_links.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/orderedset.py` & `ubelt-1.3.3/ubelt/orderedset.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 import itertools as it
 from collections import deque
 from collections.abc import MutableSet, Sequence
 
 __all__ = ['OrderedSet', 'oset']
 
 
-SLICE_ALL = slice(None)
+SLICE_ALL = slice(None)  # type: slice
 __version__ = "3.2"
 
 
 def is_iterable(obj):
     """
     Are we being asked to look up a list of things, instead of a single thing?
     We check for the `__iter__` attribute so that this can cover types that
@@ -61,20 +61,28 @@
 
 
 class OrderedSet(MutableSet, Sequence):
     """
     An OrderedSet is a custom MutableSet that remembers its order, so that
     every entry has an index that can be looked up.
 
+    Attributes:
+        items (List[Any]): internal ordered representation.
+        map (Dict[Any, int]): internal mapping from items to indices.
+
     Example:
         >>> OrderedSet([1, 1, 2, 3, 2])
         OrderedSet([1, 2, 3])
     """
 
     def __init__(self, iterable=None):
+        """
+        Args:
+            iterable (None | Iterable): input data
+        """
         self.items = []
         self.map = {}
         if iterable is not None:
             self |= iterable
 
     def __len__(self):
         """
@@ -119,14 +127,17 @@
         else:
             raise TypeError("Don't know how to index an OrderedSet by %r" % index)
 
     def copy(self):
         """
         Return a shallow copy of this object.
 
+        Returns:
+            OrderedSet
+
         Example:
             >>> this = OrderedSet([1, 2, 3])
             >>> other = this.copy()
             >>> this == other
             True
             >>> this is other
             False
@@ -151,14 +162,17 @@
         else:
             self.__init__(state)
 
     def __contains__(self, key):
         """
         Test if the item is in this ordered set
 
+        Returns:
+            bool
+
         Example:
             >>> 1 in OrderedSet([1, 3, 2])
             True
             >>> 5 in OrderedSet([1, 3, 2])
             False
         """
         return key in self.map
@@ -202,41 +216,49 @@
                 item_index = self.add(item)
         except TypeError:
             raise ValueError(
                 "Argument needs to be an iterable, got %s" % type(sequence)
             )
         return item_index
 
-    def index(self, key):
+    def index(self, key):  # type: ignore
         """
         Get the index of a given entry, raising an IndexError if it's not
         present.
 
-        `key` can be an iterable of entries that is not a string, in which case
-        this returns a list of indices.
+        `key` can be a non-string iterable of entries, in which case this
+        returns a list of indices.
 
         Example:
             >>> oset = OrderedSet([1, 2, 3])
             >>> oset.index(2)
             1
         """
+        # Note: adding in this typing information breaks mypy
+        # Args:
+        #     key (Any | List[Any]): item(s) in the set to find the index of
+        # Returns:
+        #     int | List[int]:
         if is_iterable(key):
             return [self.index(subkey) for subkey in key]
         return self.map[key]
 
     # Provide some compatibility with pd.Index
     get_loc = index
     get_indexer = index
 
     def pop(self):
         """
         Remove and return the last element from the set.
 
         Raises KeyError if the set is empty.
 
+        Returns:
+            Any
+
         Example:
             >>> oset = OrderedSet([1, 2, 3])
             >>> oset.pop()
             3
         """
         if not self.items:
             raise KeyError("Set is empty")
@@ -275,34 +297,40 @@
         Remove all items from this OrderedSet.
         """
         del self.items[:]
         self.map.clear()
 
     def __iter__(self):
         """
+        Returns:
+            Iterator
+
         Example:
             >>> list(iter(OrderedSet([1, 2, 3])))
             [1, 2, 3]
         """
         return iter(self.items)
 
     def __reversed__(self):
         """
+        Returns:
+            Iterator
+
         Example:
             >>> list(reversed(OrderedSet([1, 2, 3])))
             [3, 2, 1]
         """
         return reversed(self.items)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         if not self:
             return "%s()" % (self.__class__.__name__,)
         return "%s(%r)" % (self.__class__.__name__, list(self))
 
-    def __eq__(self, other):
+    def __eq__(self, other) -> bool:
         """
         Returns true if the containers have the same items. If `other` is a
         Sequence, then order is checked, otherwise it is ignored.
 
         Example:
             >>> oset = OrderedSet([1, 3, 2])
             >>> oset == [1, 3, 2]
@@ -329,14 +357,17 @@
             return set(self) == other_as_set
 
     def union(self, *sets):
         """
         Combines all unique items.
         Each items order is defined by its first appearance.
 
+        Returns:
+            OrderedSet
+
         Example:
             >>> oset = OrderedSet.union(OrderedSet([3, 1, 4, 1, 5]), [1, 3], [2, 0])
             >>> print(oset)
             OrderedSet([3, 1, 4, 5, 2, 0])
             >>> oset.union([8, 9])
             OrderedSet([3, 1, 4, 5, 2, 0, 8, 9])
             >>> oset | {10}
@@ -352,14 +383,17 @@
         return self.intersection(other)
 
     def intersection(self, *sets):
         """
         Returns elements in common between all sets. Order is defined only
         by the first set.
 
+        Returns:
+            OrderedSet
+
         Example:
             >>> from ubelt.orderedset import *  # NOQA
             >>> oset = OrderedSet.intersection(OrderedSet([0, 1, 2, 3]), [1, 2, 3])
             >>> print(oset)
             OrderedSet([1, 2, 3])
             >>> oset.intersection([2, 4, 5], [1, 2, 3, 4])
             OrderedSet([2])
@@ -374,14 +408,17 @@
             items = self
         return cls(items)
 
     def difference(self, *sets):
         """
         Returns all elements that are in this set but not the others.
 
+        Returns:
+            OrderedSet
+
         Example:
             >>> OrderedSet([1, 2, 3]).difference(OrderedSet([2]))
             OrderedSet([1, 3])
             >>> OrderedSet([1, 2, 3]).difference(OrderedSet([2]), OrderedSet([3]))
             OrderedSet([1])
             >>> OrderedSet([1, 2, 3]) - OrderedSet([2])
             OrderedSet([1, 3])
@@ -392,15 +429,15 @@
         if sets:
             other = set.union(*map(set, sets))
             items = (item for item in self if item not in other)
         else:
             items = self
         return cls(items)
 
-    def issubset(self, other):
+    def issubset(self, other) -> bool:
         """
         Report whether another set contains this set.
 
         Example:
             >>> OrderedSet([1, 2, 3]).issubset({1, 2})
             False
             >>> OrderedSet([1, 2, 3]).issubset({1, 2, 3, 4})
@@ -410,15 +447,15 @@
         """
         if len(self) > len(other):  # Fast check for obvious cases
             return False
         return all(item in other for item in self)
 
     # todo: contiguous subset / subsequence_index?
 
-    def issuperset(self, other):
+    def issuperset(self, other) -> bool:
         """
         Report whether this set contains another set.
 
         Example:
             >>> OrderedSet([1, 2]).issuperset([1, 2, 3])
             False
             >>> OrderedSet([1, 2, 3, 4]).issuperset({1, 2, 3})
@@ -435,14 +472,17 @@
         Return the symmetric difference of two OrderedSets as a new set.
         That is, the new set will contain all elements that are in exactly
         one of the sets.
 
         Their order will be preserved, with elements from `self` preceding
         elements from `other`.
 
+        Returns:
+            OrderedSet
+
         Example:
             >>> this = OrderedSet([1, 4, 3, 5, 7])
             >>> other = OrderedSet([9, 7, 1, 3, 2])
             >>> this.symmetric_difference(other)
             OrderedSet([4, 5, 9, 2])
         """
         cls = self.__class__ if isinstance(self, OrderedSet) else OrderedSet
```

### Comparing `ubelt-1.3.2/ubelt/orderedset.pyi` & `ubelt-1.3.3/ubelt/util_stream.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,93 +1,69 @@
+import io
+from typing import List
+from typing import Type
+from types import TracebackType
 from _typeshed import Incomplete
-from collections.abc import MutableSet, Sequence
 
-SLICE_ALL: Incomplete
 
+class TeeStringIO(io.StringIO):
+    redirect: io.IOBase | None
+    buffer: Incomplete
 
-def is_iterable(obj):
-    ...
-
-
-class OrderedSet(MutableSet, Sequence):
-    items: Incomplete
-    map: Incomplete
-
-    def __init__(self, iterable: Incomplete | None = ...) -> None:
+    def __init__(self, redirect: io.IOBase | None = None) -> None:
         ...
 
-    def __len__(self):
+    def isatty(self):
         ...
 
-    def __getitem__(self, index):
+    def fileno(self):
         ...
 
-    def copy(self):
+    @property
+    def encoding(self):
         ...
 
-    def __contains__(self, key):
+    def write(self, msg):
         ...
 
-    def add(self, key):
-        ...
-
-    append = add
-
-    def update(self, sequence):
+    def flush(self):
         ...
 
-    def index(self, key):
-        ...
-
-    get_loc = index
-    get_indexer = index
-
-    def pop(self):
-        ...
-
-    def discard(self, key) -> None:
-        ...
 
-    def clear(self) -> None:
-        ...
-
-    def __iter__(self):
-        ...
-
-    def __reversed__(self):
-        ...
-
-    def __eq__(self, other):
-        ...
+class CaptureStream:
+    ...
 
-    def union(self, *sets):
-        ...
 
-    def __and__(self, other):
-        ...
+class CaptureStdout(CaptureStream):
+    text: str | None
+    parts: List[str]
+    cap_stdout: None | TeeStringIO
+    orig_stdout: io.TextIOBase
+    started: bool
+    enabled: bool
+    suppress: bool
 
-    def intersection(self, *sets):
+    def __init__(self, suppress: bool = True, enabled: bool = True) -> None:
         ...
 
-    def difference(self, *sets):
+    def log_part(self) -> None:
         ...
 
-    def issubset(self, other):
+    def start(self) -> None:
         ...
 
-    def issuperset(self, other):
+    def stop(self) -> None:
         ...
 
-    def symmetric_difference(self, other):
+    def __enter__(self):
         ...
 
-    def difference_update(self, *sets) -> None:
+    def __del__(self) -> None:
         ...
 
-    def intersection_update(self, other) -> None:
+    def close(self) -> None:
         ...
 
-    def symmetric_difference_update(self, other) -> None:
+    def __exit__(self, ex_type: Type[BaseException] | None,
+                 ex_value: BaseException | None,
+                 ex_traceback: TracebackType | None) -> bool | None:
         ...
-
-
-oset = OrderedSet
```

### Comparing `ubelt-1.3.2/ubelt/progiter.py` & `ubelt-1.3.3/ubelt/progiter.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/progiter.pyi` & `ubelt-1.3.3/ubelt/progiter.pyi`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/util_arg.py` & `ubelt-1.3.3/ubelt/util_arg.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/util_cache.py` & `ubelt-1.3.3/ubelt/util_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,64 +124,16 @@
     Saves data to disk and reloads it based on specified dependencies.
 
     Cacher uses pickle to save/load data to/from disk. Dependencies of the
     cached process can be specified, which ensures the cached data is
     recomputed if the dependencies change. If the location of the cache is not
     specified, it will default to the system user's cache directory.
 
-    Args:
-        fname (str):
-            A file name. This is the prefix that will be used by the cache. It
-            will always be used as-is.
-
-        depends (str | List[str] | None):
-            Indicate dependencies of this cache.  If the dependencies change,
-            then the cache is recomputed.  New in version 0.8.9, replaces
-            ``cfgstr``.
-
-        dpath (str | PathLike | None):
-            Specifies where to save the cache. If unspecified, Cacher defaults
-            to an application cache dir as given by appname. See
-            :func:`ub.get_app_cache_dir` for more details.
-
-        appname (str, default='ubelt'): Application name
-            Specifies a folder in the application cache directory where to
-            cache the data if ``dpath`` is not specified.
-
-        ext (str, default='.pkl'):
-            File extension for the cache format. Can be ``'.pkl'`` or
-            ``'.json'``.
-
-        meta (object | None):
-            Metadata that is also saved with the ``cfgstr``.  This can be
-            useful to indicate how the ``cfgstr`` was constructed.
-            Note: this is a candidate for deprecation.
-
-        verbose (int, default=1): Level of verbosity. Can be 1, 2 or 3.
-
-        enabled (bool, default=True): If set to False, then the load and save
-            methods will do nothing.
-
-        log (Callable[[str], Any]):
-            Overloads the print function. Useful for sending output to loggers
-            (e.g. logging.info, tqdm.tqdm.write, ...)
-
-        hasher (str, default='sha1'):
-            Type of hashing algorithm to use if ``cfgstr`` needs to be
-            condensed to less than 49 characters.
-
-        protocol (int, default=-1): Protocol version used by pickle.
-            Defaults to the -1 which is the latest protocol.
-
-        backend (str):
-            Set to either ``'pickle'`` or ``'json'`` to force backend. Defaults
-            to auto which chooses one based on the extension.
-
-        cfgstr (str | None):
-            Deprecated in favor of ``depends``.
+    Related:
+        ..[JobLibMemory] https://joblib.readthedocs.io/en/stable/memory.html
 
     Example:
         >>> import ubelt as ub
         >>> depends = 'repr-of-params-that-uniquely-determine-the-process'
         >>> # Create a cacher and try loading the data
         >>> cacher = ub.Cacher('demo_process', depends, verbose=4)
         >>> cacher.clear()
@@ -215,14 +167,67 @@
     """
     VERBOSE = 1  # default verbosity
     FORCE_DISABLE = False  # global scope override
 
     def __init__(self, fname, depends=None, dpath=None, appname='ubelt',
                  ext='.pkl', meta=None, verbose=None, enabled=True, log=None,
                  hasher='sha1', protocol=-1, cfgstr=None, backend='auto'):
+        """
+        Args:
+            fname (str):
+                A file name. This is the prefix that will be used by the cache. It
+                will always be used as-is.
+
+            depends (str | List[str] | None):
+                Indicate dependencies of this cache.  If the dependencies change,
+                then the cache is recomputed.  New in version 0.8.9, replaces
+                ``cfgstr``.
+
+            dpath (str | PathLike | None):
+                Specifies where to save the cache. If unspecified, Cacher defaults
+                to an application cache dir as given by appname. See
+                :func:`ub.get_app_cache_dir` for more details.
+
+            appname (str): Application name
+                Specifies a folder in the application cache directory where to
+                cache the data if ``dpath`` is not specified. Defaults to
+                'ubelt'.
+
+            ext (str):
+                File extension for the cache format. Can be ``'.pkl'`` or
+                ``'.json'``. Defaults to ``'.pkl'``.
+
+            meta (object | None):
+                Metadata that is also saved with the ``cfgstr``.  This can be
+                useful to indicate how the ``cfgstr`` was constructed.
+                Note: this is a candidate for deprecation.
+
+            verbose (int): Level of verbosity. Can be 1, 2 or 3. Defaults to 1.
+
+            enabled (bool): If set to False, then the load and save
+                methods will do nothing. Defaults to True.
+
+            log (Callable[[str], Any]):
+                Overloads the print function. Useful for sending output to loggers
+                (e.g. logging.info, tqdm.tqdm.write, ...)
+
+            hasher (str):
+                Type of hashing algorithm to use if ``cfgstr`` needs to be
+                condensed to less than 49 characters. Defaults to sha1.
+
+            protocol (int): Protocol version used by pickle.
+                Defaults to the -1 which is the latest protocol.
+
+            backend (str):
+                Set to either ``'pickle'`` or ``'json'`` to force backend. Defaults
+                to auto which chooses one based on the extension.
+
+            cfgstr (str | None):
+                Deprecated in favor of ``depends``.
+        """
 
         if depends is None:
             depends = cfgstr
 
         if cfgstr is not None:  # nocover
             from ubelt import schedule_deprecation
             schedule_deprecation(
@@ -310,15 +315,15 @@
                                             base='hex')
             condensed = condensed[0:max_len]
         else:
             condensed = cfgstr
         return condensed
 
     @property
-    def fpath(self):
+    def fpath(self) -> os.PathLike:
         import ubelt as ub
         return ub.Path(self.get_fpath())
 
     def get_fpath(self, cfgstr=None):
         """
         Reports the filepath that the cacher will use.
 
@@ -425,24 +430,23 @@
     def tryload(self, cfgstr=None, on_error='raise'):
         """
         Like load, but returns None if the load fails due to a cache miss.
 
         Args:
             cfgstr (str | None): overrides the instance-level cfgstr
 
-            on_error (str, default='raise'):
+            on_error (str):
                 How to handle non-io errors errors. Either 'raise', which
                 re-raises the exception, or 'clear' which deletes the cache and
-                returns None.
+                returns None. Defaults to 'raise'.
 
         Returns:
             None | object:
                 the cached data if it exists, otherwise returns None
         """
-        # cfgstr = self._rectify_cfgstr(cfgstr)
         if self.enabled:
             try:
                 if self.verbose > 1:
                     self.log('[cacher] tryload fname={}'.format(self.fname))
                 return self.load(cfgstr)
             except IOError:
                 if self.verbose > 0:
@@ -721,62 +725,14 @@
     If the user knows what the hash of the file should be this can be specified
     to prevent renewal of the stamp unless these match the files on disk. This
     can be useful for security purposes.
 
     The stamp can also be set to expire at a specified time or after a
     specified duration using the ``expires`` argument.
 
-    Args:
-        fname (str):
-            Name of the stamp file
-
-        dpath (str | PathLike | None):
-            Where to store the cached stamp file
-
-        product (str | PathLike | Sequence[str | PathLike] | None):
-            Path or paths that we expect the computation to produce. If
-            specified the hash of the paths are stored.
-
-        hasher (str, default='sha1'):
-            The type of hasher used to compute the file hash of product.
-            If None, then we assume the file has not been corrupted or changed
-            if the mtime and size are the same. Defaults to sha1.
-
-        verbose (bool, default=None):
-            Passed to internal :class:`ubelt.Cacher` object
-
-        enabled (bool, default=True):
-            if False, expired always returns True
-
-        depends (str | List[str] | None):
-            Indicate dependencies of this cache.  If the dependencies change,
-            then the cache is recomputed.  New to CacheStamp in version 0.9.2.
-
-        meta (object | None):
-            Metadata that is also saved as a sidecar file.
-            New to CacheStamp in version 0.9.2.  Note: this is a candidate for
-            deprecation.
-
-        expires (str | int | datetime.datetime | datetime.timedelta | None):
-            If specified, sets an expiration date for the certificate. This can
-            be an absolute datetime or a timedelta offset. If specified as an
-            int, this is interpreted as a time delta in seconds.  If specified
-            as a str, this is interpreted as an absolute timestamp. Time delta
-            offsets are coerced to absolute times at "renew" time.
-
-        hash_prefix (None | str | List[str]):
-            If specified, we verify that these match the hash(s) of the
-            product(s) in the stamp certificate.
-
-        ext (str, default='.pkl'):
-            File extension for the cache format. Can be ``'.pkl'`` or
-            ``'.json'``.
-
-        cfgstr (str | None): DEPRECATED.
-
     Notes:
         The size, mtime, and hash mechanism is similar to how Makefile and redo
         caches work.
 
     Example:
         >>> import ubelt as ub
         >>> # Stamp the computation of expensive-to-compute.txt
@@ -794,14 +750,63 @@
         >>> # corrupting the output will cause the stamp to expire
         >>> product.write_text('very corrupted')
         >>> assert self.expired()
     """
     def __init__(self, fname, dpath, cfgstr=None, product=None, hasher='sha1',
                  verbose=None, enabled=True, depends=None, meta=None,
                  hash_prefix=None, expires=None, ext='.pkl'):
+        """
+        Args:
+            fname (str):
+                Name of the stamp file
+
+            dpath (str | PathLike | None):
+                Where to store the cached stamp file
+
+            product (str | PathLike | Sequence[str | PathLike] | None):
+                Path or paths that we expect the computation to produce. If
+                specified the hash of the paths are stored.
+
+            hasher (str):
+                The type of hasher used to compute the file hash of product.
+                If None, then we assume the file has not been corrupted or changed
+                if the mtime and size are the same. Defaults to sha1.
+
+            verbose (bool | None):
+                Passed to internal :class:`ubelt.Cacher` object. Defaults to None.
+
+            enabled (bool):
+                if False, expired always returns True. Defaults to True.
+
+            depends (str | List[str] | None):
+                Indicate dependencies of this cache.  If the dependencies change,
+                then the cache is recomputed.  New to CacheStamp in version 0.9.2.
+
+            meta (object | None):
+                Metadata that is also saved as a sidecar file.
+                New to CacheStamp in version 0.9.2.  Note: this is a candidate for
+                deprecation.
+
+            expires (str | int | datetime.datetime | datetime.timedelta | None):
+                If specified, sets an expiration date for the certificate. This can
+                be an absolute datetime or a timedelta offset. If specified as an
+                int, this is interpreted as a time delta in seconds.  If specified
+                as a str, this is interpreted as an absolute timestamp. Time delta
+                offsets are coerced to absolute times at "renew" time.
+
+            hash_prefix (None | str | List[str]):
+                If specified, we verify that these match the hash(s) of the
+                product(s) in the stamp certificate.
+
+            ext (str):
+                File extension for the cache format. Can be ``'.pkl'`` or
+                ``'.json'``. Defaults to ``'.pkl'``.
+
+            cfgstr (str | None): DEPRECATED.
+        """
         self.cacher = Cacher(fname, cfgstr=cfgstr, dpath=dpath,
                              verbose=verbose, enabled=enabled, depends=depends,
                              meta=meta, ext=ext)
         self.product = product
         self.hasher = hasher
         self.expires = expires
         self.hash_prefix = hash_prefix
@@ -829,15 +834,20 @@
         """
         Returns the stamp certificate if it exists
         """
         certificate = self.cacher.tryload(cfgstr=cfgstr, on_error='clear')
         return certificate
 
     def _rectify_products(self, product=None):
-        """ puts products in a normalized format """
+        """
+        puts products in a normalized format
+
+        Returns:
+            List[Path]
+        """
         from ubelt import util_path
         products = self.product if product is None else product
         if products is None:
             return None
         if not isinstance(products, (list, tuple)):
             products = [products]
         products = list(map(util_path.Path, products))
@@ -1173,14 +1183,18 @@
         return certificate
 
     def renew(self, cfgstr=None, product=None):
         """
         Recertify that the product has been recomputed by writing a new
         certificate to disk.
 
+        Args:
+            cfgstr (None | str): deprecated, do not use.
+            product (None | str | List): deprecated, do not use.
+
         Returns:
             None | dict: certificate information if enabled otherwise None.
 
         Example:
             >>> # Test that renew does nothing when the cacher is disabled
             >>> import ubelt as ub
             >>> dpath = ub.Path.appdir('ubelt/tests/cache-stamp-renew').ensuredir()
```

### Comparing `ubelt-1.3.2/ubelt/util_cache.pyi` & `ubelt-1.3.3/ubelt/util_cache.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,52 @@
+from typing import List
 from os import PathLike
 from typing import Callable
 from typing import Any
+from typing import Sequence
+import datetime
+import os
 from _typeshed import Incomplete
 from collections.abc import Generator
-from typing import Any
 
 
 class Cacher:
     VERBOSE: int
     FORCE_DISABLE: bool
-    dpath: Incomplete
-    fname: Incomplete
-    depends: Incomplete
-    cfgstr: Incomplete
-    verbose: Incomplete
-    ext: Incomplete
-    meta: Incomplete
-    enabled: Incomplete
-    protocol: Incomplete
-    hasher: Incomplete
-    log: Incomplete
-    backend: Incomplete
+    dpath: str | PathLike | None
+    fname: str
+    depends: str | List[str] | None
+    cfgstr: str | None
+    verbose: int
+    ext: str
+    meta: object | None
+    enabled: bool
+    protocol: int
+    hasher: str
+    log: Callable[[str], Any]
+    backend: str
 
     def __init__(self,
-                 fname,
-                 depends: Incomplete | None = ...,
-                 dpath: Incomplete | None = ...,
-                 appname: str = ...,
-                 ext: str = ...,
-                 meta: Incomplete | None = ...,
-                 verbose: Incomplete | None = ...,
-                 enabled: bool = ...,
-                 log: Incomplete | None = ...,
-                 hasher: str = ...,
+                 fname: str,
+                 depends: str | List[str] | None = None,
+                 dpath: str | PathLike | None = None,
+                 appname: str = 'ubelt',
+                 ext: str = '.pkl',
+                 meta: object | None = None,
+                 verbose: int | None = None,
+                 enabled: bool = True,
+                 log: Callable[[str], Any] | None = None,
+                 hasher: str = 'sha1',
                  protocol: int = ...,
-                 cfgstr: Incomplete | None = ...,
-                 backend: str = ...) -> None:
+                 cfgstr: str | None = None,
+                 backend: str = 'auto') -> None:
         ...
 
     @property
-    def fpath(self):
+    def fpath(self) -> os.PathLike:
         ...
 
     def get_fpath(self, cfgstr: str | None = None) -> str | PathLike:
         ...
 
     def exists(self, cfgstr: str | None = None) -> bool:
         ...
@@ -70,32 +73,34 @@
 
     def __call__(self, func: Callable):
         ...
 
 
 class CacheStamp:
     cacher: Incomplete
-    product: Incomplete
-    hasher: Incomplete
-    expires: Incomplete
-    hash_prefix: Incomplete
+    product: str | PathLike | Sequence[str | PathLike] | None
+    hasher: str
+    expires: str | int | datetime.datetime | datetime.timedelta | None
+    hash_prefix: None | str | List[str]
 
     def __init__(self,
-                 fname,
-                 dpath,
-                 cfgstr: Incomplete | None = ...,
-                 product: Incomplete | None = ...,
-                 hasher: str = ...,
-                 verbose: Incomplete | None = ...,
-                 enabled: bool = ...,
-                 depends: Incomplete | None = ...,
-                 meta: Incomplete | None = ...,
-                 hash_prefix: Incomplete | None = ...,
-                 expires: Incomplete | None = ...,
-                 ext: str = ...) -> None:
+                 fname: str,
+                 dpath: str | PathLike | None,
+                 cfgstr: str | None = None,
+                 product: str | PathLike | Sequence[str | PathLike]
+                 | None = None,
+                 hasher: str = 'sha1',
+                 verbose: bool | None = None,
+                 enabled: bool = True,
+                 depends: str | List[str] | None = None,
+                 meta: object | None = None,
+                 hash_prefix: None | str | List[str] = None,
+                 expires: str | int | datetime.datetime | datetime.timedelta
+                 | None = None,
+                 ext: str = '.pkl') -> None:
         ...
 
     @property
     def fpath(self):
         ...
 
     def clear(self):
@@ -103,10 +108,10 @@
 
     def expired(self,
                 cfgstr: Any | None = None,
                 product: Any | None = None) -> bool | str:
         ...
 
     def renew(self,
-              cfgstr: Incomplete | None = ...,
-              product: Incomplete | None = ...) -> None | dict:
+              cfgstr: None | str = None,
+              product: None | str | List = None) -> None | dict:
         ...
```

### Comparing `ubelt-1.3.2/ubelt/util_cmd.py` & `ubelt-1.3.3/ubelt/util_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,16 +100,16 @@
 #     level=logging.DEBUG,
 #     force=True
 # )
 # logger = logging.getLogger(__name__)
 
 __all__ = ['cmd']
 
-POSIX = 'posix' in sys.builtin_module_names
-WIN32 = sys.platform == 'win32'
+POSIX: bool = 'posix' in sys.builtin_module_names
+WIN32: bool = sys.platform == 'win32'
 
 
 class CmdOutput(dict):
     """
     An container that holds the output of :func:`ubelt.cmd`.
 
     This inherits from dictionary to be backwards compatible with older
```

### Comparing `ubelt-1.3.2/ubelt/util_cmd.pyi` & `ubelt-1.3.3/ubelt/util_cmd.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import List
 from os import PathLike
 from typing import Dict
-from _typeshed import Incomplete
 
 __pitch__: str
-POSIX: Incomplete
-WIN32: Incomplete
+POSIX: bool
+WIN32: bool
 
 
 class CmdOutput(dict):
 
     @property
     def stdout(self):
         ...
```

### Comparing `ubelt-1.3.2/ubelt/util_colors.py` & `ubelt-1.3.3/ubelt/util_colors.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/util_const.py` & `ubelt-1.3.3/ubelt/util_const.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/util_deprecate.py` & `ubelt-1.3.3/ubelt/util_deprecate.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/util_dict.py` & `ubelt-1.3.3/ubelt/util_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1013,15 +1013,15 @@
     like performing the operation on sets of keys. Value conflicts are handled
     with left-most priority (default for ``intersection`` and ``difference``),
     right-most priority (default for ``union`` and ``symmetric_difference``),
     or via a custom ``merge`` callable similar to [RubyMerge]_.
 
     The set operations are:
 
-        * union (or the ``|`` operator) combines multiple dicttionaries into
+        * union (or the ``|`` operator) combines multiple dictionaries into
             one. This is nearly identical to the update operation. Rightmost
             values take priority.
 
         * intersection (or the ``&`` operator). Takes the items from the
             first dictionary that share keys with the following dictionaries
             (or lists or sets of keys).  Leftmost values take priority.
 
@@ -1029,31 +1029,41 @@
             dictionary that do not share keys with following dictionaries.
             Leftmost values take priority.
 
         * symmetric_difference (or the ``^`` operator). Takes the items
             from all dictionaries where the key appears an odd number of times.
             Rightmost values take priority.
 
+    The full set of set operations was originally determined to be beyond the
+    scope of [Pep584]_, but there was discussion of these additional
+    operations. Some choices were ambiguous, but we believe this design could
+    be considered "natural".
+
     Note:
-        The reason righmost values take priority in union /
+        By default the right-most values take priority in union /
         symmetric_difference and left-most values take priority in intersection
-        / difference is:
+        / difference. In summary this is because we consider intersection /
+        difference to be "subtractive" operations, and union /
+        symmetric_difference to be "additive" operations. We expand on this in
+        the following points:
 
             1. intersection / difference is for removing keys --- i.e. is used
             to find values in the first (main) dictionary that are also in some
             other dictionary (or set or list of keys), whereas
 
             2. union is for adding keys --- i.e. it is basically just an alias
             for dict.update, so the new (rightmost) keys clobber the old.
 
-            3. symmetric_difference is somewhat strange. I'm don't have a great
-            argument for it, but it seemed easier to implement this way and it
-            does seem closer to a union than it is to a difference. Perhaps
-            unpaired union might have been a better name for this, but take
-            that up with the set theorists.
+            3. symmetric_difference is somewhat strange if you aren't familiar
+            with it. At a pure-set level it's not really a difference, its a
+            pairty operation (think of it more like xor or addition modulo 2).
+            You only keep items where the key appears an odd number of times.
+            Unlike intersection and difference, the results may not be a subset
+            of either input. The union has the same property. This symmetry
+            motivates having the newest (rightmost) keys cobber the old.
 
         Also, union / symmetric_difference does not make sense if arguments on
         the rights are lists/sets, whereas difference / intersection does.
 
     Note:
         The SetDict class only defines key-wise set operations.  Value-wise or
         item-wise operations are in general not hashable and therefore not
@@ -1061,14 +1071,15 @@
 
     TODO:
         - [ ] implement merge callables so the user can specify how to resolve
               value conflicts / combine values.
 
     References:
         .. [RubyMerge] https://ruby-doc.org/core-2.7.0/Hash.html#method-i-merge
+        .. [Pep584] https://peps.python.org/pep-0584/#what-about-the-full-set-api
 
     CommandLine:
         xdoctest -m ubelt.util_dict SetDict
 
     Example:
         >>> import ubelt as ub
         >>> a = ub.SetDict({'A': 'Aa', 'B': 'Ba',            'D': 'Da'})
```

### Comparing `ubelt-1.3.2/ubelt/util_dict.pyi` & `ubelt-1.3.3/ubelt/util_dict.pyi`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/util_download.py` & `ubelt-1.3.3/ubelt/util_download.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/util_download.pyi` & `ubelt-1.3.3/ubelt/util_download.pyi`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/util_download_manager.py` & `ubelt-1.3.3/ubelt/util_download_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,18 +5,14 @@
 __all__ = ['DownloadManager']
 
 
 class DownloadManager:
     """
     Simple implementation of the download manager
 
-    Attributes:
-        download_root (str | PathLike): default download location
-        jobs (List[concurrent.futures.Future]): list of jobs
-
     Example:
         >>> # xdoctest: +REQUIRES(--network)
         >>> import ubelt as ub
         >>> # Download a file with a known hash
         >>> manager = ub.DownloadManager()
         >>> job = manager.submit(
         >>>     'http://i.imgur.com/rqwaDag.png',
@@ -63,28 +59,34 @@
         >>>     fpath = job.result()
         >>>     print('fpath = {!r}'.format(fpath))
 
     """
     def __init__(self, download_root=None, mode='thread', max_workers=None,
                  cache=True):
         """
+        Args:
+            download_root (str | PathLike): default download location
+            mode (str): either thread, process, or serial
+            cache (bool): defaults to True
+            max_workers (int | None): maximum concurrent tasks
+
         TODO:
             - [ ] Will likely have to initialize and store some sort of
                   "connection state" objects.
         """
         import ubelt as ub
         if download_root is None:
             download_root = ub.ensure_app_config_dir('ubelt', 'dlman')
-        self.pool = ub.JobPool(mode=mode, max_workers=max_workers)
+        self._pool = ub.JobPool(mode=mode, max_workers=max_workers)
         self.download_root = download_root
         self.cache = cache
         if self.cache:
-            self.dl_func = ub.grabdata
+            self._dl_func = ub.grabdata
         else:
-            self.dl_func = ub.download
+            self._dl_func = ub.download
 
     def submit(self, url, dst=None, hash_prefix=None, hasher='sha256'):
         """
         Add a job to the download Queue
 
         Args:
             url (str | PathLike): pointer to the data to download
@@ -95,16 +97,16 @@
             hasher (str, default='sha256'):
                 hashing algorithm to use if hash_prefix is specified.
 
         Returns:
             concurrent.futures.Future :
                 a Future object that will point to the downloaded location.
         """
-        job = self.pool.submit(
-            self.dl_func, url, fname=dst, dpath=self.download_root,
+        job = self._pool.submit(
+            self._dl_func, url, fname=dst, dpath=self.download_root,
             hash_prefix=hash_prefix, hasher=hasher, verbose=0,
         )
         return job
 
     def as_completed(self, prog=None, desc=None, verbose=1):
         """
         Generate completed jobs as they become available
@@ -122,23 +124,23 @@
             >>> manager.shutdown()
 
         """
         if prog is True:
             import ubelt as ub
             prog = ub.ProgIter
         if prog is not None:
-            return prog(self.pool.as_completed(), total=len(self), desc=desc,
+            return prog(self._pool.as_completed(), total=len(self), desc=desc,
                         verbose=verbose)
         else:
-            return self.pool.as_completed()
+            return self._pool.as_completed()
 
     def shutdown(self):
         """
         Cancel all jobs and close all connections.
         """
-        self.pool.executor.shutdown()
+        self._pool.executor.shutdown()
 
     def __iter__(self):
         return self.as_completed()
 
     def __len__(self):
-        return len(self.pool)
+        return len(self._pool)
```

### Comparing `ubelt-1.3.2/ubelt/util_download_manager.pyi` & `ubelt-1.3.3/ubelt/util_download_manager.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from os import PathLike
-from typing import List
 import concurrent
 import concurrent.futures
 from _typeshed import Incomplete
 
 
 class DownloadManager:
     download_root: str | PathLike
-    jobs: List[concurrent.futures.Future]
-    pool: Incomplete
-    cache: Incomplete
-    dl_func: Incomplete
+    cache: bool
 
     def __init__(self,
-                 download_root: Incomplete | None = ...,
-                 mode: str = ...,
-                 max_workers: Incomplete | None = ...,
-                 cache: bool = ...) -> None:
+                 download_root: str | PathLike | None = None,
+                 mode: str = 'thread',
+                 max_workers: int | None = None,
+                 cache: bool = True) -> None:
         ...
 
     def submit(self,
                url: str | PathLike,
                dst: str | None = None,
                hash_prefix: str | None = None,
                hasher: str = 'sha256') -> concurrent.futures.Future:
```

### Comparing `ubelt-1.3.2/ubelt/util_format.py` & `ubelt-1.3.3/ubelt/util_format.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/util_func.py` & `ubelt-1.3.3/ubelt/util_func.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/util_futures.py` & `ubelt-1.3.3/ubelt/util_futures.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,14 +57,19 @@
 __all__ = ['Executor', 'JobPool']
 
 
 class SerialFuture(concurrent.futures.Future):
     """
     Non-threading / multiprocessing version of future for drop in compatibility
     with concurrent.futures.
+
+    Attributes:
+        func (Callable): function to be called
+        args (Tuple): positional arguments to call the function with
+        kw (Dict): keyword arguments to call the function with
     """
     def __init__(self, func, *args, **kw):
         super(SerialFuture, self).__init__()
         self.func = func
         self.args = args
         self.kw = kw
         # self._condition = FakeCondition()
@@ -260,14 +265,17 @@
 
     SeeAlso:
         * :class:`concurrent.futures.ThreadPoolExecutor`
         * :class:`concurrent.futures.ProcessPoolExecutor`
         * :class:`SerialExecutor`
         * :class:`JobPool`
 
+    Attributes:
+        backend (SerialExecutor | ThreadPoolExecutor | ProcessPoolExecutor):
+
     Example:
         >>> import ubelt as ub
         >>> # Prototype code using simple serial processing
         >>> executor = ub.Executor(mode='serial', max_workers=0)
         >>> jobs = [executor.submit(sum, [i + 1, i]) for i in range(10)]
         >>> print([job.result() for job in jobs])
         [1, 3, 5, 7, 9, 11, 13, 15, 17, 19]
@@ -373,26 +381,18 @@
     Abstracts away boilerplate of submitting and collecting jobs
 
     This is a basic wrapper around :class:`ubelt.util_futures.Executor` that
     simplifies the most basic case by 1. keeping track of references to
     submitted futures for you and 2. providing an as_completed method to
     consume those futures as they are ready.
 
-    Args:
-        mode (str):
-            The backend parallelism mechanism.  Can be either thread, serial,
-            or process. Defaults to 'thread'.
-
-        max_workers (int):
-            number of workers. If 0, serial is forced. Defaults to 0.
-
-        transient (bool):
-            if True, references to jobs will be discarded as they are
-            returned by :func:`as_completed`. Otherwise the ``jobs`` attribute
-            holds a reference to all jobs ever submitted. Default to False.
+    Attributes:
+        executor (Executor): internal executor object
+        jobs (List[Future]): internal job list. Note: do not rely on this attribute, it
+            may change in the future.
 
     Example:
         >>> import ubelt as ub
         >>> def worker(data):
         >>>     return data + 1
         >>> pool = ub.JobPool('thread', max_workers=16)
         >>> for data in ub.ProgIter(range(10), desc='submit jobs'):
@@ -400,14 +400,28 @@
         >>> final = []
         >>> for job in pool.as_completed(desc='collect jobs'):
         >>>     info = job.result()
         >>>     final.append(info)
         >>> print('final = {!r}'.format(final))
     """
     def __init__(self, mode='thread', max_workers=0, transient=False):
+        """
+        Args:
+            mode (str):
+                The backend parallelism mechanism.  Can be either thread, serial,
+                or process. Defaults to 'thread'.
+
+            max_workers (int):
+                number of workers. If 0, serial is forced. Defaults to 0.
+
+            transient (bool):
+                if True, references to jobs will be discarded as they are
+                returned by :func:`as_completed`. Otherwise the ``jobs`` attribute
+                holds a reference to all jobs ever submitted. Default to False.
+        """
         self.executor = Executor(mode=mode, max_workers=max_workers)
         self.transient = transient
         self.jobs = []
 
     def __len__(self):
         return len(self.jobs)
```

### Comparing `ubelt-1.3.2/ubelt/util_futures.pyi` & `ubelt-1.3.3/ubelt/util_futures.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+from typing import Callable
+from typing import Tuple
+from typing import Dict
 from typing import Type
 from types import TracebackType
 import concurrent
 import concurrent.futures
-from typing import Callable
+from concurrent.futures import Future
 from typing import Any
+from concurrent.futures import ThreadPoolExecutor
+from concurrent.futures import ProcessPoolExecutor
 from typing import List
-import concurrent.futures
-from _typeshed import Incomplete
 from collections.abc import Generator
-from typing import Any
 
 
 class SerialFuture(concurrent.futures.Future):
-    func: Incomplete
-    args: Incomplete
-    kw: Incomplete
+    func: Callable
+    args: Tuple
+    kw: Dict
 
     def __init__(self, func, *args, **kw) -> None:
         ...
 
     def set_result(self, result) -> None:
         ...
 
@@ -42,15 +44,15 @@
 
     def map(self, fn: Callable[..., Any], *iterables,
             **kwargs) -> Generator[Any, None, None]:
         ...
 
 
 class Executor:
-    backend: Incomplete
+    backend: SerialExecutor | ThreadPoolExecutor | ProcessPoolExecutor
 
     def __init__(self, mode: str = 'thread', max_workers: int = 0) -> None:
         ...
 
     def __enter__(self):
         ...
 
@@ -66,22 +68,22 @@
         ...
 
     def map(self, fn, *iterables, **kwargs):
         ...
 
 
 class JobPool:
-    executor: Incomplete
-    transient: Incomplete
-    jobs: Incomplete
+    executor: Executor
+    jobs: List[Future]
+    transient: bool
 
     def __init__(self,
-                 mode: str = ...,
-                 max_workers: int = ...,
-                 transient: bool = ...) -> None:
+                 mode: str = 'thread',
+                 max_workers: int = 0,
+                 transient: bool = False) -> None:
         ...
 
     def __len__(self):
         ...
 
     def submit(self, func: Callable[..., Any], *args,
                **kwargs) -> concurrent.futures.Future:
```

### Comparing `ubelt-1.3.2/ubelt/util_hash.py` & `ubelt-1.3.3/ubelt/util_hash.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 from ubelt.util_const import NoParam
 
 __all__ = ['hash_data', 'hash_file']
 
 # incremented when we make a change that modifies hashes
 HASH_VERSION = 2  # type: int
 
-_ALPHABET_10 = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
+_ALPHABET_10 = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']  # type: List[str]
 
 _ALPHABET_16 = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9',
                 'a', 'b', 'c', 'd', 'e', 'f']
 
 _ALPHABET_26 = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j',
                 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't',
                 'u', 'v', 'w', 'x', 'y', 'z']
```

### Comparing `ubelt-1.3.2/ubelt/util_hash.pyi` & `ubelt-1.3.3/ubelt/util_hash.pyi`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/util_import.py` & `ubelt-1.3.3/ubelt/util_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     Warning:
         Even though this context manager takes precautions, this modifies
         ``sys.path``, and things can go wrong when that happens.  This is
         generally safe as long as nothing else you do inside of this context
         modifies the path. If the path is modified in this context, we will try
         to detect it and warn.
 
-    Args:
+    Attributes:
         dpath (str | PathLike): directory to insert into the PYTHONPATH
         index (int): position to add to. Typically either -1 or 0.
 
     Example:
         >>> from ubelt.util_import import PythonPathContext
         >>> import sys
         >>> with PythonPathContext('foo', -1):
@@ -74,14 +74,19 @@
         >>> self.__enter__()
         >>> sys.path.remove('foo')
         >>> import pytest
         >>> with pytest.raises(RuntimeError):
         >>>     self.__exit__(None, None, None)
     """
     def __init__(self, dpath, index=0):
+        """
+        Args:
+            dpath (str | PathLike): directory to insert into the PYTHONPATH
+            index (int): position to add to. Typically either -1 or 0.
+        """
         self.dpath = os.fspath(dpath)
         self.index = index
 
     def __enter__(self):
         if self.index < 0:
             self.index = len(sys.path) + self.index + 1
         sys.path.insert(self.index, self.dpath)
```

### Comparing `ubelt-1.3.2/ubelt/util_import.pyi` & `ubelt-1.3.3/ubelt/util_import.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
+from os import PathLike
 from typing import Type
 from types import TracebackType
-from os import PathLike
 from types import ModuleType
 from typing import List
 from typing import Tuple
-from _typeshed import Incomplete
 
 
 class PythonPathContext:
-    dpath: Incomplete
-    index: Incomplete
+    dpath: str | PathLike
+    index: int
 
-    def __init__(self, dpath, index: int = ...) -> None:
+    def __init__(self, dpath: str | PathLike, index: int = 0) -> None:
         ...
 
     def __enter__(self) -> None:
         ...
 
     def __exit__(self, ex_type: Type[BaseException] | None,
                  ex_value: BaseException | None,
```

### Comparing `ubelt-1.3.2/ubelt/util_indexable.py` & `ubelt-1.3.3/ubelt/util_indexable.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/util_indexable.pyi` & `ubelt-1.3.3/ubelt/util_indexable.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Tuple
 from typing import List
 from typing import Any
 from typing import Dict
 from _typeshed import Incomplete
 from collections.abc import Generator
-from typing import Any
 
 
 class IndexableWalker(Generator):
     data: dict | list | tuple
     dict_cls: Tuple[type]
     list_cls: Tuple[type]
     indexable_cls: Incomplete
```

### Comparing `ubelt-1.3.2/ubelt/util_io.py` & `ubelt-1.3.3/ubelt/util_io.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/util_io.pyi` & `ubelt-1.3.3/ubelt/util_io.pyi`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/util_links.py` & `ubelt-1.3.3/ubelt/util_links.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/util_list.py` & `ubelt-1.3.3/ubelt/util_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,28 +37,14 @@
 class chunks(object):
     """
     Generates successive n-sized chunks from ``items``.
 
     If the last chunk has less than n elements, ``bordermode`` is used to
     determine fill values.
 
-    Args:
-        items (Iterable[T]): input to iterate over
-
-        chunksize (int): size of each sublist yielded
-
-        nchunks (int): number of chunks to create (
-            cannot be specified if chunksize is specified)
-
-        bordermode (str): determines how to handle the last case if the
-            length of the input is not divisible by chunksize valid values
-            are: {'none', 'cycle', 'replicate'}
-
-        total (int): hints about the length of the input
-
     Note:
         FIXME:
             When nchunks is given, that's how many chunks we should get
             but the issue is that chunksize is not well defined in that instance
             For instance how do we turn a list with 4 elements into 3 chunks
             where does the extra item go?
 
@@ -151,14 +137,33 @@
         >>> df = pd.DataFrame(rows)
         >>> for _, subdf in df.groupby('chunker'):
         >>>     print(subdf)
 
     """
     def __init__(self, items, chunksize=None, nchunks=None, total=None,
                  bordermode='none', legacy=False):
+        """
+        Args:
+            items (Iterable): input to iterate over
+
+            chunksize (int | None): size of each sublist yielded
+
+            nchunks (int | None): number of chunks to create (
+                cannot be specified if chunksize is specified)
+
+            bordermode (str): determines how to handle the last case if the
+                length of the input is not divisible by chunksize valid values
+                are: {'none', 'cycle', 'replicate'}
+
+            total (int | None): hints about the length of the input
+
+            legacy (bool):
+                if True use old behavior, defaults to False. This will be
+                removed in the future.
+        """
         if nchunks is not None and chunksize is not None:  # nocover
             raise ValueError('Cannot specify both chunksize and nchunks')
         if nchunks is None and chunksize is None:  # nocover
             raise ValueError('Must specify either chunksize or nchunks')
 
         if total is None:
             try:
@@ -175,32 +180,32 @@
             remainder = 0
         else:
             if total is None:
                 raise ValueError(
                     'Need to specify total to use nchunks on an iterable '
                     'without length hints')
             if legacy:
-                chunksize = int(math.ceil(total / nchunks))
+                chunksize: int = int(math.ceil(total / nchunks))
                 remainder = 0
             else:
                 if bordermode == 'none':
                     # I feel like this could be simpler
-                    chunksize = max(int(math.floor(total / nchunks)), 1)
-                    nchunks = min(int(math.ceil(total / chunksize)), nchunks)
-                    chunked_total = chunksize * nchunks
-                    remainder = total - chunked_total
+                    chunksize: int = max(int(math.floor(total / nchunks)), 1)
+                    nchunks: int = min(int(math.ceil(total / chunksize)), nchunks)
+                    chunked_total: int = chunksize * nchunks
+                    remainder: int = total - chunked_total
                 else:
                     # not working
-                    chunksize = max(int(math.ceil(total / nchunks)), 1)
+                    chunksize: int = max(int(math.ceil(total / nchunks)), 1)
                     # Can artificially extend the size in this case
                     # total = chunksize * nchunks
                     remainder = 0
 
         self.legacy = legacy
-        self.remainder = remainder
+        self.remainder: int = remainder
         self.items = items
         self.total = total
         self.nchunks = nchunks
         self.chunksize = chunksize
         self.bordermode = bordermode
 
     def __len__(self):
```

### Comparing `ubelt-1.3.2/ubelt/util_list.pyi` & `ubelt-1.3.3/ubelt/util_list.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,39 @@
+from typing import Iterable
 from typing import Mapping
 from typing import Sequence
-from typing import Iterable
 from typing import Any
 from typing import Callable
 from typing import Iterator
 from typing import List
 from _typeshed import Incomplete
 from collections.abc import Generator
 from typing import Any, TypeVar
 
 VT = TypeVar("VT")
 T = TypeVar("T")
 KT = TypeVar("KT")
 
 
 class chunks:
-    legacy: Incomplete
+    legacy: bool
     remainder: Incomplete
-    items: Incomplete
-    total: Incomplete
-    nchunks: Incomplete
-    chunksize: Incomplete
-    bordermode: Incomplete
+    items: Iterable
+    total: int | None
+    nchunks: int | None
+    chunksize: int | None
+    bordermode: str
 
     def __init__(self,
-                 items,
-                 chunksize: Incomplete | None = ...,
-                 nchunks: Incomplete | None = ...,
-                 total: Incomplete | None = ...,
-                 bordermode: str = ...,
-                 legacy: bool = ...) -> None:
+                 items: Iterable,
+                 chunksize: int | None = None,
+                 nchunks: int | None = None,
+                 total: int | None = None,
+                 bordermode: str = 'none',
+                 legacy: bool = False) -> None:
         ...
 
     def __len__(self):
         ...
 
     def __iter__(self):
         ...
```

### Comparing `ubelt-1.3.2/ubelt/util_memoize.py` & `ubelt-1.3.3/ubelt/util_memoize.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,17 @@
 class memoize_method(object):
     """
     memoization decorator for a method that respects args and kwargs
 
     References:
         .. [ActiveState_Miller_2010] http://code.activestate.com/recipes/577452-a-memoize-decorator-for-instance-methods
 
+    Attributes:
+        __func__ (Callable): the wrapped function
+
     Example:
         >>> import ubelt as ub
         >>> closure = {'a': 'b', 'c': 'd'}
         >>> incr = [0]
         >>> class Foo(object):
         >>>     @ub.memoize_method
         >>>     def foo_memo(self, key):
@@ -200,14 +203,18 @@
         >>> assert incr[0] == 7
         >>> self2.foo_memo('a')
         >>> assert incr[0] == 7
         >>> assert self.foo_memo.__doc__ == 'Wrapped foo_memo docstr'
         >>> assert self.foo_memo.__name__ == 'foo_memo'
     """
     def __init__(self, func):
+        """
+        Args:
+            func (Callable): method to wrap
+        """
         self._func = func
         self._cache_name = '_cache__' + func.__name__
         # Mimic attributes of a bound method
         self.__func__ = func
         functools.update_wrapper(self, func)
 
     def __get__(self, instance, cls=None):
@@ -246,14 +253,17 @@
 
     Note:
         implementation is a modified version of [estebistec_memoize]_.
 
     References:
         .. [estebistec_memoize] https://github.com/estebistec/python-memoized-property
 
+    Args:
+        fget (property | Callable): A property or a method.
+
     Example:
         >>> import ubelt as ub
         >>> class C(object):
         ...     load_name_count = 0
         ...     @ub.memoize_property
         ...     def name(self):
         ...         "name's docstring"
```

### Comparing `ubelt-1.3.2/ubelt/util_mixins.py` & `ubelt-1.3.3/ubelt/util_mixins.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     >>> print('g = {}'.format(g))
     g = <Group(3)>
 
 """
 import warnings
 
 
-class NiceRepr(object):
+class NiceRepr:
     """
     Inherit from this class and define ``__nice__`` to "nicely" print your
     objects.
 
     Defines ``__str__`` and ``__repr__`` in terms of ``__nice__`` function
     Classes that inherit from :class:`NiceRepr` should redefine ``__nice__``.
     If the inheriting class has a ``__len__``, method then the default
@@ -119,33 +119,45 @@
         <Cat()>
         <Dog()>
         <Beagle()>
         <Ragdoll()>
     """
 
     def __nice__(self):
+        """
+        Returns:
+            str
+        """
         if hasattr(self, '__len__'):
             # It is a common pattern for objects to use __len__ in __nice__
             # As a convenience we define a default __nice__ for these objects
             return str(len(self))
         else:
             # In all other cases force the subclass to overload __nice__
             raise NotImplementedError(
                 'Define the __nice__ method for {!r}'.format(self.__class__))
 
     def __repr__(self):
+        """
+        Returns:
+            str
+        """
         try:
             nice = self.__nice__()
             classname = self.__class__.__name__
             return '<{0}({1}) at {2}>'.format(classname, nice, hex(id(self)))
         except Exception as ex:
             warnings.warn(str(ex), category=RuntimeWarning)
             return object.__repr__(self)
 
     def __str__(self):
+        """
+        Returns:
+            str
+        """
         try:
             classname = self.__class__.__name__
             nice = self.__nice__()
             return '<{0}({1})>'.format(classname, nice)
         except Exception as ex:
             warnings.warn(str(ex), category=RuntimeWarning)
             return object.__repr__(self)
```

### Comparing `ubelt-1.3.2/ubelt/util_path.py` & `ubelt-1.3.3/ubelt/util_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,48 +372,55 @@
         >>>         # Dont change dirs, but reset to your cwd at context end
         >>>         with ChDir('.'):
         >>>             os.chdir(dir2)
         >>>         assert ub.Path.cwd() == dir1
         >>>     assert ub.Path.cwd() == dpath
     """
     def __init__(self, dpath):
-        self.context_dpath = dpath
-        self.orig_dpath = None
+        self._context_dpath = dpath
+        self._orig_dpath = None
 
     def __enter__(self):
-        if self.context_dpath is not None:
-            self.orig_dpath = os.getcwd()
-            os.chdir(self.context_dpath)
+        """
+        Returns:
+            ChDir: self
+        """
+        if self._context_dpath is not None:
+            self._orig_dpath = os.getcwd()
+            os.chdir(self._context_dpath)
         return self
 
     def __exit__(self, ex_type, ex_value, ex_traceback):
         """
         Args:
             ex_type (Type[BaseException] | None):
             ex_value (BaseException | None):
             ex_traceback (TracebackType | None):
 
         Returns:
             bool | None
         """
-        if self.context_dpath is not None:
-            os.chdir(self.orig_dpath)
+        if self._context_dpath is not None:
+            os.chdir(self._orig_dpath)
 
 
 class TempDir:
     """
     Context for creating and cleaning up temporary directories.
 
     DEPRECATED. Use `tempfile` instead.
 
     Note:
         This exists because :class:`tempfile.TemporaryDirectory` was
         introduced in Python 3.2. Thus once ubelt no longer supports
         python 2.7, this class will be deprecated.
 
+    Attributes:
+        dpath (str | None)
+
     Note:
         # WE MAY WANT TO KEEP THIS FOR WINDOWS.
 
     Example:
         >>> from ubelt.util_path import *  # NOQA
         >>> with TempDir() as self:
         >>>     dpath = self.dpath
```

### Comparing `ubelt-1.3.2/ubelt/util_path.pyi` & `ubelt-1.3.3/ubelt/util_path.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -36,21 +36,19 @@
               mode: int = 1023,
               verbose: int = 0,
               recreate: bool = False) -> str:
     ...
 
 
 class ChDir:
-    context_dpath: Incomplete
-    orig_dpath: Incomplete
 
     def __init__(self, dpath) -> None:
         ...
 
-    def __enter__(self):
+    def __enter__(self) -> ChDir:
         ...
 
     def __exit__(self, ex_type: Type[BaseException] | None,
                  ex_value: BaseException | None,
                  ex_traceback: TracebackType | None) -> bool | None:
         ...
```

### Comparing `ubelt-1.3.2/ubelt/util_platform.py` & `ubelt-1.3.3/ubelt/util_platform.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/util_platform.pyi` & `ubelt-1.3.3/ubelt/util_platform.pyi`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/util_repr.py` & `ubelt-1.3.3/ubelt/util_repr.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,74 +87,79 @@
             dict values use str instead of repr
 
         nl, newlines (int | bool):
             number of top level nestings to place a newline after. If true all
             items are followed by newlines regardless of nesting level.
             Defaults to 1 for lists and True for dicts.
 
-        nobr, nobraces (bool, default=False):
-            if True, text will not contain outer braces for containers
+        nobr, nobraces (bool):
+            if True, text will not contain outer braces for containers.
+            Defaults to False.
 
-        cbr, compact_brace (bool, default=False):
+        cbr, compact_brace (bool):
             if True, braces are compactified (i.e. they will not have newlines
-            placed directly after them, think java / K&R / 1TBS)
+            placed directly after them, think java / K&R / 1TBS).
+            Defaults to False.
 
         trailsep, trailing_sep (bool):
             if True, a separator is placed after the last item in a sequence.
             By default this is True if there are any ``nl > 0``.
 
-        explicit (bool, default=False):
+        explicit (bool):
             changes dict representation from ``{k1: v1, ...}`` to
-            ``dict(k1=v1, ...)``.
+            ``dict(k1=v1, ...)``.  Defaults to False.
 
             Modifies:
                 default kvsep is modified to  ``'='``
                 dict braces from `{}` to `dict()`.
 
-        compact (bool, default=False):
+        compact (bool):
             Produces values more suitable for space constrianed environments
+            Defaults to False.
 
             Modifies:
                 default kvsep is modified to ``'='``
                 default itemsep is modified to  ``''``
                 default nobraces is modified to ``1``.
                 default newlines is modified to ``0``.
                 default strkeys to ``True``
                 default strvals to ``True``
 
-        precision (int, default=None):
-            if specified floats are formatted with this precision
+        precision (int | None):
+            if specified floats are formatted with this precision.
+            Defaults to None
 
-        kvsep (str, default=': '):
-            separator between keys and values
+        kvsep (str):
+            separator between keys and values. Defaults to ': '
 
-        itemsep (str, default=' '):
+        itemsep (str):
             separator between items. This separator is placed after commas,
             which are currently not configurable. This may be modified in the
-            future.
+            future. Defaults to ' '.
 
-        sort (bool | callable, default='auto'):
+        sort (bool | callable | None):
             if 'auto', then sort unordered collections, but keep the ordering
             of ordered collections. This option attempts to be deterministic in
-            most cases.
+            most cases. Defaults to None.
 
             if True, then ALL collections will be sorted in the returned text.
 
         suppress_small (bool):
             passed to :func:`numpy.array2string` for ndarrays
 
         max_line_width (int):
             passed to :func:`numpy.array2string` for ndarrays
 
         with_dtype (bool):
             only relevant to numpy.ndarrays. if True includes the dtype.
             Defaults to `not strvals`.
 
-        align (bool | str, default=False):
-            if True, will align multi-line dictionaries by the kvsep
+        align (bool | str):
+            if True, will align multi-line dictionaries by the kvsep.
+            Defaults to False.
 
         extensions (ReprExtensions):
             a custom :class:`ReprExtensions` instance that can overwrite
             or define how different types of objects are formatted.
 
     Returns:
         str: outstr - output string
@@ -384,14 +389,20 @@
             return func
         return _decorator
 
     def lookup(self, data):
         """
         Returns an appropriate function to format ``data`` if one has been
         registered.
+
+        Args:
+            data (Any): an instance that may have a registered formatter
+
+        Returns:
+            Callable: the formatter for the given type
         """
         # Evaluate the lazy queue if anything is in it
         if self._lazy_queue:
             for func in self._lazy_queue:
                 func()
             self._lazy_queue = []
 
@@ -692,27 +703,29 @@
     Args:
         dict_ (dict):  a dictionary
         **kwargs: si, stritems, strkeys, strvals, sk, sv, nl, newlines, nobr,
                   nobraces, cbr, compact_brace, trailing_sep,
                   explicit, itemsep, precision, kvsep, sort
 
     Kwargs:
-        sort (None, default=None):
+        sort (None):
             if True, sorts ALL collections and subcollections,
             note, collections with undefined orders (e.g. dicts, sets) are
-            sorted by default.
+            sorted by default. Defaults to None.
 
-        nl (int, default=None):
-            preferred alias for newline. can be a countdown variable
+        nl (int | None):
+            preferred alias for newline. can be a countdown variable.
+            Defaults to None.
 
-        explicit (int, default=False):
+        explicit (int | bool):
             can be a countdown variable.
-            if True, uses dict(a=b) syntax instead of {'a': b}
+            if True, uses dict(a=b) syntax instead of {'a': b}.
+            Defaults to False.
 
-        nobr (bool, default=False): removes outer braces
+        nobr (bool): removes outer braces. Defaults to False.
 
     Returns:
         Tuple[str, Dict] : retstr, _leaf_info
 
     Example:
         >>> from ubelt.util_repr import *  # NOQA
         >>> dict_ = {'a': 'edf', 'bc': 'ghi'}
```

### Comparing `ubelt-1.3.2/ubelt/util_str.py` & `ubelt-1.3.3/ubelt/util_str.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/util_stream.py` & `ubelt-1.3.3/ubelt/util_stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,34 +19,40 @@
 
 
 class TeeStringIO(io.StringIO):
     """
     An IO object that writes to itself and another IO stream.
 
     Attributes:
-        redirect (io.IOBase): The other stream to write to.
+        redirect (io.IOBase | None): The other stream to write to.
 
     Example:
         >>> import ubelt as ub
         >>> redirect = io.StringIO()
         >>> self = ub.TeeStringIO(redirect)
     """
     def __init__(self, redirect=None):
+        """
+        Args:
+            redirect (io.IOBase): The other stream to write to.
+        """
         self.redirect = redirect  # type: io.IOBase
         super().__init__()
 
         # Logic taken from prompt_toolkit/output/vt100.py version 3.0.5 in
         # flush I don't have a full understanding of what the buffer
         # attribute is supposed to be capturing here, but this seems to
         # allow us to embed in IPython while still capturing and Teeing
         # stdout
         if hasattr(redirect, 'buffer'):
             self.buffer = redirect.buffer  # Py3.
         else:
             self.buffer = redirect
+        # Note: mypy doesn't like this type
+        # buffer (io.BufferedIOBase | io.IOBase | None): the redirected buffer attribute
 
     def isatty(self):  # nocover
         """
         Returns true of the redirect is a terminal.
 
         Note:
             Needed for ``IPython.embed`` to work properly when this class is
@@ -116,25 +122,24 @@
     """
 
 
 class CaptureStdout(CaptureStream):
     r"""
     Context manager that captures stdout and stores it in an internal stream
 
-    Args:
-        suppress (bool, default=True):
-            if True, stdout is not printed while captured
-        enabled (bool, default=True):
-            does nothing if this is False
-        **kwargs : used for backwards compatibility with misspelled
-            deprecated params.
-
     SeeAlso:
         :func:`contextlib.redirect_stdout`
 
+    Attributes:
+        text (str | None): internal storage for the most recent part
+        parts (List[str]): internal storage for all parts
+        cap_stdout (None | TeeStringIO): internal stream proxy
+        orig_stdout (io.TextIOBase): internal pointer to the original stdout
+            stream
+
     Example:
         >>> import ubelt as ub
         >>> self = ub.CaptureStdout(suppress=True)
         >>> print('dont capture the table flip (╯°□°）╯︵ ┻━┻')
         >>> with self:
         ...     text = 'capture the heart ♥'
         ...     print(text)
@@ -153,14 +158,21 @@
         >>> import ubelt as ub
         >>> self = ub.CaptureStdout(suppress=True, enabled=False)
         >>> with self:
         ...     print('dont capture')
         >>> assert self.text is None
     """
     def __init__(self, suppress=True, enabled=True):
+        """
+        Args:
+            suppress (bool): if True, stdout is not printed while captured.
+                Defaults to True.
+            enabled (bool):
+                does nothing if this is False. Defaults to True.
+        """
         self.text = None
         self._pos = 0  # keep track of how much has been logged
         self.parts = []
         self.started = False
         self.cap_stdout = None
         self.enabled = enabled
         self.suppress = suppress
```

### Comparing `ubelt-1.3.2/ubelt/util_stream.pyi` & `ubelt-1.3.3/ubelt/util_time.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,49 @@
-import io
+import datetime
 from typing import Type
 from types import TracebackType
-import io
 from _typeshed import Incomplete
 
 
-class TeeStringIO(io.StringIO):
-    redirect: io.IOBase
-    buffer: Incomplete
-
-    def __init__(self, redirect: Incomplete | None = ...) -> None:
-        ...
-
-    def isatty(self):
-        ...
-
-    def fileno(self):
-        ...
-
-    @property
-    def encoding(self):
-        ...
-
-    def write(self, msg):
-        ...
-
-    def flush(self):
-        ...
-
-
-class CaptureStream:
+def timestamp(datetime: datetime.datetime | datetime.date | None = None,
+              precision: int = 0,
+              default_timezone: str | datetime.timezone = 'local',
+              allow_dateutil: bool = True) -> str:
     ...
 
 
-class CaptureStdout(CaptureStream):
-    text: Incomplete
-    parts: Incomplete
-    started: bool
-    cap_stdout: Incomplete
-    enabled: Incomplete
-    suppress: Incomplete
-    orig_stdout: Incomplete
+def timeparse(stamp: str,
+              default_timezone: str = 'local',
+              allow_dateutil: bool = True) -> datetime.datetime:
+    ...
 
-    def __init__(self, suppress: bool = ..., enabled: bool = ...) -> None:
-        ...
 
-    def log_part(self) -> None:
+class Timer:
+    elapsed: float
+    tstart: float
+    label: Incomplete
+    verbose: Incomplete
+    newline: Incomplete
+    write: Incomplete
+    flush: Incomplete
+    ns: Incomplete
+
+    def __init__(self,
+                 label: str = ...,
+                 verbose: Incomplete | None = ...,
+                 newline: bool = ...,
+                 ns: bool = ...) -> None:
         ...
 
-    def start(self) -> None:
+    def tic(self):
         ...
 
-    def stop(self) -> None:
+    def toc(self):
         ...
 
     def __enter__(self):
         ...
 
-    def __del__(self) -> None:
-        ...
-
-    def close(self) -> None:
-        ...
-
     def __exit__(self, ex_type: Type[BaseException] | None,
                  ex_value: BaseException | None,
                  ex_traceback: TracebackType | None) -> bool | None:
         ...
```

### Comparing `ubelt-1.3.2/ubelt/util_time.py` & `ubelt-1.3.3/ubelt/util_time.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt/util_time.pyi` & `ubelt-1.3.3/ubelt/util_zip.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,50 @@
-import datetime
+from os import PathLike
+from typing import Tuple
 from typing import Type
 from types import TracebackType
 from _typeshed import Incomplete
+from ubelt.util_mixins import NiceRepr
 
 
-def timestamp(datetime: datetime.datetime | datetime.date | None = None,
-              precision: int = 0,
-              default_timezone: str | datetime.timezone = 'local',
-              allow_dateutil: bool = True) -> str:
+def split_archive(fpath: str | PathLike,
+                  ext: str = '.zip') -> Tuple[str, str | None]:
     ...
 
 
-def timeparse(stamp: str,
-              default_timezone: str = 'local',
-              allow_dateutil: bool = True) -> datetime.datetime:
-    ...
+class zopen(NiceRepr):
+    fpath: str | PathLike
+    ext: str
+    name: Incomplete
+    mode: str
 
+    def __init__(self,
+                 fpath: str | PathLike,
+                 mode: str = 'r',
+                 seekable: bool = False,
+                 ext: str = '.zip') -> None:
+        ...
 
-class Timer:
-    elapsed: float
-    tstart: float
-    label: Incomplete
-    verbose: Incomplete
-    newline: Incomplete
-    write: Incomplete
-    flush: Incomplete
-    ns: Incomplete
+    @property
+    def zfile(self):
+        ...
 
-    def __init__(self,
-                 label: str = ...,
-                 verbose: Incomplete | None = ...,
-                 newline: bool = ...,
-                 ns: bool = ...) -> None:
+    def namelist(self):
+        ...
+
+    def __nice__(self):
+        ...
+
+    def __getattr__(self, key):
         ...
 
-    def tic(self):
+    def __dir__(self):
         ...
 
-    def toc(self):
+    def __del__(self) -> None:
         ...
 
     def __enter__(self):
         ...
 
     def __exit__(self, ex_type: Type[BaseException] | None,
                  ex_value: BaseException | None,
```

### Comparing `ubelt-1.3.2/ubelt/util_zip.py` & `ubelt-1.3.3/ubelt/util_zip.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,21 @@
 
 
 def split_archive(fpath, ext='.zip'):
     """
     If fpath specifies a file inside a zipfile, it breaks it into two parts the
     path to the zipfile and the internal path in the zipfile.
 
+    Args:
+        fpath (str | PathLike): path that specifies a path inside of an archive
+        ext (str): archive extension
+
+    Returns:
+        Tuple[str, str | None]
+
     Example:
         >>> split_archive('/a/b/foo.txt')
         >>> split_archive('/a/b/foo.zip/bar.txt')
         >>> split_archive('/a/b/foo.zip/baz/biz.zip/bar.py')
         >>> split_archive('archive.zip')
         >>> import ubelt as ub
         >>> split_archive(ub.Path('/a/b/foo.zip/baz/biz.zip/bar.py'))
@@ -84,34 +91,14 @@
 
     TODO:
         - [ ] Fast way to open a base zipfile, query what is inside, and
               then choose a file to further zopen (and passing along the same
               open zipfile reference maybe?).
         - [ ] Write mode in some restricted setting?
 
-    Args:
-        fpath (str | PathLike):
-            path to a file, or a special path that denotes both a
-            path to a zipfile and a path to a archived file inside of
-            the zipfile.
-
-        mode (str):
-            Currently only "r" - readonly mode is supported
-
-        seekable (bool):
-            If True, attempts to force "seekability" of the underlying
-            file-object, for compressed files this will first extract
-            the file to a temporary location on disk.  If False, any underlying
-            compressed file will be opened directly which may result in the
-            object being non-seekable.
-
-        ext (str):
-            The extension of the zipfile. Modify this is a non-standard
-            extension is used (e.g. for torch packages).
-
     Example:
         >>> from ubelt.util_zip import *  # NOQA
         >>> import pickle
         >>> import ubelt as ub
         >>> dpath = ub.Path.appdir('ubelt/tests/util_zip').ensuredir()
         >>> dpath = ub.Path(dpath)
         >>> data_fpath = dpath / 'test.pkl'
@@ -236,14 +223,35 @@
         >>> print('self = {!r}'.format(self))
         >>> # pathological
         >>> self = zopen(existing_fpath, 'r')
         >>> self._handle = None
         >>> dir(self)
     """
     def __init__(self, fpath, mode='r', seekable=False, ext='.zip'):
+        """
+        Args:
+            fpath (str | PathLike):
+                path to a file, or a special path that denotes both a
+                path to a zipfile and a path to a archived file inside of
+                the zipfile.
+
+            mode (str):
+                Currently only "r" - readonly mode is supported
+
+            seekable (bool):
+                If True, attempts to force "seekability" of the underlying
+                file-object, for compressed files this will first extract
+                the file to a temporary location on disk.  If False, any underlying
+                compressed file will be opened directly which may result in the
+                object being non-seekable.
+
+            ext (str):
+                The extension of the zipfile. Modify this is a non-standard
+                extension is used (e.g. for torch packages).
+        """
         self.fpath = fpath
         self.ext = ext
         self.name = fpath
         self.mode = mode
         self._seekable = seekable
         self._zfpath = None  # points to the base zipfile (if appropriate)
         self._temp_dpath = None  # for temporary extraction
```

### Comparing `ubelt-1.3.2/ubelt.egg-info/PKG-INFO` & `ubelt-1.3.3/ubelt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubelt
-Version: 1.3.2
+Version: 1.3.3
 Summary: A Python utility belt containing simple tools, a stdlib like feel, and extra batteries.
 Home-page: https://github.com/Erotemic/ubelt
 Author: Jon Crall
 Author-email: erotemic@gmail.com
 License: Apache 2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ubelt-1.3.2/ubelt.egg-info/SOURCES.txt` & `ubelt-1.3.3/ubelt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.2/ubelt.egg-info/requires.txt` & `ubelt-1.3.3/ubelt.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 
 [:platform_system == "Windows"]
 jaraco.windows
 
+[:platform_system == "Windows" and platform_python_implementation == "PyPy"]
+pydantic<2.0
+
 [all]
 Pygments
 pytest-timeout
 python_dateutil
 requests
 xdoctest
 
@@ -16,14 +19,17 @@
 requests==2.25.1
 xdoctest==0.14.0
 
 [all-strict:platform_system == "Windows"]
 colorama==0.4.3
 jaraco.windows==3.9.1
 
+[all-strict:platform_system == "Windows" and platform_python_implementation == "PyPy"]
+pydantic<2.0
+
 [all-strict:python_version < "2.7" and python_version >= "2.6"]
 coverage==4.5
 
 [all-strict:python_version < "2.8.0" and python_version >= "2.7.0"]
 pytest-cov==2.8.1
 pytest<=4.6.11,==4.6.0
 
@@ -99,14 +105,17 @@
 [all-strict:python_version >= "3.6.0"]
 pytest-cov==3.0.0
 
 [all:platform_system == "Windows"]
 colorama
 jaraco.windows
 
+[all:platform_system == "Windows" and platform_python_implementation == "PyPy"]
+pydantic<2.0
+
 [all:python_version < "2.7" and python_version >= "2.6"]
 coverage
 
 [all:python_version < "2.8.0" and python_version >= "2.7.0"]
 pytest
 pytest-cov
 
@@ -289,14 +298,17 @@
 numpy
 
 [runtime-strict]
 
 [runtime-strict:platform_system == "Windows"]
 jaraco.windows==3.9.1
 
+[runtime-strict:platform_system == "Windows" and platform_python_implementation == "PyPy"]
+pydantic<2.0
+
 [tests]
 pytest-timeout
 requests
 xdoctest
 
 [tests-strict]
 pytest-timeout==1.4.2
```

