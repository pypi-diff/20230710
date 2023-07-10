# Comparing `tmp/SGtSNEpiPy-1.0.3.tar.gz` & `tmp/SGtSNEpiPy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SGtSNEpiPy-1.0.3.tar", last modified: Mon Jul 10 09:49:19 2023, max compression
+gzip compressed data, was "SGtSNEpiPy-1.0.4.tar", last modified: Mon Jul 10 09:54:29 2023, max compression
```

## Comparing `SGtSNEpiPy-1.0.3.tar` & `SGtSNEpiPy-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 09:49:19.216101 SGtSNEpiPy-1.0.3/
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      506 2023-07-10 09:49:19.215922 SGtSNEpiPy-1.0.3/PKG-INFO
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 09:49:19.214872 SGtSNEpiPy-1.0.3/SGtSNEpiPy/
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 02:34:15.000000 SGtSNEpiPy-1.0.3/SGtSNEpiPy/__init__.py
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     1110 2023-07-10 09:47:54.000000 SGtSNEpiPy-1.0.3/SGtSNEpiPy/sgtsnepipy.py
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 09:49:19.215696 SGtSNEpiPy-1.0.3/SGtSNEpiPy.egg-info/
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      506 2023-07-10 09:49:19.000000 SGtSNEpiPy-1.0.3/SGtSNEpiPy.egg-info/PKG-INFO
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      225 2023-07-10 09:49:19.000000 SGtSNEpiPy-1.0.3/SGtSNEpiPy.egg-info/SOURCES.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        1 2023-07-10 09:49:19.000000 SGtSNEpiPy-1.0.3/SGtSNEpiPy.egg-info/dependency_links.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       10 2023-07-10 09:49:19.000000 SGtSNEpiPy-1.0.3/SGtSNEpiPy.egg-info/requires.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       11 2023-07-10 09:49:19.000000 SGtSNEpiPy-1.0.3/SGtSNEpiPy.egg-info/top_level.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       38 2023-07-10 09:49:19.216163 SGtSNEpiPy-1.0.3/setup.cfg
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      689 2023-07-10 09:47:52.000000 SGtSNEpiPy-1.0.3/setup.py
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 09:54:29.049459 SGtSNEpiPy-1.0.4/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      647 2023-07-10 09:54:29.049275 SGtSNEpiPy-1.0.4/PKG-INFO
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 09:54:29.048084 SGtSNEpiPy-1.0.4/SGtSNEpiPy/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 02:34:15.000000 SGtSNEpiPy-1.0.4/SGtSNEpiPy/__init__.py
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     1110 2023-07-10 09:47:54.000000 SGtSNEpiPy-1.0.4/SGtSNEpiPy/sgtsnepipy.py
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 09:54:29.049069 SGtSNEpiPy-1.0.4/SGtSNEpiPy.egg-info/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      647 2023-07-10 09:54:28.000000 SGtSNEpiPy-1.0.4/SGtSNEpiPy.egg-info/PKG-INFO
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      225 2023-07-10 09:54:29.000000 SGtSNEpiPy-1.0.4/SGtSNEpiPy.egg-info/SOURCES.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        1 2023-07-10 09:54:28.000000 SGtSNEpiPy-1.0.4/SGtSNEpiPy.egg-info/dependency_links.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       10 2023-07-10 09:54:28.000000 SGtSNEpiPy-1.0.4/SGtSNEpiPy.egg-info/requires.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       11 2023-07-10 09:54:28.000000 SGtSNEpiPy-1.0.4/SGtSNEpiPy.egg-info/top_level.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       38 2023-07-10 09:54:29.049525 SGtSNEpiPy-1.0.4/setup.cfg
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      830 2023-07-10 09:53:49.000000 SGtSNEpiPy-1.0.4/setup.py
```

### Comparing `SGtSNEpiPy-1.0.3/SGtSNEpiPy/sgtsnepipy.py` & `SGtSNEpiPy-1.0.4/SGtSNEpiPy/sgtsnepipy.py`

 * *Files identical despite different names*

