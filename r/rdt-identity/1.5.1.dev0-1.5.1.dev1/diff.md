# Comparing `tmp/rdt_identity-1.5.1.dev0.tar.gz` & `tmp/rdt_identity-1.5.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdt_identity-1.5.1.dev0.tar", last modified: Thu Jun 29 00:04:38 2023, max compression
+gzip compressed data, was "rdt_identity-1.5.1.dev1.tar", last modified: Mon Jul 10 20:51:23 2023, max compression
```

## Comparing `rdt_identity-1.5.1.dev0.tar` & `rdt_identity-1.5.1.dev1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:38.530970 rdt_identity-1.5.1.dev0/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev0/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22812 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev0/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    44576 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev0/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev0/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev0/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8014 2023-06-29 00:04:38.531064 rdt_identity-1.5.1.dev0/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev0/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev0/RELEASE.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:38.519896 rdt_identity-1.5.1.dev0/rdt/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:38.519961 rdt_identity-1.5.1.dev0/rdt/transformers/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:38.520026 rdt_identity-1.5.1.dev0/rdt/transformers/addons/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:38.523135 rdt_identity-1.5.1.dev0/rdt/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev0/rdt/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1170 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev0/rdt/transformers/addons/identity/identity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-06-29 00:04:38.531693 rdt_identity-1.5.1.dev0/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4183 2023-06-01 21:47:10.000000 rdt_identity-1.5.1.dev0/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:38.523564 rdt_identity-1.5.1.dev0/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev0/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev0/tests/code_style.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18316 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev0/tests/contributing.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:38.520273 rdt_identity-1.5.1.dev0/tests/datasets/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:38.524789 rdt_identity-1.5.1.dev0/tests/datasets/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev0/tests/datasets/tests/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev0/tests/datasets/tests/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev0/tests/datasets/tests/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev0/tests/datasets/tests/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev0/tests/datasets/tests/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:38.525326 rdt_identity-1.5.1.dev0/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev0/tests/integration/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    45119 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev0/tests/integration/test_hyper_transformer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9434 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev0/tests/integration/test_transformers.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:38.526515 rdt_identity-1.5.1.dev0/tests/integration/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev0/tests/integration/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:38.526857 rdt_identity-1.5.1.dev0/tests/integration/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev0/tests/integration/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6410 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev0/tests/integration/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev0/tests/integration/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3425 2023-06-28 22:45:00.000000 rdt_identity-1.5.1.dev0/tests/integration/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt_identity-1.5.1.dev0/tests/integration/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4386 2023-06-28 22:45:00.000000 rdt_identity-1.5.1.dev0/tests/integration/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10507 2023-06-28 22:45:00.000000 rdt_identity-1.5.1.dev0/tests/integration/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt_identity-1.5.1.dev0/tests/integration/transformers/test_text.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:38.527304 rdt_identity-1.5.1.dev0/tests/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev0/tests/performance/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev0/tests/performance/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt_identity-1.5.1.dev0/tests/performance/test_performance.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:38.527598 rdt_identity-1.5.1.dev0/tests/performance/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev0/tests/performance/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt_identity-1.5.1.dev0/tests/performance/tests/test_profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:38.528044 rdt_identity-1.5.1.dev0/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev0/tests/unit/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5961 2023-06-20 18:01:47.000000 rdt_identity-1.5.1.dev0/tests/unit/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   103941 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev0/tests/unit/test_hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:38.529909 rdt_identity-1.5.1.dev0/tests/unit/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev0/tests/unit/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:38.530054 rdt_identity-1.5.1.dev0/tests/unit/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev0/tests/unit/transformers/addons/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:38.530372 rdt_identity-1.5.1.dev0/tests/unit/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev0/tests/unit/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev0/tests/unit/transformers/addons/identity/test_identity.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-29 00:04:38.530841 rdt_identity-1.5.1.dev0/tests/unit/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev0/tests/unit/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    27923 2023-04-13 17:39:49.000000 rdt_identity-1.5.1.dev0/tests/unit/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev0/tests/unit/transformers/pii/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev0/tests/unit/transformers/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    42015 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev0/tests/unit/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8973 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev0/tests/unit/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt_identity-1.5.1.dev0/tests/unit/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    17137 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev0/tests/unit/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    19138 2023-06-28 22:45:00.000000 rdt_identity-1.5.1.dev0/tests/unit/transformers/test_null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    57532 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev0/tests/unit/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt_identity-1.5.1.dev0/tests/unit/transformers/test_text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt_identity-1.5.1.dev0/tests/unit/transformers/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.896900 rdt_identity-1.5.1.dev1/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev1/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22812 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev1/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    44576 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev1/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev1/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7964 2023-07-10 20:51:23.897003 rdt_identity-1.5.1.dev1/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev1/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/RELEASE.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.884719 rdt_identity-1.5.1.dev1/rdt/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.884791 rdt_identity-1.5.1.dev1/rdt/transformers/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.884859 rdt_identity-1.5.1.dev1/rdt/transformers/addons/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.888351 rdt_identity-1.5.1.dev1/rdt/transformers/addons/identity/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/rdt/transformers/addons/identity/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1170 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev1/rdt/transformers/addons/identity/identity.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-07-10 20:51:23.897564 rdt_identity-1.5.1.dev1/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4134 2023-07-10 19:31:05.000000 rdt_identity-1.5.1.dev1/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.888840 rdt_identity-1.5.1.dev1/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev1/tests/code_style.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18316 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev1/tests/contributing.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.885124 rdt_identity-1.5.1.dev1/tests/datasets/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.889681 rdt_identity-1.5.1.dev1/tests/datasets/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/datasets/tests/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/datasets/tests/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/datasets/tests/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/datasets/tests/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/datasets/tests/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.890220 rdt_identity-1.5.1.dev1/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/integration/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    45119 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev1/tests/integration/test_hyper_transformer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9434 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev1/tests/integration/test_transformers.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.891770 rdt_identity-1.5.1.dev1/tests/integration/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/integration/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.892133 rdt_identity-1.5.1.dev1/tests/integration/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/integration/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6410 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev1/tests/integration/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev1/tests/integration/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3425 2023-06-28 22:45:00.000000 rdt_identity-1.5.1.dev1/tests/integration/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt_identity-1.5.1.dev1/tests/integration/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5946 2023-07-05 23:04:49.000000 rdt_identity-1.5.1.dev1/tests/integration/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10507 2023-06-28 22:45:00.000000 rdt_identity-1.5.1.dev1/tests/integration/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt_identity-1.5.1.dev1/tests/integration/transformers/test_text.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.892671 rdt_identity-1.5.1.dev1/tests/performance/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/performance/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/performance/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt_identity-1.5.1.dev1/tests/performance/test_performance.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.893015 rdt_identity-1.5.1.dev1/tests/performance/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/performance/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt_identity-1.5.1.dev1/tests/performance/tests/test_profiling.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.893518 rdt_identity-1.5.1.dev1/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/unit/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5961 2023-06-20 18:01:47.000000 rdt_identity-1.5.1.dev1/tests/unit/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   103941 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev1/tests/unit/test_hyper_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.895367 rdt_identity-1.5.1.dev1/tests/unit/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.895543 rdt_identity-1.5.1.dev1/tests/unit/transformers/addons/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/addons/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.895888 rdt_identity-1.5.1.dev1/tests/unit/transformers/addons/identity/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/addons/identity/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/addons/identity/test_identity.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.896723 rdt_identity-1.5.1.dev1/tests/unit/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    27923 2023-04-13 17:39:49.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/pii/test_utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    42015 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8973 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18310 2023-07-05 23:04:49.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    19138 2023-06-28 22:45:00.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/test_null.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    57532 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/test_text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/test_utils.py
```

### Comparing `rdt_identity-1.5.1.dev0/CONTRIBUTING.rst` & `rdt_identity-1.5.1.dev1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/HISTORY.md` & `rdt_identity-1.5.1.dev1/HISTORY.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/LICENSE` & `rdt_identity-1.5.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/PKG-INFO` & `rdt_identity-1.5.1.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: rdt_identity
-Version: 1.5.1.dev0
+Version: 1.5.1.dev1
 Summary: Reversible Data Transforms
 Home-page: https://github.com/sdv-dev/RDT
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: rdt,rdt_identity
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
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 <div align="center">
 <br/>
 <p align="center">
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 2.1 Name: rdt_identity Version: 1.5.1.dev0 Summary:
+Metadata-Version: 2.1 Name: rdt_identity Version: 1.5.1.dev1 Summary:
 Reversible Data Transforms Home-page: https://github.com/sdv-dev/RDT Author:
 DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1 Keywords:
 rdt,rdt_identity Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: Free for non-commercial
 use Classifier: Natural Language :: English Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Requires-Python: >=3.7,<3.12
-Description-Content-Type: text/markdown License-File: LICENSE License-File:
-AUTHORS.rst
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Scientific/Engineering :: Artificial Intelligence Requires-Python:
+>=3.8,<3.12 Description-Content-Type: text/markdown License-File: LICENSE
+License-File: AUTHORS.rst
 
   This repository is part of The_Synthetic_Data_Vault_Project, a project from
                                    DataCebo.
 [![Development Status](https://img.shields.io/badge/Development%20Status-3%20--
                   %20Alpha-yellow)](https://pypi.org/search/
     ?q=&o=&c=Development+Status+%3A%3A+3+-+Alpha) [![PyPi Shield](https://
    img.shields.io/pypi/v/RDT.svg)](https://pypi.python.org/pypi/RDT) [![Unit
```

### Comparing `rdt_identity-1.5.1.dev0/README.md` & `rdt_identity-1.5.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/RELEASE.md` & `rdt_identity-1.5.1.dev1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/rdt/transformers/addons/identity/identity.py` & `rdt_identity-1.5.1.dev1/rdt/transformers/addons/identity/identity.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/setup.cfg` & `rdt_identity-1.5.1.dev1/setup.cfg`

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

### Comparing `rdt_identity-1.5.1.dev0/setup.py` & `rdt_identity-1.5.1.dev1/setup.py`

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

### Comparing `rdt_identity-1.5.1.dev0/tests/__init__.py` & `rdt_identity-1.5.1.dev1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/code_style.py` & `rdt_identity-1.5.1.dev1/tests/code_style.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/contributing.py` & `rdt_identity-1.5.1.dev1/tests/contributing.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/datasets/tests/test_boolean.py` & `rdt_identity-1.5.1.dev1/tests/datasets/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/datasets/tests/test_categorical.py` & `rdt_identity-1.5.1.dev1/tests/datasets/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/datasets/tests/test_datetime.py` & `rdt_identity-1.5.1.dev1/tests/datasets/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/datasets/tests/test_numerical.py` & `rdt_identity-1.5.1.dev1/tests/datasets/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/datasets/tests/test_utils.py` & `rdt_identity-1.5.1.dev1/tests/datasets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/integration/test_hyper_transformer.py` & `rdt_identity-1.5.1.dev1/tests/integration/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/integration/test_transformers.py` & `rdt_identity-1.5.1.dev1/tests/integration/test_transformers.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/integration/transformers/pii/test_anonymizer.py` & `rdt_identity-1.5.1.dev1/tests/integration/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/integration/transformers/test_base.py` & `rdt_identity-1.5.1.dev1/tests/integration/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/integration/transformers/test_boolean.py` & `rdt_identity-1.5.1.dev1/tests/integration/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/integration/transformers/test_categorical.py` & `rdt_identity-1.5.1.dev1/tests/integration/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/integration/transformers/test_datetime.py` & `rdt_identity-1.5.1.dev1/tests/integration/transformers/test_datetime.py`

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

### Comparing `rdt_identity-1.5.1.dev0/tests/integration/transformers/test_numerical.py` & `rdt_identity-1.5.1.dev1/tests/integration/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/integration/transformers/test_text.py` & `rdt_identity-1.5.1.dev1/tests/integration/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/performance/test_performance.py` & `rdt_identity-1.5.1.dev1/tests/performance/test_performance.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/performance/tests/test_profiling.py` & `rdt_identity-1.5.1.dev1/tests/performance/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/unit/test___init__.py` & `rdt_identity-1.5.1.dev1/tests/unit/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/unit/test_hyper_transformer.py` & `rdt_identity-1.5.1.dev1/tests/unit/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/unit/transformers/addons/identity/test_identity.py` & `rdt_identity-1.5.1.dev1/tests/unit/transformers/addons/identity/test_identity.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/unit/transformers/pii/test_anonymizer.py` & `rdt_identity-1.5.1.dev1/tests/unit/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/unit/transformers/pii/test_utils.py` & `rdt_identity-1.5.1.dev1/tests/unit/transformers/pii/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/unit/transformers/test___init__.py` & `rdt_identity-1.5.1.dev1/tests/unit/transformers/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/unit/transformers/test_base.py` & `rdt_identity-1.5.1.dev1/tests/unit/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/unit/transformers/test_boolean.py` & `rdt_identity-1.5.1.dev1/tests/unit/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/unit/transformers/test_categorical.py` & `rdt_identity-1.5.1.dev1/tests/unit/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/unit/transformers/test_datetime.py` & `rdt_identity-1.5.1.dev1/tests/unit/transformers/test_datetime.py`

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

### Comparing `rdt_identity-1.5.1.dev0/tests/unit/transformers/test_null.py` & `rdt_identity-1.5.1.dev1/tests/unit/transformers/test_null.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/unit/transformers/test_numerical.py` & `rdt_identity-1.5.1.dev1/tests/unit/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/unit/transformers/test_text.py` & `rdt_identity-1.5.1.dev1/tests/unit/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev0/tests/unit/transformers/test_utils.py` & `rdt_identity-1.5.1.dev1/tests/unit/transformers/test_utils.py`

 * *Files identical despite different names*

