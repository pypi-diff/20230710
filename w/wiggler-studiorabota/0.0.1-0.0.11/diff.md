# Comparing `tmp/wiggler_studiorabota-0.0.1.tar.gz` & `tmp/wiggler_studiorabota-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiggler_studiorabota-0.0.1.tar", last modified: Mon Jul 10 20:09:37 2023, max compression
+gzip compressed data, was "wiggler_studiorabota-0.0.11.tar", last modified: Mon Jul 10 20:06:31 2023, max compression
```

## Comparing `wiggler_studiorabota-0.0.1.tar` & `wiggler_studiorabota-0.0.11.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-10 20:09:37.053799 wiggler_studiorabota-0.0.1/
--rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-10 20:09:37.053635 wiggler_studiorabota-0.0.1/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)       91 2023-07-10 20:08:40.000000 wiggler_studiorabota-0.0.1/README.md
--rw-r--r--   0 vincent    (501) staff       (20)      458 2023-07-10 20:07:37.000000 wiggler_studiorabota-0.0.1/pyproject.toml
--rw-r--r--   0 vincent    (501) staff       (20)       38 2023-07-10 20:09:37.053837 wiggler_studiorabota-0.0.1/setup.cfg
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-10 20:09:37.052302 wiggler_studiorabota-0.0.1/wiggler/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-07-09 16:41:51.000000 wiggler_studiorabota-0.0.1/wiggler/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)      321 2023-07-09 20:24:07.000000 wiggler_studiorabota-0.0.1/wiggler/cli.py
--rw-r--r--   0 vincent    (501) staff       (20)      709 2023-07-10 19:47:45.000000 wiggler_studiorabota-0.0.1/wiggler/main.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-10 20:09:37.053385 wiggler_studiorabota-0.0.1/wiggler_studiorabota.egg-info/
--rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-10 20:09:37.000000 wiggler_studiorabota-0.0.1/wiggler_studiorabota.egg-info/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)      298 2023-07-10 20:09:37.000000 wiggler_studiorabota-0.0.1/wiggler_studiorabota.egg-info/SOURCES.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2023-07-10 20:09:37.000000 wiggler_studiorabota-0.0.1/wiggler_studiorabota.egg-info/dependency_links.txt
--rw-r--r--   0 vincent    (501) staff       (20)       45 2023-07-10 20:09:37.000000 wiggler_studiorabota-0.0.1/wiggler_studiorabota.egg-info/entry_points.txt
--rw-r--r--   0 vincent    (501) staff       (20)        8 2023-07-10 20:09:37.000000 wiggler_studiorabota-0.0.1/wiggler_studiorabota.egg-info/top_level.txt
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-10 20:06:31.806705 wiggler_studiorabota-0.0.11/
+-rw-r--r--   0 vincent    (501) staff       (20)      391 2023-07-10 20:06:31.806558 wiggler_studiorabota-0.0.11/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)      459 2023-07-10 20:05:41.000000 wiggler_studiorabota-0.0.11/pyproject.toml
+-rw-r--r--   0 vincent    (501) staff       (20)       38 2023-07-10 20:06:31.806740 wiggler_studiorabota-0.0.11/setup.cfg
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-10 20:06:31.805499 wiggler_studiorabota-0.0.11/wiggler/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-07-09 16:41:51.000000 wiggler_studiorabota-0.0.11/wiggler/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)      321 2023-07-09 20:24:07.000000 wiggler_studiorabota-0.0.11/wiggler/cli.py
+-rw-r--r--   0 vincent    (501) staff       (20)      709 2023-07-10 19:47:45.000000 wiggler_studiorabota-0.0.11/wiggler/main.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-10 20:06:31.806356 wiggler_studiorabota-0.0.11/wiggler_studiorabota.egg-info/
+-rw-r--r--   0 vincent    (501) staff       (20)      391 2023-07-10 20:06:31.000000 wiggler_studiorabota-0.0.11/wiggler_studiorabota.egg-info/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)      288 2023-07-10 20:06:31.000000 wiggler_studiorabota-0.0.11/wiggler_studiorabota.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        1 2023-07-10 20:06:31.000000 wiggler_studiorabota-0.0.11/wiggler_studiorabota.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       45 2023-07-10 20:06:31.000000 wiggler_studiorabota-0.0.11/wiggler_studiorabota.egg-info/entry_points.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        8 2023-07-10 20:06:31.000000 wiggler_studiorabota-0.0.11/wiggler_studiorabota.egg-info/top_level.txt
```

### Comparing `wiggler_studiorabota-0.0.1/wiggler/main.py` & `wiggler_studiorabota-0.0.11/wiggler/main.py`

 * *Files identical despite different names*

