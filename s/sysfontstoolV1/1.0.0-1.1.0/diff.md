# Comparing `tmp/sysfontstoolV1-1.0.0.tar.gz` & `tmp/sysfontstoolV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysfontstoolV1-1.0.0.tar", last modified: Mon Jul 10 21:49:51 2023, max compression
+gzip compressed data, was "sysfontstoolV1-1.1.0.tar", last modified: Mon Jul 10 21:51:59 2023, max compression
```

## Comparing `sysfontstoolV1-1.0.0.tar` & `sysfontstoolV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:49:51.609873 sysfontstoolV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      347 2023-07-10 21:49:51.609873 sysfontstoolV1-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 21:49:51.609873 sysfontstoolV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      560 2023-07-10 21:49:50.000000 sysfontstoolV1-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:49:51.609873 sysfontstoolV1-1.0.0/sysfontstoolV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-10 21:49:50.000000 sysfontstoolV1-1.0.0/sysfontstoolV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:49:51.609873 sysfontstoolV1-1.0.0/sysfontstoolV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      347 2023-07-10 21:49:51.000000 sysfontstoolV1-1.0.0/sysfontstoolV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      187 2023-07-10 21:49:51.000000 sysfontstoolV1-1.0.0/sysfontstoolV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 21:49:51.000000 sysfontstoolV1-1.0.0/sysfontstoolV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-10 21:49:51.000000 sysfontstoolV1-1.0.0/sysfontstoolV1.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:51:59.157459 sysfontstoolV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-10 21:51:59.157459 sysfontstoolV1-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 21:51:59.157459 sysfontstoolV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      560 2023-07-10 21:51:58.000000 sysfontstoolV1-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:51:59.157459 sysfontstoolV1-1.1.0/sysfontstoolV1/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-07-10 21:51:58.000000 sysfontstoolV1-1.1.0/sysfontstoolV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:51:59.157459 sysfontstoolV1-1.1.0/sysfontstoolV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-10 21:51:59.000000 sysfontstoolV1-1.1.0/sysfontstoolV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      187 2023-07-10 21:51:59.000000 sysfontstoolV1-1.1.0/sysfontstoolV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 21:51:59.000000 sysfontstoolV1-1.1.0/sysfontstoolV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-10 21:51:59.000000 sysfontstoolV1-1.1.0/sysfontstoolV1.egg-info/top_level.txt
```

### Comparing `sysfontstoolV1-1.0.0/setup.py` & `sysfontstoolV1-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="sysfontstoolV1",
     version=VERSION,
```

