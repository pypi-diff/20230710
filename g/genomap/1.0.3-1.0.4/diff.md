# Comparing `tmp/genomap-1.0.3.tar.gz` & `tmp/genomap-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomap-1.0.3.tar", last modified: Mon Jul 10 17:40:39 2023, max compression
+gzip compressed data, was "genomap-1.0.4.tar", last modified: Mon Jul 10 18:27:47 2023, max compression
```

## Comparing `genomap-1.0.3.tar` & `genomap-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:40:39.066959 genomap-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-10 17:37:26.000000 genomap-1.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-10 17:37:26.000000 genomap-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-10 17:40:39.066959 genomap-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-10 17:37:26.000000 genomap-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:40:39.062959 genomap-1.0.3/data/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-10 17:37:26.000000 genomap-1.0.3/data/TM_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:40:39.062959 genomap-1.0.3/genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 17:37:26.000000 genomap-1.0.3/genomap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:40:39.062959 genomap-1.0.3/genomap/bregman_genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 17:37:26.000000 genomap-1.0.3/genomap/bregman_genomap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-10 17:37:26.000000 genomap-1.0.3/genomap/bregman_genomap/bregman_genomap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-10 17:37:26.000000 genomap-1.0.3/genomap/genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:40:39.066959 genomap-1.0.3/genomap/genomapOPT/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 17:37:26.000000 genomap-1.0.3/genomap/genomapOPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-10 17:37:26.000000 genomap-1.0.3/genomap/genomapOPT/genomapOPT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:40:39.062959 genomap-1.0.3/genomap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-10 17:40:38.000000 genomap-1.0.3/genomap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-10 17:40:39.000000 genomap-1.0.3/genomap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 17:40:38.000000 genomap-1.0.3/genomap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-10 17:40:38.000000 genomap-1.0.3/genomap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 17:40:38.000000 genomap-1.0.3/genomap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 17:37:26.000000 genomap-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 17:40:39.066959 genomap-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-10 17:37:26.000000 genomap-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:27:47.092911 genomap-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-10 18:27:06.000000 genomap-1.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-10 18:27:06.000000 genomap-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-10 18:27:47.092911 genomap-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-10 18:27:06.000000 genomap-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:27:47.088911 genomap-1.0.4/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-10 18:27:06.000000 genomap-1.0.4/data/TM_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:27:47.088911 genomap-1.0.4/genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 18:27:06.000000 genomap-1.0.4/genomap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:27:47.092911 genomap-1.0.4/genomap/bregman_genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 18:27:06.000000 genomap-1.0.4/genomap/bregman_genomap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-10 18:27:06.000000 genomap-1.0.4/genomap/bregman_genomap/bregman_genomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-10 18:27:06.000000 genomap-1.0.4/genomap/genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:27:47.092911 genomap-1.0.4/genomap/genomapOPT/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 18:27:06.000000 genomap-1.0.4/genomap/genomapOPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-10 18:27:06.000000 genomap-1.0.4/genomap/genomapOPT/genomapOPT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:27:47.088911 genomap-1.0.4/genomap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-10 18:27:47.000000 genomap-1.0.4/genomap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-10 18:27:47.000000 genomap-1.0.4/genomap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:27:47.000000 genomap-1.0.4/genomap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 18:27:47.000000 genomap-1.0.4/genomap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 18:27:47.000000 genomap-1.0.4/genomap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 18:27:06.000000 genomap-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:27:47.092911 genomap-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-10 18:27:06.000000 genomap-1.0.4/setup.py
```

### Comparing `genomap-1.0.3/LICENSE.txt` & `genomap-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.0.3/PKG-INFO` & `genomap-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.0.3
+Version: 1.0.4
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `genomap-1.0.3/README.md` & `genomap-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `genomap-1.0.3/genomap/bregman_genomap/bregman_genomap.py` & `genomap-1.0.4/genomap/bregman_genomap/bregman_genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.3/genomap/genomap.py` & `genomap-1.0.4/genomap/genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.3/genomap/genomapOPT/genomapOPT.py` & `genomap-1.0.4/genomap/genomapOPT/genomapOPT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.3/genomap.egg-info/PKG-INFO` & `genomap-1.0.4/genomap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.0.3
+Version: 1.0.4
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `genomap-1.0.3/setup.py` & `genomap-1.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="genomap",
-    version="1.0.3",
+    version="1.0.4",
     author="Md Tauhidul Islam",
     author_email="tauhid@stanford.edu",
     description="Genomap converts tabular gene expression data into spatially meaningful images.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinglab-ai/genomap",
     classifiers=[
```

