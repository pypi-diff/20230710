# Comparing `tmp/read_tydex_file_pkg-0.0.1.tar.gz` & `tmp/read_tydex_file_pkg-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "read_tydex_file_pkg-0.0.1.tar", last modified: Sun Jul  9 21:42:21 2023, max compression
+gzip compressed data, was "read_tydex_file_pkg-0.0.2.tar", last modified: Sun Jul  9 22:38:44 2023, max compression
```

## Comparing `read_tydex_file_pkg-0.0.1.tar` & `read_tydex_file_pkg-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 21:42:21.528637 read_tydex_file_pkg-0.0.1/
--rw-rw-rw-   0        0        0     1093 2023-07-09 21:17:19.000000 read_tydex_file_pkg-0.0.1/LICENCE.md
--rw-rw-rw-   0        0        0      441 2023-07-09 21:42:21.528637 read_tydex_file_pkg-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        1 2023-07-09 20:46:29.000000 read_tydex_file_pkg-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 21:42:21.509623 read_tydex_file_pkg-0.0.1/my_pkg/
--rw-rw-rw-   0        0        0       41 2023-07-09 20:32:11.000000 read_tydex_file_pkg-0.0.1/my_pkg/__init__.py
--rw-rw-rw-   0        0        0      157 2023-07-09 20:03:28.000000 read_tydex_file_pkg-0.0.1/my_pkg/main_tydex.py
--rw-rw-rw-   0        0        0     4334 2023-07-09 20:03:03.000000 read_tydex_file_pkg-0.0.1/my_pkg/read_tydex.py
-drwxrwxrwx   0        0        0        0 2023-07-09 21:42:21.528637 read_tydex_file_pkg-0.0.1/read_tydex_file_pkg.egg-info/
--rw-rw-rw-   0        0        0      441 2023-07-09 21:42:21.000000 read_tydex_file_pkg-0.0.1/read_tydex_file_pkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-07-09 21:42:21.000000 read_tydex_file_pkg-0.0.1/read_tydex_file_pkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 21:42:21.000000 read_tydex_file_pkg-0.0.1/read_tydex_file_pkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-09 21:42:21.000000 read_tydex_file_pkg-0.0.1/read_tydex_file_pkg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 21:42:21.528637 read_tydex_file_pkg-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      661 2023-07-09 21:26:30.000000 read_tydex_file_pkg-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 22:38:44.411363 read_tydex_file_pkg-0.0.2/
+-rw-rw-rw-   0        0        0     1093 2023-07-09 21:17:19.000000 read_tydex_file_pkg-0.0.2/LICENCE.md
+-rw-rw-rw-   0        0        0      441 2023-07-09 22:38:44.411363 read_tydex_file_pkg-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        1 2023-07-09 20:46:29.000000 read_tydex_file_pkg-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 22:38:44.411363 read_tydex_file_pkg-0.0.2/my_pkg/
+-rw-rw-rw-   0        0        0      203 2023-07-09 22:27:38.000000 read_tydex_file_pkg-0.0.2/my_pkg/__init__.py
+-rw-rw-rw-   0        0        0     4334 2023-07-09 20:03:03.000000 read_tydex_file_pkg-0.0.2/my_pkg/read_tydex.py
+drwxrwxrwx   0        0        0        0 2023-07-09 22:38:44.411363 read_tydex_file_pkg-0.0.2/read_tydex_file_pkg.egg-info/
+-rw-rw-rw-   0        0        0      441 2023-07-09 22:38:44.000000 read_tydex_file_pkg-0.0.2/read_tydex_file_pkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-07-09 22:38:44.000000 read_tydex_file_pkg-0.0.2/read_tydex_file_pkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 22:38:44.000000 read_tydex_file_pkg-0.0.2/read_tydex_file_pkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-09 22:38:44.000000 read_tydex_file_pkg-0.0.2/read_tydex_file_pkg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 22:38:44.411363 read_tydex_file_pkg-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      661 2023-07-09 22:34:29.000000 read_tydex_file_pkg-0.0.2/setup.py
```

### Comparing `read_tydex_file_pkg-0.0.1/LICENCE.md` & `read_tydex_file_pkg-0.0.2/LICENCE.md`

 * *Files identical despite different names*

### Comparing `read_tydex_file_pkg-0.0.1/my_pkg/read_tydex.py` & `read_tydex_file_pkg-0.0.2/my_pkg/read_tydex.py`

 * *Files identical despite different names*

### Comparing `read_tydex_file_pkg-0.0.1/setup.py` & `read_tydex_file_pkg-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="read_tydex_file_pkg",
-    version="0.0.1",
+    version="0.0.2",
     author="Xuyi Shi",
     author_email="usyqu@kit.student.edu",
     description="A package for reading tydex file",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/",
     packages=setuptools.find_packages(),
```

