# Comparing `tmp/dccsx-0.0.1.tar.gz` & `tmp/dccsx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dccsx-0.0.1.tar", last modified: Mon Jul 10 13:05:01 2023, max compression
+gzip compressed data, was "dccsx-0.0.2.tar", last modified: Mon Jul 10 19:39:01 2023, max compression
```

## Comparing `dccsx-0.0.1.tar` & `dccsx-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-10 13:05:01.071562 dccsx-0.0.1/
--rw-rw----   0 root         (0) everybody  (9997)     1036 2023-07-10 12:00:56.000000 dccsx-0.0.1/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)     3156 2023-07-10 13:05:01.071562 dccsx-0.0.1/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     2446 2023-07-10 12:55:38.000000 dccsx-0.0.1/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-10 13:05:01.063562 dccsx-0.0.1/dccsx/
--rw-rw----   0 root         (0) everybody  (9997)       83 2023-07-07 06:35:56.000000 dccsx-0.0.1/dccsx/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    31342 2023-07-10 12:02:39.000000 dccsx-0.0.1/dccsx/lan_change.py
--rw-rw----   0 root         (0) everybody  (9997)    27126 2023-07-10 12:02:50.000000 dccsx-0.0.1/dccsx/logo.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-10 13:05:01.071562 dccsx-0.0.1/dccsx.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     3156 2023-07-10 13:05:00.000000 dccsx-0.0.1/dccsx.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      292 2023-07-10 13:05:01.000000 dccsx-0.0.1/dccsx.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-10 13:05:00.000000 dccsx-0.0.1/dccsx.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       46 2023-07-10 13:05:01.000000 dccsx-0.0.1/dccsx.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-10 12:56:23.000000 dccsx-0.0.1/dccsx.egg-info/not-zip-safe
--rw-rw----   0 root         (0) everybody  (9997)       13 2023-07-10 13:05:01.000000 dccsx-0.0.1/dccsx.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        6 2023-07-10 13:05:01.000000 dccsx-0.0.1/dccsx.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)      650 2023-07-10 13:05:01.075562 dccsx-0.0.1/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1046 2023-07-10 11:57:16.000000 dccsx-0.0.1/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-10 19:39:01.100000 dccsx-0.0.2/
+-rw-rw----   0 root         (0) everybody  (9997)     1036 2023-07-10 12:00:56.000000 dccsx-0.0.2/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)     5462 2023-07-10 19:39:01.100000 dccsx-0.0.2/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     4752 2023-07-10 19:10:37.000000 dccsx-0.0.2/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-10 19:39:01.096000 dccsx-0.0.2/dccsx/
+-rw-rw----   0 root         (0) everybody  (9997)      111 2023-07-10 19:29:46.000000 dccsx-0.0.2/dccsx/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    40419 2023-07-10 19:32:11.000000 dccsx-0.0.2/dccsx/dccsfb.py
+-rw-rw----   0 root         (0) everybody  (9997)    31342 2023-07-10 12:02:39.000000 dccsx-0.0.2/dccsx/lan_change.py
+-rw-rw----   0 root         (0) everybody  (9997)    27126 2023-07-10 12:02:50.000000 dccsx-0.0.2/dccsx/logo.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-10 19:39:01.100000 dccsx-0.0.2/dccsx.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     5462 2023-07-10 19:39:01.000000 dccsx-0.0.2/dccsx.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      308 2023-07-10 19:39:01.000000 dccsx-0.0.2/dccsx.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-10 19:39:01.000000 dccsx-0.0.2/dccsx.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       46 2023-07-10 19:39:01.000000 dccsx-0.0.2/dccsx.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-10 19:35:05.000000 dccsx-0.0.2/dccsx.egg-info/not-zip-safe
+-rw-rw----   0 root         (0) everybody  (9997)       13 2023-07-10 19:39:01.000000 dccsx-0.0.2/dccsx.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        6 2023-07-10 19:39:01.000000 dccsx-0.0.2/dccsx.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)      650 2023-07-10 19:39:01.104000 dccsx-0.0.2/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1046 2023-07-10 19:34:26.000000 dccsx-0.0.2/setup.py
```

### Comparing `dccsx-0.0.1/LICENSE` & `dccsx-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dccsx-0.0.1/dccsx/lan_change.py` & `dccsx-0.0.2/dccsx/lan_change.py`

 * *Files identical despite different names*

### Comparing `dccsx-0.0.1/dccsx/logo.py` & `dccsx-0.0.2/dccsx/logo.py`

 * *Files identical despite different names*

### Comparing `dccsx-0.0.1/setup.cfg` & `dccsx-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `dccsx-0.0.1/setup.py` & `dccsx-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="dccsx",
-    version="0.0.1",
+    version="0.0.2",
     author="Md Saimun",
     author_email="teamdccs@gmail.com",
     description="this module team dccs personal module for using shortcut python code",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Dccs-team/dccsx",
     packages=["dccsx"],
```

