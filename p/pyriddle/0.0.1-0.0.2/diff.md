# Comparing `tmp/pyriddle-0.0.1.tar.gz` & `tmp/pyriddle-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriddle-0.0.1.tar", last modified: Mon Jul 10 21:31:54 2023, max compression
+gzip compressed data, was "pyriddle-0.0.2.tar", last modified: Mon Jul 10 21:54:48 2023, max compression
```

## Comparing `pyriddle-0.0.1.tar` & `pyriddle-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 clementp  (1000) clementp  (1000)        0 2023-07-10 21:31:54.106484 pyriddle-0.0.1/
--rw-rw-r--   0 clementp  (1000) clementp  (1000)      731 2023-07-10 21:31:54.106484 pyriddle-0.0.1/PKG-INFO
--rw-rw-r--   0 clementp  (1000) clementp  (1000)      159 2023-07-10 21:05:26.000000 pyriddle-0.0.1/README.md
-drwxrwxr-x   0 clementp  (1000) clementp  (1000)        0 2023-07-10 21:31:54.106484 pyriddle-0.0.1/pyriddle/
--rw-rw-r--   0 clementp  (1000) clementp  (1000)        1 2023-07-10 21:05:55.000000 pyriddle-0.0.1/pyriddle/__init__.py
-drwxrwxr-x   0 clementp  (1000) clementp  (1000)        0 2023-07-10 21:31:54.106484 pyriddle-0.0.1/pyriddle.egg-info/
--rw-rw-r--   0 clementp  (1000) clementp  (1000)      731 2023-07-10 21:31:54.000000 pyriddle-0.0.1/pyriddle.egg-info/PKG-INFO
--rw-rw-r--   0 clementp  (1000) clementp  (1000)      198 2023-07-10 21:31:54.000000 pyriddle-0.0.1/pyriddle.egg-info/SOURCES.txt
--rw-rw-r--   0 clementp  (1000) clementp  (1000)        1 2023-07-10 21:31:54.000000 pyriddle-0.0.1/pyriddle.egg-info/dependency_links.txt
--rw-rw-r--   0 clementp  (1000) clementp  (1000)        6 2023-07-10 21:31:54.000000 pyriddle-0.0.1/pyriddle.egg-info/requires.txt
--rw-rw-r--   0 clementp  (1000) clementp  (1000)        9 2023-07-10 21:31:54.000000 pyriddle-0.0.1/pyriddle.egg-info/top_level.txt
--rw-rw-r--   0 clementp  (1000) clementp  (1000)       38 2023-07-10 21:31:54.106484 pyriddle-0.0.1/setup.cfg
--rw-rw-r--   0 clementp  (1000) clementp  (1000)     1133 2023-07-10 21:31:48.000000 pyriddle-0.0.1/setup.py
+drwxrwxr-x   0 clementp  (1000) clementp  (1000)        0 2023-07-10 21:54:48.401336 pyriddle-0.0.2/
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)     1554 2023-07-10 21:54:48.401336 pyriddle-0.0.2/PKG-INFO
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)      982 2023-07-10 21:52:04.000000 pyriddle-0.0.2/README.md
+drwxrwxr-x   0 clementp  (1000) clementp  (1000)        0 2023-07-10 21:54:48.401336 pyriddle-0.0.2/pyriddle/
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)        1 2023-07-10 21:05:55.000000 pyriddle-0.0.2/pyriddle/__init__.py
+drwxrwxr-x   0 clementp  (1000) clementp  (1000)        0 2023-07-10 21:54:48.401336 pyriddle-0.0.2/pyriddle.egg-info/
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)     1554 2023-07-10 21:54:48.000000 pyriddle-0.0.2/pyriddle.egg-info/PKG-INFO
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)      198 2023-07-10 21:54:48.000000 pyriddle-0.0.2/pyriddle.egg-info/SOURCES.txt
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)        1 2023-07-10 21:54:48.000000 pyriddle-0.0.2/pyriddle.egg-info/dependency_links.txt
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)        6 2023-07-10 21:54:48.000000 pyriddle-0.0.2/pyriddle.egg-info/requires.txt
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)        9 2023-07-10 21:54:48.000000 pyriddle-0.0.2/pyriddle.egg-info/top_level.txt
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)       38 2023-07-10 21:54:48.401336 pyriddle-0.0.2/setup.cfg
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)     1133 2023-07-10 21:53:19.000000 pyriddle-0.0.2/setup.py
```

### Comparing `pyriddle-0.0.1/setup.py` & `pyriddle-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION                     = "0.0.1"
+VERSION                     = "0.0.2"
 DESCRIPTION                 = "Browser based fully customisable User Interface"
 LONG_DESCRIPTION            = "pyriddle gives you a simple and powerfull way to display graphics, text infos, video stream and so on, only using your browser as support."
 if os.path.isfile("./README.md"):
     with open("./README.md", 'r') as f:
         LONG_DESCRIPTION    = f.read()
 
 # Setting up
```

