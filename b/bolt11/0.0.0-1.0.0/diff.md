# Comparing `tmp/bolt11-0.0.0.tar.gz` & `tmp/bolt11-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bolt11-0.0.0.tar", last modified: Sat Dec 14 14:46:44 2019, max compression
+gzip compressed data, was "bolt11-1.0.0.tar", max compression
```

## Comparing `bolt11-0.0.0.tar` & `bolt11-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 eillarra   (501) staff       (20)        0 2019-12-14 14:46:44.000000 bolt11-0.0.0/
--rw-r--r--   0 eillarra   (501) staff       (20)     1896 2019-12-14 14:46:44.000000 bolt11-0.0.0/PKG-INFO
--rwxr-xr-x   0 eillarra   (501) staff       (20)      915 2019-12-14 14:38:01.000000 bolt11-0.0.0/README.md
-drwxr-xr-x   0 eillarra   (501) staff       (20)        0 2019-12-14 14:46:44.000000 bolt11-0.0.0/bolt11/
--rw-r--r--   0 eillarra   (501) staff       (20)        0 2019-12-11 15:09:59.000000 bolt11-0.0.0/bolt11/__init__.py
--rw-r--r--   0 eillarra   (501) staff       (20)       50 2019-12-11 15:02:11.000000 bolt11-0.0.0/bolt11/core.py
--rw-r--r--   0 eillarra   (501) staff       (20)      244 2019-12-11 16:16:06.000000 bolt11-0.0.0/bolt11/types.py
--rw-r--r--   0 eillarra   (501) staff       (20)      786 2019-12-11 16:29:33.000000 bolt11-0.0.0/bolt11/utils.py
-drwxr-xr-x   0 eillarra   (501) staff       (20)        0 2019-12-14 14:46:44.000000 bolt11-0.0.0/bolt11.egg-info/
--rw-r--r--   0 eillarra   (501) staff       (20)     1896 2019-12-14 14:46:43.000000 bolt11-0.0.0/bolt11.egg-info/PKG-INFO
--rw-r--r--   0 eillarra   (501) staff       (20)      233 2019-12-14 14:46:43.000000 bolt11-0.0.0/bolt11.egg-info/SOURCES.txt
--rw-r--r--   0 eillarra   (501) staff       (20)        1 2019-12-14 14:46:43.000000 bolt11-0.0.0/bolt11.egg-info/dependency_links.txt
--rw-r--r--   0 eillarra   (501) staff       (20)        1 2019-12-11 14:47:44.000000 bolt11-0.0.0/bolt11.egg-info/not-zip-safe
--rw-r--r--   0 eillarra   (501) staff       (20)        7 2019-12-14 14:46:43.000000 bolt11-0.0.0/bolt11.egg-info/top_level.txt
--rw-r--r--   0 eillarra   (501) staff       (20)       38 2019-12-14 14:46:44.000000 bolt11-0.0.0/setup.cfg
--rw-r--r--   0 eillarra   (501) staff       (20)     1108 2019-12-14 14:42:19.000000 bolt11-0.0.0/setup.py
+-rw-r--r--   0        0        0     1112 2023-07-10 18:02:06.217296 bolt11-1.0.0/LICENSE
+-rwxr-xr-x   0        0        0     3119 2023-07-10 18:02:06.217296 bolt11-1.0.0/README.md
+-rw-r--r--   0        0        0      353 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/__init__.py
+-rw-r--r--   0        0        0     1127 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/bit_utils.py
+-rw-r--r--   0        0        0      599 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/cli.py
+-rw-r--r--   0        0        0      243 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/compat.py
+-rw-r--r--   0        0        0     3932 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/decode.py
+-rw-r--r--   0        0        0     2926 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/encode.py
+-rw-r--r--   0        0        0     2850 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/models/fallback.py
+-rw-r--r--   0        0        0     3486 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/models/features.py
+-rw-r--r--   0        0        0     1768 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/models/routehint.py
+-rw-r--r--   0        0        0     2322 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/models/signature.py
+-rw-r--r--   0        0        0       26 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/py.typed
+-rw-r--r--   0        0        0     3940 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/types.py
+-rw-r--r--   0        0        0     1947 2023-07-10 18:02:06.217296 bolt11-1.0.0/bolt11/utils.py
+-rw-r--r--   0        0        0     1549 2023-07-10 18:02:06.217296 bolt11-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3932 1970-01-01 00:00:00.000000 bolt11-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

