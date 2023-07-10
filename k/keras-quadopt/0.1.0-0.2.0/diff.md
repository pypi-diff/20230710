# Comparing `tmp/keras-quadopt-0.1.0.tar.gz` & `tmp/keras-quadopt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/keras-quadopt-0.1.0.tar", last modified: Mon Apr  4 22:42:11 2022, max compression
+gzip compressed data, was "keras-quadopt-0.2.0.tar", last modified: Mon Jul 10 15:44:27 2023, max compression
```

## Comparing `keras-quadopt-0.1.0.tar` & `keras-quadopt-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2022-04-04 22:42:11.000000 keras-quadopt-0.1.0/
--rw-r--r--   0 uh         (501) staff       (20)    11340 2022-04-04 19:10:58.000000 keras-quadopt-0.1.0/LICENSE
--rw-r--r--   0 uh         (501) staff       (20)       65 2022-04-04 19:10:58.000000 keras-quadopt-0.1.0/MANIFEST.in
--rw-r--r--   0 uh         (501) staff       (20)     3308 2022-04-04 22:42:11.000000 keras-quadopt-0.1.0/PKG-INFO
--rw-r--r--   0 uh         (501) staff       (20)     2625 2022-04-04 22:32:03.000000 keras-quadopt-0.1.0/README.md
--rw-r--r--   0 uh         (501) staff       (20)     2992 2022-04-04 22:42:03.000000 keras-quadopt-0.1.0/README.rst
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2022-04-04 22:42:11.000000 keras-quadopt-0.1.0/keras_quadopt/
--rw-r--r--   0 uh         (501) staff       (20)       94 2022-04-04 22:33:55.000000 keras-quadopt-0.1.0/keras_quadopt/__init__.py
--rw-r--r--   0 uh         (501) staff       (20)     1997 2022-04-04 22:35:20.000000 keras-quadopt-0.1.0/keras_quadopt/problem.py
--rw-r--r--   0 uh         (501) staff       (20)      490 2022-04-04 22:30:25.000000 keras-quadopt-0.1.0/keras_quadopt/utils.py
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2022-04-04 22:42:11.000000 keras-quadopt-0.1.0/keras_quadopt.egg-info/
--rw-r--r--   0 uh         (501) staff       (20)     3308 2022-04-04 22:42:08.000000 keras-quadopt-0.1.0/keras_quadopt.egg-info/PKG-INFO
--rw-r--r--   0 uh         (501) staff       (20)      413 2022-04-04 22:42:10.000000 keras-quadopt-0.1.0/keras_quadopt.egg-info/SOURCES.txt
--rw-r--r--   0 uh         (501) staff       (20)        1 2022-04-04 22:42:08.000000 keras-quadopt-0.1.0/keras_quadopt.egg-info/dependency_links.txt
--rw-r--r--   0 uh         (501) staff       (20)       21 2022-04-04 22:42:10.000000 keras-quadopt-0.1.0/keras_quadopt.egg-info/requires.txt
--rw-r--r--   0 uh         (501) staff       (20)       14 2022-04-04 22:42:10.000000 keras-quadopt-0.1.0/keras_quadopt.egg-info/top_level.txt
--rw-r--r--   0 uh         (501) staff       (20)        1 2022-04-04 22:40:50.000000 keras-quadopt-0.1.0/keras_quadopt.egg-info/zip-safe
--rw-r--r--   0 uh         (501) staff       (20)       38 2022-04-04 22:42:11.000000 keras-quadopt-0.1.0/setup.cfg
--rw-r--r--   0 uh         (501) staff       (20)      961 2022-04-04 22:40:44.000000 keras-quadopt-0.1.0/setup.py
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2022-04-04 22:42:11.000000 keras-quadopt-0.1.0/test/
--rw-r--r--   0 uh         (501) staff       (20)        0 2022-04-04 19:08:01.000000 keras-quadopt-0.1.0/test/__init__.py
--rw-r--r--   0 uh         (501) staff       (20)      874 2022-04-04 22:34:42.000000 keras-quadopt-0.1.0/test/test_aggregate_matrices.py
--rw-r--r--   0 uh         (501) staff       (20)     1288 2022-04-04 22:19:55.000000 keras-quadopt-0.1.0/test/test_get_weights.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:44:27.696743 keras-quadopt-0.2.0/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)    11340 2023-07-10 08:48:27.000000 keras-quadopt-0.2.0/LICENSE
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       65 2023-07-10 08:48:27.000000 keras-quadopt-0.2.0/MANIFEST.in
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     3310 2023-07-10 15:44:27.696743 keras-quadopt-0.2.0/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     2959 2023-07-10 15:43:23.000000 keras-quadopt-0.2.0/README.md
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:44:27.692743 keras-quadopt-0.2.0/keras_quadopt/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       94 2023-07-10 14:25:12.000000 keras-quadopt-0.2.0/keras_quadopt/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     1997 2023-07-10 08:48:27.000000 keras-quadopt-0.2.0/keras_quadopt/problem.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      490 2023-07-10 08:48:27.000000 keras-quadopt-0.2.0/keras_quadopt/utils.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:44:27.692743 keras-quadopt-0.2.0/keras_quadopt.egg-info/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     3310 2023-07-10 15:44:27.000000 keras-quadopt-0.2.0/keras_quadopt.egg-info/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      402 2023-07-10 15:44:27.000000 keras-quadopt-0.2.0/keras_quadopt.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-10 15:44:27.000000 keras-quadopt-0.2.0/keras_quadopt.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       21 2023-07-10 15:44:27.000000 keras-quadopt-0.2.0/keras_quadopt.egg-info/requires.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       14 2023-07-10 15:44:27.000000 keras-quadopt-0.2.0/keras_quadopt.egg-info/top_level.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-10 15:44:27.000000 keras-quadopt-0.2.0/keras_quadopt.egg-info/zip-safe
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       38 2023-07-10 15:44:27.696743 keras-quadopt-0.2.0/setup.cfg
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     1006 2023-07-10 14:25:12.000000 keras-quadopt-0.2.0/setup.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:44:27.692743 keras-quadopt-0.2.0/test/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        0 2023-07-10 08:48:27.000000 keras-quadopt-0.2.0/test/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      874 2023-07-10 08:48:27.000000 keras-quadopt-0.2.0/test/test_aggregate_matrices.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     1288 2023-07-10 08:48:27.000000 keras-quadopt-0.2.0/test/test_get_weights.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `keras-quadopt-0.1.0/LICENSE` & `keras-quadopt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keras-quadopt-0.1.0/keras_quadopt/problem.py` & `keras-quadopt-0.2.0/keras_quadopt/problem.py`

 * *Files identical despite different names*

### Comparing `keras-quadopt-0.1.0/setup.py` & `keras-quadopt-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,19 +18,20 @@
     raise RuntimeError("Unable to find version string.")
 
 
 setuptools.setup(
     name='keras-quadopt',
     version=get_version("keras_quadopt/__init__.py"),
     description='Solving quadratic optimization problems with Keras.',
-    long_description=read('README.rst'),
-    url='http://github.com/satzbeleg/keras-quadopt',
+    long_description=read('README.md'),
+    long_description_content_type='text/markdown',
+    url='http://github.com/ulf1/keras-quadopt',
     author='Ulf Hamster',
     author_email='554c46@gmail.com',
     license='Apache License 2.0',
     packages=['keras_quadopt'],
     install_requires=[
         "tensorflow>=2.4.0,<3"
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     zip_safe=True
 )
```

### Comparing `keras-quadopt-0.1.0/test/test_aggregate_matrices.py` & `keras-quadopt-0.2.0/test/test_aggregate_matrices.py`

 * *Files identical despite different names*

### Comparing `keras-quadopt-0.1.0/test/test_get_weights.py` & `keras-quadopt-0.2.0/test/test_get_weights.py`

 * *Files identical despite different names*

