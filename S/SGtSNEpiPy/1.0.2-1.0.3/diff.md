# Comparing `tmp/SGtSNEpiPy-1.0.2.tar.gz` & `tmp/SGtSNEpiPy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SGtSNEpiPy-1.0.2.tar", last modified: Mon Jul 10 09:01:22 2023, max compression
+gzip compressed data, was "SGtSNEpiPy-1.0.3.tar", last modified: Mon Jul 10 09:49:19 2023, max compression
```

## Comparing `SGtSNEpiPy-1.0.2.tar` & `SGtSNEpiPy-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 09:01:22.839170 SGtSNEpiPy-1.0.2/
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      386 2023-07-10 09:01:22.838966 SGtSNEpiPy-1.0.2/PKG-INFO
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 09:01:22.837549 SGtSNEpiPy-1.0.2/SGtSNEpiPy/
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 02:34:15.000000 SGtSNEpiPy-1.0.2/SGtSNEpiPy/__init__.py
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     1134 2023-07-10 08:11:37.000000 SGtSNEpiPy-1.0.2/SGtSNEpiPy/sgtsnepipy.py
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 09:01:22.838721 SGtSNEpiPy-1.0.2/SGtSNEpiPy.egg-info/
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      386 2023-07-10 09:01:22.000000 SGtSNEpiPy-1.0.2/SGtSNEpiPy.egg-info/PKG-INFO
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      225 2023-07-10 09:01:22.000000 SGtSNEpiPy-1.0.2/SGtSNEpiPy.egg-info/SOURCES.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        1 2023-07-10 09:01:22.000000 SGtSNEpiPy-1.0.2/SGtSNEpiPy.egg-info/dependency_links.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       10 2023-07-10 09:01:22.000000 SGtSNEpiPy-1.0.2/SGtSNEpiPy.egg-info/requires.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       11 2023-07-10 09:01:22.000000 SGtSNEpiPy-1.0.2/SGtSNEpiPy.egg-info/top_level.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       38 2023-07-10 09:01:22.839246 SGtSNEpiPy-1.0.2/setup.cfg
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      569 2023-07-10 09:00:33.000000 SGtSNEpiPy-1.0.2/setup.py
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 09:49:19.216101 SGtSNEpiPy-1.0.3/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      506 2023-07-10 09:49:19.215922 SGtSNEpiPy-1.0.3/PKG-INFO
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 09:49:19.214872 SGtSNEpiPy-1.0.3/SGtSNEpiPy/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 02:34:15.000000 SGtSNEpiPy-1.0.3/SGtSNEpiPy/__init__.py
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     1110 2023-07-10 09:47:54.000000 SGtSNEpiPy-1.0.3/SGtSNEpiPy/sgtsnepipy.py
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 09:49:19.215696 SGtSNEpiPy-1.0.3/SGtSNEpiPy.egg-info/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      506 2023-07-10 09:49:19.000000 SGtSNEpiPy-1.0.3/SGtSNEpiPy.egg-info/PKG-INFO
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      225 2023-07-10 09:49:19.000000 SGtSNEpiPy-1.0.3/SGtSNEpiPy.egg-info/SOURCES.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        1 2023-07-10 09:49:19.000000 SGtSNEpiPy-1.0.3/SGtSNEpiPy.egg-info/dependency_links.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       10 2023-07-10 09:49:19.000000 SGtSNEpiPy-1.0.3/SGtSNEpiPy.egg-info/requires.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       11 2023-07-10 09:49:19.000000 SGtSNEpiPy-1.0.3/SGtSNEpiPy.egg-info/top_level.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       38 2023-07-10 09:49:19.216163 SGtSNEpiPy-1.0.3/setup.cfg
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      689 2023-07-10 09:47:52.000000 SGtSNEpiPy-1.0.3/setup.py
```

### Comparing `SGtSNEpiPy-1.0.2/SGtSNEpiPy/sgtsnepipy.py` & `SGtSNEpiPy-1.0.3/SGtSNEpiPy/sgtsnepipy.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,10 +20,9 @@
     column_array = jl.Array(column)
     value_array = jl.Array(value)
     m,n = CSR_matrix.shape
     result_py = jl.SparseArrays.sparse(row_array,column_array,value_array,m,n)
     jl.result_jl = jl.sgtsnepi(result_py)
     result_py = np.array(jl.result_jl,dtype = np.float64)
     result_list = result_py.tolist()
-    print(result_list)
 
-    return jl.result_jl
+    return result_list
```

### Comparing `SGtSNEpiPy-1.0.2/setup.py` & `SGtSNEpiPy-1.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 import setuptools
 
 setup(
     name='SGtSNEpiPy',
-    version='1.0.2',
+    version='1.0.3',
     description='SGtSNEpiPy is a Python interface for the SG-t-SNE-П algorithm, a powerful tool for visualizing large, sparse, stochastic graphs.',
-    long_description= "If you meet any issue, feel free to contact authors.\nEmail:\nchenshuhao.qin@duke.edu\nyihua.zhong@duke.edu",
+    long_description= "This is a Python wrapper for SG-t-SNE-П, implemented using the JuliaCall module from PythonCall & JuliaCall package. /nIf you meet any issue, feel free to contact authors.\nEmail:\nchenshuhao.qin@duke.edu\nyihua.zhong@duke.edu",
     author=['Chenshuhao Qin','Yihua Zhong'],
     author_email="cq27@duke.edu, yz737@duke.edu,",
     packages=setuptools.find_packages(),
     install_requires=[
         'juliacall',
     ]
 )
```

