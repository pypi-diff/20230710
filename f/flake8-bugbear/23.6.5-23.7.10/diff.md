# Comparing `tmp/flake8-bugbear-23.6.5.tar.gz` & `tmp/flake8-bugbear-23.7.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-bugbear-23.6.5.tar", last modified: Mon Jun  5 16:20:50 2023, max compression
+gzip compressed data, was "flake8-bugbear-23.7.10.tar", last modified: Mon Jul 10 16:29:34 2023, max compression
```

## Comparing `flake8-bugbear-23.6.5.tar` & `flake8-bugbear-23.7.10.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:20:50.367162 flake8-bugbear-23.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    26492 2023-06-05 16:20:50.367162 flake8-bugbear-23.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25173 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    65990 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/bugbear.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:20:50.363162 flake8-bugbear-23.6.5/flake8_bugbear.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26492 2023-06-05 16:20:50.000000 flake8-bugbear-23.6.5/flake8_bugbear.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-05 16:20:50.000000 flake8-bugbear-23.6.5/flake8_bugbear.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:20:50.000000 flake8-bugbear-23.6.5/flake8_bugbear.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-05 16:20:50.000000 flake8-bugbear-23.6.5/flake8_bugbear.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:20:50.000000 flake8-bugbear-23.6.5/flake8_bugbear.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-05 16:20:50.000000 flake8-bugbear-23.6.5/flake8_bugbear.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 16:20:50.000000 flake8-bugbear-23.6.5/flake8_bugbear.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-05 16:20:50.367162 flake8-bugbear-23.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:20:50.367162 flake8-bugbear-23.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b001.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b002.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b003.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b004.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b005.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b006_b008.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b007.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b008_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b009_b010.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b011.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b012.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b013.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b014.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b015.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b016.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b017.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b018_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b018_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b018_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b019.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b020.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b021.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b022.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b023.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b024.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b025.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b026.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b027.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b028.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b029.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b030.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b031.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b032.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b033.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b901.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b902.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b902_py38.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b903.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b904.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b905_py310.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b906.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b907.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b908.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/b950.py
--rw-r--r--   0 runner    (1001) docker     (123)    29309 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tests/test_bugbear.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-05 16:20:41.000000 flake8-bugbear-23.6.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:29:34.876180 flake8-bugbear-23.7.10/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    27418 2023-07-10 16:29:34.876180 flake8-bugbear-23.7.10/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26047 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    68449 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/bugbear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:29:34.872180 flake8-bugbear-23.7.10/flake8_bugbear.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27418 2023-07-10 16:29:34.000000 flake8-bugbear-23.7.10/flake8_bugbear.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-10 16:29:34.000000 flake8-bugbear-23.7.10/flake8_bugbear.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:29:34.000000 flake8-bugbear-23.7.10/flake8_bugbear.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 16:29:34.000000 flake8-bugbear-23.7.10/flake8_bugbear.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:29:34.000000 flake8-bugbear-23.7.10/flake8_bugbear.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-10 16:29:34.000000 flake8-bugbear-23.7.10/flake8_bugbear.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 16:29:34.000000 flake8-bugbear-23.7.10/flake8_bugbear.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-10 16:29:34.876180 flake8-bugbear-23.7.10/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:29:34.876180 flake8-bugbear-23.7.10/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b001.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b002.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b003.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b004.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b005.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b006_b008.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b007.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b008_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b009_b010.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b011.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b012.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b013.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b014.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b015.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b016.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b017.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b018_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b018_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b018_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b019.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b020.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b021.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b022.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b023.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b025.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b026.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b027.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b028.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b029.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b030.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b031.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b032.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b033.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b034.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b901.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b902.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b902_py38.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b903.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b904.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b905_py310.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b906.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b907.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b908.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/b950.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30922 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tests/test_bugbear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-10 16:29:25.000000 flake8-bugbear-23.7.10/tox.ini
```

### Comparing `flake8-bugbear-23.6.5/LICENSE` & `flake8-bugbear-23.7.10/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/PKG-INFO` & `flake8-bugbear-23.7.10/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-bugbear
-Version: 23.6.5
+Version: 23.7.10
 Summary: A plugin for flake8 finding likely bugs and design problems in your program. Contains warnings that don't belong in pyflakes and pycodestyle.
 Author-email: Łukasz Langa <lukasz@langa.pl>
 License: MIT
 Project-URL: Homepage, https://github.com/PyCQA/flake8-bugbear
 Project-URL: Change Log, https://github.com/PyCQA/flake8-bugbear#change-log
 Keywords: flake8,bugbear,bugs,pyflakes,pylint,linter,qa
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,14 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.8.1
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
@@ -213,14 +214,16 @@
 **B031**: Using the generator returned from `itertools.groupby()` more than once will do nothing on the
 second usage. Save the result to a list if the result is needed multiple times.
 
 **B032**: Possible unintentional type annotation (using ``:``). Did you mean to assign (using ``=``)?
 
 **B033**: Sets should not contain duplicate items. Duplicate items will be replaced with a single item at runtime.
 
+**B034**: Calls to `re.sub`, `re.subn` or `re.split` should pass `flags` or `count`/`maxsplit` as keyword arguments. It is commonly assumed that `flags` is the third positional parameter, forgetting about `count`/`maxsplit`, since many other `re` module functions are of the form `f(pattern, string, flags)`.
+
 Opinionated warnings
 ~~~~~~~~~~~~~~~~~~~~
 
 The following warnings are disabled by default because they are
 controversial.  They may or may not apply to you, enable them explicitly
 in your configuration if you find them useful.  Read below on how to
 enable.
@@ -245,16 +248,19 @@
 
 **B904**: Within an ``except`` clause, raise exceptions with ``raise ... from err``
 or ``raise ... from None`` to distinguish them from errors in exception handling.
 See `the exception chaining tutorial <https://docs.python.org/3/tutorial/errors.html#exception-chaining>`_
 for details.
 
 **B905**: ``zip()`` without an explicit `strict=` parameter set. ``strict=True`` causes the resulting iterator
-to raise a ``ValueError`` if the arguments are exhausted at differing lengths. The ``strict=`` argument
-was added in Python 3.10, so don't enable this flag for code that should work on <3.10.
+to raise a ``ValueError`` if the arguments are exhausted at differing lengths.
+
+Exclusions are `itertools.count <https://docs.python.org/3/library/itertools.html#itertools.count>`_, `itertools.cycle <https://docs.python.org/3/library/itertools.html#itertools.cycle>`_ and `itertools.repeat <https://docs.python.org/3/library/itertools.html#itertools.repeat>`_ (with times=None) since they are infinite iterators.
+
+The ``strict=`` argument was added in Python 3.10, so don't enable this flag for code that should work on <3.10.
 For more information: https://peps.python.org/pep-0618/
 
 **B906**: ``visit_`` function with no further call to a ``visit`` function. This is often an error, and will stop the visitor from recursing into the subnodes of a visited node. Consider adding a call ``self.generic_visit(node)`` at the end of the function.
 Will only trigger on function names where the part after ``visit_`` is a valid ``ast`` type with a non-empty ``_fields`` attribute.
 This is meant to be enabled by developers writing visitors using the ``ast`` module, such as flake8 plugin writers.
 
 **B907**: Consider replacing ``f"'{foo}'"`` with ``f"{foo!r}"`` which is both easier to read and will escape quotes inside ``foo`` if that would appear. The check tries to filter out any format specs that are invalid together with ``!r``. If you're using other conversion flags then e.g. ``f"'{foo!a}'"`` can be replaced with ``f"{ascii(foo)!r}"``. Not currently implemented for python<3.8 or ``str.format()`` calls.
@@ -354,14 +360,22 @@
 
 MIT
 
 
 Change Log
 ----------
 
+23.7.10
+~~~~~~~~~~
+
+* Add B034: re.sub/subn/split must pass flags/count/maxsplit as keyword arguments.
+* Fix a crash and several test failures on Python 3.12, all relating to the B907
+  check.
+* Declare support for Python 3.12.
+
 23.6.5
 ~~~~~~
 
 * Include tox.ini in MANIFEST.in for sdist. (#389)
 * Improve B033 (duplicate set items) (#385)
 
 23.5.9
```

### Comparing `flake8-bugbear-23.6.5/README.rst` & `flake8-bugbear-23.7.10/flake8_bugbear.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+Metadata-Version: 2.1
+Name: flake8-bugbear
+Version: 23.7.10
+Summary: A plugin for flake8 finding likely bugs and design problems in your program. Contains warnings that don't belong in pyflakes and pycodestyle.
+Author-email: Łukasz Langa <lukasz@langa.pl>
+License: MIT
+Project-URL: Homepage, https://github.com/PyCQA/flake8-bugbear
+Project-URL: Change Log, https://github.com/PyCQA/flake8-bugbear#change-log
+Keywords: flake8,bugbear,bugs,pyflakes,pylint,linter,qa
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Framework :: Flake8
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Quality Assurance
+Requires-Python: >=3.8.1
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+License-File: LICENSE
+
 ==============
 flake8-bugbear
 ==============
 
 .. image:: https://github.com/PyCQA/flake8-bugbear/actions/workflows/ci.yml/badge.svg
    :target: https://github.com/PyCQA/flake8-bugbear/actions/workflows/ci.yml
 
@@ -184,14 +214,16 @@
 **B031**: Using the generator returned from `itertools.groupby()` more than once will do nothing on the
 second usage. Save the result to a list if the result is needed multiple times.
 
 **B032**: Possible unintentional type annotation (using ``:``). Did you mean to assign (using ``=``)?
 
 **B033**: Sets should not contain duplicate items. Duplicate items will be replaced with a single item at runtime.
 
+**B034**: Calls to `re.sub`, `re.subn` or `re.split` should pass `flags` or `count`/`maxsplit` as keyword arguments. It is commonly assumed that `flags` is the third positional parameter, forgetting about `count`/`maxsplit`, since many other `re` module functions are of the form `f(pattern, string, flags)`.
+
 Opinionated warnings
 ~~~~~~~~~~~~~~~~~~~~
 
 The following warnings are disabled by default because they are
 controversial.  They may or may not apply to you, enable them explicitly
 in your configuration if you find them useful.  Read below on how to
 enable.
@@ -216,16 +248,19 @@
 
 **B904**: Within an ``except`` clause, raise exceptions with ``raise ... from err``
 or ``raise ... from None`` to distinguish them from errors in exception handling.
 See `the exception chaining tutorial <https://docs.python.org/3/tutorial/errors.html#exception-chaining>`_
 for details.
 
 **B905**: ``zip()`` without an explicit `strict=` parameter set. ``strict=True`` causes the resulting iterator
-to raise a ``ValueError`` if the arguments are exhausted at differing lengths. The ``strict=`` argument
-was added in Python 3.10, so don't enable this flag for code that should work on <3.10.
+to raise a ``ValueError`` if the arguments are exhausted at differing lengths.
+
+Exclusions are `itertools.count <https://docs.python.org/3/library/itertools.html#itertools.count>`_, `itertools.cycle <https://docs.python.org/3/library/itertools.html#itertools.cycle>`_ and `itertools.repeat <https://docs.python.org/3/library/itertools.html#itertools.repeat>`_ (with times=None) since they are infinite iterators.
+
+The ``strict=`` argument was added in Python 3.10, so don't enable this flag for code that should work on <3.10.
 For more information: https://peps.python.org/pep-0618/
 
 **B906**: ``visit_`` function with no further call to a ``visit`` function. This is often an error, and will stop the visitor from recursing into the subnodes of a visited node. Consider adding a call ``self.generic_visit(node)`` at the end of the function.
 Will only trigger on function names where the part after ``visit_`` is a valid ``ast`` type with a non-empty ``_fields`` attribute.
 This is meant to be enabled by developers writing visitors using the ``ast`` module, such as flake8 plugin writers.
 
 **B907**: Consider replacing ``f"'{foo}'"`` with ``f"{foo!r}"`` which is both easier to read and will escape quotes inside ``foo`` if that would appear. The check tries to filter out any format specs that are invalid together with ``!r``. If you're using other conversion flags then e.g. ``f"'{foo!a}'"`` can be replaced with ``f"{ascii(foo)!r}"``. Not currently implemented for python<3.8 or ``str.format()`` calls.
@@ -325,14 +360,22 @@
 
 MIT
 
 
 Change Log
 ----------
 
+23.7.10
+~~~~~~~~~~
+
+* Add B034: re.sub/subn/split must pass flags/count/maxsplit as keyword arguments.
+* Fix a crash and several test failures on Python 3.12, all relating to the B907
+  check.
+* Declare support for Python 3.12.
+
 23.6.5
 ~~~~~~
 
 * Include tox.ini in MANIFEST.in for sdist. (#389)
 * Improve B033 (duplicate set items) (#385)
 
 23.5.9
```

### Comparing `flake8-bugbear-23.6.5/bugbear.py` & `flake8-bugbear-23.7.10/bugbear.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import ast
 import builtins
 import itertools
 import logging
 import math
 import re
 import sys
+import warnings
 from collections import namedtuple
 from contextlib import suppress
 from functools import lru_cache, partial
 from keyword import iskeyword
 
 import attr
 import pycodestyle
 
-__version__ = "23.6.5"
+__version__ = "23.7.10"
 
 LOG = logging.getLogger("flake8.bugbear")
 CONTEXTFUL_NODES = (
     ast.Module,
     ast.ClassDef,
     ast.AsyncFunctionDef,
     ast.FunctionDef,
@@ -196,15 +197,15 @@
 def _is_identifier(arg):
     # Return True if arg is a valid identifier, per
     # https://docs.python.org/2/reference/lexical_analysis.html#identifiers
 
     if not isinstance(arg, ast.Constant) or not isinstance(arg.value, str):
         return False
 
-    return re.match(r"^[A-Za-z_][A-Za-z0-9_]*$", arg.s) is not None
+    return re.match(r"^[A-Za-z_][A-Za-z0-9_]*$", arg.value) is not None
 
 
 def _flatten_excepthandler(node):
     if not isinstance(node, ast.Tuple):
         yield node
         return
     expr_list = node.elts.copy()
@@ -397,37 +398,38 @@
     def visit_Call(self, node):
         if isinstance(node.func, ast.Attribute):
             self.check_for_b005(node)
         else:
             with suppress(AttributeError, IndexError):
                 if (
                     node.func.id in ("getattr", "hasattr")
-                    and node.args[1].s == "__call__"
+                    and node.args[1].value == "__call__"
                 ):
                     self.errors.append(B004(node.lineno, node.col_offset))
                 if (
                     node.func.id == "getattr"
                     and len(node.args) == 2
                     and _is_identifier(node.args[1])
-                    and not iskeyword(node.args[1].s)
+                    and not iskeyword(node.args[1].value)
                 ):
                     self.errors.append(B009(node.lineno, node.col_offset))
                 elif (
                     not any(isinstance(n, ast.Lambda) for n in self.node_stack)
                     and node.func.id == "setattr"
                     and len(node.args) == 3
                     and _is_identifier(node.args[1])
-                    and not iskeyword(node.args[1].s)
+                    and not iskeyword(node.args[1].value)
                 ):
                     self.errors.append(B010(node.lineno, node.col_offset))
 
             self.check_for_b026(node)
 
-        self.check_for_b905(node)
         self.check_for_b028(node)
+        self.check_for_b034(node)
+        self.check_for_b905(node)
         self.generic_visit(node)
 
     def visit_Module(self, node):
         self.check_for_b018(node)
         self.generic_visit(node)
 
     def visit_Assign(self, node):
@@ -552,19 +554,19 @@
             ):
                 return  # used arguments don't match the builtin strip
 
             call_path = ".".join(compose_call_path(node.func.value))
             if call_path in B005.valid_paths:
                 return  # path is exempt
 
-            s = node.args[0].s
-            if len(s) == 1:
+            value = node.args[0].value
+            if len(value) == 1:
                 return  # stripping just one character
 
-            if len(s) == len(set(s)):
+            if len(value) == len(set(value)):
                 return  # no characters appear more than once
 
             self.errors.append(B005(node.lineno, node.col_offset))
 
     def check_for_b006_and_b008(self, node):
         visitor = FuntionDefDefaultsVisitor(self.b008_extend_immutable_calls)
         visitor.visit(node.args.defaults + node.args.kw_defaults)
@@ -1164,29 +1166,68 @@
                     uniques.add(name)
                 seen.extend(uniques)
         # sort to have a deterministic output
         duplicates = sorted({x for x in seen if seen.count(x) > 1})
         for duplicate in duplicates:
             self.errors.append(B025(node.lineno, node.col_offset, vars=(duplicate,)))
 
-    def check_for_b905(self, node):
-        if (
-            isinstance(node.func, ast.Name)
-            and node.func.id == "zip"
-            and not any(kw.arg == "strict" for kw in node.keywords)
+    @staticmethod
+    def _is_infinite_iterator(node: ast.expr) -> bool:
+        if not (
+            isinstance(node, ast.Call)
+            and isinstance(node.func, ast.Attribute)
+            and isinstance(node.func.value, ast.Name)
+            and node.func.value.id == "itertools"
         ):
+            return False
+        if node.func.attr in {"cycle", "count"}:
+            return True
+        elif node.func.attr == "repeat":
+            if len(node.args) == 1 and len(node.keywords) == 0:
+                # itertools.repeat(iterable)
+                return True
+            if (
+                len(node.args) == 2
+                and isinstance(node.args[1], ast.Constant)
+                and node.args[1].value is None
+            ):
+                # itertools.repeat(iterable, None)
+                return True
+            for kw in node.keywords:
+                # itertools.repeat(iterable, times=None)
+                if (
+                    kw.arg == "times"
+                    and isinstance(kw.value, ast.Constant)
+                    and kw.value.value is None
+                ):
+                    return True
+
+        return False
+
+    def check_for_b905(self, node):
+        if not (isinstance(node.func, ast.Name) and node.func.id == "zip"):
+            return
+        for arg in node.args:
+            if self._is_infinite_iterator(arg):
+                return
+        if not any(kw.arg == "strict" for kw in node.keywords):
             self.errors.append(B905(node.lineno, node.col_offset))
 
     def check_for_b906(self, node: ast.FunctionDef):
         if not node.name.startswith("visit_"):
             return
 
         # extract what's visited
         class_name = node.name[len("visit_") :]
-        class_type = getattr(ast, class_name, None)
+
+        # silence any DeprecationWarnings
+        # that might come from accessing a deprecated AST node
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", category=DeprecationWarning)
+            class_type = getattr(ast, class_name, None)
 
         if (
             # not a valid ast subclass
             class_type is None
             # doesn't have a non-empty '_fields' attribute - which is what's
             # iterated over in ast.NodeVisitor.generic_visit
             or not getattr(class_type, "_fields", None)
@@ -1235,44 +1276,42 @@
             # as a last resort, just give the type name
             return type(node).__name__
 
         quote_marks = "'\""
         current_mark = None
         variable = None
         for value in node.values:
-            # check for quote mark after pre-marked variable
-            if (
-                current_mark is not None
-                and variable is not None
-                and isinstance(value, ast.Constant)
-                and isinstance(value.value, str)
-                and value.value[0] == current_mark
-            ):
-                self.errors.append(
-                    B907(
-                        variable.lineno,
-                        variable.col_offset,
-                        vars=(myunparse(variable.value),),
-                    )
-                )
-                current_mark = variable = None
-                # don't continue with length>1, so we can detect a new pre-mark
-                # in the same string as a post-mark, e.g. `"{foo}" "{bar}"`
-                if len(value.value) == 1:
+            if isinstance(value, ast.Constant) and isinstance(value.value, str):
+                if not value.value:
                     continue
 
-            # detect pre-mark
-            if (
-                isinstance(value, ast.Constant)
-                and isinstance(value.value, str)
-                and value.value[-1] in quote_marks
-            ):
-                current_mark = value.value[-1]
-                variable = None
-                continue
+                # check for quote mark after pre-marked variable
+                if (
+                    current_mark is not None
+                    and variable is not None
+                    and value.value[0] == current_mark
+                ):
+                    self.errors.append(
+                        B907(
+                            variable.lineno,
+                            variable.col_offset,
+                            vars=(myunparse(variable.value),),
+                        )
+                    )
+                    current_mark = variable = None
+                    # don't continue with length>1, so we can detect a new pre-mark
+                    # in the same string as a post-mark, e.g. `"{foo}" "{bar}"`
+                    if len(value.value) == 1:
+                        continue
+
+                # detect pre-mark
+                if value.value[-1] in quote_marks:
+                    current_mark = value.value[-1]
+                    variable = None
+                    continue
 
             # detect variable, if there's a pre-mark
             if (
                 current_mark is not None
                 and variable is None
                 and isinstance(value, ast.FormattedValue)
                 and value.conversion != ord("r")
@@ -1358,14 +1397,35 @@
             if elt.value in seen:
                 self.errors.append(
                     B033(elt.lineno, elt.col_offset, vars=(repr(elt.value),))
                 )
             else:
                 seen.add(elt.value)
 
+    def check_for_b034(self, node: ast.Call):
+        if not isinstance(node.func, ast.Attribute):
+            return
+        if not isinstance(node.func.value, ast.Name) or node.func.value.id != "re":
+            return
+
+        def check(num_args, param_name):
+            if len(node.args) > num_args:
+                self.errors.append(
+                    B034(
+                        node.args[num_args].lineno,
+                        node.args[num_args].col_offset,
+                        vars=(node.func.attr, param_name),
+                    )
+                )
+
+        if node.func.attr in ("sub", "subn"):
+            check(3, "count")
+        elif node.func.attr == "split":
+            check(2, "maxsplit")
+
 
 def compose_call_path(node):
     if isinstance(node, ast.Attribute):
         yield from compose_call_path(node.value)
         yield node.attr
     elif isinstance(node, ast.Call):
         yield from compose_call_path(node.func)
@@ -1762,14 +1822,21 @@
 B033 = Error(
     message=(
         "B033 Set should not contain duplicate item {}. Duplicate items will be"
         " replaced with a single item at runtime."
     )
 )
 
+B034 = Error(
+    message=(
+        "B034 {} should pass `{}` and `flags` as keyword arguments to avoid confusion"
+        " due to unintuitive argument positions."
+    )
+)
+
 # Warnings disabled by default.
 B901 = Error(
     message=(
         "B901 Using `yield` together with `return x`. Use native "
         "`async def` coroutines or put a `# noqa` comment on this "
         "line if this was intentional."
     )
```

### Comparing `flake8-bugbear-23.6.5/flake8_bugbear.egg-info/PKG-INFO` & `flake8-bugbear-23.7.10/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: flake8-bugbear
-Version: 23.6.5
-Summary: A plugin for flake8 finding likely bugs and design problems in your program. Contains warnings that don't belong in pyflakes and pycodestyle.
-Author-email: Łukasz Langa <lukasz@langa.pl>
-License: MIT
-Project-URL: Homepage, https://github.com/PyCQA/flake8-bugbear
-Project-URL: Change Log, https://github.com/PyCQA/flake8-bugbear#change-log
-Keywords: flake8,bugbear,bugs,pyflakes,pylint,linter,qa
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Framework :: Flake8
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Python: >=3.8.1
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-License-File: LICENSE
-
 ==============
 flake8-bugbear
 ==============
 
 .. image:: https://github.com/PyCQA/flake8-bugbear/actions/workflows/ci.yml/badge.svg
    :target: https://github.com/PyCQA/flake8-bugbear/actions/workflows/ci.yml
 
@@ -213,14 +184,16 @@
 **B031**: Using the generator returned from `itertools.groupby()` more than once will do nothing on the
 second usage. Save the result to a list if the result is needed multiple times.
 
 **B032**: Possible unintentional type annotation (using ``:``). Did you mean to assign (using ``=``)?
 
 **B033**: Sets should not contain duplicate items. Duplicate items will be replaced with a single item at runtime.
 
+**B034**: Calls to `re.sub`, `re.subn` or `re.split` should pass `flags` or `count`/`maxsplit` as keyword arguments. It is commonly assumed that `flags` is the third positional parameter, forgetting about `count`/`maxsplit`, since many other `re` module functions are of the form `f(pattern, string, flags)`.
+
 Opinionated warnings
 ~~~~~~~~~~~~~~~~~~~~
 
 The following warnings are disabled by default because they are
 controversial.  They may or may not apply to you, enable them explicitly
 in your configuration if you find them useful.  Read below on how to
 enable.
@@ -245,16 +218,19 @@
 
 **B904**: Within an ``except`` clause, raise exceptions with ``raise ... from err``
 or ``raise ... from None`` to distinguish them from errors in exception handling.
 See `the exception chaining tutorial <https://docs.python.org/3/tutorial/errors.html#exception-chaining>`_
 for details.
 
 **B905**: ``zip()`` without an explicit `strict=` parameter set. ``strict=True`` causes the resulting iterator
-to raise a ``ValueError`` if the arguments are exhausted at differing lengths. The ``strict=`` argument
-was added in Python 3.10, so don't enable this flag for code that should work on <3.10.
+to raise a ``ValueError`` if the arguments are exhausted at differing lengths.
+
+Exclusions are `itertools.count <https://docs.python.org/3/library/itertools.html#itertools.count>`_, `itertools.cycle <https://docs.python.org/3/library/itertools.html#itertools.cycle>`_ and `itertools.repeat <https://docs.python.org/3/library/itertools.html#itertools.repeat>`_ (with times=None) since they are infinite iterators.
+
+The ``strict=`` argument was added in Python 3.10, so don't enable this flag for code that should work on <3.10.
 For more information: https://peps.python.org/pep-0618/
 
 **B906**: ``visit_`` function with no further call to a ``visit`` function. This is often an error, and will stop the visitor from recursing into the subnodes of a visited node. Consider adding a call ``self.generic_visit(node)`` at the end of the function.
 Will only trigger on function names where the part after ``visit_`` is a valid ``ast`` type with a non-empty ``_fields`` attribute.
 This is meant to be enabled by developers writing visitors using the ``ast`` module, such as flake8 plugin writers.
 
 **B907**: Consider replacing ``f"'{foo}'"`` with ``f"{foo!r}"`` which is both easier to read and will escape quotes inside ``foo`` if that would appear. The check tries to filter out any format specs that are invalid together with ``!r``. If you're using other conversion flags then e.g. ``f"'{foo!a}'"`` can be replaced with ``f"{ascii(foo)!r}"``. Not currently implemented for python<3.8 or ``str.format()`` calls.
@@ -354,14 +330,22 @@
 
 MIT
 
 
 Change Log
 ----------
 
+23.7.10
+~~~~~~~~~~
+
+* Add B034: re.sub/subn/split must pass flags/count/maxsplit as keyword arguments.
+* Fix a crash and several test failures on Python 3.12, all relating to the B907
+  check.
+* Declare support for Python 3.12.
+
 23.6.5
 ~~~~~~
 
 * Include tox.ini in MANIFEST.in for sdist. (#389)
 * Improve B033 (duplicate set items) (#385)
 
 23.5.9
```

### Comparing `flake8-bugbear-23.6.5/flake8_bugbear.egg-info/SOURCES.txt` & `flake8-bugbear-23.7.10/flake8_bugbear.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 tests/b027.py
 tests/b028.py
 tests/b029.py
 tests/b030.py
 tests/b031.py
 tests/b032.py
 tests/b033.py
+tests/b034.py
 tests/b901.py
 tests/b902.py
 tests/b902_py38.py
 tests/b903.py
 tests/b904.py
 tests/b905_py310.py
 tests/b906.py
```

### Comparing `flake8-bugbear-23.6.5/pyproject.toml` & `flake8-bugbear-23.7.10/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
 ]
 requires-python = ">=3.8.1"
 dependencies = ["flake8>=6.0.0", "attrs>=19.2.0"]
 dynamic = ["version"]
```

### Comparing `flake8-bugbear-23.6.5/tests/b001.py` & `flake8-bugbear-23.7.10/tests/b001.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b005.py` & `flake8-bugbear-23.7.10/tests/b005.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b006_b008.py` & `flake8-bugbear-23.7.10/tests/b006_b008.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b007.py` & `flake8-bugbear-23.7.10/tests/b007.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b009_b010.py` & `flake8-bugbear-23.7.10/tests/b009_b010.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b012.py` & `flake8-bugbear-23.7.10/tests/b012.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b013.py` & `flake8-bugbear-23.7.10/tests/b013.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b014.py` & `flake8-bugbear-23.7.10/tests/b014.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b017.py` & `flake8-bugbear-23.7.10/tests/b017.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b019.py` & `flake8-bugbear-23.7.10/tests/b019.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b020.py` & `flake8-bugbear-23.7.10/tests/b020.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b021.py` & `flake8-bugbear-23.7.10/tests/b021.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b023.py` & `flake8-bugbear-23.7.10/tests/b023.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b024.py` & `flake8-bugbear-23.7.10/tests/b024.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b027.py` & `flake8-bugbear-23.7.10/tests/b027.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b030.py` & `flake8-bugbear-23.7.10/tests/b030.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b031.py` & `flake8-bugbear-23.7.10/tests/b031.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b901.py` & `flake8-bugbear-23.7.10/tests/b901.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b902.py` & `flake8-bugbear-23.7.10/tests/b902.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b902_py38.py` & `flake8-bugbear-23.7.10/tests/b902_py38.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b903.py` & `flake8-bugbear-23.7.10/tests/b903.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b904.py` & `flake8-bugbear-23.7.10/tests/b904.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b906.py` & `flake8-bugbear-23.7.10/tests/b906.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b907.py` & `flake8-bugbear-23.7.10/tests/b907.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 f'"{var}" end'
 f'begin "{var}"'
 
 f'a "{"hello"}" b'
 f'a "{foo()}" b'
 
 # fmt: off
-k = (f'"' # error emitted on this line since all values are assigned the same lineno
+k = (f'"' # Error emitted here on <py312 (all values assigned the same lineno)
      f'{var}'
      f'"'
      f'"')
 
-k = (f'"' # error emitted on this line
+k = (f'"' # error emitted on this line on <py312
      f'{var}'
      '"'
      f'"')
 # fmt: on
 
 f'{"hello"}"{var}"'  # warn for var and not hello
 f'"{var}"{"hello"}'  # warn for var and not hello
```

### Comparing `flake8-bugbear-23.6.5/tests/b908.py` & `flake8-bugbear-23.7.10/tests/b908.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/b950.py` & `flake8-bugbear-23.7.10/tests/b950.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.6.5/tests/test_bugbear.py` & `flake8-bugbear-23.7.10/tests/test_bugbear.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 import site
 import subprocess
 import sys
 import unittest
 from argparse import Namespace
 from pathlib import Path
 
-from hypothesis import HealthCheck, given, settings
-from hypothesmith import from_grammar
-
 from bugbear import (
     B001,
     B002,
     B003,
     B004,
     B005,
     B006,
@@ -41,14 +38,15 @@
     B027,
     B028,
     B029,
     B030,
     B031,
     B032,
     B033,
+    B034,
     B901,
     B902,
     B903,
     B904,
     B905,
     B906,
     B907,
@@ -501,14 +499,31 @@
             B033(11, 11, vars=("True",)),
             B033(12, 11, vars=("False",)),
             B033(16, 4, vars=("True",)),
             B033(18, 4, vars=("False",)),
         )
         self.assertEqual(errors, expected)
 
+    def test_b034(self):
+        filename = Path(__file__).absolute().parent / "b034.py"
+        bbc = BugBearChecker(filename=str(filename))
+        errors = list(bbc.run())
+        expected = self.errors(
+            B034(5, 24, vars=("sub", "count")),
+            B034(6, 24, vars=("sub", "count")),
+            B034(7, 24, vars=("sub", "count")),
+            B034(8, 25, vars=("subn", "count")),
+            B034(9, 25, vars=("subn", "count")),
+            B034(10, 25, vars=("subn", "count")),
+            B034(11, 25, vars=("split", "maxsplit")),
+            B034(12, 25, vars=("split", "maxsplit")),
+            B034(13, 25, vars=("split", "maxsplit")),
+        )
+        self.assertEqual(errors, expected)
+
     def test_b908(self):
         filename = Path(__file__).absolute().parent / "b908.py"
         bbc = BugBearChecker(filename=str(filename))
         errors = list(bbc.run())
         expected = self.errors(
             B908(7, 0),
             B908(15, 8),
@@ -520,51 +535,59 @@
         )
         self.assertEqual(errors, expected)
 
     def test_b907(self):
         filename = Path(__file__).absolute().parent / "b907.py"
         bbc = BugBearChecker(filename=str(filename))
         errors = list(bbc.run())
-        expected = self.errors(
-            B907(8, 0, vars=("var",)),
-            B907(9, 0, vars=("var",)),
-            B907(10, 0, vars=("var",)),
-            B907(12, 0, vars=("var",)),
-            B907(13, 0, vars=("var",)),
-            B907(14, 0, vars=("var",)),
-            B907(16, 0, vars=("'hello'",)),
-            B907(17, 0, vars=("foo()",)),
-            B907(20, 5, vars=("var",)),
-            B907(25, 5, vars=("var",)),
-            B907(31, 0, vars=("var",)),
-            B907(32, 0, vars=("var",)),
-            B907(33, 0, vars=("var",)),
-            B907(33, 0, vars=("var2",)),
-            B907(34, 0, vars=("var",)),
-            B907(34, 0, vars=("var2",)),
-            B907(35, 0, vars=("var",)),
-            B907(35, 0, vars=("var2",)),
-            B907(38, 0, vars=("var2",)),
-            B907(41, 0, vars=("var",)),
-            B907(42, 0, vars=("var.__str__",)),
-            B907(43, 0, vars=("var.__str__.__repr__",)),
-            B907(44, 0, vars=("3 + 5" if sys.version_info >= (3, 9) else "BinOp",)),
-            B907(45, 0, vars=("foo()",)),
-            B907(46, 0, vars=("None",)),
-            B907(47, 0, vars=("..." if sys.version_info >= (3, 9) else "Ellipsis",)),
-            B907(48, 0, vars=("True",)),
-            B907(51, 0, vars=("var",)),
-            B907(52, 0, vars=("var",)),
-            B907(53, 0, vars=("var",)),
-            B907(54, 0, vars=("var",)),
-            B907(57, 0, vars=("var",)),
-            B907(60, 0, vars=("var",)),
-            B907(64, 0, vars=("var",)),
-            B907(66, 0, vars=("var",)),
-            B907(68, 0, vars=("var",)),
+        py39 = sys.version_info >= (3, 9)
+        py312 = sys.version_info >= (3, 12)
+
+        def on_py312(number):
+            """F-string nodes have column numbers set to 0 on <py312"""
+            return number if py312 else 0
+
+        expected = self.errors(
+            B907(8, on_py312(9), vars=("var",)),
+            B907(9, on_py312(3), vars=("var",)),
+            B907(10, on_py312(9), vars=("var",)),
+            B907(12, on_py312(9), vars=("var",)),
+            B907(13, on_py312(3), vars=("var",)),
+            B907(14, on_py312(9), vars=("var",)),
+            B907(16, on_py312(5), vars=("'hello'",)),
+            B907(17, on_py312(5), vars=("foo()",)),
+            # Multiline f-strings have lineno changes as well as colno changes on py312+
+            B907(21 if py312 else 20, 7 if py312 else 5, vars=("var",)),
+            B907(26 if py312 else 25, 7 if py312 else 5, vars=("var",)),
+            B907(31, on_py312(12), vars=("var",)),
+            B907(32, on_py312(3), vars=("var",)),
+            B907(33, on_py312(3), vars=("var",)),
+            B907(33, on_py312(29), vars=("var2",)),
+            B907(34, on_py312(3), vars=("var",)),
+            B907(34, on_py312(15), vars=("var2",)),
+            B907(35, on_py312(3), vars=("var",)),
+            B907(35, on_py312(10), vars=("var2",)),
+            B907(38, on_py312(13), vars=("var2",)),
+            B907(41, on_py312(3), vars=("var",)),
+            B907(42, on_py312(3), vars=("var.__str__",)),
+            B907(43, on_py312(3), vars=("var.__str__.__repr__",)),
+            B907(44, on_py312(3), vars=("3 + 5" if py39 else "BinOp",)),
+            B907(45, on_py312(3), vars=("foo()",)),
+            B907(46, on_py312(3), vars=("None",)),
+            B907(47, on_py312(3), vars=("..." if py39 else "Ellipsis",)),
+            B907(48, on_py312(3), vars=("True",)),
+            B907(51, on_py312(3), vars=("var",)),
+            B907(52, on_py312(3), vars=("var",)),
+            B907(53, on_py312(3), vars=("var",)),
+            B907(54, on_py312(3), vars=("var",)),
+            B907(57, on_py312(3), vars=("var",)),
+            B907(60, on_py312(3), vars=("var",)),
+            B907(64, on_py312(5), vars=("var",)),
+            B907(66, on_py312(3), vars=("var",)),
+            B907(68, on_py312(3), vars=("var",)),
         )
         self.assertEqual(errors, expected)
 
     # manual permutations to save overhead when doing >60k permutations
     # see format spec at
     # https://docs.python.org/3/library/string.html#format-specification-mini-language
     def test_b907_format_specifier_permutations(self):
@@ -691,14 +714,16 @@
             B905(1, 0),
             B905(2, 0),
             B905(3, 0),
             B905(4, 0),
             B905(4, 15),
             B905(5, 4),
             B905(6, 0),
+            B905(21, 0),
+            B905(22, 0),
         ]
         self.assertEqual(errors, self.errors(*expected))
 
     def test_b906(self):
         filename = Path(__file__).absolute().parent / "b906.py"
         bbc = BugBearChecker(filename=str(filename))
         errors = list(bbc.run())
@@ -791,21 +816,26 @@
         )
         self.assertEqual(proc.returncode, 0, proc.stdout.decode("utf8"))
         self.assertEqual(proc.stdout, b"")
         self.assertEqual(proc.stderr, b"")
 
 
 class TestFuzz(unittest.TestCase):
-    @settings(suppress_health_check=[HealthCheck.too_slow])
-    @given(from_grammar().map(ast.parse))
-    def test_does_not_crash_on_any_valid_code(self, syntax_tree):
-        # Given any syntatically-valid source code, flake8-bugbear should
-        # not crash.  This tests doesn't check that we do the *right* thing,
-        # just that we don't crash on valid-if-poorly-styled code!
-        BugBearVisitor(filename="<string>", lines=[]).visit(syntax_tree)
+    # TODO: enable this test on py312 once hypothesmith supports py312
+    if sys.version_info < (3, 12):
+        from hypothesis import HealthCheck, given, settings
+        from hypothesmith import from_grammar
+
+        @settings(suppress_health_check=[HealthCheck.too_slow])
+        @given(from_grammar().map(ast.parse))
+        def test_does_not_crash_on_any_valid_code(self, syntax_tree):
+            # Given any syntatically-valid source code, flake8-bugbear should
+            # not crash.  This tests doesn't check that we do the *right* thing,
+            # just that we don't crash on valid-if-poorly-styled code!
+            BugBearVisitor(filename="<string>", lines=[]).visit(syntax_tree)
 
     def test_does_not_crash_on_site_code(self):
         # Because the generator isn't perfect, we'll also test on all the code
         # we can easily find in our current Python environment - this includes
         # the standard library, and all installed packages.
         for base in sorted(set(site.PREFIXES)):
             for dirname, _, files in os.walk(base):
```

