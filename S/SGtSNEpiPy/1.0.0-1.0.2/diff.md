# Comparing `tmp/SGtSNEpiPy-1.0.0.tar.gz` & `tmp/SGtSNEpiPy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SGtSNEpiPy-1.0.0.tar", last modified: Mon Jul 10 04:42:36 2023, max compression
+gzip compressed data, was "SGtSNEpiPy-1.0.2.tar", last modified: Mon Jul 10 09:01:22 2023, max compression
```

## Comparing `SGtSNEpiPy-1.0.0.tar` & `SGtSNEpiPy-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 aaronzhong   (501) staff       (20)        0 2023-07-10 04:42:36.031532 SGtSNEpiPy-1.0.0/
--rw-r--r--   0 aaronzhong   (501) staff       (20)      278 2023-07-10 04:42:36.031292 SGtSNEpiPy-1.0.0/PKG-INFO
-drwxr-xr-x   0 aaronzhong   (501) staff       (20)        0 2023-07-10 04:42:36.030126 SGtSNEpiPy-1.0.0/SGtSNEpiPy/
--rw-r--r--   0 aaronzhong   (501) staff       (20)        0 2023-07-10 02:34:15.000000 SGtSNEpiPy-1.0.0/SGtSNEpiPy/__init__.py
--rw-r--r--   0 aaronzhong   (501) staff       (20)     1133 2023-07-10 02:51:33.000000 SGtSNEpiPy-1.0.0/SGtSNEpiPy/pytojuliafunc.py
-drwxr-xr-x   0 aaronzhong   (501) staff       (20)        0 2023-07-10 04:42:36.031059 SGtSNEpiPy-1.0.0/SGtSNEpiPy.egg-info/
--rw-r--r--   0 aaronzhong   (501) staff       (20)      278 2023-07-10 04:42:35.000000 SGtSNEpiPy-1.0.0/SGtSNEpiPy.egg-info/PKG-INFO
--rw-r--r--   0 aaronzhong   (501) staff       (20)      228 2023-07-10 04:42:35.000000 SGtSNEpiPy-1.0.0/SGtSNEpiPy.egg-info/SOURCES.txt
--rw-r--r--   0 aaronzhong   (501) staff       (20)        1 2023-07-10 04:42:35.000000 SGtSNEpiPy-1.0.0/SGtSNEpiPy.egg-info/dependency_links.txt
--rw-r--r--   0 aaronzhong   (501) staff       (20)       10 2023-07-10 04:42:35.000000 SGtSNEpiPy-1.0.0/SGtSNEpiPy.egg-info/requires.txt
--rw-r--r--   0 aaronzhong   (501) staff       (20)       11 2023-07-10 04:42:35.000000 SGtSNEpiPy-1.0.0/SGtSNEpiPy.egg-info/top_level.txt
--rw-r--r--   0 aaronzhong   (501) staff       (20)       38 2023-07-10 04:42:36.031603 SGtSNEpiPy-1.0.0/setup.cfg
--rw-r--r--   0 aaronzhong   (501) staff       (20)      434 2023-07-10 04:42:27.000000 SGtSNEpiPy-1.0.0/setup.py
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 09:01:22.839170 SGtSNEpiPy-1.0.2/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      386 2023-07-10 09:01:22.838966 SGtSNEpiPy-1.0.2/PKG-INFO
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 09:01:22.837549 SGtSNEpiPy-1.0.2/SGtSNEpiPy/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 02:34:15.000000 SGtSNEpiPy-1.0.2/SGtSNEpiPy/__init__.py
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     1134 2023-07-10 08:11:37.000000 SGtSNEpiPy-1.0.2/SGtSNEpiPy/sgtsnepipy.py
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 09:01:22.838721 SGtSNEpiPy-1.0.2/SGtSNEpiPy.egg-info/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      386 2023-07-10 09:01:22.000000 SGtSNEpiPy-1.0.2/SGtSNEpiPy.egg-info/PKG-INFO
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      225 2023-07-10 09:01:22.000000 SGtSNEpiPy-1.0.2/SGtSNEpiPy.egg-info/SOURCES.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        1 2023-07-10 09:01:22.000000 SGtSNEpiPy-1.0.2/SGtSNEpiPy.egg-info/dependency_links.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       10 2023-07-10 09:01:22.000000 SGtSNEpiPy-1.0.2/SGtSNEpiPy.egg-info/requires.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       11 2023-07-10 09:01:22.000000 SGtSNEpiPy-1.0.2/SGtSNEpiPy.egg-info/top_level.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       38 2023-07-10 09:01:22.839246 SGtSNEpiPy-1.0.2/setup.cfg
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      569 2023-07-10 09:00:33.000000 SGtSNEpiPy-1.0.2/setup.py
```

### Comparing `SGtSNEpiPy-1.0.0/SGtSNEpiPy/pytojuliafunc.py` & `SGtSNEpiPy-1.0.2/SGtSNEpiPy/sgtsnepipy.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import scipy.sparse as sp
 import numpy as np
 
 # This function uses julia package SGtSNEpi within Python to process a sparse array in python
 # input of the function can be any type of sparse array, namely COO,CSR or CSC
 # If this function does not operate normally, check your python interpreter, make sure you use the one under anaconda file, because that is where the juliacall would be automatically installed
 
-def pytojulia(CSR_matrix):
+def sgtsnepipy(CSR_matrix):
     jl.seval('using Pkg')
     jl.seval('Pkg.add("SGtSNEpi")')
     jl.seval('Pkg.status()') 
     jl.seval("using SparseArrays")
     jl.seval("using SGtSNEpi")
 
     row,column,value = sp.find(CSR_matrix)
```

