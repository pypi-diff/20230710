# Comparing `tmp/bool-to-int8-ray-0.1.1.tar.gz` & `tmp/bool-to-int8-ray-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bool-to-int8-ray-0.1.1.tar", last modified: Tue May 16 13:13:11 2023, max compression
+gzip compressed data, was "bool-to-int8-ray-0.2.0.tar", last modified: Mon Jul 10 08:31:15 2023, max compression
```

## Comparing `bool-to-int8-ray-0.1.1.tar` & `bool-to-int8-ray-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-05-16 13:13:11.993179 bool-to-int8-ray-0.1.1/
--rw-rw-r--   0 hamster   (1000) hamster   (1000)    11340 2023-05-09 13:33:12.000000 bool-to-int8-ray-0.1.1/LICENSE
--rw-rw-r--   0 hamster   (1000) hamster   (1000)       65 2023-05-09 13:33:12.000000 bool-to-int8-ray-0.1.1/MANIFEST.in
--rw-rw-r--   0 hamster   (1000) hamster   (1000)     2879 2023-05-16 13:13:11.993179 bool-to-int8-ray-0.1.1/PKG-INFO
--rw-rw-r--   0 hamster   (1000) hamster   (1000)     2530 2023-05-16 13:12:58.000000 bool-to-int8-ray-0.1.1/README.md
-drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-05-16 13:13:11.993179 bool-to-int8-ray-0.1.1/bool_to_int8_ray/
--rw-rw-r--   0 hamster   (1000) hamster   (1000)      116 2023-05-16 13:12:58.000000 bool-to-int8-ray-0.1.1/bool_to_int8_ray/__init__.py
--rw-rw-r--   0 hamster   (1000) hamster   (1000)     2178 2023-05-16 13:12:58.000000 bool-to-int8-ray-0.1.1/bool_to_int8_ray/serialize.py
-drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-05-16 13:13:11.993179 bool-to-int8-ray-0.1.1/bool_to_int8_ray.egg-info/
--rw-rw-r--   0 hamster   (1000) hamster   (1000)     2879 2023-05-16 13:13:11.000000 bool-to-int8-ray-0.1.1/bool_to_int8_ray.egg-info/PKG-INFO
--rw-rw-r--   0 hamster   (1000) hamster   (1000)      389 2023-05-16 13:13:11.000000 bool-to-int8-ray-0.1.1/bool_to_int8_ray.egg-info/SOURCES.txt
--rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-05-16 13:13:11.000000 bool-to-int8-ray-0.1.1/bool_to_int8_ray.egg-info/dependency_links.txt
--rw-rw-r--   0 hamster   (1000) hamster   (1000)       37 2023-05-16 13:13:11.000000 bool-to-int8-ray-0.1.1/bool_to_int8_ray.egg-info/requires.txt
--rw-rw-r--   0 hamster   (1000) hamster   (1000)       17 2023-05-16 13:13:11.000000 bool-to-int8-ray-0.1.1/bool_to_int8_ray.egg-info/top_level.txt
--rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-05-09 16:04:11.000000 bool-to-int8-ray-0.1.1/bool_to_int8_ray.egg-info/zip-safe
--rw-rw-r--   0 hamster   (1000) hamster   (1000)       38 2023-05-16 13:13:11.993179 bool-to-int8-ray-0.1.1/setup.cfg
--rw-rw-r--   0 hamster   (1000) hamster   (1000)     1048 2023-05-09 14:24:59.000000 bool-to-int8-ray-0.1.1/setup.py
-drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-05-16 13:13:11.993179 bool-to-int8-ray-0.1.1/test/
--rw-rw-r--   0 hamster   (1000) hamster   (1000)        0 2023-05-09 13:33:12.000000 bool-to-int8-ray-0.1.1/test/__init__.py
--rw-rw-r--   0 hamster   (1000) hamster   (1000)     1544 2023-05-09 15:52:41.000000 bool-to-int8-ray-0.1.1/test/speedtest.py
--rw-rw-r--   0 hamster   (1000) hamster   (1000)      657 2023-05-09 15:45:00.000000 bool-to-int8-ray-0.1.1/test/test_serialize.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 08:31:15.530958 bool-to-int8-ray-0.2.0/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)    11340 2023-05-09 13:33:12.000000 bool-to-int8-ray-0.2.0/LICENSE
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       65 2023-05-09 13:33:12.000000 bool-to-int8-ray-0.2.0/MANIFEST.in
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     3337 2023-07-10 08:31:15.530958 bool-to-int8-ray-0.2.0/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     2993 2023-07-10 08:02:19.000000 bool-to-int8-ray-0.2.0/README.md
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 08:31:15.526958 bool-to-int8-ray-0.2.0/bool_to_int8_ray/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      116 2023-07-10 08:00:49.000000 bool-to-int8-ray-0.2.0/bool_to_int8_ray/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     2178 2023-05-16 13:12:58.000000 bool-to-int8-ray-0.2.0/bool_to_int8_ray/serialize.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 08:31:15.526958 bool-to-int8-ray-0.2.0/bool_to_int8_ray.egg-info/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     3337 2023-07-10 08:31:15.000000 bool-to-int8-ray-0.2.0/bool_to_int8_ray.egg-info/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      389 2023-07-10 08:31:15.000000 bool-to-int8-ray-0.2.0/bool_to_int8_ray.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-10 08:31:15.000000 bool-to-int8-ray-0.2.0/bool_to_int8_ray.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       37 2023-07-10 08:31:15.000000 bool-to-int8-ray-0.2.0/bool_to_int8_ray.egg-info/requires.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       17 2023-07-10 08:31:15.000000 bool-to-int8-ray-0.2.0/bool_to_int8_ray.egg-info/top_level.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-10 08:31:15.000000 bool-to-int8-ray-0.2.0/bool_to_int8_ray.egg-info/zip-safe
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       38 2023-07-10 08:31:15.530958 bool-to-int8-ray-0.2.0/setup.cfg
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     1043 2023-07-08 16:55:31.000000 bool-to-int8-ray-0.2.0/setup.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 08:31:15.526958 bool-to-int8-ray-0.2.0/test/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        0 2023-05-09 13:33:12.000000 bool-to-int8-ray-0.2.0/test/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     1544 2023-05-09 15:52:41.000000 bool-to-int8-ray-0.2.0/test/speedtest.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      657 2023-05-09 15:45:00.000000 bool-to-int8-ray-0.2.0/test/test_serialize.py
```

### Comparing `bool-to-int8-ray-0.1.1/LICENSE` & `bool-to-int8-ray-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bool-to-int8-ray-0.1.1/PKG-INFO` & `bool-to-int8-ray-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: bool-to-int8-ray
-Version: 0.1.1
-Summary: bool to int8 serialization with ray.io
-Home-page: http://github.com/satzbeleg/bool-to-int8-ray
-Author: Ulf Hamster
-Author-email: 554c46@gmail.com
-License: Apache License 2.0
-Platform: UNKNOWN
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![PyPI version](https://badge.fury.io/py/bool-to-int8-ray.svg)](https://badge.fury.io/py/bool-to-int8-ray)
 [![PyPi downloads](https://img.shields.io/pypi/dm/bool-to-int8-ray)](https://img.shields.io/pypi/dm/bool-to-int8-ray)
 
 # bool-to-int8-ray
 bool to int8 serialization with ray.io
 
 ## Installation
@@ -59,19 +46,19 @@
  2.308446 -- ray.io version, hash to int8
  3.023865 -- ray.io version, int8 to hash
 ```
 
 ## Appendix
 
 ### Installation
-The `bool-to-int8-ray` [git repo](http://github.com/satzbeleg/bool-to-int8-ray) is available as [PyPi package](https://pypi.org/project/bool-to-int8-ray)
+The `bool-to-int8-ray` [git repo](http://github.com/ulf1/bool-to-int8-ray) is available as [PyPi package](https://pypi.org/project/bool-to-int8-ray)
 
 ```sh
 pip install bool-to-int8-ray
-pip install git+ssh://git@github.com/satzbeleg/bool-to-int8-ray.git
+pip install git+ssh://git@github.com/ulf1/bool-to-int8-ray.git
 ```
 
 ### Install a virtual environment
 
 ```sh
 python3 -m venv .venv
 source .venv/bin/activate
@@ -104,14 +91,19 @@
 find . -type d -name "__pycache__" | xargs rm -r
 rm -r .pytest_cache
 rm -r .venv
 ```
 
 
 ### Support
-Please [open an issue](https://github.com/satzbeleg/bool-to-int8-ray/issues/new) for support.
+Please [open an issue](https://github.com/ulf1/bool-to-int8-ray/issues/new) for support.
 
 
 ### Contributing
-Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/satzbeleg/bool-to-int8-ray/compare/).
+Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/ulf1/bool-to-int8-ray/compare/).
 
+### Acknowledgements
+The "Evidence" project was funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) - [433249742](https://gepris.dfg.de/gepris/projekt/433249742) (GU 798/27-1; GE 1119/11-1).
 
+### Maintenance
+- till 31.Aug.2023 (v0.1.1) the code repository was maintained within the DFG project [433249742](https://gepris.dfg.de/gepris/projekt/433249742)
+- since 01.Sep.2023 (v0.2.0) the code repository is maintained by [@ulf1](https://github.com/ulf1).
```

### Comparing `bool-to-int8-ray-0.1.1/bool_to_int8_ray/serialize.py` & `bool-to-int8-ray-0.2.0/bool_to_int8_ray/serialize.py`

 * *Files identical despite different names*

### Comparing `bool-to-int8-ray-0.1.1/bool_to_int8_ray.egg-info/PKG-INFO` & `bool-to-int8-ray-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: bool-to-int8-ray
-Version: 0.1.1
+Version: 0.2.0
 Summary: bool to int8 serialization with ray.io
-Home-page: http://github.com/satzbeleg/bool-to-int8-ray
+Home-page: http://github.com/ulf1/bool-to-int8-ray
 Author: Ulf Hamster
 Author-email: 554c46@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -59,19 +59,19 @@
  2.308446 -- ray.io version, hash to int8
  3.023865 -- ray.io version, int8 to hash
 ```
 
 ## Appendix
 
 ### Installation
-The `bool-to-int8-ray` [git repo](http://github.com/satzbeleg/bool-to-int8-ray) is available as [PyPi package](https://pypi.org/project/bool-to-int8-ray)
+The `bool-to-int8-ray` [git repo](http://github.com/ulf1/bool-to-int8-ray) is available as [PyPi package](https://pypi.org/project/bool-to-int8-ray)
 
 ```sh
 pip install bool-to-int8-ray
-pip install git+ssh://git@github.com/satzbeleg/bool-to-int8-ray.git
+pip install git+ssh://git@github.com/ulf1/bool-to-int8-ray.git
 ```
 
 ### Install a virtual environment
 
 ```sh
 python3 -m venv .venv
 source .venv/bin/activate
@@ -104,14 +104,21 @@
 find . -type d -name "__pycache__" | xargs rm -r
 rm -r .pytest_cache
 rm -r .venv
 ```
 
 
 ### Support
-Please [open an issue](https://github.com/satzbeleg/bool-to-int8-ray/issues/new) for support.
+Please [open an issue](https://github.com/ulf1/bool-to-int8-ray/issues/new) for support.
 
 
 ### Contributing
-Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/satzbeleg/bool-to-int8-ray/compare/).
+Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/ulf1/bool-to-int8-ray/compare/).
+
+### Acknowledgements
+The "Evidence" project was funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) - [433249742](https://gepris.dfg.de/gepris/projekt/433249742) (GU 798/27-1; GE 1119/11-1).
+
+### Maintenance
+- till 31.Aug.2023 (v0.1.1) the code repository was maintained within the DFG project [433249742](https://gepris.dfg.de/gepris/projekt/433249742)
+- since 01.Sep.2023 (v0.2.0) the code repository is maintained by [@ulf1](https://github.com/ulf1).
```

### Comparing `bool-to-int8-ray-0.1.1/setup.py` & `bool-to-int8-ray-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 setuptools.setup(
     name='bool-to-int8-ray',
     version=get_version("bool_to_int8_ray/__init__.py"),
     description='bool to int8 serialization with ray.io',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
-    url='http://github.com/satzbeleg/bool-to-int8-ray',
+    url='http://github.com/ulf1/bool-to-int8-ray',
     author='Ulf Hamster',
     author_email='554c46@gmail.com',
     license='Apache License 2.0',
     packages=['bool_to_int8_ray'],
     install_requires=[
         "numpy>=1.19.5,<2",
         "ray>=2,<3",
```

### Comparing `bool-to-int8-ray-0.1.1/test/speedtest.py` & `bool-to-int8-ray-0.2.0/test/speedtest.py`

 * *Files identical despite different names*

### Comparing `bool-to-int8-ray-0.1.1/test/test_serialize.py` & `bool-to-int8-ray-0.2.0/test/test_serialize.py`

 * *Files identical despite different names*

