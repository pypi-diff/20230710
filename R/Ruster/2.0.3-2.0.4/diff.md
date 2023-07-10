# Comparing `tmp/Ruster-2.0.3.tar.gz` & `tmp/Ruster-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ruster-2.0.3.tar", last modified: Mon Jul 10 20:59:44 2023, max compression
+gzip compressed data, was "Ruster-2.0.4.tar", last modified: Mon Jul 10 21:02:29 2023, max compression
```

## Comparing `Ruster-2.0.3.tar` & `Ruster-2.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 20:59:44.991968 Ruster-2.0.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-07-10 20:59:44.991968 Ruster-2.0.3/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 20:59:44.987969 Ruster-2.0.3/Ruster.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-07-10 20:59:44.000000 Ruster-2.0.3/Ruster.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      383 2023-07-10 20:59:44.000000 Ruster-2.0.3/Ruster.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-10 20:59:44.000000 Ruster-2.0.3/Ruster.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       39 2023-07-10 20:59:44.000000 Ruster-2.0.3/Ruster.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       71 2023-07-10 20:59:44.000000 Ruster-2.0.3/Ruster.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-07-10 20:59:44.000000 Ruster-2.0.3/Ruster.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 20:59:44.991968 Ruster-2.0.3/ruster/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-07 17:26:00.000000 Ruster-2.0.3/ruster/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13383 2023-07-10 20:43:07.000000 Ruster-2.0.3/ruster/app.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1345 2023-07-06 08:52:08.000000 Ruster-2.0.3/ruster/blueprints.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      182 2023-07-04 18:04:16.000000 Ruster-2.0.3/ruster/exceptions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3761 2023-07-06 17:39:42.000000 Ruster-2.0.3/ruster/hasher.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7955 2023-07-06 17:40:00.000000 Ruster-2.0.3/ruster/jwt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2664 2023-07-06 08:37:16.000000 Ruster-2.0.3/ruster/limiter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2923 2023-07-06 17:39:06.000000 Ruster-2.0.3/ruster/mailer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1089 2023-07-08 20:35:21.000000 Ruster-2.0.3/ruster/sanitizer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1453 2023-07-05 18:45:58.000000 Ruster-2.0.3/ruster/session.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2679 2023-07-06 17:40:22.000000 Ruster-2.0.3/ruster/wtf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-10 20:59:44.991968 Ruster-2.0.3/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      788 2023-07-10 20:58:59.000000 Ruster-2.0.3/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:02:29.526190 Ruster-2.0.4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-07-10 21:02:29.526190 Ruster-2.0.4/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:02:29.522188 Ruster-2.0.4/Ruster/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-07 17:26:00.000000 Ruster-2.0.4/Ruster/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13383 2023-07-10 20:43:07.000000 Ruster-2.0.4/Ruster/app.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1345 2023-07-06 08:52:08.000000 Ruster-2.0.4/Ruster/blueprints.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      182 2023-07-04 18:04:16.000000 Ruster-2.0.4/Ruster/exceptions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3761 2023-07-06 17:39:42.000000 Ruster-2.0.4/Ruster/hasher.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7955 2023-07-06 17:40:00.000000 Ruster-2.0.4/Ruster/jwt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2664 2023-07-06 08:37:16.000000 Ruster-2.0.4/Ruster/limiter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2923 2023-07-06 17:39:06.000000 Ruster-2.0.4/Ruster/mailer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1089 2023-07-08 20:35:21.000000 Ruster-2.0.4/Ruster/sanitizer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1453 2023-07-05 18:45:58.000000 Ruster-2.0.4/Ruster/session.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2679 2023-07-06 17:40:22.000000 Ruster-2.0.4/Ruster/wtf.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 21:02:29.526190 Ruster-2.0.4/Ruster.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-07-10 21:02:29.000000 Ruster-2.0.4/Ruster.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      383 2023-07-10 21:02:29.000000 Ruster-2.0.4/Ruster.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-10 21:02:29.000000 Ruster-2.0.4/Ruster.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       39 2023-07-10 21:02:29.000000 Ruster-2.0.4/Ruster.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       71 2023-07-10 21:02:29.000000 Ruster-2.0.4/Ruster.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-07-10 21:02:29.000000 Ruster-2.0.4/Ruster.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-10 21:02:29.526190 Ruster-2.0.4/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      788 2023-07-10 21:02:25.000000 Ruster-2.0.4/setup.py
```

### Comparing `Ruster-2.0.3/ruster/app.py` & `Ruster-2.0.4/Ruster/app.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.3/ruster/blueprints.py` & `Ruster-2.0.4/Ruster/blueprints.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.3/ruster/hasher.py` & `Ruster-2.0.4/Ruster/hasher.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.3/ruster/jwt.py` & `Ruster-2.0.4/Ruster/jwt.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.3/ruster/limiter.py` & `Ruster-2.0.4/Ruster/limiter.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.3/ruster/mailer.py` & `Ruster-2.0.4/Ruster/mailer.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.3/ruster/sanitizer.py` & `Ruster-2.0.4/Ruster/sanitizer.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.3/ruster/session.py` & `Ruster-2.0.4/Ruster/session.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.3/ruster/wtf.py` & `Ruster-2.0.4/Ruster/wtf.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.3/setup.py` & `Ruster-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Ruster',
-    version='2.0.3',
+    version='2.0.4',
     author='Pawan Kumar',
     author_email='control@vvfin.in',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
@@ -22,11 +22,11 @@
         "pyjwt",
         "jinja2",
         "itsdangerous",
         "nexusdb"
     ],
     entry_points={
         'console_scripts': [
-            'ruster = ruster.app',
+            'ruster = Ruster.app',
         ],
     },
 )
```

