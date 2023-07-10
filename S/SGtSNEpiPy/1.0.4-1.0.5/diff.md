# Comparing `tmp/SGtSNEpiPy-1.0.4.tar.gz` & `tmp/SGtSNEpiPy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SGtSNEpiPy-1.0.4.tar", last modified: Mon Jul 10 09:54:29 2023, max compression
+gzip compressed data, was "SGtSNEpiPy-1.0.5.tar", last modified: Mon Jul 10 14:55:10 2023, max compression
```

## Comparing `SGtSNEpiPy-1.0.4.tar` & `SGtSNEpiPy-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 09:54:29.049459 SGtSNEpiPy-1.0.4/
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      647 2023-07-10 09:54:29.049275 SGtSNEpiPy-1.0.4/PKG-INFO
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 09:54:29.048084 SGtSNEpiPy-1.0.4/SGtSNEpiPy/
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 02:34:15.000000 SGtSNEpiPy-1.0.4/SGtSNEpiPy/__init__.py
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     1110 2023-07-10 09:47:54.000000 SGtSNEpiPy-1.0.4/SGtSNEpiPy/sgtsnepipy.py
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 09:54:29.049069 SGtSNEpiPy-1.0.4/SGtSNEpiPy.egg-info/
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      647 2023-07-10 09:54:28.000000 SGtSNEpiPy-1.0.4/SGtSNEpiPy.egg-info/PKG-INFO
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      225 2023-07-10 09:54:29.000000 SGtSNEpiPy-1.0.4/SGtSNEpiPy.egg-info/SOURCES.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        1 2023-07-10 09:54:28.000000 SGtSNEpiPy-1.0.4/SGtSNEpiPy.egg-info/dependency_links.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       10 2023-07-10 09:54:28.000000 SGtSNEpiPy-1.0.4/SGtSNEpiPy.egg-info/requires.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       11 2023-07-10 09:54:28.000000 SGtSNEpiPy-1.0.4/SGtSNEpiPy.egg-info/top_level.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       38 2023-07-10 09:54:29.049525 SGtSNEpiPy-1.0.4/setup.cfg
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      830 2023-07-10 09:53:49.000000 SGtSNEpiPy-1.0.4/setup.py
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 14:55:10.786829 SGtSNEpiPy-1.0.5/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      647 2023-07-10 14:55:10.786641 SGtSNEpiPy-1.0.5/PKG-INFO
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 14:55:10.785211 SGtSNEpiPy-1.0.5/SGtSNEpiPy/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     1089 2023-07-10 14:53:11.000000 SGtSNEpiPy-1.0.5/SGtSNEpiPy/SGtSNEpiPy.py
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 02:34:15.000000 SGtSNEpiPy-1.0.5/SGtSNEpiPy/__init__.py
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 14:55:10.786296 SGtSNEpiPy-1.0.5/SGtSNEpiPy.egg-info/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      647 2023-07-10 14:55:10.000000 SGtSNEpiPy-1.0.5/SGtSNEpiPy.egg-info/PKG-INFO
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      225 2023-07-10 14:55:10.000000 SGtSNEpiPy-1.0.5/SGtSNEpiPy.egg-info/SOURCES.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        1 2023-07-10 14:55:10.000000 SGtSNEpiPy-1.0.5/SGtSNEpiPy.egg-info/dependency_links.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       10 2023-07-10 14:55:10.000000 SGtSNEpiPy-1.0.5/SGtSNEpiPy.egg-info/requires.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       11 2023-07-10 14:55:10.000000 SGtSNEpiPy-1.0.5/SGtSNEpiPy.egg-info/top_level.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       38 2023-07-10 14:55:10.786895 SGtSNEpiPy-1.0.5/setup.cfg
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      830 2023-07-10 14:54:41.000000 SGtSNEpiPy-1.0.5/setup.py
```

### Comparing `SGtSNEpiPy-1.0.4/PKG-INFO` & `SGtSNEpiPy-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SGtSNEpiPy
-Version: 1.0.4
+Version: 1.0.5
 Summary: SGtSNEpiPy is a Python interface for the SG-t-SNE-П algorithm, a powerful tool for visualizing large, sparse, stochastic graphs.
 Author: ['Chenshuhao Qin', 'Yihua Zhong']
 Author-email: cq27@duke.edu, yz737@duke.edu,
 
 This is a Python wrapper for SG-t-SNE-П (https://github.com/fcdimitr/SGtSNEpi.jl), implemented using the JuliaCall module (https://cjdoris.github.io/PythonCall.jl/stable/juliacall) from PythonCall & JuliaCall package (https://cjdoris.github.io/PythonCall.jl). If you meet any issue, feel free to contact authors.
 Email:
 chenshuhao.qin@duke.edu
```

### Comparing `SGtSNEpiPy-1.0.4/SGtSNEpiPy/sgtsnepipy.py` & `SGtSNEpiPy-1.0.5/SGtSNEpiPy/SGtSNEpiPy.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from juliacall import Main as jl
 import scipy.sparse as sp
 import numpy as np
 
 # This function uses julia package SGtSNEpi within Python to process a sparse array in python
 # input of the function can be any type of sparse array, namely COO,CSR or CSC
-# If this function does not operate normally, check your python interpreter, make sure you use the one under anaconda file, because that is where the juliacall would be automatically installed
+# If this function does not operate normally, find which path your downloaded juliacall, then use the corresopongding python interepter 
+# We use the Conda package manager
 
 def sgtsnepipy(CSR_matrix):
     jl.seval('using Pkg')
     jl.seval('Pkg.add("SGtSNEpi")')
     jl.seval('Pkg.status()') 
     jl.seval("using SparseArrays")
     jl.seval("using SGtSNEpi")
```

### Comparing `SGtSNEpiPy-1.0.4/SGtSNEpiPy.egg-info/PKG-INFO` & `SGtSNEpiPy-1.0.5/SGtSNEpiPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SGtSNEpiPy
-Version: 1.0.4
+Version: 1.0.5
 Summary: SGtSNEpiPy is a Python interface for the SG-t-SNE-П algorithm, a powerful tool for visualizing large, sparse, stochastic graphs.
 Author: ['Chenshuhao Qin', 'Yihua Zhong']
 Author-email: cq27@duke.edu, yz737@duke.edu,
 
 This is a Python wrapper for SG-t-SNE-П (https://github.com/fcdimitr/SGtSNEpi.jl), implemented using the JuliaCall module (https://cjdoris.github.io/PythonCall.jl/stable/juliacall) from PythonCall & JuliaCall package (https://cjdoris.github.io/PythonCall.jl). If you meet any issue, feel free to contact authors.
 Email:
 chenshuhao.qin@duke.edu
```

### Comparing `SGtSNEpiPy-1.0.4/setup.py` & `SGtSNEpiPy-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 import setuptools
 
 setup(
     name='SGtSNEpiPy',
-    version='1.0.4',
+    version='1.0.5',
     description='SGtSNEpiPy is a Python interface for the SG-t-SNE-П algorithm, a powerful tool for visualizing large, sparse, stochastic graphs.',
     long_description= "This is a Python wrapper for SG-t-SNE-П (https://github.com/fcdimitr/SGtSNEpi.jl), implemented using the JuliaCall module (https://cjdoris.github.io/PythonCall.jl/stable/juliacall) from PythonCall & JuliaCall package (https://cjdoris.github.io/PythonCall.jl). If you meet any issue, feel free to contact authors.\nEmail:\nchenshuhao.qin@duke.edu\nyihua.zhong@duke.edu",
     author=['Chenshuhao Qin','Yihua Zhong'],
     author_email="cq27@duke.edu, yz737@duke.edu,",
     packages=setuptools.find_packages(),
     install_requires=[
         'juliacall',
```

