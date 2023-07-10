# Comparing `tmp/wiggler_studiorabota-0.0.1.tar.gz` & `tmp/wiggler_studiorabota-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiggler_studiorabota-0.0.1.tar", last modified: Mon Jul 10 20:09:37 2023, max compression
+gzip compressed data, was "wiggler_studiorabota-0.0.2.tar", last modified: Mon Jul 10 20:16:21 2023, max compression
```

## Comparing `wiggler_studiorabota-0.0.1.tar` & `wiggler_studiorabota-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
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
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-10 20:16:21.864207 wiggler_studiorabota-0.0.2/
+-rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-10 20:16:21.864062 wiggler_studiorabota-0.0.2/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)       91 2023-07-10 20:08:40.000000 wiggler_studiorabota-0.0.2/README.md
+-rw-r--r--   0 vincent    (501) staff       (20)      458 2023-07-10 20:16:15.000000 wiggler_studiorabota-0.0.2/pyproject.toml
+-rw-r--r--   0 vincent    (501) staff       (20)       38 2023-07-10 20:16:21.864241 wiggler_studiorabota-0.0.2/setup.cfg
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-10 20:16:21.862861 wiggler_studiorabota-0.0.2/wiggler/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-07-09 16:41:51.000000 wiggler_studiorabota-0.0.2/wiggler/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)      318 2023-07-10 20:15:53.000000 wiggler_studiorabota-0.0.2/wiggler/cli.py
+-rw-r--r--   0 vincent    (501) staff       (20)      709 2023-07-10 19:47:45.000000 wiggler_studiorabota-0.0.2/wiggler/main.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-10 20:16:21.863877 wiggler_studiorabota-0.0.2/wiggler_studiorabota.egg-info/
+-rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-10 20:16:21.000000 wiggler_studiorabota-0.0.2/wiggler_studiorabota.egg-info/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)      298 2023-07-10 20:16:21.000000 wiggler_studiorabota-0.0.2/wiggler_studiorabota.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        1 2023-07-10 20:16:21.000000 wiggler_studiorabota-0.0.2/wiggler_studiorabota.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       45 2023-07-10 20:16:21.000000 wiggler_studiorabota-0.0.2/wiggler_studiorabota.egg-info/entry_points.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        8 2023-07-10 20:16:21.000000 wiggler_studiorabota-0.0.2/wiggler_studiorabota.egg-info/top_level.txt
```

### Comparing `wiggler_studiorabota-0.0.1/wiggler/main.py` & `wiggler_studiorabota-0.0.2/wiggler/main.py`

 * *Files identical despite different names*

