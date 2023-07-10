# Comparing `tmp/velilogger-1.0.0.tar.gz` & `tmp/velilogger-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velilogger-1.0.0.tar", last modified: Mon Jul 10 10:32:48 2023, max compression
+gzip compressed data, was "velilogger-1.0.1.tar", last modified: Mon Jul 10 16:15:35 2023, max compression
```

## Comparing `velilogger-1.0.0.tar` & `velilogger-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-10 10:32:48.548033 velilogger-1.0.0/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-07-05 09:25:18.000000 velilogger-1.0.0/MANIFEST.in
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1652 2023-07-10 10:32:48.547928 velilogger-1.0.0/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1477 2023-07-05 09:25:18.000000 velilogger-1.0.0/readme.md
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-10 10:32:48.548064 velilogger-1.0.0/setup.cfg
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      373 2023-07-10 10:32:04.000000 velilogger-1.0.0/setup.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-10 10:32:48.547789 velilogger-1.0.0/velilogger.egg-info/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1652 2023-07-10 10:32:48.000000 velilogger-1.0.0/velilogger.egg-info/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      180 2023-07-10 10:32:48.000000 velilogger-1.0.0/velilogger.egg-info/SOURCES.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-10 10:32:48.000000 velilogger-1.0.0/velilogger.egg-info/dependency_links.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       11 2023-07-10 10:32:48.000000 velilogger-1.0.0/velilogger.egg-info/top_level.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      995 2023-07-10 10:03:37.000000 velilogger-1.0.0/velilogger.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-10 16:15:35.705651 velilogger-1.0.1/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-07-05 09:25:18.000000 velilogger-1.0.1/MANIFEST.in
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2471 2023-07-10 16:15:35.705552 velilogger-1.0.1/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2297 2023-07-10 16:13:56.000000 velilogger-1.0.1/readme.md
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-10 16:15:35.705680 velilogger-1.0.1/setup.cfg
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      373 2023-07-10 16:15:20.000000 velilogger-1.0.1/setup.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-10 16:15:35.705424 velilogger-1.0.1/velilogger.egg-info/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2471 2023-07-10 16:15:35.000000 velilogger-1.0.1/velilogger.egg-info/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      180 2023-07-10 16:15:35.000000 velilogger-1.0.1/velilogger.egg-info/SOURCES.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-10 16:15:35.000000 velilogger-1.0.1/velilogger.egg-info/dependency_links.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       11 2023-07-10 16:15:35.000000 velilogger-1.0.1/velilogger.egg-info/top_level.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      995 2023-07-10 10:03:37.000000 velilogger-1.0.1/velilogger.py
```

### Comparing `velilogger-1.0.0/velilogger.py` & `velilogger-1.0.1/velilogger.py`

 * *Files identical despite different names*

