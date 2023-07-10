# Comparing `tmp/scipy-quadopt-0.1.2.tar.gz` & `tmp/scipy-quadopt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scipy-quadopt-0.1.2.tar", last modified: Wed Apr 28 19:20:14 2021, max compression
+gzip compressed data, was "scipy-quadopt-0.2.0.tar", last modified: Mon Jul 10 15:40:35 2023, max compression
```

## Comparing `scipy-quadopt-0.1.2.tar` & `scipy-quadopt-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2021-04-28 19:20:14.000000 scipy-quadopt-0.1.2/
--rw-r--r--   0 uh         (501) staff       (20)    11341 2021-04-07 10:32:11.000000 scipy-quadopt-0.1.2/LICENSE
--rw-r--r--   0 uh         (501) staff       (20)       46 2021-04-07 10:32:10.000000 scipy-quadopt-0.1.2/MANIFEST.in
--rw-r--r--   0 uh         (501) staff       (20)     5364 2021-04-28 19:20:14.000000 scipy-quadopt-0.1.2/PKG-INFO
--rw-r--r--   0 uh         (501) staff       (20)     3440 2021-04-28 17:17:24.000000 scipy-quadopt-0.1.2/README.md
--rw-r--r--   0 uh         (501) staff       (20)     3885 2021-04-28 19:20:12.000000 scipy-quadopt-0.1.2/README.rst
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2021-04-28 19:20:14.000000 scipy-quadopt-0.1.2/scipy_quadopt/
--rw-r--r--   0 uh         (501) staff       (20)       94 2021-04-28 17:10:53.000000 scipy-quadopt-0.1.2/scipy_quadopt/__init__.py
--rw-r--r--   0 uh         (501) staff       (20)     2091 2021-04-07 17:57:05.000000 scipy-quadopt-0.1.2/scipy_quadopt/problem.py
--rw-r--r--   0 uh         (501) staff       (20)      431 2021-04-07 12:21:00.000000 scipy-quadopt-0.1.2/scipy_quadopt/utils.py
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2021-04-28 19:20:14.000000 scipy-quadopt-0.1.2/scipy_quadopt.egg-info/
--rw-r--r--   0 uh         (501) staff       (20)     5364 2021-04-28 19:20:13.000000 scipy-quadopt-0.1.2/scipy_quadopt.egg-info/PKG-INFO
--rw-r--r--   0 uh         (501) staff       (20)      413 2021-04-28 19:20:13.000000 scipy-quadopt-0.1.2/scipy_quadopt.egg-info/SOURCES.txt
--rw-r--r--   0 uh         (501) staff       (20)        1 2021-04-28 19:20:13.000000 scipy-quadopt-0.1.2/scipy_quadopt.egg-info/dependency_links.txt
--rw-r--r--   0 uh         (501) staff       (20)       49 2021-04-28 19:20:13.000000 scipy-quadopt-0.1.2/scipy_quadopt.egg-info/requires.txt
--rw-r--r--   0 uh         (501) staff       (20)       14 2021-04-28 19:20:13.000000 scipy-quadopt-0.1.2/scipy_quadopt.egg-info/top_level.txt
--rw-r--r--   0 uh         (501) staff       (20)        1 2021-04-28 19:20:13.000000 scipy-quadopt-0.1.2/scipy_quadopt.egg-info/zip-safe
--rw-r--r--   0 uh         (501) staff       (20)       38 2021-04-28 19:20:14.000000 scipy-quadopt-0.1.2/setup.cfg
--rw-r--r--   0 uh         (501) staff       (20)     1132 2021-04-28 17:09:45.000000 scipy-quadopt-0.1.2/setup.py
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2021-04-28 19:20:14.000000 scipy-quadopt-0.1.2/test/
--rw-r--r--   0 uh         (501) staff       (20)        0 2021-04-07 08:39:58.000000 scipy-quadopt-0.1.2/test/__init__.py
--rw-r--r--   0 uh         (501) staff       (20)      822 2021-04-07 15:03:48.000000 scipy-quadopt-0.1.2/test/test_aggregate_matrices.py
--rw-r--r--   0 uh         (501) staff       (20)     1273 2021-04-07 18:04:33.000000 scipy-quadopt-0.1.2/test/test_get_weights.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:40:35.387648 scipy-quadopt-0.2.0/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)    11341 2023-07-10 08:48:11.000000 scipy-quadopt-0.2.0/LICENSE
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       46 2023-07-10 08:48:11.000000 scipy-quadopt-0.2.0/MANIFEST.in
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     3349 2023-07-10 15:40:35.387648 scipy-quadopt-0.2.0/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     2904 2023-07-10 14:52:32.000000 scipy-quadopt-0.2.0/README.md
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:40:35.383648 scipy-quadopt-0.2.0/scipy_quadopt/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       94 2023-07-10 14:25:03.000000 scipy-quadopt-0.2.0/scipy_quadopt/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     2091 2023-07-10 08:48:11.000000 scipy-quadopt-0.2.0/scipy_quadopt/problem.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      431 2023-07-10 08:48:11.000000 scipy-quadopt-0.2.0/scipy_quadopt/utils.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:40:35.387648 scipy-quadopt-0.2.0/scipy_quadopt.egg-info/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     3349 2023-07-10 15:40:35.000000 scipy-quadopt-0.2.0/scipy_quadopt.egg-info/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      402 2023-07-10 15:40:35.000000 scipy-quadopt-0.2.0/scipy_quadopt.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-10 15:40:35.000000 scipy-quadopt-0.2.0/scipy_quadopt.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       49 2023-07-10 15:40:35.000000 scipy-quadopt-0.2.0/scipy_quadopt.egg-info/requires.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       14 2023-07-10 15:40:35.000000 scipy-quadopt-0.2.0/scipy_quadopt.egg-info/top_level.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-10 15:40:35.000000 scipy-quadopt-0.2.0/scipy_quadopt.egg-info/zip-safe
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       38 2023-07-10 15:40:35.387648 scipy-quadopt-0.2.0/setup.cfg
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     1177 2023-07-10 14:25:03.000000 scipy-quadopt-0.2.0/setup.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:40:35.387648 scipy-quadopt-0.2.0/test/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        0 2023-07-10 08:48:11.000000 scipy-quadopt-0.2.0/test/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      822 2023-07-10 08:48:11.000000 scipy-quadopt-0.2.0/test/test_aggregate_matrices.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     1273 2023-07-10 08:48:11.000000 scipy-quadopt-0.2.0/test/test_get_weights.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scipy-quadopt-0.1.2/LICENSE` & `scipy-quadopt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scipy-quadopt-0.1.2/README.md` & `scipy-quadopt-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 [![PyPI version](https://badge.fury.io/py/scipy-quadopt.svg)](https://badge.fury.io/py/scipy-quadopt)
+[![PyPi downloads](https://img.shields.io/pypi/dm/scipy-quadopt)](https://img.shields.io/pypi/dm/scipy-quadopt)
 [![DOI](https://zenodo.org/badge/355471428.svg)](https://zenodo.org/badge/latestdoi/355471428)
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/satzbeleg/scipy-quadopt.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/satzbeleg/scipy-quadopt/alerts/)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/satzbeleg/scipy-quadopt.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/satzbeleg/scipy-quadopt/context:python)
-[![deepcode](https://www.deepcode.ai/api/gh/badge?key=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJwbGF0Zm9ybTEiOiJnaCIsIm93bmVyMSI6InNhdHpiZWxlZyIsInJlcG8xIjoic2NpcHktcXVhZG9wdCIsImluY2x1ZGVMaW50IjpmYWxzZSwiYXV0aG9ySWQiOjI5NDUyLCJpYXQiOjE2MTk2Mjk4Nzd9.-Vgd3-HgM72l4K7DXLCrnNnxX11tzO7Qp23c7zMl3Zo)](https://www.deepcode.ai/app/gh/satzbeleg/scipy-quadopt/_/dashboard?utm_content=gh%2Fsatzbeleg%2Fscipy-quadopt)
-[![scipy-quadopt](https://snyk.io/advisor/python/scipy-quadopt/badge.svg)](https://snyk.io/advisor/python/scipy-quadopt)
 
-# scipy-quadopt
+# scipy-quadopt: Quadratic optimization with constraints and upper boundaries
 Wrapper and utility functions to apply scipy's SLSQP algorithm to quadratic optimization problems with resource constraints and upper boundaries.
 
 ## Usage
 
 ```py
 import numpy as np
 import scipy_quadopt as sqp
@@ -41,19 +38,19 @@
 simi = sqp.aggregate_matrices(simi_1, beta_1, simi_2, beta_2)
 weights, _ = sqp.get_weights(good, simi, lam)
 ```
 
 ## Appendix
 
 ### Installation
-The `scipy-quadopt` [git repo](http://github.com/satzbeleg/scipy-quadopt) is available as [PyPi package](https://pypi.org/project/scipy-quadopt)
+The `scipy-quadopt` [git repo](http://github.com/ulf1/scipy-quadopt) is available as [PyPi package](https://pypi.org/project/scipy-quadopt)
 
 ```
 pip install scipy-quadopt
-pip install git+ssh://git@github.com/satzbeleg/scipy-quadopt.git
+pip install git+ssh://git@github.com/ulf1/scipy-quadopt.git
 ```
 
 ### Install a virtual environment
 
 ```
 python3 -m venv .venv
 source .venv/bin/activate
@@ -69,15 +66,14 @@
 * Jupyter for the examples: `jupyter lab`
 * Check syntax: `flake8 --ignore=F401 --exclude=$(grep -v '^#' .gitignore | xargs | sed -e 's/ /,/g')`
 * Run Unit Tests: `PYTHONPATH=. pytest`
 
 Publish
 
 ```sh
-pandoc README.md --from markdown --to rst -s -o README.rst
 python setup.py sdist 
 twine upload -r pypi dist/*
 ```
 
 ### Clean up 
 
 ```
@@ -85,16 +81,20 @@
 find . -type d -name "__pycache__" | xargs rm -r
 rm -r .pytest_cache
 rm -r .venv
 ```
 
 
 ### Support
-Please [open an issue](https://github.com/satzbeleg/scipy-quadopt/issues/new) for support.
+Please [open an issue](https://github.com/ulf1/scipy-quadopt/issues/new) for support.
 
 
 ### Contributing
-Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/satzbeleg/scipy-quadopt/compare/).
+Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/ulf1/scipy-quadopt/compare/).
 
 
 ### Acknowledgements
-This work was funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) - [433249742](https://gepris.dfg.de/gepris/projekt/433249742). Project duration: 2020-2023.
+The "Evidence" project was funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) - [433249742](https://gepris.dfg.de/gepris/projekt/433249742) (GU 798/27-1; GE 1119/11-1).
+
+### Maintenance
+- till 31.Aug.2023 (v0.1.2) the code repository was maintained within the DFG project [433249742](https://gepris.dfg.de/gepris/projekt/433249742)
+- since 01.Sep.2023 (v0.2.0) the code repository is maintained by Ulf Hamster.
```

### Comparing `scipy-quadopt-0.1.2/scipy_quadopt/problem.py` & `scipy-quadopt-0.2.0/scipy_quadopt/problem.py`

 * *Files identical despite different names*

### Comparing `scipy-quadopt-0.1.2/setup.py` & `scipy-quadopt-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,16 +21,17 @@
 setuptools.setup(
     name='scipy-quadopt',
     version=get_version("scipy_quadopt/__init__.py"),
     description=(
         "Wrapper and utility functions to apply scipy's SLSQP algorithm "
         "to quadratic optimization problems with resource constraints and "
         "upper boundaries."),
-    long_description=read('README.rst'),
-    url='http://github.com/satzbeleg/scipy-quadopt',
+    long_description=read('README.md'),
+    long_description_content_type='text/markdown',
+    url='http://github.com/ulf1/scipy-quadopt',
     author='Ulf Hamster',
     author_email='554c46@gmail.com',
     license='Apache License 2.0',
     packages=['scipy_quadopt'],
     install_requires=[
         'setuptools>=40.0.0',
         'numpy>=1.19.5',
```

### Comparing `scipy-quadopt-0.1.2/test/test_aggregate_matrices.py` & `scipy-quadopt-0.2.0/test/test_aggregate_matrices.py`

 * *Files identical despite different names*

### Comparing `scipy-quadopt-0.1.2/test/test_get_weights.py` & `scipy-quadopt-0.2.0/test/test_get_weights.py`

 * *Files identical despite different names*

