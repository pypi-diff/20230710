# Comparing `tmp/python-swiftly-0.0.0.tar.gz` & `tmp/python-swiftly-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-swiftly-0.0.0.tar", last modified: Mon Jul 10 12:39:07 2023, max compression
+gzip compressed data, was "python-swiftly-0.1.0.tar", last modified: Mon Jul 10 12:38:17 2023, max compression
```

## Comparing `python-swiftly-0.0.0.tar` & `python-swiftly-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 12:39:07.159609 python-swiftly-0.0.0/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-09 21:05:09.000000 python-swiftly-0.0.0/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       80 2023-07-10 12:39:07.159485 python-swiftly-0.0.0/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 12:39:07.158925 python-swiftly-0.0.0/python_swiftly.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       80 2023-07-10 12:39:07.000000 python-swiftly-0.0.0/python_swiftly.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      220 2023-07-10 12:39:07.000000 python-swiftly-0.0.0/python_swiftly.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-10 12:39:07.000000 python-swiftly-0.0.0/python_swiftly.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        8 2023-07-10 12:39:07.000000 python-swiftly-0.0.0/python_swiftly.egg-info/top_level.txt
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 12:39:07.159037 python-swiftly-0.0.0/scripts/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1569 2023-07-10 12:19:16.000000 python-swiftly-0.0.0/scripts/swiftly
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-10 12:39:07.159644 python-swiftly-0.0.0/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      164 2023-07-10 12:38:59.000000 python-swiftly-0.0.0/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 12:39:07.159350 python-swiftly-0.0.0/swiftly/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 11:28:08.000000 python-swiftly-0.0.0/swiftly/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 11:28:13.000000 python-swiftly-0.0.0/swiftly/main.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 12:38:17.713998 python-swiftly-0.1.0/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-09 21:05:09.000000 python-swiftly-0.1.0/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       80 2023-07-10 12:38:17.713858 python-swiftly-0.1.0/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 12:38:17.713160 python-swiftly-0.1.0/python_swiftly.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       80 2023-07-10 12:38:17.000000 python-swiftly-0.1.0/python_swiftly.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      220 2023-07-10 12:38:17.000000 python-swiftly-0.1.0/python_swiftly.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-10 12:38:17.000000 python-swiftly-0.1.0/python_swiftly.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        8 2023-07-10 12:38:17.000000 python-swiftly-0.1.0/python_swiftly.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 12:38:17.713273 python-swiftly-0.1.0/scripts/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1569 2023-07-10 12:19:16.000000 python-swiftly-0.1.0/scripts/swiftly
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-10 12:38:17.715662 python-swiftly-0.1.0/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      164 2023-07-10 11:27:49.000000 python-swiftly-0.1.0/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 12:38:17.713705 python-swiftly-0.1.0/swiftly/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 11:28:08.000000 python-swiftly-0.1.0/swiftly/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 11:28:13.000000 python-swiftly-0.1.0/swiftly/main.py
```

### Comparing `python-swiftly-0.0.0/LICENSE` & `python-swiftly-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-swiftly-0.0.0/scripts/swiftly` & `python-swiftly-0.1.0/scripts/swiftly`

 * *Files identical despite different names*

