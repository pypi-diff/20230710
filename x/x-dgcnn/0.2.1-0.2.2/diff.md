# Comparing `tmp/x-dgcnn-0.2.1.tar.gz` & `tmp/x-dgcnn-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x-dgcnn-0.2.1.tar", last modified: Sun Jul  9 18:48:27 2023, max compression
+gzip compressed data, was "x-dgcnn-0.2.2.tar", last modified: Mon Jul 10 04:31:32 2023, max compression
```

## Comparing `x-dgcnn-0.2.1.tar` & `x-dgcnn-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:48:27.875172 x-dgcnn-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-09 18:48:17.000000 x-dgcnn-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-09 18:48:27.875172 x-dgcnn-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-09 18:48:17.000000 x-dgcnn-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 18:48:27.875172 x-dgcnn-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-09 18:48:17.000000 x-dgcnn-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:48:27.875172 x-dgcnn-0.2.1/x_dgcnn/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-09 18:48:17.000000 x-dgcnn-0.2.1/x_dgcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-07-09 18:48:17.000000 x-dgcnn-0.2.1/x_dgcnn/dgcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-09 18:48:17.000000 x-dgcnn-0.2.1/x_dgcnn/route.py
--rw-r--r--   0 runner    (1001) docker     (123)    10048 2023-07-09 18:48:17.000000 x-dgcnn-0.2.1/x_dgcnn/x_dgcnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:48:27.875172 x-dgcnn-0.2.1/x_dgcnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-09 18:48:27.000000 x-dgcnn-0.2.1/x_dgcnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-09 18:48:27.000000 x-dgcnn-0.2.1/x_dgcnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 18:48:27.000000 x-dgcnn-0.2.1/x_dgcnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-09 18:48:27.000000 x-dgcnn-0.2.1/x_dgcnn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 18:48:27.000000 x-dgcnn-0.2.1/x_dgcnn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:31:32.054778 x-dgcnn-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-10 04:31:20.000000 x-dgcnn-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-10 04:31:32.054778 x-dgcnn-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-10 04:31:20.000000 x-dgcnn-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 04:31:32.054778 x-dgcnn-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-10 04:31:20.000000 x-dgcnn-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:31:32.054778 x-dgcnn-0.2.2/x_dgcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-10 04:31:20.000000 x-dgcnn-0.2.2/x_dgcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-07-10 04:31:20.000000 x-dgcnn-0.2.2/x_dgcnn/dgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-10 04:31:20.000000 x-dgcnn-0.2.2/x_dgcnn/route.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:31:32.054778 x-dgcnn-0.2.2/x_dgcnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-10 04:31:32.000000 x-dgcnn-0.2.2/x_dgcnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-10 04:31:32.000000 x-dgcnn-0.2.2/x_dgcnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 04:31:32.000000 x-dgcnn-0.2.2/x_dgcnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 04:31:32.000000 x-dgcnn-0.2.2/x_dgcnn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 04:31:32.000000 x-dgcnn-0.2.2/x_dgcnn.egg-info/top_level.txt
```

### Comparing `x-dgcnn-0.2.1/LICENSE` & `x-dgcnn-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `x-dgcnn-0.2.1/PKG-INFO` & `x-dgcnn-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-dgcnn
-Version: 0.2.1
+Version: 0.2.2
 Summary: X-DGCNN - Pytorch
 Home-page: https://github.com/kentechx/x-dgcnn
 Author: Kaidi Shen
 License: MIT
 Keywords: 3D segmentation,3D classification,point cloud understanding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `x-dgcnn-0.2.1/README.md` & `x-dgcnn-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `x-dgcnn-0.2.1/setup.py` & `x-dgcnn-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='x-dgcnn',
     packages=find_packages(),
-    version='0.2.1',
+    version='0.2.2',
     license='MIT',
     description='X-DGCNN - Pytorch',
     author='Kaidi Shen',
     url='https://github.com/kentechx/x-dgcnn',
     long_description_content_type='text/markdown',
     keywords=[
         '3D segmentation',
```

### Comparing `x-dgcnn-0.2.1/x_dgcnn/dgcnn.py` & `x-dgcnn-0.2.2/x_dgcnn/dgcnn.py`

 * *Files identical despite different names*

### Comparing `x-dgcnn-0.2.1/x_dgcnn/route.py` & `x-dgcnn-0.2.2/x_dgcnn/route.py`

 * *Files identical despite different names*

### Comparing `x-dgcnn-0.2.1/x_dgcnn.egg-info/PKG-INFO` & `x-dgcnn-0.2.2/x_dgcnn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-dgcnn
-Version: 0.2.1
+Version: 0.2.2
 Summary: X-DGCNN - Pytorch
 Home-page: https://github.com/kentechx/x-dgcnn
 Author: Kaidi Shen
 License: MIT
 Keywords: 3D segmentation,3D classification,point cloud understanding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

