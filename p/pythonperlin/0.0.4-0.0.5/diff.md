# Comparing `tmp/pythonperlin-0.0.4.tar.gz` & `tmp/pythonperlin-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonperlin-0.0.4.tar", last modified: Sun Jul  9 20:27:08 2023, max compression
+gzip compressed data, was "pythonperlin-0.0.5.tar", last modified: Mon Jul 10 14:35:49 2023, max compression
```

## Comparing `pythonperlin-0.0.4.tar` & `pythonperlin-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-09 20:27:08.460412 pythonperlin-0.0.4/
--rw-r--r--   0 timpyrkov   (501) staff       (20)     1067 2022-11-01 23:50:58.000000 pythonperlin-0.0.4/LICENSE
--rw-r--r--   0 timpyrkov   (501) staff       (20)     4955 2023-07-09 20:27:08.460301 pythonperlin-0.0.4/PKG-INFO
--rw-r--r--   0 timpyrkov   (501) staff       (20)     4459 2023-07-09 20:22:37.000000 pythonperlin-0.0.4/README.md
-drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-09 20:27:08.459393 pythonperlin-0.0.4/pythonperlin/
--rw-r--r--   0 timpyrkov   (501) staff       (20)      162 2022-11-01 23:50:58.000000 pythonperlin-0.0.4/pythonperlin/__init__.py
--rw-r--r--   0 timpyrkov   (501) staff       (20)     8254 2023-07-09 20:18:56.000000 pythonperlin-0.0.4/pythonperlin/perlin.py
-drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-09 20:27:08.460130 pythonperlin-0.0.4/pythonperlin.egg-info/
--rw-r--r--   0 timpyrkov   (501) staff       (20)     4955 2023-07-09 20:27:08.000000 pythonperlin-0.0.4/pythonperlin.egg-info/PKG-INFO
--rw-r--r--   0 timpyrkov   (501) staff       (20)      253 2023-07-09 20:27:08.000000 pythonperlin-0.0.4/pythonperlin.egg-info/SOURCES.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)        1 2023-07-09 20:27:08.000000 pythonperlin-0.0.4/pythonperlin.egg-info/dependency_links.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)        6 2023-07-09 20:27:08.000000 pythonperlin-0.0.4/pythonperlin.egg-info/requires.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)       13 2023-07-09 20:27:08.000000 pythonperlin-0.0.4/pythonperlin.egg-info/top_level.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)       38 2023-07-09 20:27:08.460454 pythonperlin-0.0.4/setup.cfg
--rw-r--r--   0 timpyrkov   (501) staff       (20)      832 2023-07-09 20:19:35.000000 pythonperlin-0.0.4/setup.py
+drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-10 14:35:49.282590 pythonperlin-0.0.5/
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     1067 2022-11-01 23:50:58.000000 pythonperlin-0.0.5/LICENSE
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     5144 2023-07-10 14:35:49.282478 pythonperlin-0.0.5/PKG-INFO
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     4648 2023-07-10 14:34:06.000000 pythonperlin-0.0.5/README.md
+drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-10 14:35:49.281506 pythonperlin-0.0.5/pythonperlin/
+-rw-r--r--   0 timpyrkov   (501) staff       (20)      170 2023-07-10 14:16:25.000000 pythonperlin-0.0.5/pythonperlin/__init__.py
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     8254 2023-07-09 20:18:56.000000 pythonperlin-0.0.5/pythonperlin/perlin.py
+drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-10 14:35:49.282332 pythonperlin-0.0.5/pythonperlin.egg-info/
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     5144 2023-07-10 14:35:48.000000 pythonperlin-0.0.5/pythonperlin.egg-info/PKG-INFO
+-rw-r--r--   0 timpyrkov   (501) staff       (20)      253 2023-07-10 14:35:49.000000 pythonperlin-0.0.5/pythonperlin.egg-info/SOURCES.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)        1 2023-07-10 14:35:49.000000 pythonperlin-0.0.5/pythonperlin.egg-info/dependency_links.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)        6 2023-07-10 14:35:49.000000 pythonperlin-0.0.5/pythonperlin.egg-info/requires.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)       13 2023-07-10 14:35:49.000000 pythonperlin-0.0.5/pythonperlin.egg-info/top_level.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)       38 2023-07-10 14:35:49.282627 pythonperlin-0.0.5/setup.cfg
+-rw-r--r--   0 timpyrkov   (501) staff       (20)      832 2023-07-10 14:16:51.000000 pythonperlin-0.0.5/setup.py
```

### Comparing `pythonperlin-0.0.4/LICENSE` & `pythonperlin-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pythonperlin-0.0.4/PKG-INFO` & `pythonperlin-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonperlin
-Version: 0.0.4
+Version: 0.0.5
 Summary: Perlin noise in python - seamlessly tile in any dimensions
 Home-page: https://github.com/timpyrkov/pythonperlin
 Author: Tim Pyrkov
 Author-email: tim.pyrkov@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,14 +17,17 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/pythonperlin?style=plastic)](https://pypi.org/project/pythonperlin/)
 [![PyPI](https://img.shields.io/pypi/v/pythonperlin?style=plastic)](https://pypi.org/project/pythonperlin/)
 [![License](https://img.shields.io/pypi/l/pythonperlin?style=plastic)](https://opensource.org/licenses/MIT)
 [![Documentation Status](https://readthedocs.org/projects/pythonperlin/badge/?version=latest)](https://pythonperlin.readthedocs.io/en/latest/?badge=latest)
 
 # PythonPerlin
 ## Perlin noise in python -- procedural generative art tool to seamlessly tile texture patterns in any dimensions
+<br>
+
+## In 1997 professor Ken Perlin won an Oscar for Technical Achievement from the Academy of Motion Picture Arts and Sciences for his invention of Perlin noise for the Tron 1982 movie.
 #
 
 
 # Installation
 ```
 pip install pythonperlin
 ```
```

### Comparing `pythonperlin-0.0.4/README.md` & `pythonperlin-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/pythonperlin?style=plastic)](https://pypi.org/project/pythonperlin/)
 [![PyPI](https://img.shields.io/pypi/v/pythonperlin?style=plastic)](https://pypi.org/project/pythonperlin/)
 [![License](https://img.shields.io/pypi/l/pythonperlin?style=plastic)](https://opensource.org/licenses/MIT)
 [![Documentation Status](https://readthedocs.org/projects/pythonperlin/badge/?version=latest)](https://pythonperlin.readthedocs.io/en/latest/?badge=latest)
 
 # PythonPerlin
 ## Perlin noise in python -- procedural generative art tool to seamlessly tile texture patterns in any dimensions
+<br>
+
+## In 1997 professor Ken Perlin won an Oscar for Technical Achievement from the Academy of Motion Picture Arts and Sciences for his invention of Perlin noise for the Tron 1982 movie.
 #
 
 
 # Installation
 ```
 pip install pythonperlin
 ```
```

### Comparing `pythonperlin-0.0.4/pythonperlin/perlin.py` & `pythonperlin-0.0.5/pythonperlin/perlin.py`

 * *Files identical despite different names*

### Comparing `pythonperlin-0.0.4/pythonperlin.egg-info/PKG-INFO` & `pythonperlin-0.0.5/pythonperlin.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonperlin
-Version: 0.0.4
+Version: 0.0.5
 Summary: Perlin noise in python - seamlessly tile in any dimensions
 Home-page: https://github.com/timpyrkov/pythonperlin
 Author: Tim Pyrkov
 Author-email: tim.pyrkov@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,14 +17,17 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/pythonperlin?style=plastic)](https://pypi.org/project/pythonperlin/)
 [![PyPI](https://img.shields.io/pypi/v/pythonperlin?style=plastic)](https://pypi.org/project/pythonperlin/)
 [![License](https://img.shields.io/pypi/l/pythonperlin?style=plastic)](https://opensource.org/licenses/MIT)
 [![Documentation Status](https://readthedocs.org/projects/pythonperlin/badge/?version=latest)](https://pythonperlin.readthedocs.io/en/latest/?badge=latest)
 
 # PythonPerlin
 ## Perlin noise in python -- procedural generative art tool to seamlessly tile texture patterns in any dimensions
+<br>
+
+## In 1997 professor Ken Perlin won an Oscar for Technical Achievement from the Academy of Motion Picture Arts and Sciences for his invention of Perlin noise for the Tron 1982 movie.
 #
 
 
 # Installation
 ```
 pip install pythonperlin
 ```
```

### Comparing `pythonperlin-0.0.4/setup.py` & `pythonperlin-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name="pythonperlin",
-    version="0.0.4",
+    version="0.0.5",
     author="Tim Pyrkov",
     author_email="tim.pyrkov@gmail.com",
     description="Perlin noise in python - seamlessly tile in any dimensions",
     long_description=read("README.md"),
     license = "MIT License",
     long_description_content_type="text/markdown",
     url="https://github.com/timpyrkov/pythonperlin",
```

