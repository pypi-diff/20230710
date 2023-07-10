# Comparing `tmp/pyispace-0.3.6.tar.gz` & `tmp/pyispace-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyispace-0.3.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyispace-0.3.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyispace-0.3.6.tar` & `pyispace-0.3.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1710 2023-07-10 13:45:05.361795 pyispace-0.3.6/README.md
--rw-r--r--   0        0        0      310 2023-07-10 13:45:05.361795 pyispace-0.3.6/options.json
--rw-r--r--   0        0        0      340 2023-07-10 13:45:05.361795 pyispace-0.3.6/pyispace/__init__.py
--rw-r--r--   0        0        0       70 2023-07-10 13:45:05.361795 pyispace-0.3.6/pyispace/__main__.py
--rw-r--r--   0        0        0     1495 2023-07-10 13:45:05.361795 pyispace-0.3.6/pyispace/cli.py
--rw-r--r--   0        0        0     1171 2023-07-10 13:45:05.361795 pyispace-0.3.6/pyispace/example.py
--rw-r--r--   0        0        0     3382 2023-07-10 13:45:05.361795 pyispace-0.3.6/pyispace/pilot.py
--rw-r--r--   0        0        0      495 2023-07-10 13:45:05.361795 pyispace-0.3.6/pyispace/preprocessing.py
--rw-r--r--   0        0        0    18129 2023-07-10 13:45:05.365795 pyispace-0.3.6/pyispace/trace.py
--rw-r--r--   0        0        0     6482 2023-07-10 13:45:05.366795 pyispace-0.3.6/pyispace/train.py
--rw-r--r--   0        0        0     3414 2023-07-10 13:45:05.366795 pyispace-0.3.6/pyispace/utils.py
--rw-r--r--   0        0        0      975 2023-07-10 13:45:05.366795 pyispace-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     2482 1970-01-01 00:00:00.000000 pyispace-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1710 2023-07-10 15:19:29.222436 pyispace-0.3.7/README.md
+-rw-r--r--   0        0        0      310 2023-07-10 15:19:29.222436 pyispace-0.3.7/options.json
+-rw-r--r--   0        0        0      340 2023-07-10 15:19:29.222436 pyispace-0.3.7/pyispace/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-10 15:19:29.222436 pyispace-0.3.7/pyispace/__main__.py
+-rw-r--r--   0        0        0     1495 2023-07-10 15:19:29.222436 pyispace-0.3.7/pyispace/cli.py
+-rw-r--r--   0        0        0     1171 2023-07-10 15:19:29.222436 pyispace-0.3.7/pyispace/example.py
+-rw-r--r--   0        0        0     3382 2023-07-10 15:19:29.222436 pyispace-0.3.7/pyispace/pilot.py
+-rw-r--r--   0        0        0      495 2023-07-10 15:19:29.222436 pyispace-0.3.7/pyispace/preprocessing.py
+-rw-r--r--   0        0        0    18078 2023-07-10 15:19:29.226436 pyispace-0.3.7/pyispace/trace.py
+-rw-r--r--   0        0        0     6482 2023-07-10 15:19:29.226436 pyispace-0.3.7/pyispace/train.py
+-rw-r--r--   0        0        0     3414 2023-07-10 15:19:29.226436 pyispace-0.3.7/pyispace/utils.py
+-rw-r--r--   0        0        0      996 2023-07-10 15:19:29.226436 pyispace-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     2511 1970-01-01 00:00:00.000000 pyispace-0.3.7/PKG-INFO
```

### Comparing `pyispace-0.3.6/README.md` & `pyispace-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pyispace-0.3.6/pyispace/cli.py` & `pyispace-0.3.7/pyispace/cli.py`

 * *Files identical despite different names*

### Comparing `pyispace-0.3.6/pyispace/example.py` & `pyispace-0.3.7/pyispace/example.py`

 * *Files identical despite different names*

### Comparing `pyispace-0.3.6/pyispace/pilot.py` & `pyispace-0.3.7/pyispace/pilot.py`

 * *Files identical despite different names*

### Comparing `pyispace-0.3.6/pyispace/trace.py` & `pyispace-0.3.7/pyispace/trace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
 import time
 import warnings
 from dataclasses import dataclass
-from itertools import repeat
 from math import ceil
-from multiprocessing import Pool, cpu_count
+from multiprocessing import cpu_count
 from typing import List, Union, Tuple
 
 import alphashape
 import numpy as np
 import pandas as pd
+from joblib import Parallel, delayed
 from scipy.spatial import Delaunay
 from scipy.spatial.qhull import QhullError
 from scipy.special import gamma
 from shapely import geometry
 from shapely.ops import polygonize, triangulate, unary_union
 from sklearn.cluster import DBSCAN
 
@@ -178,26 +178,30 @@
     _logger.debug(f"Space area: {space.area}")
     _logger.debug(f"Space density: {space.density}")
 
     _logger.info("TRACE is calculating the algorithm footprints.")
     if parallel:
         _logger.warning("Some log messages are temporarily disabled in parallel mode. This functionality will be added "
                         "in future versions")
-        with Pool(processes=cpu_count()) as pool:
-            _logger.info(f"Calculating footprints...")
-            good = pool.starmap_async(
-                trace_build_wrapper,
-                zip(repeat(Z), (Ybin[:, i] for i in range(nalgos)), repeat(kwargs['PI']))
-            )
-            best = pool.starmap_async(
-                trace_build_wrapper,
-                zip(repeat(Z), (P == i for i in range(nalgos)), repeat(kwargs['PI']))
-            )
-            good = good.get()
-            best = best.get()
+        _logger.info(f"Calculating footprints...")
+
+        good = Parallel(n_jobs=cpu_count())(
+            delayed(trace_build_wrapper)(
+                Z,
+                Ybin[:, i],
+                kwargs['PI']
+            ) for i in range(nalgos)
+        )
+        best = Parallel(n_jobs=cpu_count())(
+            delayed(trace_build_wrapper)(
+                Z,
+                P == i,
+                kwargs['PI']
+            ) for i in range(nalgos)
+        )
     else:
         good = []
         best = []
         for i in range(nalgos):
             start = time.time()
             _logger.info(f"Good performance footprint for {repr(algolabels[i])}")
             good.append(trace_build_wrapper(Z, Ybin[:, i], kwargs['PI']))
```

### Comparing `pyispace-0.3.6/pyispace/train.py` & `pyispace-0.3.7/pyispace/train.py`

 * *Files identical despite different names*

### Comparing `pyispace-0.3.6/pyispace/utils.py` & `pyispace-0.3.7/pyispace/utils.py`

 * *Files identical despite different names*

### Comparing `pyispace-0.3.6/pyproject.toml` & `pyispace-0.3.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 dynamic = ["version"]
 dependencies = [
     "numpy>=1.18.5",
     "scipy>=1.9.0",
     "scikit-learn>=0.23.1",
     "shapely~=1.8.0",
     "pandas>=1.1",
-    "alphashape>=1.3.1"
+    "alphashape>=1.3.1",
+    "joblib>=1.3.0"
 ]
 
 [project.scripts]
 isa = "pyispace.cli:main"
 
 [project.urls]
 repository = "https://gitlab.com/ita-ml/pyispace"
```

### Comparing `pyispace-0.3.6/PKG-INFO` & `pyispace-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyispace
-Version: 0.3.6
+Version: 0.3.7
 Summary: Instance Space Analysis Python package
 Author-email: Pedro Paiva <paiva@ita.br>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Classifier: Intended Audience :: Science/Research
 Requires-Dist: numpy>=1.18.5
 Requires-Dist: scipy>=1.9.0
 Requires-Dist: scikit-learn>=0.23.1
 Requires-Dist: shapely~=1.8.0
 Requires-Dist: pandas>=1.1
 Requires-Dist: alphashape>=1.3.1
+Requires-Dist: joblib>=1.3.0
 Project-URL: repository, https://gitlab.com/ita-ml/pyispace
 
 # PyISpace
 
 _Python Instance Space Analysis Toolkit_
 
 <!--![picture](docs/img/circle-fs.png)-->
```

