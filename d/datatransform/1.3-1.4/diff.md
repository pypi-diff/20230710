# Comparing `tmp/datatransform-1.3.tar.gz` & `tmp/datatransform-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatransform-1.3.tar", last modified: Mon Jul 10 17:46:06 2023, max compression
+gzip compressed data, was "datatransform-1.4.tar", last modified: Mon Jul 10 20:29:34 2023, max compression
```

## Comparing `datatransform-1.3.tar` & `datatransform-1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 17:46:06.375855 datatransform-1.3/
--rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-10 17:46:06.375713 datatransform-1.3/PKG-INFO
-drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 17:46:06.374908 datatransform-1.3/datatransform/
--rw-r--r--   0 janitsharma   (501) staff       (20)       80 2023-07-05 21:01:31.000000 datatransform-1.3/datatransform/__init__.py
--rw-r--r--   0 janitsharma   (501) staff       (20)     1608 2023-07-10 17:17:05.000000 datatransform-1.3/datatransform/datatransform.py
--rw-r--r--   0 janitsharma   (501) staff       (20)      793 2023-07-10 17:38:12.000000 datatransform-1.3/datatransform/leave_one_out.py
--rw-r--r--   0 janitsharma   (501) staff       (20)     1318 2023-07-10 17:38:07.000000 datatransform-1.3/datatransform/mca.py
--rw-r--r--   0 janitsharma   (501) staff       (20)      775 2023-07-10 17:38:01.000000 datatransform-1.3/datatransform/pca.py
-drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 17:46:06.375506 datatransform-1.3/datatransform.egg-info/
--rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-10 17:46:06.000000 datatransform-1.3/datatransform.egg-info/PKG-INFO
--rw-r--r--   0 janitsharma   (501) staff       (20)      286 2023-07-10 17:46:06.000000 datatransform-1.3/datatransform.egg-info/SOURCES.txt
--rw-r--r--   0 janitsharma   (501) staff       (20)        1 2023-07-10 17:46:06.000000 datatransform-1.3/datatransform.egg-info/dependency_links.txt
--rw-r--r--   0 janitsharma   (501) staff       (20)       14 2023-07-10 17:46:06.000000 datatransform-1.3/datatransform.egg-info/top_level.txt
--rw-r--r--   0 janitsharma   (501) staff       (20)       38 2023-07-10 17:46:06.375894 datatransform-1.3/setup.cfg
--rw-r--r--   0 janitsharma   (501) staff       (20)      128 2023-07-10 17:45:23.000000 datatransform-1.3/setup.py
+drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 20:29:34.540568 datatransform-1.4/
+-rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-10 20:29:34.540440 datatransform-1.4/PKG-INFO
+drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 20:29:34.539514 datatransform-1.4/datatransform/
+-rw-r--r--   0 janitsharma   (501) staff       (20)       80 2023-07-05 21:01:31.000000 datatransform-1.4/datatransform/__init__.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)     1608 2023-07-10 17:17:05.000000 datatransform-1.4/datatransform/datatransform.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)      793 2023-07-10 17:38:12.000000 datatransform-1.4/datatransform/leave_one_out.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)     1318 2023-07-10 17:38:07.000000 datatransform-1.4/datatransform/mca.py
+-rw-r--r--   0 janitsharma   (501) staff       (20)      775 2023-07-10 18:16:49.000000 datatransform-1.4/datatransform/pca.py
+drwxr-xr-x   0 janitsharma   (501) staff       (20)        0 2023-07-10 20:29:34.540257 datatransform-1.4/datatransform.egg-info/
+-rw-r--r--   0 janitsharma   (501) staff       (20)       55 2023-07-10 20:29:34.000000 datatransform-1.4/datatransform.egg-info/PKG-INFO
+-rw-r--r--   0 janitsharma   (501) staff       (20)      286 2023-07-10 20:29:34.000000 datatransform-1.4/datatransform.egg-info/SOURCES.txt
+-rw-r--r--   0 janitsharma   (501) staff       (20)        1 2023-07-10 20:29:34.000000 datatransform-1.4/datatransform.egg-info/dependency_links.txt
+-rw-r--r--   0 janitsharma   (501) staff       (20)       14 2023-07-10 20:29:34.000000 datatransform-1.4/datatransform.egg-info/top_level.txt
+-rw-r--r--   0 janitsharma   (501) staff       (20)       38 2023-07-10 20:29:34.540603 datatransform-1.4/setup.cfg
+-rw-r--r--   0 janitsharma   (501) staff       (20)      128 2023-07-10 20:23:26.000000 datatransform-1.4/setup.py
```

### Comparing `datatransform-1.3/datatransform/datatransform.py` & `datatransform-1.4/datatransform/datatransform.py`

 * *Files identical despite different names*

### Comparing `datatransform-1.3/datatransform/leave_one_out.py` & `datatransform-1.4/datatransform/leave_one_out.py`

 * *Files identical despite different names*

### Comparing `datatransform-1.3/datatransform/mca.py` & `datatransform-1.4/datatransform/mca.py`

 * *Files identical despite different names*

### Comparing `datatransform-1.3/datatransform/pca.py` & `datatransform-1.4/datatransform/pca.py`

 * *Files identical despite different names*

