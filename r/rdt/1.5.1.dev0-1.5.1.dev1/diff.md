# Comparing `tmp/rdt-1.5.1.dev0.tar.gz` & `tmp/rdt-1.5.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdt-1.5.1.dev0.tar", last modified: Thu Jun 29 00:04:34 2023, max compression
+gzip compressed data, was "rdt-1.5.1.dev1.tar", last modified: Mon Jul 10 20:51:21 2023, max compression
```

## Comparing `rdt-1.5.1.dev0.tar` & `rdt-1.5.1.dev1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:34.453358 rdt-1.5.1.dev0/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt-1.5.1.dev0/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22812 2023-06-01 21:46:38.000000 rdt-1.5.1.dev0/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    44576 2023-06-01 21:46:38.000000 rdt-1.5.1.dev0/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt-1.5.1.dev0/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    52635 2023-06-29 00:04:34.453563 rdt-1.5.1.dev0/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt-1.5.1.dev0/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/RELEASE.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:34.434451 rdt-1.5.1.dev0/rdt/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5342 2023-06-20 18:01:47.000000 rdt-1.5.1.dev0/rdt/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      729 2023-01-18 20:52:41.000000 rdt-1.5.1.dev0/rdt/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    30929 2023-01-18 20:52:41.000000 rdt-1.5.1.dev0/rdt/hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:34.436406 rdt-1.5.1.dev0/rdt/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      262 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/rdt/performance/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:34.438433 rdt-1.5.1.dev0/rdt/performance/datasets/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      847 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/rdt/performance/datasets/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1158 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/rdt/performance/datasets/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6125 2022-08-18 00:01:17.000000 rdt-1.5.1.dev0/rdt/performance/datasets/boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11724 2023-06-01 21:46:38.000000 rdt-1.5.1.dev0/rdt/performance/datasets/categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5734 2023-01-18 20:52:41.000000 rdt-1.5.1.dev0/rdt/performance/datasets/datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8406 2023-01-18 20:52:41.000000 rdt-1.5.1.dev0/rdt/performance/datasets/numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1893 2023-06-01 21:46:38.000000 rdt-1.5.1.dev0/rdt/performance/datasets/pii.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1898 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/rdt/performance/datasets/text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      558 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/rdt/performance/datasets/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3372 2023-06-01 21:46:38.000000 rdt-1.5.1.dev0/rdt/performance/performance.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3442 2022-08-18 00:01:17.000000 rdt-1.5.1.dev0/rdt/performance/profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:34.440926 rdt-1.5.1.dev0/rdt/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4940 2023-04-13 17:39:49.000000 rdt-1.5.1.dev0/rdt/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:34.441236 rdt-1.5.1.dev0/rdt/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3398 2023-01-18 20:52:41.000000 rdt-1.5.1.dev0/rdt/transformers/addons/addons_setup.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    15934 2023-06-01 21:46:38.000000 rdt-1.5.1.dev0/rdt/transformers/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3792 2023-06-01 21:46:38.000000 rdt-1.5.1.dev0/rdt/transformers/boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21411 2023-04-13 17:39:49.000000 rdt-1.5.1.dev0/rdt/transformers/categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9245 2023-06-01 21:46:38.000000 rdt-1.5.1.dev0/rdt/transformers/datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5878 2023-06-28 22:45:00.000000 rdt-1.5.1.dev0/rdt/transformers/null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22319 2023-06-01 21:46:38.000000 rdt-1.5.1.dev0/rdt/transformers/numerical.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:34.441988 rdt-1.5.1.dev0/rdt/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2022-08-18 00:01:17.000000 rdt-1.5.1.dev0/rdt/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12447 2023-06-01 21:46:38.000000 rdt-1.5.1.dev0/rdt/transformers/pii/anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1052 2023-01-18 20:52:41.000000 rdt-1.5.1.dev0/rdt/transformers/pii/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4847 2023-01-18 20:52:41.000000 rdt-1.5.1.dev0/rdt/transformers/text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4576 2023-04-26 21:05:25.000000 rdt-1.5.1.dev0/rdt/transformers/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:34.435835 rdt-1.5.1.dev0/rdt.egg-info/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    52635 2023-06-29 00:04:34.000000 rdt-1.5.1.dev0/rdt.egg-info/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2835 2023-06-29 00:04:34.000000 rdt-1.5.1.dev0/rdt.egg-info/SOURCES.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-06-29 00:04:34.000000 rdt-1.5.1.dev0/rdt.egg-info/dependency_links.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-06-29 00:04:34.000000 rdt-1.5.1.dev0/rdt.egg-info/not-zip-safe
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1448 2023-06-29 00:04:34.000000 rdt-1.5.1.dev0/rdt.egg-info/requires.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        4 2023-06-29 00:04:34.000000 rdt-1.5.1.dev0/rdt.egg-info/top_level.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-06-29 00:04:34.454116 rdt-1.5.1.dev0/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4183 2023-06-01 21:47:10.000000 rdt-1.5.1.dev0/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:34.442540 rdt-1.5.1.dev0/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt-1.5.1.dev0/tests/code_style.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18316 2023-06-01 21:46:38.000000 rdt-1.5.1.dev0/tests/contributing.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:34.430446 rdt-1.5.1.dev0/tests/datasets/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:34.443515 rdt-1.5.1.dev0/tests/datasets/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/tests/datasets/tests/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/tests/datasets/tests/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/tests/datasets/tests/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/tests/datasets/tests/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/tests/datasets/tests/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:34.444092 rdt-1.5.1.dev0/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/tests/integration/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    45119 2023-06-01 21:46:38.000000 rdt-1.5.1.dev0/tests/integration/test_hyper_transformer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9434 2023-06-01 21:46:38.000000 rdt-1.5.1.dev0/tests/integration/test_transformers.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:34.445667 rdt-1.5.1.dev0/tests/integration/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/tests/integration/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:34.446017 rdt-1.5.1.dev0/tests/integration/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/tests/integration/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6410 2023-01-18 20:52:41.000000 rdt-1.5.1.dev0/tests/integration/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt-1.5.1.dev0/tests/integration/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3425 2023-06-28 22:45:00.000000 rdt-1.5.1.dev0/tests/integration/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt-1.5.1.dev0/tests/integration/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4386 2023-06-28 22:45:00.000000 rdt-1.5.1.dev0/tests/integration/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10507 2023-06-28 22:45:00.000000 rdt-1.5.1.dev0/tests/integration/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt-1.5.1.dev0/tests/integration/transformers/test_text.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:34.446870 rdt-1.5.1.dev0/tests/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/tests/performance/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/tests/performance/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt-1.5.1.dev0/tests/performance/test_performance.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:34.447335 rdt-1.5.1.dev0/tests/performance/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/tests/performance/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt-1.5.1.dev0/tests/performance/tests/test_profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:34.448233 rdt-1.5.1.dev0/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/tests/unit/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5961 2023-06-20 18:01:47.000000 rdt-1.5.1.dev0/tests/unit/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   103941 2023-06-01 21:46:38.000000 rdt-1.5.1.dev0/tests/unit/test_hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:34.451496 rdt-1.5.1.dev0/tests/unit/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/tests/unit/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:34.451797 rdt-1.5.1.dev0/tests/unit/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/tests/unit/transformers/addons/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:34.452174 rdt-1.5.1.dev0/tests/unit/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/tests/unit/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt-1.5.1.dev0/tests/unit/transformers/addons/identity/test_identity.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:34.453085 rdt-1.5.1.dev0/tests/unit/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt-1.5.1.dev0/tests/unit/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    27923 2023-04-13 17:39:49.000000 rdt-1.5.1.dev0/tests/unit/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt-1.5.1.dev0/tests/unit/transformers/pii/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt-1.5.1.dev0/tests/unit/transformers/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    42015 2023-06-01 21:46:38.000000 rdt-1.5.1.dev0/tests/unit/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8973 2023-06-01 21:46:38.000000 rdt-1.5.1.dev0/tests/unit/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt-1.5.1.dev0/tests/unit/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    17137 2023-06-01 21:46:38.000000 rdt-1.5.1.dev0/tests/unit/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    19138 2023-06-28 22:45:00.000000 rdt-1.5.1.dev0/tests/unit/transformers/test_null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    57532 2023-06-01 21:46:38.000000 rdt-1.5.1.dev0/tests/unit/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt-1.5.1.dev0/tests/unit/transformers/test_text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt-1.5.1.dev0/tests/unit/transformers/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.622820 rdt-1.5.1.dev1/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22812 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    44576 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    52585 2023-07-10 20:51:21.623031 rdt-1.5.1.dev1/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/RELEASE.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.603252 rdt-1.5.1.dev1/rdt/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5342 2023-06-29 00:04:59.000000 rdt-1.5.1.dev1/rdt/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      729 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/rdt/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    30929 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/rdt/hyper_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.605381 rdt-1.5.1.dev1/rdt/performance/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      262 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/rdt/performance/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.607368 rdt-1.5.1.dev1/rdt/performance/datasets/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      847 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/rdt/performance/datasets/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1158 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/rdt/performance/datasets/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6125 2022-08-18 00:01:17.000000 rdt-1.5.1.dev1/rdt/performance/datasets/boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11724 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/rdt/performance/datasets/categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5734 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/rdt/performance/datasets/datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8406 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/rdt/performance/datasets/numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1893 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/rdt/performance/datasets/pii.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1898 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/rdt/performance/datasets/text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      558 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/rdt/performance/datasets/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3372 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/rdt/performance/performance.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3442 2022-08-18 00:01:17.000000 rdt-1.5.1.dev1/rdt/performance/profiling.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.609571 rdt-1.5.1.dev1/rdt/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4940 2023-04-13 17:39:49.000000 rdt-1.5.1.dev1/rdt/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.609874 rdt-1.5.1.dev1/rdt/transformers/addons/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3345 2023-07-10 19:31:05.000000 rdt-1.5.1.dev1/rdt/transformers/addons/addons_setup.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    15934 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/rdt/transformers/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3792 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/rdt/transformers/boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21411 2023-04-13 17:39:49.000000 rdt-1.5.1.dev1/rdt/transformers/categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10281 2023-07-05 23:04:49.000000 rdt-1.5.1.dev1/rdt/transformers/datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5878 2023-06-28 22:45:00.000000 rdt-1.5.1.dev1/rdt/transformers/null.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22319 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/rdt/transformers/numerical.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.610523 rdt-1.5.1.dev1/rdt/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2022-08-18 00:01:17.000000 rdt-1.5.1.dev1/rdt/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12447 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/rdt/transformers/pii/anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1052 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/rdt/transformers/pii/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4847 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/rdt/transformers/text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4576 2023-04-26 21:05:25.000000 rdt-1.5.1.dev1/rdt/transformers/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.604701 rdt-1.5.1.dev1/rdt.egg-info/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    52585 2023-07-10 20:51:21.000000 rdt-1.5.1.dev1/rdt.egg-info/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2835 2023-07-10 20:51:21.000000 rdt-1.5.1.dev1/rdt.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-07-10 20:51:21.000000 rdt-1.5.1.dev1/rdt.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-07-10 20:51:21.000000 rdt-1.5.1.dev1/rdt.egg-info/not-zip-safe
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1448 2023-07-10 20:51:21.000000 rdt-1.5.1.dev1/rdt.egg-info/requires.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        4 2023-07-10 20:51:21.000000 rdt-1.5.1.dev1/rdt.egg-info/top_level.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-07-10 20:51:21.623563 rdt-1.5.1.dev1/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4134 2023-07-10 19:31:05.000000 rdt-1.5.1.dev1/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.611028 rdt-1.5.1.dev1/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/tests/code_style.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18316 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/tests/contributing.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.599424 rdt-1.5.1.dev1/tests/datasets/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.612002 rdt-1.5.1.dev1/tests/datasets/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/datasets/tests/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/datasets/tests/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/datasets/tests/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/datasets/tests/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/datasets/tests/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.612600 rdt-1.5.1.dev1/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/integration/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    45119 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/tests/integration/test_hyper_transformer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9434 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/tests/integration/test_transformers.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.614165 rdt-1.5.1.dev1/tests/integration/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/integration/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.614517 rdt-1.5.1.dev1/tests/integration/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/integration/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6410 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/tests/integration/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/tests/integration/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3425 2023-06-28 22:45:00.000000 rdt-1.5.1.dev1/tests/integration/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt-1.5.1.dev1/tests/integration/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5946 2023-07-05 23:04:49.000000 rdt-1.5.1.dev1/tests/integration/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10507 2023-06-28 22:45:00.000000 rdt-1.5.1.dev1/tests/integration/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt-1.5.1.dev1/tests/integration/transformers/test_text.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.615245 rdt-1.5.1.dev1/tests/performance/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/performance/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/performance/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt-1.5.1.dev1/tests/performance/test_performance.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.615580 rdt-1.5.1.dev1/tests/performance/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/performance/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt-1.5.1.dev1/tests/performance/tests/test_profiling.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.616280 rdt-1.5.1.dev1/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/unit/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5961 2023-06-20 18:01:47.000000 rdt-1.5.1.dev1/tests/unit/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   103941 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/tests/unit/test_hyper_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.619763 rdt-1.5.1.dev1/tests/unit/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/unit/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.620691 rdt-1.5.1.dev1/tests/unit/transformers/addons/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/unit/transformers/addons/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.621658 rdt-1.5.1.dev1/tests/unit/transformers/addons/identity/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/unit/transformers/addons/identity/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/tests/unit/transformers/addons/identity/test_identity.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.622565 rdt-1.5.1.dev1/tests/unit/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/unit/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    27923 2023-04-13 17:39:49.000000 rdt-1.5.1.dev1/tests/unit/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/tests/unit/transformers/pii/test_utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/tests/unit/transformers/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    42015 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/tests/unit/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8973 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/tests/unit/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt-1.5.1.dev1/tests/unit/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18310 2023-07-05 23:04:49.000000 rdt-1.5.1.dev1/tests/unit/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    19138 2023-06-28 22:45:00.000000 rdt-1.5.1.dev1/tests/unit/transformers/test_null.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    57532 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/tests/unit/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt-1.5.1.dev1/tests/unit/transformers/test_text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt-1.5.1.dev1/tests/unit/transformers/test_utils.py
```

### Comparing `rdt-1.5.1.dev0/CONTRIBUTING.rst` & `rdt-1.5.1.dev1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/HISTORY.md` & `rdt-1.5.1.dev1/HISTORY.md`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/LICENSE` & `rdt-1.5.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/PKG-INFO` & `rdt-1.5.1.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: rdt
-Version: 1.5.1.dev0
+Version: 1.5.1.dev1
 Summary: Reversible Data Transforms
 Home-page: https://github.com/sdv-dev/RDT
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: rdt
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7,<3.12
+Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 Provides-Extra: copulas
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS.rst
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 2.1 Name: rdt Version: 1.5.1.dev0 Summary: Reversible Data
+Metadata-Version: 2.1 Name: rdt Version: 1.5.1.dev1 Summary: Reversible Data
 Transforms Home-page: https://github.com/sdv-dev/RDT Author: DataCebo, Inc.
 Author-email: info@sdv.dev License: BSL-1.1 Keywords: rdt Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Requires-Python: >=3.7,<3.12 Description-Content-Type: text/
-markdown Provides-Extra: copulas Provides-Extra: test Provides-Extra: dev
-License-File: LICENSE License-File: AUTHORS.rst
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Requires-Python: >=3.8,<3.12
+Description-Content-Type: text/markdown Provides-Extra: copulas Provides-Extra:
+test Provides-Extra: dev License-File: LICENSE License-File: AUTHORS.rst
 
   This repository is part of The_Synthetic_Data_Vault_Project, a project from
                                    DataCebo.
 [![Development Status](https://img.shields.io/badge/Development%20Status-3%20--
                   %20Alpha-yellow)](https://pypi.org/search/
     ?q=&o=&c=Development+Status+%3A%3A+3+-+Alpha) [![PyPi Shield](https://
    img.shields.io/pypi/v/RDT.svg)](https://pypi.python.org/pypi/RDT) [![Unit
```

### Comparing `rdt-1.5.1.dev0/README.md` & `rdt-1.5.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/RELEASE.md` & `rdt-1.5.1.dev1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/__init__.py` & `rdt-1.5.1.dev1/rdt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for RDT."""
 
 
 __author__ = 'DataCebo, Inc.'
 __email__ = 'info@sdv.dev'
-__version__ = '1.5.1.dev0'
+__version__ = '1.5.1.dev1'
 
 
 import sys
 import warnings
 from operator import attrgetter
 from types import ModuleType
```

### Comparing `rdt-1.5.1.dev0/rdt/errors.py` & `rdt-1.5.1.dev1/rdt/errors.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/hyper_transformer.py` & `rdt-1.5.1.dev1/rdt/hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/performance/datasets/__init__.py` & `rdt-1.5.1.dev1/rdt/performance/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/performance/datasets/base.py` & `rdt-1.5.1.dev1/rdt/performance/datasets/base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/performance/datasets/boolean.py` & `rdt-1.5.1.dev1/rdt/performance/datasets/boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/performance/datasets/categorical.py` & `rdt-1.5.1.dev1/rdt/performance/datasets/categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/performance/datasets/datetime.py` & `rdt-1.5.1.dev1/rdt/performance/datasets/datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/performance/datasets/numerical.py` & `rdt-1.5.1.dev1/rdt/performance/datasets/numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/performance/datasets/pii.py` & `rdt-1.5.1.dev1/rdt/performance/datasets/pii.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/performance/datasets/text.py` & `rdt-1.5.1.dev1/rdt/performance/datasets/text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/performance/datasets/utils.py` & `rdt-1.5.1.dev1/rdt/performance/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/performance/performance.py` & `rdt-1.5.1.dev1/rdt/performance/performance.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/performance/profiling.py` & `rdt-1.5.1.dev1/rdt/performance/profiling.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/transformers/__init__.py` & `rdt-1.5.1.dev1/rdt/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/transformers/addons/addons_setup.py` & `rdt-1.5.1.dev1/rdt/transformers/addons/addons_setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,14 @@
         author_email='info@sdv.dev',
         classifiers=[
             'Development Status :: 2 - Pre-Alpha',
             'Intended Audience :: Developers',
             'License :: Free for non-commercial use',
             'Natural Language :: English',
             'Programming Language :: Python :: 3',
-            'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
             'Programming Language :: Python :: 3.11',
             'Topic :: Scientific/Engineering :: Artificial Intelligence',
         ],
         description='Reversible Data Transforms',
@@ -55,15 +54,15 @@
         install_requires=install_requires,
         keywords=['rdt', addon_name],
         license='BSL-1.1',
         long_description=README,
         long_description_content_type='text/markdown',
         name=addon_name,
         packages=find_namespace_packages(include=[addon_module]),
-        python_requires='>=3.7,<3.12',
+        python_requires='>=3.8,<3.12',
         url='https://github.com/sdv-dev/RDT',
         version=RDT_VERSION,
         zip_safe=False,
     )
 
 
 def _run():
```

### Comparing `rdt-1.5.1.dev0/rdt/transformers/base.py` & `rdt-1.5.1.dev1/rdt/transformers/base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/transformers/boolean.py` & `rdt-1.5.1.dev1/rdt/transformers/boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/transformers/categorical.py` & `rdt-1.5.1.dev1/rdt/transformers/categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/transformers/datetime.py` & `rdt-1.5.1.dev1/rdt/transformers/datetime.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Transformer for datetime data."""
 import numpy as np
 import pandas as pd
-from pandas.api.types import is_datetime64_dtype
+from pandas.api.types import is_datetime64_dtype, is_numeric_dtype
 from pandas.core.tools.datetimes import _guess_datetime_format_for_array
 
 from rdt.transformers.base import BaseTransformer
 from rdt.transformers.null import NullTransformer
 
 
 class UnixTimestampEncoder(BaseTransformer):
@@ -51,15 +51,34 @@
         if model_missing_values is not None:
             self._set_model_missing_values(model_missing_values)
 
         self.datetime_format = datetime_format
         self._dtype = None
 
     def _convert_to_datetime(self, data):
-        if data.dtype == 'object':
+        """Convert datetime column into datetime dtype.
+
+        Convert the datetime column to datetime dtype using the ``datetime_format``.
+        All non-numeric columns will automatically be cast to datetimes. Numeric columns
+        with a ``datetime_format`` will be treated as strings and cast to datetime. Numeric
+        columns without a ``datetime_format`` will be treated as already converted datetimes.
+
+        Args:
+            data (pandas.Series):
+                The datetime column.
+
+        Raises:
+            - ``TypeError`` if data cannot be converted to datetime.
+            - ``ValueError`` if data does not match the specified datetime format
+
+        Returns:
+            pandas.Series:
+                The datetime column converted to the datetime dtype.
+        """
+        if self.datetime_format or not is_numeric_dtype(data):
             try:
                 pandas_datetime_format = None
                 if self.datetime_format:
                     pandas_datetime_format = self.datetime_format.replace('%-', '%')
 
                 data = pd.to_datetime(data, format=pandas_datetime_format)
 
@@ -134,21 +153,24 @@
 
         Returns:
             pandas.Series
         """
         data = self._reverse_transform_helper(data)
         datetime_data = pd.to_datetime(data)
         if self.datetime_format:
-            if self._dtype == 'object':
-                datetime_data = datetime_data.dt.strftime(self.datetime_format)
-            elif is_datetime64_dtype(self._dtype) and '.%f' not in self.datetime_format:
+            if is_datetime64_dtype(self._dtype) and '.%f' not in self.datetime_format:
                 datetime_data = pd.to_datetime(
                     datetime_data.dt.strftime(self.datetime_format),
                     format=self.datetime_format,
                 )
+            else:
+                datetime_data = datetime_data.dt.strftime(self.datetime_format).astype(self._dtype)
+        elif is_numeric_dtype(self._dtype):
+            datetime_data = pd.to_numeric(datetime_data.astype('object'), errors='coerce')
+            datetime_data = datetime_data.astype(self._dtype)
 
         return datetime_data
 
 
 class OptimizedTimestampEncoder(UnixTimestampEncoder):
     """Optimized transformer for datetime data.
```

### Comparing `rdt-1.5.1.dev0/rdt/transformers/null.py` & `rdt-1.5.1.dev1/rdt/transformers/null.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/transformers/numerical.py` & `rdt-1.5.1.dev1/rdt/transformers/numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/transformers/pii/anonymizer.py` & `rdt-1.5.1.dev1/rdt/transformers/pii/anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/transformers/pii/utils.py` & `rdt-1.5.1.dev1/rdt/transformers/pii/utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/transformers/text.py` & `rdt-1.5.1.dev1/rdt/transformers/text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt/transformers/utils.py` & `rdt-1.5.1.dev1/rdt/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt.egg-info/PKG-INFO` & `rdt-1.5.1.dev1/rdt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: rdt
-Version: 1.5.1.dev0
+Version: 1.5.1.dev1
 Summary: Reversible Data Transforms
 Home-page: https://github.com/sdv-dev/RDT
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: rdt
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7,<3.12
+Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 Provides-Extra: copulas
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS.rst
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 2.1 Name: rdt Version: 1.5.1.dev0 Summary: Reversible Data
+Metadata-Version: 2.1 Name: rdt Version: 1.5.1.dev1 Summary: Reversible Data
 Transforms Home-page: https://github.com/sdv-dev/RDT Author: DataCebo, Inc.
 Author-email: info@sdv.dev License: BSL-1.1 Keywords: rdt Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Requires-Python: >=3.7,<3.12 Description-Content-Type: text/
-markdown Provides-Extra: copulas Provides-Extra: test Provides-Extra: dev
-License-File: LICENSE License-File: AUTHORS.rst
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Requires-Python: >=3.8,<3.12
+Description-Content-Type: text/markdown Provides-Extra: copulas Provides-Extra:
+test Provides-Extra: dev License-File: LICENSE License-File: AUTHORS.rst
 
   This repository is part of The_Synthetic_Data_Vault_Project, a project from
                                    DataCebo.
 [![Development Status](https://img.shields.io/badge/Development%20Status-3%20--
                   %20Alpha-yellow)](https://pypi.org/search/
     ?q=&o=&c=Development+Status+%3A%3A+3+-+Alpha) [![PyPi Shield](https://
    img.shields.io/pypi/v/RDT.svg)](https://pypi.python.org/pypi/RDT) [![Unit
```

### Comparing `rdt-1.5.1.dev0/rdt.egg-info/SOURCES.txt` & `rdt-1.5.1.dev1/rdt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/rdt.egg-info/requires.txt` & `rdt-1.5.1.dev1/rdt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/setup.cfg` & `rdt-1.5.1.dev1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.5.1.dev0
+current_version = 1.5.1.dev1
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `rdt-1.5.1.dev0/setup.py` & `rdt-1.5.1.dev1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,14 @@
     author_email='info@sdv.dev',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: Free for non-commercial use',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
     description='Reversible Data Transforms',
@@ -131,15 +130,15 @@
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     name='rdt',
     packages=find_namespace_packages(
         include=['rdt', 'rdt.*'],
         exclude=['rdt.transformers.addons.*']
     ),
-    python_requires='>=3.7,<3.12',
+    python_requires='>=3.8,<3.12',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/RDT',
-    version='1.5.1.dev0',
+    version='1.5.1.dev1',
     zip_safe=False,
 )
```

### Comparing `rdt-1.5.1.dev0/tests/__init__.py` & `rdt-1.5.1.dev1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/code_style.py` & `rdt-1.5.1.dev1/tests/code_style.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/contributing.py` & `rdt-1.5.1.dev1/tests/contributing.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/datasets/tests/test_boolean.py` & `rdt-1.5.1.dev1/tests/datasets/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/datasets/tests/test_categorical.py` & `rdt-1.5.1.dev1/tests/datasets/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/datasets/tests/test_datetime.py` & `rdt-1.5.1.dev1/tests/datasets/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/datasets/tests/test_numerical.py` & `rdt-1.5.1.dev1/tests/datasets/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/datasets/tests/test_utils.py` & `rdt-1.5.1.dev1/tests/datasets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/integration/test_hyper_transformer.py` & `rdt-1.5.1.dev1/tests/integration/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/integration/test_transformers.py` & `rdt-1.5.1.dev1/tests/integration/test_transformers.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/integration/transformers/pii/test_anonymizer.py` & `rdt-1.5.1.dev1/tests/integration/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/integration/transformers/test_base.py` & `rdt-1.5.1.dev1/tests/integration/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/integration/transformers/test_boolean.py` & `rdt-1.5.1.dev1/tests/integration/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/integration/transformers/test_categorical.py` & `rdt-1.5.1.dev1/tests/integration/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/integration/transformers/test_datetime.py` & `rdt-1.5.1.dev1/tests/integration/transformers/test_datetime.py`

 * *Files 16% similar despite different names*

```diff
@@ -86,14 +86,55 @@
             'column': [3.500064e+17, 845510400000000000, -145497600000000000],
             'column.is_null': [1., 0., 0.]
         })
 
         pd.testing.assert_frame_equal(expected_transformed, transformed)
         pd.testing.assert_frame_equal(reverted, data)
 
+    def test_unixtimestampencoder_with_integer_datetimes(self):
+        """Test that the transformer properly handles integer columns."""
+        # Setup
+        ute = UnixTimestampEncoder('mean', True, datetime_format='%m%d%Y')
+        data = pd.DataFrame({'column': [1201992, 11022028, 10011990]})
+
+        # Run
+        ute.fit(data, column='column')
+        ute.set_random_state(np.random.RandomState(7), 'reverse_transform')
+        transformed = ute.transform(data)
+        reverted = ute.reverse_transform(transformed)
+
+        # Asserts
+        expected_transformed = pd.DataFrame({
+            'column': [6.958656e+17, 1.856736e+18, 6.547392e+17],
+        })
+
+        pd.testing.assert_frame_equal(expected_transformed, transformed)
+        pd.testing.assert_frame_equal(reverted, data)
+
+    def test_unixtimestampencoder_with_nans(self):
+        """Test that the transformer properly handles null columns."""
+        # Setup
+        ute = UnixTimestampEncoder('mean', True)
+        data = pd.DataFrame({'column': [np.nan, np.nan, np.nan]})
+
+        # Run
+        ute.fit(data, column='column')
+        ute.set_random_state(np.random.RandomState(7), 'reverse_transform')
+        transformed = ute.transform(data)
+        reverted = ute.reverse_transform(transformed)
+
+        # Asserts
+        expected_transformed = pd.DataFrame({
+            'column': [0., 0., 0.],
+            'column.is_null': [1., 1., 1.]
+        })
+
+        pd.testing.assert_frame_equal(expected_transformed, transformed)
+        pd.testing.assert_frame_equal(reverted, data)
+
 
 class TestOptimizedTimestampEncoder:
     def test_optimizedtimestampencoder(self):
         ote = OptimizedTimestampEncoder(missing_value_replacement='mean')
         data = pd.DataFrame({'column': pd.to_datetime([None, '1996-10-17', '1965-05-23'])})
 
         # Run
```

### Comparing `rdt-1.5.1.dev0/tests/integration/transformers/test_numerical.py` & `rdt-1.5.1.dev1/tests/integration/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/integration/transformers/test_text.py` & `rdt-1.5.1.dev1/tests/integration/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/performance/test_performance.py` & `rdt-1.5.1.dev1/tests/performance/test_performance.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/performance/tests/test_profiling.py` & `rdt-1.5.1.dev1/tests/performance/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/unit/test___init__.py` & `rdt-1.5.1.dev1/tests/unit/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/unit/test_hyper_transformer.py` & `rdt-1.5.1.dev1/tests/unit/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/unit/transformers/addons/identity/test_identity.py` & `rdt-1.5.1.dev1/tests/unit/transformers/addons/identity/test_identity.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/unit/transformers/pii/test_anonymizer.py` & `rdt-1.5.1.dev1/tests/unit/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/unit/transformers/pii/test_utils.py` & `rdt-1.5.1.dev1/tests/unit/transformers/pii/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/unit/transformers/test___init__.py` & `rdt-1.5.1.dev1/tests/unit/transformers/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/unit/transformers/test_base.py` & `rdt-1.5.1.dev1/tests/unit/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/unit/transformers/test_boolean.py` & `rdt-1.5.1.dev1/tests/unit/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/unit/transformers/test_categorical.py` & `rdt-1.5.1.dev1/tests/unit/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/unit/transformers/test_datetime.py` & `rdt-1.5.1.dev1/tests/unit/transformers/test_datetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -426,14 +426,45 @@
         output = ute._reverse_transform(transformed)
 
         # Assert
         expected = pd.Series(['Jan 1, 2020', 'Feb 1, 2020', 'Mar 1, 2020'])
         if 'windows' not in platform.system().lower():
             pd.testing.assert_series_equal(output, expected)
 
+    def test__reverse_transform_datetime_format_with_nans(self):
+        """Test the ``_reverse_transform`` method returns the correct datetime format with nans."""
+        # Setup
+        ute = UnixTimestampEncoder()
+        ute.datetime_format = '%b %d, %Y'
+        transformed = np.array([1.5778368e+18, 1.5805152e+18, np.nan])
+        ute._dtype = 'object'
+        ute.null_transformer = NullTransformer('mean')
+
+        # Run
+        output = ute._reverse_transform(transformed)
+
+        # Assert
+        expected = pd.Series(['Jan 01, 2020', 'Feb 01, 2020', np.nan])
+        pd.testing.assert_series_equal(output, expected)
+
+    def test__reverse_transform_only_nans(self):
+        """Test the ``_reverse_transform`` method returns the correct datetime format with nans."""
+        # Setup
+        ute = UnixTimestampEncoder()
+        transformed = np.array([np.nan, np.nan, np.nan])
+        ute._dtype = 'float'
+        ute.null_transformer = NullTransformer('mean')
+
+        # Run
+        output = ute._reverse_transform(transformed)
+
+        # Assert
+        expected = pd.Series([np.nan, np.nan, np.nan])
+        pd.testing.assert_series_equal(output, expected)
+
 
 class TestOptimizedTimestampEncoder:
 
     def test__find_divider(self):
         """Test the ``_find_divider`` method.
 
         Find the greatest common denominator out of these values: [10] * 9 + [60, 60, 24],
```

### Comparing `rdt-1.5.1.dev0/tests/unit/transformers/test_null.py` & `rdt-1.5.1.dev1/tests/unit/transformers/test_null.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/unit/transformers/test_numerical.py` & `rdt-1.5.1.dev1/tests/unit/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/unit/transformers/test_text.py` & `rdt-1.5.1.dev1/tests/unit/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev0/tests/unit/transformers/test_utils.py` & `rdt-1.5.1.dev1/tests/unit/transformers/test_utils.py`

 * *Files identical despite different names*

