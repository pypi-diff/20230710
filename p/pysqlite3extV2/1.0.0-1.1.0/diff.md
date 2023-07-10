# Comparing `tmp/pysqlite3extV2-1.0.0.tar.gz` & `tmp/pysqlite3extV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysqlite3extV2-1.0.0.tar", last modified: Mon Jul 10 18:44:59 2023, max compression
+gzip compressed data, was "pysqlite3extV2-1.1.0.tar", last modified: Mon Jul 10 18:47:08 2023, max compression
```

## Comparing `pysqlite3extV2-1.0.0.tar` & `pysqlite3extV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:44:59.343315 pysqlite3extV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      347 2023-07-10 18:44:59.343315 pysqlite3extV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:44:59.343315 pysqlite3extV2-1.0.0/pysqlite3extV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-10 18:44:58.000000 pysqlite3extV2-1.0.0/pysqlite3extV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:44:59.343315 pysqlite3extV2-1.0.0/pysqlite3extV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      347 2023-07-10 18:44:59.000000 pysqlite3extV2-1.0.0/pysqlite3extV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      187 2023-07-10 18:44:59.000000 pysqlite3extV2-1.0.0/pysqlite3extV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 18:44:59.000000 pysqlite3extV2-1.0.0/pysqlite3extV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-10 18:44:59.000000 pysqlite3extV2-1.0.0/pysqlite3extV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 18:44:59.343315 pysqlite3extV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      560 2023-07-10 18:44:58.000000 pysqlite3extV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:47:08.786969 pysqlite3extV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-10 18:47:08.786969 pysqlite3extV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:47:08.782969 pysqlite3extV2-1.1.0/pysqlite3extV2/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-07-10 18:47:08.000000 pysqlite3extV2-1.1.0/pysqlite3extV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:47:08.786969 pysqlite3extV2-1.1.0/pysqlite3extV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-10 18:47:08.000000 pysqlite3extV2-1.1.0/pysqlite3extV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      187 2023-07-10 18:47:08.000000 pysqlite3extV2-1.1.0/pysqlite3extV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 18:47:08.000000 pysqlite3extV2-1.1.0/pysqlite3extV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-10 18:47:08.000000 pysqlite3extV2-1.1.0/pysqlite3extV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 18:47:08.786969 pysqlite3extV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      560 2023-07-10 18:47:08.000000 pysqlite3extV2-1.1.0/setup.py
```

### Comparing `pysqlite3extV2-1.0.0/setup.py` & `pysqlite3extV2-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pysqlite3extV2",
     version=VERSION,
```

