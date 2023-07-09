# Comparing `tmp/edp_redy_py-0.1.8.tar.gz` & `tmp/edp_redy_py-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edp_redy_py-0.1.8.tar", last modified: Sun Jul  9 22:11:37 2023, max compression
+gzip compressed data, was "edp_redy_py-0.1.9.tar", last modified: Sun Jul  9 23:00:16 2023, max compression
```

## Comparing `edp_redy_py-0.1.8.tar` & `edp_redy_py-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 22:11:37.739086 edp_redy_py-0.1.8/
--rw-rw-rw-   0        0        0    11556 2023-07-08 16:56:32.000000 edp_redy_py-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      283 2023-07-09 22:11:37.739086 edp_redy_py-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-08 17:07:46.000000 edp_redy_py-0.1.8/README.md
--rw-rw-rw-   0        0        0      111 2023-07-09 22:11:37.742009 edp_redy_py-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      557 2023-07-09 22:11:35.000000 edp_redy_py-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 22:11:37.697740 edp_redy_py-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-09 22:11:37.711001 edp_redy_py-0.1.8/src/edp_redy/
--rw-rw-rw-   0        0        0        0 2023-07-08 15:14:43.000000 edp_redy_py-0.1.8/src/edp_redy/__init__.py
--rw-rw-rw-   0        0        0     1953 2023-07-08 17:53:36.000000 edp_redy_py-0.1.8/src/edp_redy/authenticate.py
--rw-rw-rw-   0        0        0      204 2023-07-08 16:51:43.000000 edp_redy_py-0.1.8/src/edp_redy/consts.py
--rw-rw-rw-   0        0        0     2549 2023-07-08 18:05:54.000000 edp_redy_py-0.1.8/src/edp_redy/edp_mqtt.py
-drwxrwxrwx   0        0        0        0 2023-07-09 22:11:37.713720 edp_redy_py-0.1.8/src/edp_redy/equipment/
--rw-rw-rw-   0        0        0        0 2023-07-08 16:25:40.000000 edp_redy_py-0.1.8/src/edp_redy/equipment/__init__.py
--rw-rw-rw-   0        0        0     7618 2023-07-08 17:33:47.000000 edp_redy_py-0.1.8/src/edp_redy/equipment/equipment.py
--rw-rw-rw-   0        0        0     1003 2023-07-08 16:51:43.000000 edp_redy_py-0.1.8/src/edp_redy/helpers.py
--rw-rw-rw-   0        0        0      721 2023-07-08 17:37:45.000000 edp_redy_py-0.1.8/src/edp_redy/redy.py
-drwxrwxrwx   0        0        0        0 2023-07-09 22:11:37.716432 edp_redy_py-0.1.8/src/edp_redy/usermanagement/
--rw-rw-rw-   0        0        0        0 2023-07-08 15:24:38.000000 edp_redy_py-0.1.8/src/edp_redy/usermanagement/__init__.py
--rw-rw-rw-   0        0        0     2296 2023-07-08 17:33:51.000000 edp_redy_py-0.1.8/src/edp_redy/usermanagement/usermanagement.py
-drwxrwxrwx   0        0        0        0 2023-07-09 22:11:37.737470 edp_redy_py-0.1.8/src/edp_redy_py.egg-info/
--rw-rw-rw-   0        0        0      283 2023-07-09 22:11:37.000000 edp_redy_py-0.1.8/src/edp_redy_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2023-07-09 22:11:37.000000 edp_redy_py-0.1.8/src/edp_redy_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 22:11:37.000000 edp_redy_py-0.1.8/src/edp_redy_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-07-09 22:11:37.000000 edp_redy_py-0.1.8/src/edp_redy_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-09 22:11:37.000000 edp_redy_py-0.1.8/src/edp_redy_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 23:00:16.037955 edp_redy_py-0.1.9/
+-rw-rw-rw-   0        0        0    11556 2023-07-08 16:56:32.000000 edp_redy_py-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      283 2023-07-09 23:00:16.037955 edp_redy_py-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-08 17:07:46.000000 edp_redy_py-0.1.9/README.md
+-rw-rw-rw-   0        0        0      111 2023-07-09 23:00:16.040105 edp_redy_py-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-07-09 23:00:13.000000 edp_redy_py-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:00:15.997392 edp_redy_py-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-09 23:00:16.011451 edp_redy_py-0.1.9/src/edp_redy/
+-rw-rw-rw-   0        0        0        0 2023-07-08 15:14:43.000000 edp_redy_py-0.1.9/src/edp_redy/__init__.py
+-rw-rw-rw-   0        0        0     1953 2023-07-08 17:53:36.000000 edp_redy_py-0.1.9/src/edp_redy/authenticate.py
+-rw-rw-rw-   0        0        0      204 2023-07-08 16:51:43.000000 edp_redy_py-0.1.9/src/edp_redy/consts.py
+-rw-rw-rw-   0        0        0     2549 2023-07-08 18:05:54.000000 edp_redy_py-0.1.9/src/edp_redy/edp_mqtt.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:00:16.013604 edp_redy_py-0.1.9/src/edp_redy/equipment/
+-rw-rw-rw-   0        0        0        0 2023-07-08 16:25:40.000000 edp_redy_py-0.1.9/src/edp_redy/equipment/__init__.py
+-rw-rw-rw-   0        0        0     7618 2023-07-08 17:33:47.000000 edp_redy_py-0.1.9/src/edp_redy/equipment/equipment.py
+-rw-rw-rw-   0        0        0     1003 2023-07-08 16:51:43.000000 edp_redy_py-0.1.9/src/edp_redy/helpers.py
+-rw-rw-rw-   0        0        0      721 2023-07-08 17:37:45.000000 edp_redy_py-0.1.9/src/edp_redy/redy.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:00:16.015729 edp_redy_py-0.1.9/src/edp_redy/usermanagement/
+-rw-rw-rw-   0        0        0        0 2023-07-08 15:24:38.000000 edp_redy_py-0.1.9/src/edp_redy/usermanagement/__init__.py
+-rw-rw-rw-   0        0        0     2296 2023-07-08 17:33:51.000000 edp_redy_py-0.1.9/src/edp_redy/usermanagement/usermanagement.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:00:16.036344 edp_redy_py-0.1.9/src/edp_redy_py.egg-info/
+-rw-rw-rw-   0        0        0      283 2023-07-09 23:00:15.000000 edp_redy_py-0.1.9/src/edp_redy_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2023-07-09 23:00:15.000000 edp_redy_py-0.1.9/src/edp_redy_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 23:00:15.000000 edp_redy_py-0.1.9/src/edp_redy_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-07-09 23:00:15.000000 edp_redy_py-0.1.9/src/edp_redy_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-09 23:00:15.000000 edp_redy_py-0.1.9/src/edp_redy_py.egg-info/top_level.txt
```

### Comparing `edp_redy_py-0.1.8/LICENSE` & `edp_redy_py-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.8/setup.py` & `edp_redy_py-0.1.9/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='edp_redy_py',
-    version='0.1.8',
+    version='0.1.9',
     license='Apache 2.0',
     author="Fábio Ferreira",
     author_email='fabiorcferreira@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/skyborgff/edp_redy',
     keywords='EDP',
     install_requires=[
         "python-dateutil~=2.8.2",
         "awscrt~=0.16.23",
         "awsiot~=0.1.3",
         "requests~=2.31.0",
-        "warrant~=0.6.1",
+        "warrant-ext>=0.6.2",
         "setuptools~=58.1.0",
     ],
 
 )
```

### Comparing `edp_redy_py-0.1.8/src/edp_redy/authenticate.py` & `edp_redy_py-0.1.9/src/edp_redy/authenticate.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.8/src/edp_redy/edp_mqtt.py` & `edp_redy_py-0.1.9/src/edp_redy/edp_mqtt.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.8/src/edp_redy/equipment/equipment.py` & `edp_redy_py-0.1.9/src/edp_redy/equipment/equipment.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.8/src/edp_redy/helpers.py` & `edp_redy_py-0.1.9/src/edp_redy/helpers.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.8/src/edp_redy/redy.py` & `edp_redy_py-0.1.9/src/edp_redy/redy.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.8/src/edp_redy/usermanagement/usermanagement.py` & `edp_redy_py-0.1.9/src/edp_redy/usermanagement/usermanagement.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.8/src/edp_redy_py.egg-info/SOURCES.txt` & `edp_redy_py-0.1.9/src/edp_redy_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

