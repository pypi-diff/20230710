# Comparing `tmp/swiftly-unix-0.0.3.tar.gz` & `tmp/swiftly-unix-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-unix-0.0.3.tar", last modified: Mon Jul 10 17:24:06 2023, max compression
+gzip compressed data, was "swiftly-unix-0.0.4.tar", last modified: Mon Jul 10 18:07:12 2023, max compression
```

## Comparing `swiftly-unix-0.0.3.tar` & `swiftly-unix-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:24:06.548278 swiftly-unix-0.0.3/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.0.3/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 17:24:06.548168 swiftly-unix-0.0.3/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:24:06.546944 swiftly-unix-0.0.3/scripts/
--rwxr-xr-x   0 brainspoof   (501) staff       (20)      134 2023-07-10 17:19:19.000000 swiftly-unix-0.0.3/scripts/swiftly
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-10 17:24:06.548314 swiftly-unix-0.0.3/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      162 2023-07-10 17:23:38.000000 swiftly-unix-0.0.3/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:24:06.547366 swiftly-unix-0.0.3/swiftly_unix/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.0.3/swiftly_unix/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)       46 2023-07-10 17:03:04.000000 swiftly-unix-0.0.3/swiftly_unix/script.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:24:06.548011 swiftly-unix-0.0.3/swiftly_unix.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 17:24:06.000000 swiftly-unix-0.0.3/swiftly_unix.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      224 2023-07-10 17:24:06.000000 swiftly-unix-0.0.3/swiftly_unix.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-10 17:24:06.000000 swiftly-unix-0.0.3/swiftly_unix.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-10 17:24:06.000000 swiftly-unix-0.0.3/swiftly_unix.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 18:07:12.243915 swiftly-unix-0.0.4/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.0.4/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 18:07:12.243797 swiftly-unix-0.0.4/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 18:07:12.242726 swiftly-unix-0.0.4/scripts/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)      134 2023-07-10 17:19:19.000000 swiftly-unix-0.0.4/scripts/swiftly
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-10 18:07:12.243950 swiftly-unix-0.0.4/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      162 2023-07-10 18:07:07.000000 swiftly-unix-0.0.4/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 18:07:12.243096 swiftly-unix-0.0.4/swiftly_unix/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.0.4/swiftly_unix/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      134 2023-07-10 18:04:55.000000 swiftly-unix-0.0.4/swiftly_unix/script.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 18:07:12.243622 swiftly-unix-0.0.4/swiftly_unix.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 18:07:12.000000 swiftly-unix-0.0.4/swiftly_unix.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      224 2023-07-10 18:07:12.000000 swiftly-unix-0.0.4/swiftly_unix.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-10 18:07:12.000000 swiftly-unix-0.0.4/swiftly_unix.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-10 18:07:12.000000 swiftly-unix-0.0.4/swiftly_unix.egg-info/top_level.txt
```

### Comparing `swiftly-unix-0.0.3/LICENSE` & `swiftly-unix-0.0.4/LICENSE`

 * *Files identical despite different names*

