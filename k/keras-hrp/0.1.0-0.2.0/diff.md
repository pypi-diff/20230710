# Comparing `tmp/keras-hrp-0.1.0.tar.gz` & `tmp/keras-hrp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/keras-hrp-0.1.0.tar", last modified: Thu Jun 30 10:57:21 2022, max compression
+gzip compressed data, was "keras-hrp-0.2.0.tar", last modified: Mon Jul 10 08:11:54 2023, max compression
```

## Comparing `keras-hrp-0.1.0.tar` & `keras-hrp-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2022-06-30 10:57:21.000000 keras-hrp-0.1.0/
--rw-r--r--   0 uh         (501) staff       (20)    11340 2022-06-30 07:54:27.000000 keras-hrp-0.1.0/LICENSE
--rw-r--r--   0 uh         (501) staff       (20)       65 2022-06-30 07:54:27.000000 keras-hrp-0.1.0/MANIFEST.in
--rw-r--r--   0 uh         (501) staff       (20)      280 2022-06-30 10:57:21.000000 keras-hrp-0.1.0/PKG-INFO
--rw-r--r--   0 uh         (501) staff       (20)     4097 2022-06-30 10:52:39.000000 keras-hrp-0.1.0/README.md
--rw-r--r--   0 uh         (501) staff       (20)        0 2022-06-30 10:56:11.000000 keras-hrp-0.1.0/README.rst
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2022-06-30 10:57:21.000000 keras-hrp-0.1.0/keras_hrp/
--rw-r--r--   0 uh         (501) staff       (20)      219 2022-06-30 10:12:10.000000 keras-hrp-0.1.0/keras_hrp/__init__.py
--rw-r--r--   0 uh         (501) staff       (20)     1284 2022-06-30 10:07:25.000000 keras-hrp-0.1.0/keras_hrp/distance.py
--rw-r--r--   0 uh         (501) staff       (20)     1973 2022-06-30 10:07:21.000000 keras-hrp-0.1.0/keras_hrp/hrp.py
--rw-r--r--   0 uh         (501) staff       (20)      363 2022-06-30 10:12:04.000000 keras-hrp-0.1.0/keras_hrp/serialize.py
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2022-06-30 10:57:21.000000 keras-hrp-0.1.0/keras_hrp.egg-info/
--rw-r--r--   0 uh         (501) staff       (20)      280 2022-06-30 10:57:19.000000 keras-hrp-0.1.0/keras_hrp.egg-info/PKG-INFO
--rw-r--r--   0 uh         (501) staff       (20)      404 2022-06-30 10:57:21.000000 keras-hrp-0.1.0/keras_hrp.egg-info/SOURCES.txt
--rw-r--r--   0 uh         (501) staff       (20)        1 2022-06-30 10:57:19.000000 keras-hrp-0.1.0/keras_hrp.egg-info/dependency_links.txt
--rw-r--r--   0 uh         (501) staff       (20)       71 2022-06-30 10:57:20.000000 keras-hrp-0.1.0/keras_hrp.egg-info/requires.txt
--rw-r--r--   0 uh         (501) staff       (20)       10 2022-06-30 10:57:20.000000 keras-hrp-0.1.0/keras_hrp.egg-info/top_level.txt
--rw-r--r--   0 uh         (501) staff       (20)        1 2022-06-30 10:57:19.000000 keras-hrp-0.1.0/keras_hrp.egg-info/zip-safe
--rw-r--r--   0 uh         (501) staff       (20)       38 2022-06-30 10:57:21.000000 keras-hrp-0.1.0/setup.cfg
--rw-r--r--   0 uh         (501) staff       (20)     1022 2022-06-30 10:57:10.000000 keras-hrp-0.1.0/setup.py
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2022-06-30 10:57:21.000000 keras-hrp-0.1.0/test/
--rw-r--r--   0 uh         (501) staff       (20)        0 2022-06-30 07:53:44.000000 keras-hrp-0.1.0/test/__init__.py
--rw-r--r--   0 uh         (501) staff       (20)      897 2022-06-30 10:53:52.000000 keras-hrp-0.1.0/test/test_distance.py
--rw-r--r--   0 uh         (501) staff       (20)     2106 2022-06-30 10:53:27.000000 keras-hrp-0.1.0/test/test_hrp.py
--rw-r--r--   0 uh         (501) staff       (20)      268 2022-06-30 10:13:40.000000 keras-hrp-0.1.0/test/test_serialize.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 08:11:54.858279 keras-hrp-0.2.0/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)    11340 2023-05-09 08:44:48.000000 keras-hrp-0.2.0/LICENSE
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       65 2023-05-09 08:44:48.000000 keras-hrp-0.2.0/MANIFEST.in
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     5039 2023-07-10 08:11:54.858279 keras-hrp-0.2.0/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     4703 2023-07-10 08:00:38.000000 keras-hrp-0.2.0/README.md
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 08:11:54.854279 keras-hrp-0.2.0/keras_hrp/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      219 2023-07-10 08:03:38.000000 keras-hrp-0.2.0/keras_hrp/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     1284 2023-05-09 08:44:48.000000 keras-hrp-0.2.0/keras_hrp/distance.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     1973 2023-05-09 08:44:48.000000 keras-hrp-0.2.0/keras_hrp/hrp.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      363 2023-05-09 16:18:17.000000 keras-hrp-0.2.0/keras_hrp/serialize.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 08:11:54.858279 keras-hrp-0.2.0/keras_hrp.egg-info/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     5039 2023-07-10 08:11:54.000000 keras-hrp-0.2.0/keras_hrp.egg-info/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      393 2023-07-10 08:11:54.000000 keras-hrp-0.2.0/keras_hrp.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-10 08:11:54.000000 keras-hrp-0.2.0/keras_hrp.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       71 2023-07-10 08:11:54.000000 keras-hrp-0.2.0/keras_hrp.egg-info/requires.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       10 2023-07-10 08:11:54.000000 keras-hrp-0.2.0/keras_hrp.egg-info/top_level.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-10 08:11:54.000000 keras-hrp-0.2.0/keras_hrp.egg-info/zip-safe
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       38 2023-07-10 08:11:54.858279 keras-hrp-0.2.0/setup.cfg
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     1067 2023-07-08 16:55:22.000000 keras-hrp-0.2.0/setup.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 08:11:54.858279 keras-hrp-0.2.0/test/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        0 2023-05-09 08:44:48.000000 keras-hrp-0.2.0/test/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      897 2023-05-09 08:44:48.000000 keras-hrp-0.2.0/test/test_distance.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     2106 2023-05-09 08:44:48.000000 keras-hrp-0.2.0/test/test_hrp.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      268 2023-05-09 08:44:48.000000 keras-hrp-0.2.0/test/test_serialize.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `keras-hrp-0.1.0/LICENSE` & `keras-hrp-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keras-hrp-0.1.0/keras_hrp/distance.py` & `keras-hrp-0.2.0/keras_hrp/distance.py`

 * *Files identical despite different names*

### Comparing `keras-hrp-0.1.0/keras_hrp/hrp.py` & `keras-hrp-0.2.0/keras_hrp/hrp.py`

 * *Files identical despite different names*

### Comparing `keras-hrp-0.1.0/setup.py` & `keras-hrp-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,16 +18,17 @@
     raise RuntimeError("Unable to find version string.")
 
 
 setuptools.setup(
     name='keras-hrp',
     version=get_version("keras_hrp/__init__.py"),
     description='Hashed Random Projection layer for TF2/Keras',
-    long_description=read('README.rst'),
-    url='http://github.com/satzbeleg/keras-hrp',
+    long_description=read('README.md'),
+    long_description_content_type='text/markdown',
+    url='http://github.com/ulf1/keras-hrp',
     author='Ulf Hamster',
     author_email='554c46@gmail.com',
     license='Apache License 2.0',
     packages=['keras_hrp'],
     install_requires=[
         'tensorflow>=2.8.0,<3',
         'numpy>=1.19.5,<2',
```

### Comparing `keras-hrp-0.1.0/test/test_distance.py` & `keras-hrp-0.2.0/test/test_distance.py`

 * *Files identical despite different names*

### Comparing `keras-hrp-0.1.0/test/test_hrp.py` & `keras-hrp-0.2.0/test/test_hrp.py`

 * *Files identical despite different names*

