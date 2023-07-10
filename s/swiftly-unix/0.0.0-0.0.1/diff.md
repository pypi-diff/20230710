# Comparing `tmp/swiftly-unix-0.0.0.tar.gz` & `tmp/swiftly-unix-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-unix-0.0.0.tar", last modified: Mon Jul 10 17:05:28 2023, max compression
+gzip compressed data, was "swiftly-unix-0.0.1.tar", last modified: Mon Jul 10 17:12:58 2023, max compression
```

## Comparing `swiftly-unix-0.0.0.tar` & `swiftly-unix-0.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:05:28.648775 swiftly-unix-0.0.0/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.0.0/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 17:05:28.648663 swiftly-unix-0.0.0/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:05:28.647987 swiftly-unix-0.0.0/scripts/
--rw-r--r--   0 brainspoof   (501) staff       (20)      121 2023-07-10 17:03:22.000000 swiftly-unix-0.0.0/scripts/swiftly
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-10 17:05:28.648815 swiftly-unix-0.0.0/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      162 2023-07-10 15:03:42.000000 swiftly-unix-0.0.0/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:05:28.648512 swiftly-unix-0.0.0/swiftly_unix.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 17:05:28.000000 swiftly-unix-0.0.0/swiftly_unix.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      176 2023-07-10 17:05:28.000000 swiftly-unix-0.0.0/swiftly_unix.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-10 17:05:28.000000 swiftly-unix-0.0.0/swiftly_unix.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-10 17:05:28.000000 swiftly-unix-0.0.0/swiftly_unix.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:12:58.847342 swiftly-unix-0.0.1/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.0.1/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 17:12:58.847234 swiftly-unix-0.0.1/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:12:58.846529 swiftly-unix-0.0.1/scripts/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)      121 2023-07-10 17:08:23.000000 swiftly-unix-0.0.1/scripts/swiftly
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-10 17:12:58.847381 swiftly-unix-0.0.1/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      162 2023-07-10 17:12:55.000000 swiftly-unix-0.0.1/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:12:58.847063 swiftly-unix-0.0.1/swiftly_unix.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 17:12:58.000000 swiftly-unix-0.0.1/swiftly_unix.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      176 2023-07-10 17:12:58.000000 swiftly-unix-0.0.1/swiftly_unix.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-10 17:12:58.000000 swiftly-unix-0.0.1/swiftly_unix.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-10 17:12:58.000000 swiftly-unix-0.0.1/swiftly_unix.egg-info/top_level.txt
```

### Comparing `swiftly-unix-0.0.0/LICENSE` & `swiftly-unix-0.0.1/LICENSE`

 * *Files identical despite different names*

