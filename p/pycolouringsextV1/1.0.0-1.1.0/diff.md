# Comparing `tmp/pycolouringsextV1-1.0.0.tar.gz` & `tmp/pycolouringsextV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycolouringsextV1-1.0.0.tar", last modified: Mon Jul 10 13:59:55 2023, max compression
+gzip compressed data, was "pycolouringsextV1-1.1.0.tar", last modified: Mon Jul 10 14:02:05 2023, max compression
```

## Comparing `pycolouringsextV1-1.0.0.tar` & `pycolouringsextV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:59:55.768450 pycolouringsextV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      350 2023-07-10 13:59:55.764450 pycolouringsextV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:59:55.764450 pycolouringsextV1-1.0.0/pycolouringsextV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-10 13:59:54.000000 pycolouringsextV1-1.0.0/pycolouringsextV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:59:55.764450 pycolouringsextV1-1.0.0/pycolouringsextV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      350 2023-07-10 13:59:55.000000 pycolouringsextV1-1.0.0/pycolouringsextV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      202 2023-07-10 13:59:55.000000 pycolouringsextV1-1.0.0/pycolouringsextV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 13:59:55.000000 pycolouringsextV1-1.0.0/pycolouringsextV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-10 13:59:55.000000 pycolouringsextV1-1.0.0/pycolouringsextV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 13:59:55.768450 pycolouringsextV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      563 2023-07-10 13:59:54.000000 pycolouringsextV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:02:05.144093 pycolouringsextV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-07-10 14:02:05.144093 pycolouringsextV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:02:05.144093 pycolouringsextV1-1.1.0/pycolouringsextV1/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-07-10 14:02:03.000000 pycolouringsextV1-1.1.0/pycolouringsextV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:02:05.144093 pycolouringsextV1-1.1.0/pycolouringsextV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-07-10 14:02:04.000000 pycolouringsextV1-1.1.0/pycolouringsextV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      202 2023-07-10 14:02:05.000000 pycolouringsextV1-1.1.0/pycolouringsextV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 14:02:04.000000 pycolouringsextV1-1.1.0/pycolouringsextV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-10 14:02:04.000000 pycolouringsextV1-1.1.0/pycolouringsextV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 14:02:05.144093 pycolouringsextV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      563 2023-07-10 14:02:03.000000 pycolouringsextV1-1.1.0/setup.py
```

### Comparing `pycolouringsextV1-1.0.0/setup.py` & `pycolouringsextV1-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pycolouringsextV1",
     version=VERSION,
```

