# Comparing `tmp/swiftly-unix-0.0.2.tar.gz` & `tmp/swiftly-unix-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-unix-0.0.2.tar", last modified: Mon Jul 10 17:19:54 2023, max compression
+gzip compressed data, was "swiftly-unix-0.0.3.tar", last modified: Mon Jul 10 17:24:06 2023, max compression
```

## Comparing `swiftly-unix-0.0.2.tar` & `swiftly-unix-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:19:54.122316 swiftly-unix-0.0.2/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.0.2/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 17:19:54.122206 swiftly-unix-0.0.2/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:19:54.121524 swiftly-unix-0.0.2/scripts/
--rwxr-xr-x   0 brainspoof   (501) staff       (20)      134 2023-07-10 17:19:19.000000 swiftly-unix-0.0.2/scripts/swiftly
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-10 17:19:54.122351 swiftly-unix-0.0.2/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      162 2023-07-10 17:17:58.000000 swiftly-unix-0.0.2/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:19:54.122046 swiftly-unix-0.0.2/swiftly_unix.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 17:19:54.000000 swiftly-unix-0.0.2/swiftly_unix.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      176 2023-07-10 17:19:54.000000 swiftly-unix-0.0.2/swiftly_unix.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-10 17:19:54.000000 swiftly-unix-0.0.2/swiftly_unix.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-10 17:19:54.000000 swiftly-unix-0.0.2/swiftly_unix.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:24:06.548278 swiftly-unix-0.0.3/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.0.3/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 17:24:06.548168 swiftly-unix-0.0.3/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:24:06.546944 swiftly-unix-0.0.3/scripts/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)      134 2023-07-10 17:19:19.000000 swiftly-unix-0.0.3/scripts/swiftly
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-10 17:24:06.548314 swiftly-unix-0.0.3/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      162 2023-07-10 17:23:38.000000 swiftly-unix-0.0.3/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:24:06.547366 swiftly-unix-0.0.3/swiftly_unix/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.0.3/swiftly_unix/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)       46 2023-07-10 17:03:04.000000 swiftly-unix-0.0.3/swiftly_unix/script.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:24:06.548011 swiftly-unix-0.0.3/swiftly_unix.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 17:24:06.000000 swiftly-unix-0.0.3/swiftly_unix.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      224 2023-07-10 17:24:06.000000 swiftly-unix-0.0.3/swiftly_unix.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-10 17:24:06.000000 swiftly-unix-0.0.3/swiftly_unix.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-10 17:24:06.000000 swiftly-unix-0.0.3/swiftly_unix.egg-info/top_level.txt
```

### Comparing `swiftly-unix-0.0.2/LICENSE` & `swiftly-unix-0.0.3/LICENSE`

 * *Files identical despite different names*

