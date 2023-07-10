# Comparing `tmp/swiftly-unix-0.0.1.tar.gz` & `tmp/swiftly-unix-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-unix-0.0.1.tar", last modified: Mon Jul 10 17:12:58 2023, max compression
+gzip compressed data, was "swiftly-unix-0.0.2.tar", last modified: Mon Jul 10 17:19:54 2023, max compression
```

## Comparing `swiftly-unix-0.0.1.tar` & `swiftly-unix-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:12:58.847342 swiftly-unix-0.0.1/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.0.1/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 17:12:58.847234 swiftly-unix-0.0.1/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:12:58.846529 swiftly-unix-0.0.1/scripts/
--rwxr-xr-x   0 brainspoof   (501) staff       (20)      121 2023-07-10 17:08:23.000000 swiftly-unix-0.0.1/scripts/swiftly
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-10 17:12:58.847381 swiftly-unix-0.0.1/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      162 2023-07-10 17:12:55.000000 swiftly-unix-0.0.1/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:12:58.847063 swiftly-unix-0.0.1/swiftly_unix.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 17:12:58.000000 swiftly-unix-0.0.1/swiftly_unix.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      176 2023-07-10 17:12:58.000000 swiftly-unix-0.0.1/swiftly_unix.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-10 17:12:58.000000 swiftly-unix-0.0.1/swiftly_unix.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-10 17:12:58.000000 swiftly-unix-0.0.1/swiftly_unix.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:19:54.122316 swiftly-unix-0.0.2/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.0.2/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 17:19:54.122206 swiftly-unix-0.0.2/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:19:54.121524 swiftly-unix-0.0.2/scripts/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)      134 2023-07-10 17:19:19.000000 swiftly-unix-0.0.2/scripts/swiftly
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-10 17:19:54.122351 swiftly-unix-0.0.2/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      162 2023-07-10 17:17:58.000000 swiftly-unix-0.0.2/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:19:54.122046 swiftly-unix-0.0.2/swiftly_unix.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 17:19:54.000000 swiftly-unix-0.0.2/swiftly_unix.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      176 2023-07-10 17:19:54.000000 swiftly-unix-0.0.2/swiftly_unix.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-10 17:19:54.000000 swiftly-unix-0.0.2/swiftly_unix.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-10 17:19:54.000000 swiftly-unix-0.0.2/swiftly_unix.egg-info/top_level.txt
```

### Comparing `swiftly-unix-0.0.1/LICENSE` & `swiftly-unix-0.0.2/LICENSE`

 * *Files identical despite different names*

