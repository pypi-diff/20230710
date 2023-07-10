# Comparing `tmp/starred_repo_finder-0.1.tar.gz` & `tmp/starred_repo_finder-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starred_repo_finder-0.1.tar", last modified: Mon Jul 10 00:30:26 2023, max compression
+gzip compressed data, was "starred_repo_finder-0.2.0.tar", last modified: Mon Jul 10 02:53:47 2023, max compression
```

## Comparing `starred_repo_finder-0.1.tar` & `starred_repo_finder-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-10 00:30:26.924218 starred_repo_finder-0.1/
--rw-r--r--   0 tyler      (501) staff       (20)     2679 2023-07-10 00:30:26.923778 starred_repo_finder-0.1/PKG-INFO
--rw-r--r--   0 tyler      (501) staff       (20)     2139 2023-07-10 00:22:35.000000 starred_repo_finder-0.1/README.md
--rw-r--r--   0 tyler      (501) staff       (20)       38 2023-07-10 00:30:26.924341 starred_repo_finder-0.1/setup.cfg
--rw-r--r--   0 tyler      (501) staff       (20)      934 2023-07-10 00:29:04.000000 starred_repo_finder-0.1/setup.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-10 00:30:26.919898 starred_repo_finder-0.1/starred_repo_finder/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2023-07-10 00:17:27.000000 starred_repo_finder-0.1/starred_repo_finder/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     7775 2023-07-10 00:17:39.000000 starred_repo_finder-0.1/starred_repo_finder/starred_repo_finder.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-10 00:30:26.922582 starred_repo_finder-0.1/starred_repo_finder.egg-info/
--rw-r--r--   0 tyler      (501) staff       (20)     2679 2023-07-10 00:30:26.000000 starred_repo_finder-0.1/starred_repo_finder.egg-info/PKG-INFO
--rw-r--r--   0 tyler      (501) staff       (20)      405 2023-07-10 00:30:26.000000 starred_repo_finder-0.1/starred_repo_finder.egg-info/SOURCES.txt
--rw-r--r--   0 tyler      (501) staff       (20)        1 2023-07-10 00:30:26.000000 starred_repo_finder-0.1/starred_repo_finder.egg-info/dependency_links.txt
--rw-r--r--   0 tyler      (501) staff       (20)       85 2023-07-10 00:30:26.000000 starred_repo_finder-0.1/starred_repo_finder.egg-info/entry_points.txt
--rw-r--r--   0 tyler      (501) staff       (20)       23 2023-07-10 00:30:26.000000 starred_repo_finder-0.1/starred_repo_finder.egg-info/requires.txt
--rw-r--r--   0 tyler      (501) staff       (20)       26 2023-07-10 00:30:26.000000 starred_repo_finder-0.1/starred_repo_finder.egg-info/top_level.txt
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-10 00:30:26.923294 starred_repo_finder-0.1/tests/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2023-07-10 00:17:54.000000 starred_repo_finder-0.1/tests/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     3983 2023-07-10 00:25:17.000000 starred_repo_finder-0.1/tests/test_starred_repo_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:47.938266 starred_repo_finder-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 02:53:36.000000 starred_repo_finder-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-07-10 02:53:47.938266 starred_repo_finder-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-07-10 02:53:36.000000 starred_repo_finder-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 02:53:47.938266 starred_repo_finder-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-10 02:53:36.000000 starred_repo_finder-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:47.938266 starred_repo_finder-0.2.0/starred_repo_finder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:36.000000 starred_repo_finder-0.2.0/starred_repo_finder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-07-10 02:53:36.000000 starred_repo_finder-0.2.0/starred_repo_finder/starred_repo_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:47.938266 starred_repo_finder-0.2.0/starred_repo_finder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-07-10 02:53:47.000000 starred_repo_finder-0.2.0/starred_repo_finder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-10 02:53:47.000000 starred_repo_finder-0.2.0/starred_repo_finder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 02:53:47.000000 starred_repo_finder-0.2.0/starred_repo_finder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 02:53:47.000000 starred_repo_finder-0.2.0/starred_repo_finder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 02:53:47.000000 starred_repo_finder-0.2.0/starred_repo_finder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 02:53:47.000000 starred_repo_finder-0.2.0/starred_repo_finder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:47.938266 starred_repo_finder-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 02:53:36.000000 starred_repo_finder-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-10 02:53:36.000000 starred_repo_finder-0.2.0/tests/test_starred_repo_finder.py
```

### Comparing `starred_repo_finder-0.1/setup.py` & `starred_repo_finder-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="starred_repo_finder",
-    version="0.1",
+    version="0.2.0",
     description="A simple command line tool to find and explore GitHub repositories through stargazers for a given repository.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tylercb/starred_repo_finder",
     author="Tyler Hanway",
     author_email="hanway.tyler@gmail.com",
     license="MIT",
```

### Comparing `starred_repo_finder-0.1/starred_repo_finder/starred_repo_finder.py` & `starred_repo_finder-0.2.0/starred_repo_finder/starred_repo_finder.py`

 * *Files identical despite different names*

### Comparing `starred_repo_finder-0.1/tests/test_starred_repo_finder.py` & `starred_repo_finder-0.2.0/tests/test_starred_repo_finder.py`

 * *Files identical despite different names*

