# Comparing `tmp/antimeridian-0.3.0.tar.gz` & `tmp/antimeridian-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antimeridian-0.3.0.tar", last modified: Thu Jun 29 13:43:08 2023, max compression
+gzip compressed data, was "antimeridian-0.3.1.tar", last modified: Mon Jul 10 14:54:18 2023, max compression
```

## Comparing `antimeridian-0.3.0.tar` & `antimeridian-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:43:08.762039 antimeridian-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-06-29 13:42:59.000000 antimeridian-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-29 13:43:08.762039 antimeridian-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-29 13:42:59.000000 antimeridian-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-29 13:42:59.000000 antimeridian-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:43:08.762039 antimeridian-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:43:08.754038 antimeridian-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:43:08.758039 antimeridian-0.3.0/src/antimeridian/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-29 13:42:59.000000 antimeridian-0.3.0/src/antimeridian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-29 13:42:59.000000 antimeridian-0.3.0/src/antimeridian/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    20697 2023-06-29 13:42:59.000000 antimeridian-0.3.0/src/antimeridian/_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:43:08.758039 antimeridian-0.3.0/src/antimeridian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-29 13:43:08.000000 antimeridian-0.3.0/src/antimeridian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-29 13:43:08.000000 antimeridian-0.3.0/src/antimeridian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:43:08.000000 antimeridian-0.3.0/src/antimeridian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-29 13:43:08.000000 antimeridian-0.3.0/src/antimeridian.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-29 13:43:08.000000 antimeridian-0.3.0/src/antimeridian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 13:43:08.000000 antimeridian-0.3.0/src/antimeridian.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:43:08.758039 antimeridian-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-29 13:42:59.000000 antimeridian-0.3.0/tests/test_bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-29 13:42:59.000000 antimeridian-0.3.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-29 13:42:59.000000 antimeridian-0.3.0/tests/test_geojson.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-29 13:42:59.000000 antimeridian-0.3.0/tests/test_multi_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-29 13:42:59.000000 antimeridian-0.3.0/tests/test_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-29 13:42:59.000000 antimeridian-0.3.0/tests/test_segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:54:18.276951 antimeridian-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-07-10 14:54:07.000000 antimeridian-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-10 14:54:18.272951 antimeridian-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-10 14:54:07.000000 antimeridian-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-10 14:54:07.000000 antimeridian-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 14:54:18.276951 antimeridian-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:54:18.272951 antimeridian-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:54:18.272951 antimeridian-0.3.1/src/antimeridian/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-10 14:54:07.000000 antimeridian-0.3.1/src/antimeridian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-10 14:54:07.000000 antimeridian-0.3.1/src/antimeridian/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22858 2023-07-10 14:54:07.000000 antimeridian-0.3.1/src/antimeridian/_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:54:18.272951 antimeridian-0.3.1/src/antimeridian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-10 14:54:18.000000 antimeridian-0.3.1/src/antimeridian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-10 14:54:18.000000 antimeridian-0.3.1/src/antimeridian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:54:18.000000 antimeridian-0.3.1/src/antimeridian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-10 14:54:18.000000 antimeridian-0.3.1/src/antimeridian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-10 14:54:18.000000 antimeridian-0.3.1/src/antimeridian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 14:54:18.000000 antimeridian-0.3.1/src/antimeridian.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:54:18.272951 antimeridian-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-10 14:54:07.000000 antimeridian-0.3.1/tests/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-10 14:54:07.000000 antimeridian-0.3.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-10 14:54:07.000000 antimeridian-0.3.1/tests/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-10 14:54:07.000000 antimeridian-0.3.1/tests/test_line_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-10 14:54:07.000000 antimeridian-0.3.1/tests/test_multi_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-10 14:54:07.000000 antimeridian-0.3.1/tests/test_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-10 14:54:07.000000 antimeridian-0.3.1/tests/test_segment.py
```

### Comparing `antimeridian-0.3.0/LICENSE` & `antimeridian-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antimeridian-0.3.0/PKG-INFO` & `antimeridian-0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,23 @@
-Metadata-Version: 2.1
-Name: antimeridian
-Version: 0.3.0
-Summary: Fix GeoJSON geometries that cross the antimeridian
-Author-email: Pete Gadomski <pete.gadomski@gmail.com>
-License: Apache-2.0
-Project-URL: documentation, https://antimeridian.readthedocs.io
-Project-URL: repository, https://github.com/gadomski/antimeridan
-Project-URL: changelog, https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md
-Keywords: geojson,antimeridian,shapely
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: cli
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE
-
 # antimeridian
 
 [![CI Status](https://img.shields.io/github/actions/workflow/status/gadomski/antimeridian/ci.yaml?style=for-the-badge&label=CI)](https://github.com/gadomski/antimeridian/actions/workflows/ci.yaml)
 [![Read the Docs](https://img.shields.io/readthedocs/antimeridian?style=for-the-badge)](https://antimeridian.readthedocs.io/en/stable/)
 [![PyPI](https://img.shields.io/pypi/v/antimeridian?style=for-the-badge)](https://pypi.org/project/antimeridian/)
 
 [![GitHub](https://img.shields.io/github/license/gadomski/antimeridian?style=for-the-badge)](https://github.com/gadomski/antimeridian/blob/main/LICENSE)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg?style=for-the-badge)](https://github.com/gadomski/antimeridian/blob/main/CODE_OF_CONDUCT)
 
-Fix polygons that cross the antimeridian.
+Fix shapes that cross the antimeridian.
 See [the documentation](https://antimeridian.readthedocs.io) for information about the underlying algorithm.
-Depends on [shapely](https://shapely.readthedocs.io).
+Depends on [shapely](https://shapely.readthedocs.io) and [numpy](https://numpy.org/).
 
 Can fix:
 
-- Shapely [`Polygon`](https://shapely.readthedocs.io/en/stable/reference/shapely.Polygon.html#shapely.Polygon) and [`MultiPolygon`](https://shapely.readthedocs.io/en/stable/reference/shapely.MultiPolygon.html#shapely.MultiPolygon) objects
+- Shapely [`Polygon`](https://shapely.readthedocs.io/en/stable/reference/shapely.Polygon.html#shapely.Polygon), [`MultiPolygon`](https://shapely.readthedocs.io/en/stable/reference/shapely.MultiPolygon.html#shapely.MultiPolygon), [`LineString`](https://shapely.readthedocs.io/en/stable/reference/shapely.LineString.html#shapely.LineString), and [`MultiLineString`](https://shapely.readthedocs.io/en/stable/reference/shapely.MultiLineString.html#shapely.MultiLineString) objects
 - GeoJSON [Polygons](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.6), [MultiPolygons](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.7), [Features](https://datatracker.ietf.org/doc/html/rfc7946#section-3.2) and [FeatureCollections](https://datatracker.ietf.org/doc/html/rfc7946#section-3.3), as dictionaries
 - Anything that has a [`__geo_interface__`](https://gist.github.com/sgillies/2217756)
 
 ## Usage
 
 ```shell
 pip install antimeridian
```

### Comparing `antimeridian-0.3.0/pyproject.toml` & `antimeridian-0.3.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [project]
 name = "antimeridian"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
     {name = "Pete Gadomski", email = "pete.gadomski@gmail.com"}
 ]
 description = "Fix GeoJSON geometries that cross the antimeridian"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["geojson", "antimeridian", "shapely"]
 license = {text = "Apache-2.0"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
 ]
 dependencies = [
-    "shapely>=2.0"
+    "numpy>=1.17.4",
+    "shapely>=2.0",
 ]
 
 [project.urls]
 documentation = "https://antimeridian.readthedocs.io"
 repository = "https://github.com/gadomski/antimeridan"
 changelog = "https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md"
 
@@ -31,15 +32,16 @@
     "blacken-docs~=1.13",
     "mypy~=1.2",
     "packaging~=23.1",
     "pre-commit~=3.2",
     "pytest~=7.3",
     "pytest-console-scripts~=1.3",
     "ruff==0.0.275",
-    "tomli~=2.0; python_version<'3.11'"
+    "tomli~=2.0; python_version<'3.11'",
+    "typing_extensions; python_version<'3.10'",
 ]
 docs = [
     "cartopy~=0.21",
     "ipykernel~=6.22",
     "jupytext~=1.14",
     "nbsphinx~=0.9",
     "pydata-sphinx-theme~=0.13",
@@ -47,19 +49,22 @@
     "sphinx~=7.0",
     "sphinx-click~=4.4",
 ]
 
 [project.scripts]
 antimeridian = "antimeridian._cli:cli"
 
-[tool.ruff]
-select = ["F", "E", "W", "I", "ERA", "RUF"]
-
 [tool.mypy]
 strict = true
 
 [[tool.mypy.overrides]]
 module = ["shapely", "shapely.geometry"]
 ignore_missing_imports = true
 
+[tool.pytest.ini_options]
+filterwarnings = ["error"]
+
+[tool.ruff]
+select = ["F", "E", "W", "I", "ERA", "RUF"]
+
 [build-system]
 requires = ["setuptools >= 64"]
```

### Comparing `antimeridian-0.3.0/src/antimeridian/_cli.py` & `antimeridian-0.3.1/src/antimeridian/_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import fileinput
+
 try:
     import click
 except ImportError:
     import sys
 
     print(
         """"The `antimeridian` command line interface depends on the click package.
@@ -53,20 +55,23 @@
     ),
 )
 def fix(
     infile: str, force_north_pole: bool, force_south_pole: bool, fix_winding: bool
 ) -> None:
     """Fixes any antimeridian problems a GeoJSON file
 
-    Writes the fixed GeoJSON to standard output.
+    Writes the fixed GeoJSON to standard output. If the filename is ``-`` the
+    input GeoJSON is read from standard input.
     """
-    with open(infile) as f:
-        data = json.load(f)
+    data = ""
+    with fileinput.input(infile) as f:
+        for line in f:
+            data += line + "\n"
     fixed = antimeridian.fix_geojson(
-        data,
+        json.loads(data),
         force_north_pole=force_north_pole,
         force_south_pole=force_south_pole,
         fix_winding=fix_winding,
     )
     print(json.dumps(fixed))
```

### Comparing `antimeridian-0.3.0/src/antimeridian/_implementation.py` & `antimeridian-0.3.1/src/antimeridian/_implementation.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,24 @@
 
 from __future__ import annotations
 
 import copy
 import warnings
 from typing import Any, Dict, List, Optional, Protocol, Tuple, Union, cast
 
+import numpy
 import shapely
 import shapely.geometry
-from shapely.geometry import LinearRing, MultiLineString, MultiPolygon, Polygon
+from shapely.geometry import (
+    LinearRing,
+    LineString,
+    MultiLineString,
+    MultiPolygon,
+    Polygon,
+)
 
 Point = Tuple[float, float]
 
 
 class AntimeridianWarning(UserWarning):
     """Base class for all package-specific warnings."""
 
@@ -158,17 +165,17 @@
 ) -> Dict[str, Any]:
     """Fixes a shape that crosses the antimeridian.
 
     See :py:func:`fix_polygon` for a description of the ``force_north_pole``,
     ``force_south_pole``, and ``fix_winding`` arguments.
 
     Args:
-        shape: A polygon or multi-polygon, either as a dictionary or as a
-            :py:class:`GeoInterface`. Uses :py:func:`shapely.geometry.shape`
-            under the hood.
+        shape: A polygon, multi-polygon, line string, or multi-line string,
+            either as a dictionary or as a :py:class:`GeoInterface`. Uses
+            :py:func:`shapely.geometry.shape` under the hood.
         force_north_pole: If the polygon crosses the antimeridian, force the
             joined segments to enclose the north pole.
         force_south_pole: If the polygon crosses the antimeridian, force the
             joined segments to enclose the south pole.
         fix_winding: If the polygon is wound clockwise, reverse its
             coordinates before applying the algorithm.
 
@@ -196,14 +203,20 @@
                     geom,
                     force_north_pole=force_north_pole,
                     force_south_pole=force_south_pole,
                     fix_winding=fix_winding,
                 )
             ),
         )
+    elif geom.geom_type == "LineString":
+        return cast(Dict[str, Any], shapely.geometry.mapping(fix_line_string(geom)))
+    elif geom.geom_type == "MultiLineString":
+        return cast(
+            Dict[str, Any], shapely.geometry.mapping(fix_multi_line_string(geom))
+        )
     else:
         raise ValueError(f"unsupported geom_type: {geom.geom_type}")
 
 
 def segment_shape(shape: Dict[str, Any] | GeoInterface) -> List[List[Point]]:
     geom = shapely.geometry.shape(shape)
     if geom.geom_type == "Polygon":
@@ -306,14 +319,50 @@
                 [(-180, 90), (-180, -90), (180, -90), (180, 90)],
                 [polygon.exterior.coords],
             )
     else:
         return MultiPolygon(polygons)
 
 
+def fix_line_string(line_string: LineString) -> Union[LineString, MultiLineString]:
+    """Fixes a :py:class:`shapely.geometry.LineString`.
+
+    Args:
+        line_string: The input line string
+
+    Returns:
+        The fixed line string, either as a single line string or a multi-line
+        string (if it was split)
+    """
+    segments = segment(list(line_string.coords))
+    if not segments:
+        return line_string
+    else:
+        return MultiLineString(segments)
+
+
+def fix_multi_line_string(multi_line_string: MultiLineString) -> MultiLineString:
+    """Fixes a :py:class:`shapely.geometry.MultiLineString`.
+
+    Args:
+        multi_line_string: The input multi line string
+
+    Returns:
+        The fixed multi line string
+    """
+    line_strings = list()
+    for line_string in multi_line_string.geoms:
+        fixed = fix_line_string(line_string)
+        if isinstance(fixed, LineString):
+            line_strings.append(fixed)
+        else:
+            line_strings.extend(fixed.geoms)
+    return MultiLineString(line_strings)
+
+
 def segment_polygon(polygon: Polygon) -> List[List[Point]]:
     segments = segment(list(polygon.exterior.coords))
     if not segments:
         segments = [list(polygon.exterior.coords)]
     for interior in polygon.interiors:
         interior_segments = segment(list(interior.coords))
         if interior_segments:
@@ -374,16 +423,21 @@
     return polygons
 
 
 def segment(coords: List[Point]) -> List[List[Point]]:
     segment = []
     segments = []
     for i, point in enumerate(coords):
-        # Ensure all longitudes are between -180 and 180
-        if point[0] != 180:
+        # Ensure all longitudes are between -180 and 180, and that tiny floating
+        # point differences are ignored.
+        if numpy.isclose(point[0], 180):
+            coords[i] = (180, point[1])
+        elif numpy.isclose(point[0], -180):
+            coords[i] = (-180, point[1])
+        else:
             coords[i] = (((point[0] + 180) % 360) - 180, point[1])
     for start, end in zip(coords, coords[1:]):
         segment.append(start)
         if (end[0] - start[0] > 180) and (end[0] - start[0] != 360):  # left
             latitude = crossing_latitude(start, end)
             segment.append((-180, latitude))
             segments.append(segment)
@@ -395,18 +449,25 @@
             segment = [(-180, latitude)]
     if not segments:
         # No antimeridian crossings
         return []
     elif coords[-1] == segments[0][0]:
         # Join polygons
         segments[0] = segment + segments[0]
+    else:
+        segment.append(coords[-1])
+        segments.append(segment)
     return segments
 
 
 def crossing_latitude(start: Point, end: Point) -> float:
+    if abs(start[0]) == 180:
+        return start[1]
+    elif abs(end[0]) == 180:
+        return end[1]
     latitude_delta = end[1] - start[1]
     if end[0] > 0:
         return round(
             start[1]
             + (180.0 - start[0]) * latitude_delta / (end[0] + 360.0 - start[0]),
             7,
         )
@@ -518,15 +579,20 @@
         segment = segment + segments.pop(index)
         segments.append(segment)
         return build_polygons(segments)
     else:
         # This segment should self-joining, so just build the rest of the
         # polygons without it.
         polygons = build_polygons(segments)
-        polygons.append(Polygon(segment))
+        if not all(p == segment[0] for p in segment):
+            # If every point is the same, then we don't need it in the output
+            # set of polygons. This happens if, e.g., one corner of an input
+            # polygon is on the antimeridian.
+            # https://github.com/gadomski/antimeridian/issues/45#issuecomment-1614586166
+            polygons.append(Polygon(segment))
         return polygons
 
 
 def is_self_closing(segment: List[Point]) -> bool:
     is_right = segment[-1][0] == 180
     return segment[0][0] == segment[-1][0] and (
         (is_right and segment[0][1] > segment[-1][1])
```

### Comparing `antimeridian-0.3.0/src/antimeridian.egg-info/PKG-INFO` & `antimeridian-0.3.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antimeridian
-Version: 0.3.0
+Version: 0.3.1
 Summary: Fix GeoJSON geometries that cross the antimeridian
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: documentation, https://antimeridian.readthedocs.io
 Project-URL: repository, https://github.com/gadomski/antimeridan
 Project-URL: changelog, https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md
 Keywords: geojson,antimeridian,shapely
@@ -22,21 +22,21 @@
 [![CI Status](https://img.shields.io/github/actions/workflow/status/gadomski/antimeridian/ci.yaml?style=for-the-badge&label=CI)](https://github.com/gadomski/antimeridian/actions/workflows/ci.yaml)
 [![Read the Docs](https://img.shields.io/readthedocs/antimeridian?style=for-the-badge)](https://antimeridian.readthedocs.io/en/stable/)
 [![PyPI](https://img.shields.io/pypi/v/antimeridian?style=for-the-badge)](https://pypi.org/project/antimeridian/)
 
 [![GitHub](https://img.shields.io/github/license/gadomski/antimeridian?style=for-the-badge)](https://github.com/gadomski/antimeridian/blob/main/LICENSE)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg?style=for-the-badge)](https://github.com/gadomski/antimeridian/blob/main/CODE_OF_CONDUCT)
 
-Fix polygons that cross the antimeridian.
+Fix shapes that cross the antimeridian.
 See [the documentation](https://antimeridian.readthedocs.io) for information about the underlying algorithm.
-Depends on [shapely](https://shapely.readthedocs.io).
+Depends on [shapely](https://shapely.readthedocs.io) and [numpy](https://numpy.org/).
 
 Can fix:
 
-- Shapely [`Polygon`](https://shapely.readthedocs.io/en/stable/reference/shapely.Polygon.html#shapely.Polygon) and [`MultiPolygon`](https://shapely.readthedocs.io/en/stable/reference/shapely.MultiPolygon.html#shapely.MultiPolygon) objects
+- Shapely [`Polygon`](https://shapely.readthedocs.io/en/stable/reference/shapely.Polygon.html#shapely.Polygon), [`MultiPolygon`](https://shapely.readthedocs.io/en/stable/reference/shapely.MultiPolygon.html#shapely.MultiPolygon), [`LineString`](https://shapely.readthedocs.io/en/stable/reference/shapely.LineString.html#shapely.LineString), and [`MultiLineString`](https://shapely.readthedocs.io/en/stable/reference/shapely.MultiLineString.html#shapely.MultiLineString) objects
 - GeoJSON [Polygons](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.6), [MultiPolygons](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.7), [Features](https://datatracker.ietf.org/doc/html/rfc7946#section-3.2) and [FeatureCollections](https://datatracker.ietf.org/doc/html/rfc7946#section-3.3), as dictionaries
 - Anything that has a [`__geo_interface__`](https://gist.github.com/sgillies/2217756)
 
 ## Usage
 
 ```shell
 pip install antimeridian
```

### Comparing `antimeridian-0.3.0/tests/test_cli.py` & `antimeridian-0.3.1/tests/test_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from pytest_console_scripts import ScriptRunner
 
 pytest.importorskip("click")
 
 
 def test_fix(script_runner: ScriptRunner, input_path: Callable[[str], Path]) -> None:
     path = input_path("simple")
-    result = script_runner.run("antimeridian", "fix", str(path))
+    result = script_runner.run(["antimeridian", "fix", str(path)])
     assert result.success
 
 
 def test_segment(
     script_runner: ScriptRunner, input_path: Callable[[str], Path]
 ) -> None:
     path = input_path("simple")
-    result = script_runner.run("antimeridian", "segment", str(path))
+    result = script_runner.run(["antimeridian", "segment", str(path)])
     assert result.success
```

### Comparing `antimeridian-0.3.0/tests/test_geojson.py` & `antimeridian-0.3.1/tests/test_geojson.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.3.0/tests/test_multi_polygon.py` & `antimeridian-0.3.1/tests/test_multi_polygon.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.3.0/tests/test_polygon.py` & `antimeridian-0.3.1/tests/test_polygon.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,37 +6,39 @@
 
 from .conftest import Reader
 
 
 @pytest.mark.parametrize(
     ("name"),
     [
+        "almost-180",
         "complex-split",
         "crossing-latitude",
         "extra-crossing",
         "latitude-band",
         "north-pole",
         "one-hole",
         "over-180",
         "overlap",
+        "point-on-antimeridian",
         "simple",
         "south-pole",
         "split",
         "two-holes",
     ],
 )
 def test_fix_polygon(
     name: str,
     read_input: Reader,
     read_output: Reader,
 ) -> None:
     input = read_input(name)
     assert isinstance(input, Polygon)
     output = read_output(name)
-    assert isinstance(input, Polygon | MultiPolygon)
+    assert isinstance(input, Polygon) or isinstance(input, MultiPolygon)
     fixed = antimeridian.fix_polygon(input).normalize()
     assert fixed == output.normalize()
 
 
 def test_both_poles(read_input: Reader, read_output: Reader) -> None:
     input = read_input("both-poles")
     assert isinstance(input, Polygon)
```

