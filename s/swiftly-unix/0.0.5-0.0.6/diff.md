# Comparing `tmp/swiftly-unix-0.0.5.tar.gz` & `tmp/swiftly-unix-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-unix-0.0.5.tar", last modified: Mon Jul 10 19:17:24 2023, max compression
+gzip compressed data, was "swiftly-unix-0.0.6.tar", last modified: Mon Jul 10 19:27:09 2023, max compression
```

## Comparing `swiftly-unix-0.0.5.tar` & `swiftly-unix-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 19:17:24.147159 swiftly-unix-0.0.5/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.0.5/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 19:17:24.147048 swiftly-unix-0.0.5/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 19:17:24.145404 swiftly-unix-0.0.5/scripts/
--rwxr-xr-x   0 brainspoof   (501) staff       (20)     1887 2023-07-10 19:09:17.000000 swiftly-unix-0.0.5/scripts/swiftly
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-10 19:17:24.147207 swiftly-unix-0.0.5/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      162 2023-07-10 19:16:54.000000 swiftly-unix-0.0.5/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 19:17:24.146355 swiftly-unix-0.0.5/swiftly_unix/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.0.5/swiftly_unix/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      695 2023-07-10 19:14:51.000000 swiftly-unix-0.0.5/swiftly_unix/init.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      291 2023-07-10 19:16:43.000000 swiftly-unix-0.0.5/swiftly_unix/installs.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      128 2023-07-10 19:15:27.000000 swiftly-unix-0.0.5/swiftly_unix/makeapp.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      148 2023-07-10 19:15:55.000000 swiftly-unix-0.0.5/swiftly_unix/run_app.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 19:17:24.146883 swiftly-unix-0.0.5/swiftly_unix.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 19:17:24.000000 swiftly-unix-0.0.5/swiftly_unix.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      295 2023-07-10 19:17:24.000000 swiftly-unix-0.0.5/swiftly_unix.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-10 19:17:24.000000 swiftly-unix-0.0.5/swiftly_unix.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-10 19:17:24.000000 swiftly-unix-0.0.5/swiftly_unix.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 19:27:09.503290 swiftly-unix-0.0.6/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.0.6/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 19:27:09.503139 swiftly-unix-0.0.6/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 19:27:09.501169 swiftly-unix-0.0.6/scripts/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)     1890 2023-07-10 19:25:05.000000 swiftly-unix-0.0.6/scripts/swiftly
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-10 19:27:09.503336 swiftly-unix-0.0.6/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      162 2023-07-10 19:26:59.000000 swiftly-unix-0.0.6/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 19:27:09.502312 swiftly-unix-0.0.6/swiftly_unix/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.0.6/swiftly_unix/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      695 2023-07-10 19:14:51.000000 swiftly-unix-0.0.6/swiftly_unix/init.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      291 2023-07-10 19:16:43.000000 swiftly-unix-0.0.6/swiftly_unix/installs.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      128 2023-07-10 19:15:27.000000 swiftly-unix-0.0.6/swiftly_unix/makeapp.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      148 2023-07-10 19:15:55.000000 swiftly-unix-0.0.6/swiftly_unix/run_app.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 19:27:09.502913 swiftly-unix-0.0.6/swiftly_unix.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 19:27:09.000000 swiftly-unix-0.0.6/swiftly_unix.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      295 2023-07-10 19:27:09.000000 swiftly-unix-0.0.6/swiftly_unix.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-10 19:27:09.000000 swiftly-unix-0.0.6/swiftly_unix.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-10 19:27:09.000000 swiftly-unix-0.0.6/swiftly_unix.egg-info/top_level.txt
```

### Comparing `swiftly-unix-0.0.5/LICENSE` & `swiftly-unix-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.0.5/swiftly_unix/init.py` & `swiftly-unix-0.0.6/swiftly_unix/init.py`

 * *Files identical despite different names*

