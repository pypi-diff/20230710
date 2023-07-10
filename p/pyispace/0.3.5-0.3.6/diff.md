# Comparing `tmp/pyispace-0.3.5.tar.gz` & `tmp/pyispace-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyispace-0.3.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyispace-0.3.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyispace-0.3.5.tar` & `pyispace-0.3.6.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1710 2023-07-07 19:18:02.786790 pyispace-0.3.5/README.md
--rw-r--r--   0        0        0      340 2023-07-07 19:18:02.786790 pyispace-0.3.5/pyispace/__init__.py
--rw-r--r--   0        0        0       70 2023-07-07 19:18:02.786790 pyispace-0.3.5/pyispace/__main__.py
--rw-r--r--   0        0        0     1495 2023-07-07 19:18:02.786790 pyispace-0.3.5/pyispace/cli.py
--rw-r--r--   0        0        0     1171 2023-07-07 19:18:02.787790 pyispace-0.3.5/pyispace/example.py
--rw-r--r--   0        0        0     3382 2023-07-07 19:18:02.787790 pyispace-0.3.5/pyispace/pilot.py
--rw-r--r--   0        0        0      495 2023-07-07 19:18:02.787790 pyispace-0.3.5/pyispace/preprocessing.py
--rw-r--r--   0        0        0    18062 2023-07-07 19:18:02.791790 pyispace-0.3.5/pyispace/trace.py
--rw-r--r--   0        0        0     6482 2023-07-07 19:18:02.791790 pyispace-0.3.5/pyispace/train.py
--rw-r--r--   0        0        0     3414 2023-07-07 19:18:02.791790 pyispace-0.3.5/pyispace/utils.py
--rw-r--r--   0        0        0      948 2023-07-07 19:18:02.791790 pyispace-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     2482 1970-01-01 00:00:00.000000 pyispace-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1710 2023-07-10 13:45:05.361795 pyispace-0.3.6/README.md
+-rw-r--r--   0        0        0      310 2023-07-10 13:45:05.361795 pyispace-0.3.6/options.json
+-rw-r--r--   0        0        0      340 2023-07-10 13:45:05.361795 pyispace-0.3.6/pyispace/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-10 13:45:05.361795 pyispace-0.3.6/pyispace/__main__.py
+-rw-r--r--   0        0        0     1495 2023-07-10 13:45:05.361795 pyispace-0.3.6/pyispace/cli.py
+-rw-r--r--   0        0        0     1171 2023-07-10 13:45:05.361795 pyispace-0.3.6/pyispace/example.py
+-rw-r--r--   0        0        0     3382 2023-07-10 13:45:05.361795 pyispace-0.3.6/pyispace/pilot.py
+-rw-r--r--   0        0        0      495 2023-07-10 13:45:05.361795 pyispace-0.3.6/pyispace/preprocessing.py
+-rw-r--r--   0        0        0    18129 2023-07-10 13:45:05.365795 pyispace-0.3.6/pyispace/trace.py
+-rw-r--r--   0        0        0     6482 2023-07-10 13:45:05.366795 pyispace-0.3.6/pyispace/train.py
+-rw-r--r--   0        0        0     3414 2023-07-10 13:45:05.366795 pyispace-0.3.6/pyispace/utils.py
+-rw-r--r--   0        0        0      975 2023-07-10 13:45:05.366795 pyispace-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     2482 1970-01-01 00:00:00.000000 pyispace-0.3.6/PKG-INFO
```

### Comparing `pyispace-0.3.5/README.md` & `pyispace-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pyispace-0.3.5/pyispace/cli.py` & `pyispace-0.3.6/pyispace/cli.py`

 * *Files identical despite different names*

### Comparing `pyispace-0.3.5/pyispace/example.py` & `pyispace-0.3.6/pyispace/example.py`

 * *Files identical despite different names*

### Comparing `pyispace-0.3.5/pyispace/pilot.py` & `pyispace-0.3.6/pyispace/pilot.py`

 * *Files identical despite different names*

### Comparing `pyispace-0.3.5/pyispace/trace.py` & `pyispace-0.3.6/pyispace/trace.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import time
 import warnings
 from dataclasses import dataclass
 from itertools import repeat
 from math import ceil
 from multiprocessing import Pool, cpu_count
-from typing import List, Union
+from typing import List, Union, Tuple
 
 import alphashape
 import numpy as np
 import pandas as pd
 from scipy.spatial import Delaunay
 from scipy.spatial.qhull import QhullError
 from scipy.special import gamma
@@ -117,15 +117,18 @@
         return 1
     elif pts.type == 'MultiPoint':
         return len(pts.geoms)
     else:
         raise TypeError
 
 
-def inner_intersection(poly: geometry.Polygon, pts: geometry.MultiPoint) -> Union[geometry.Point, geometry.MultiPoint]:
+def inner_intersection(
+        poly: geometry.Polygon,
+        pts: geometry.MultiPoint
+) -> Union[geometry.Point, geometry.MultiPoint]:
     intersec = poly.intersection(pts)
     intersec_bound = poly.boundary.intersection(intersec)
     return intersec.difference(intersec_bound)
 
 
 def copy_polygon(poly: Union[geometry.Polygon, geometry.MultiPolygon]):
     return poly.__class__(poly)
@@ -133,15 +136,20 @@
 
 def estimate_epsilon(x, k):
     m, n = np.shape(x)
     eps = ((np.prod(x.max(axis=0) - x.min(axis=0)) * k * gamma(.5 * n + 1)) / (m * np.sqrt(np.pi ** n))) ** (1 / n)
     return eps
 
 
-def make_summary(space: FootprintOutput, good: List[FootprintOutput], best: List[FootprintOutput], algolabels: List):
+def make_summary(
+        space: FootprintOutput,
+        good: List[FootprintOutput],
+        best: List[FootprintOutput],
+        algolabels: List[str]
+) -> pd.DataFrame:
     assert len(good) == len(best)
     cols = ['Area_Good_Normalized', 'Density_Good_Normalized', 'Purity_Good',
             'Area_Best_Normalized', 'Density_Best_Normalized', 'Purity_Best']
     rows = []
     for i in range(len(good)):
         rows.append([good[i].area / space.area,
                      good[i].density / space.density,
@@ -150,52 +158,56 @@
                      best[i].density / space.density,
                      best[i].purity]
                     )
     summary = pd.DataFrame(rows, index=pd.Index(algolabels, name='Row'), columns=cols)
     return summary
 
 
-def trace(Z: np.ndarray, Ybin: np.ndarray, P: np.ndarray, beta: np.ndarray, algolabels: list, parallel=True, **kwargs):
+def trace(
+        Z: np.ndarray,
+        Ybin: np.ndarray,
+        P: np.ndarray,
+        beta: np.ndarray,
+        algolabels: List[str],
+        parallel: bool = True,
+        **kwargs
+) -> TraceOutput:
     _logger.info("TRACE is calculating the space area and density.")
     ninst = Z.shape[0]
     nalgos = Ybin.shape[1]
     space = trace_build(Z, np.ones(ninst, dtype=bool), kwargs['PI'])
     _logger.debug(f"Space area: {space.area}")
     _logger.debug(f"Space density: {space.density}")
 
     _logger.info("TRACE is calculating the algorithm footprints.")
     if parallel:
         _logger.warning("Some log messages are temporarily disabled in parallel mode. This functionality will be added "
                         "in future versions")
         with Pool(processes=cpu_count()) as pool:
             _logger.info(f"Calculating footprints...")
-            good = pool.starmap_async(trace_build_wrapper,
-                                      zip(repeat(Z), (Ybin[:, i] for i in range(nalgos)), repeat(kwargs['PI'])))
-            best = pool.starmap_async(trace_build_wrapper,
-                                      zip(repeat(Z), (P == i for i in range(nalgos)), repeat(kwargs['PI'])))
+            good = pool.starmap_async(
+                trace_build_wrapper,
+                zip(repeat(Z), (Ybin[:, i] for i in range(nalgos)), repeat(kwargs['PI']))
+            )
+            best = pool.starmap_async(
+                trace_build_wrapper,
+                zip(repeat(Z), (P == i for i in range(nalgos)), repeat(kwargs['PI']))
+            )
             good = good.get()
             best = best.get()
     else:
         good = []
         best = []
         for i in range(nalgos):
             start = time.time()
             _logger.info(f"Good performance footprint for {repr(algolabels[i])}")
-            try:
-                good.append(trace_build(Z, Ybin[:, i], kwargs['PI']))
-            except TraceException as e:
-                good.append(_empty_footprint())
-                _logger.warning(str(e))
+            good.append(trace_build_wrapper(Z, Ybin[:, i], kwargs['PI']))
 
             _logger.info(f"Best performance footprint for {repr(algolabels[i])}")
-            try:
-                best.append(trace_build(Z, P == i, kwargs['PI']))
-            except TraceException as e:
-                good.append(_empty_footprint())
-                _logger.warning(str(e))
+            best.append(trace_build_wrapper(Z, P == i, kwargs['PI']))
 
             end = time.time()
             _logger.debug(f"Algorithm {repr(algolabels[i])} completed. Elapsed time: {(end - start):.2f} s")
 
     _logger.info("TRACE is detecting and removing contradictory sections of the footprints.")
     for i in range(nalgos - 1):
         _logger.debug(f"Base algorithm {repr(algolabels[i])}")
@@ -210,29 +222,34 @@
 
     _logger.info("TRACE is preparing the summary table.")
     summary = make_summary(space, good, best, algolabels)
     _logger.info("TRACE has completed.")
     return TraceOutput(space, good, best, hard, summary)
 
 
-def trace_build_wrapper(*args):
+def trace_build_wrapper(*args) -> FootprintOutput:
     try:
         return trace_build(*args)
     except TraceException:
         return _empty_footprint()
 
 
-def trace_build(Z, Ybin, PI) -> FootprintOutput:
+def trace_build(
+        Z: np.ndarray,
+        Ybin: np.ndarray,
+        PI: float
+) -> FootprintOutput:
     Ig = np.unique(Z[Ybin, :], axis=0)
     if Ig.shape[0] < 3:
         raise TraceException
 
     nn = max(min(ceil(sum(Ybin) / 20), 50), 3)
     eps = estimate_epsilon(Ig, nn)
-    clustering = DBSCAN(eps=eps, min_samples=nn).fit(Ig)
+    clustering = DBSCAN(eps=eps, min_samples=nn)
+    clustering.fit(Ig)
 
     polygon = geometry.Polygon()
     for i in range(np.max(clustering.labels_) + 1):
         polydata = Ig[clustering.labels_ == i, :]
         if polydata.shape[0] < 3:
             continue
 
@@ -257,16 +274,22 @@
         density = elements / area
         purity = good_elements / elements
         return FootprintOutput(polygon, area, elements, good_elements, density, purity)
     else:
         raise TraceException
 
 
-def trace_contra(base: FootprintOutput, test: FootprintOutput, Z: np.ndarray,
-                 Ybase: np.ndarray, Ytest: np.ndarray, *args):
+def trace_contra(
+        base: FootprintOutput,
+        test: FootprintOutput,
+        Z: np.ndarray,
+        Ybase: np.ndarray,
+        Ytest: np.ndarray,
+        *args
+) -> Tuple[FootprintOutput, FootprintOutput]:
     if base.polygon.is_empty or test.polygon.is_empty:
         return base, test
 
     def degenerate(p):
         if not (isinstance(p, geometry.Polygon) or isinstance(p, geometry.MultiPolygon)):
             return True
         else:
```

### Comparing `pyispace-0.3.5/pyispace/train.py` & `pyispace-0.3.6/pyispace/train.py`

 * *Files identical despite different names*

### Comparing `pyispace-0.3.5/pyispace/utils.py` & `pyispace-0.3.6/pyispace/utils.py`

 * *Files identical despite different names*

### Comparing `pyispace-0.3.5/pyproject.toml` & `pyispace-0.3.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -31,8 +31,9 @@
 repository = "https://gitlab.com/ita-ml/pyispace"
 
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.8.0,<4"]
 
 [tool.flit.sdist]
+include = ["options.json"]
 exclude = ["pyispace/tests/", ".pytest_cache/"]
```

### Comparing `pyispace-0.3.5/PKG-INFO` & `pyispace-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyispace
-Version: 0.3.5
+Version: 0.3.6
 Summary: Instance Space Analysis Python package
 Author-email: Pedro Paiva <paiva@ita.br>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

