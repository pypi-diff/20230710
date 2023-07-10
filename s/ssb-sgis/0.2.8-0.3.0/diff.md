# Comparing `tmp/ssb_sgis-0.2.8.tar.gz` & `tmp/ssb_sgis-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_sgis-0.2.8.tar", max compression
+gzip compressed data, was "ssb_sgis-0.3.0.tar", max compression
```

## Comparing `ssb_sgis-0.2.8.tar` & `ssb_sgis-0.3.0.tar`

### file list

```diff
@@ -1,40 +1,48 @@
--rw-r--r--   0        0        0     1074 2023-06-30 09:31:18.003938 ssb_sgis-0.2.8/LICENSE
--rw-r--r--   0        0        0     7543 2023-06-30 09:31:18.003938 ssb_sgis-0.2.8/README.md
--rw-r--r--   0        0        0     2539 2023-06-30 09:31:34.076245 ssb_sgis-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     2445 2023-06-30 09:31:34.076245 ssb_sgis-0.2.8/src/sgis/__init__.py
--rw-r--r--   0        0        0     3542 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/dapla.py
--rw-r--r--   0        0        0      576 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/geopandas_tools/__init__.py
--rw-r--r--   0        0        0     8780 2023-06-30 09:31:34.076245 ssb_sgis-0.2.8/src/sgis/geopandas_tools/buffer_dissolve_explode.py
--rw-r--r--   0        0        0    17930 2023-06-30 09:31:34.076245 ssb_sgis-0.2.8/src/sgis/geopandas_tools/general.py
--rw-r--r--   0        0        0     5870 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/geopandas_tools/geometry_types.py
--rw-r--r--   0        0        0    14520 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/geopandas_tools/neighbors.py
--rw-r--r--   0        0        0    11862 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/geopandas_tools/overlay.py
--rw-r--r--   0        0        0     6888 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/geopandas_tools/point_operations.py
--rw-r--r--   0        0        0    22635 2023-06-30 09:31:34.076245 ssb_sgis-0.2.8/src/sgis/geopandas_tools/polygon_operations.py
--rw-r--r--   0        0        0    12458 2023-06-30 09:31:34.076245 ssb_sgis-0.2.8/src/sgis/geopandas_tools/to_geodataframe.py
--rw-r--r--   0        0        0     2669 2023-06-30 09:31:34.076245 ssb_sgis-0.2.8/src/sgis/helpers.py
--rw-r--r--   0        0        0        0 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/maps/__init__.py
--rw-r--r--   0        0        0     6479 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/maps/examine.py
--rw-r--r--   0        0        0    25138 2023-06-30 09:31:34.076245 ssb_sgis-0.2.8/src/sgis/maps/explore.py
--rw-r--r--   0        0        0     1923 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/maps/httpserver.py
--rw-r--r--   0        0        0    20499 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/maps/legend.py
--rw-r--r--   0        0        0    18611 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/maps/map.py
--rw-r--r--   0        0        0    15961 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/maps/maps.py
--rw-r--r--   0        0        0    14132 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/maps/thematicmap.py
--rw-r--r--   0        0        0        0 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/__init__.py
--rw-r--r--   0        0        0     6218 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/_get_route.py
--rw-r--r--   0        0        0     2017 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/_od_cost_matrix.py
--rw-r--r--   0        0        0     4206 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/_points.py
--rw-r--r--   0        0        0     4487 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/_service_area.py
--rw-r--r--   0        0        0    12433 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/closing_network_holes.py
--rw-r--r--   0        0        0    12369 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/cutting_lines.py
--rw-r--r--   0        0        0     9375 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/directednetwork.py
--rw-r--r--   0        0        0     3359 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/finding_isolated_networks.py
--rw-r--r--   0        0        0     7686 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/network.py
--rw-r--r--   0        0        0    66761 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/networkanalysis.py
--rw-r--r--   0        0        0    12643 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/networkanalysisrules.py
--rw-r--r--   0        0        0     6767 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/nodes.py
--rw-r--r--   0        0        0        0 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/py.typed
--rw-r--r--   0        0        0     3774 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/read_parquet.py
--rw-r--r--   0        0        0     8831 1970-01-01 00:00:00.000000 ssb_sgis-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-10 10:06:42.660886 ssb_sgis-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7543 2023-07-10 10:06:42.660886 ssb_sgis-0.3.0/README.md
+-rw-r--r--   0        0        0     2597 2023-07-10 10:06:58.249040 ssb_sgis-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2937 2023-07-10 10:06:58.249040 ssb_sgis-0.3.0/src/sgis/__init__.py
+-rw-r--r--   0        0        0      576 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/geopandas_tools/__init__.py
+-rw-r--r--   0        0        0    11243 2023-07-10 10:06:58.249040 ssb_sgis-0.3.0/src/sgis/geopandas_tools/bounds.py
+-rw-r--r--   0        0        0    10967 2023-07-10 10:06:58.249040 ssb_sgis-0.3.0/src/sgis/geopandas_tools/buffer_dissolve_explode.py
+-rw-r--r--   0        0        0    12700 2023-07-10 10:06:58.249040 ssb_sgis-0.3.0/src/sgis/geopandas_tools/general.py
+-rw-r--r--   0        0        0     5870 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/geopandas_tools/geometry_types.py
+-rw-r--r--   0        0        0    14520 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/geopandas_tools/neighbors.py
+-rw-r--r--   0        0        0    11862 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/geopandas_tools/overlay.py
+-rw-r--r--   0        0        0     6888 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/geopandas_tools/point_operations.py
+-rw-r--r--   0        0        0    23748 2023-07-10 10:06:58.249040 ssb_sgis-0.3.0/src/sgis/geopandas_tools/polygon_operations.py
+-rw-r--r--   0        0        0    13227 2023-07-10 10:06:58.249040 ssb_sgis-0.3.0/src/sgis/geopandas_tools/to_geodataframe.py
+-rw-r--r--   0        0        0     3331 2023-07-10 10:06:58.249040 ssb_sgis-0.3.0/src/sgis/helpers.py
+-rw-r--r--   0        0        0     6355 2023-07-10 10:06:58.249040 ssb_sgis-0.3.0/src/sgis/io/dapla.py
+-rw-r--r--   0        0        0     3774 2023-07-10 10:06:58.249040 ssb_sgis-0.3.0/src/sgis/io/read_parquet.py
+-rw-r--r--   0        0        0     3858 2023-07-10 10:06:58.249040 ssb_sgis-0.3.0/src/sgis/io/write_municipality_data.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/maps/__init__.py
+-rw-r--r--   0        0        0     6479 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/maps/examine.py
+-rw-r--r--   0        0        0    24288 2023-07-10 10:06:58.253039 ssb_sgis-0.3.0/src/sgis/maps/explore.py
+-rw-r--r--   0        0        0     1923 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/maps/httpserver.py
+-rw-r--r--   0        0        0    20498 2023-07-10 10:06:58.253039 ssb_sgis-0.3.0/src/sgis/maps/legend.py
+-rw-r--r--   0        0        0    19356 2023-07-10 10:06:58.253039 ssb_sgis-0.3.0/src/sgis/maps/map.py
+-rw-r--r--   0        0        0    16217 2023-07-10 10:06:58.253039 ssb_sgis-0.3.0/src/sgis/maps/maps.py
+-rw-r--r--   0        0        0    14132 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/maps/thematicmap.py
+-rw-r--r--   0        0        0      924 2023-07-10 10:06:58.253039 ssb_sgis-0.3.0/src/sgis/multiprocessing/base.py
+-rw-r--r--   0        0        0     3117 2023-07-10 10:06:58.253039 ssb_sgis-0.3.0/src/sgis/multiprocessing/multiprocessingmapper.py
+-rw-r--r--   0        0        0    11676 2023-07-10 10:06:58.253039 ssb_sgis-0.3.0/src/sgis/multiprocessing/multiprocessingpool.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/networkanalysis/__init__.py
+-rw-r--r--   0        0        0     6218 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/networkanalysis/_get_route.py
+-rw-r--r--   0        0        0     2017 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/networkanalysis/_od_cost_matrix.py
+-rw-r--r--   0        0        0     4206 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/networkanalysis/_points.py
+-rw-r--r--   0        0        0     4487 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/networkanalysis/_service_area.py
+-rw-r--r--   0        0        0    12433 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/networkanalysis/closing_network_holes.py
+-rw-r--r--   0        0        0    12369 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/networkanalysis/cutting_lines.py
+-rw-r--r--   0        0        0    11189 2023-07-10 10:06:58.253039 ssb_sgis-0.3.0/src/sgis/networkanalysis/directednetwork.py
+-rw-r--r--   0        0        0     3359 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/networkanalysis/finding_isolated_networks.py
+-rw-r--r--   0        0        0     7686 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/networkanalysis/network.py
+-rw-r--r--   0        0        0    66909 2023-07-10 10:06:58.253039 ssb_sgis-0.3.0/src/sgis/networkanalysis/networkanalysis.py
+-rw-r--r--   0        0        0    12643 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/networkanalysis/networkanalysisrules.py
+-rw-r--r--   0        0        0     6767 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/networkanalysis/nodes.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:06:42.692886 ssb_sgis-0.3.0/src/sgis/py.typed
+-rw-r--r--   0        0        0        0 2023-07-10 10:06:58.253039 ssb_sgis-0.3.0/src/sgis/raster/__init__.py
+-rw-r--r--   0        0        0     4835 2023-07-10 10:06:58.253039 ssb_sgis-0.3.0/src/sgis/raster/elevationraster.py
+-rw-r--r--   0        0        0    36176 2023-07-10 10:06:58.253039 ssb_sgis-0.3.0/src/sgis/raster/raster.py
+-rw-r--r--   0        0        0     8952 1970-01-01 00:00:00.000000 ssb_sgis-0.3.0/PKG-INFO
```

### Comparing `ssb_sgis-0.2.8/LICENSE` & `ssb_sgis-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.8/README.md` & `ssb_sgis-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.8/pyproject.toml` & `ssb_sgis-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-sgis"
-version = "0.2.8"
+version = "0.3.0"
 description = "GIS functions used at Statistics Norway."
 authors = ["Statistics Norway <ort@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "sgis", from = "src"}]
 homepage = "https://github.com/statisticsnorway/ssb-sgis"
 repository = "https://github.com/statisticsnorway/ssb-sgis"
@@ -30,14 +30,17 @@
 pyarrow = ">=11.0.0"
 requests = ">=2.28.2"
 scikit-learn = ">=1.2.1"
 shapely = ">=2.0.1"
 xyzservices = ">=2023.2.0"
 jenkspy = ">=0.3.2"
 ipython = ">=8.13.2"
+rtree = "^1.0.1"
+geocoder = "^1.38.1"
+rasterio = "^1.3.8"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["d", "jupyter"], version = ">=23.1.0"}
 coverage = {extras = ["toml"], version = ">=7.2.1"}
 darglint = ">=1.8.1"
 deptry = ">=0.8.0"
 flake8 = ">=6.0.0"
```

### Comparing `ssb_sgis-0.2.8/src/sgis/__init__.py` & `ssb_sgis-0.3.0/src/sgis/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # flake8: noqa: F401
+from .geopandas_tools.bounds import (
+    bounds_to_points,
+    bounds_to_polygon,
+    make_grid,
+    make_grid_from_bbox,
+    make_ssb_grid,
+    points_in_bounds,
+)
 from .geopandas_tools.buffer_dissolve_explode import (
     buff,
     buffdiss,
     buffdissexp,
     buffdissexp_by_cluster,
     dissexp,
     dissexp_by_cluster,
 )
 from .geopandas_tools.general import (
-    bounds_to_points,
-    bounds_to_polygon,
+    address_to_coords,
+    address_to_gdf,
     clean_clip,
     clean_geoms,
     coordinate_array,
     drop_inactive_geometry_columns,
-    make_grid,
-    make_grid_from_bbox,
-    make_ssb_grid,
-    points_in_bounds,
     random_points,
     rename_geometry_if,
     to_lines,
 )
 from .geopandas_tools.geometry_types import (
     get_geom_type,
     is_single_geom_type,
@@ -45,14 +49,15 @@
     get_overlapping_polygon_indices,
     get_overlapping_polygon_product,
     get_overlapping_polygons,
     get_polygon_clusters,
 )
 from .geopandas_tools.to_geodataframe import to_gdf
 from .helpers import get_name
+from .io.read_parquet import read_parquet_url
 from .maps.examine import Examine
 from .maps.explore import Explore
 from .maps.httpserver import run_html_server
 from .maps.legend import Legend
 from .maps.maps import clipmap, explore, qtm, samplemap
 from .maps.thematicmap import ThematicMap
 from .networkanalysis.closing_network_holes import (
@@ -76,14 +81,23 @@
 from .networkanalysis.networkanalysis import NetworkAnalysis
 from .networkanalysis.networkanalysisrules import NetworkAnalysisRules
 from .networkanalysis.nodes import (
     make_edge_coords_cols,
     make_edge_wkt_cols,
     make_node_ids,
 )
-from .read_parquet import read_parquet_url
+
+# from .raster.cube import GeoDataCube
+from .raster.elevationraster import ElevationRaster
+from .raster.raster import Raster
 
 
 try:
-    from .dapla import exists, read_geopandas, write_geopandas
+    from .io.dapla import exists, read_geopandas, write_geopandas
+    from .io.write_municipality_data import (
+        write_municipality_data,
+        write_neighbor_municipality_data,
+    )
+    from .multiprocessing.multiprocessingmapper import MultiProcessingMapper
+    from .multiprocessing.multiprocessingpool import MultiProcessingPool
 except ImportError:
     pass
```

### Comparing `ssb_sgis-0.2.8/src/sgis/exceptions.py` & `ssb_sgis-0.3.0/src/sgis/exceptions.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.8/src/sgis/geopandas_tools/buffer_dissolve_explode.py` & `ssb_sgis-0.3.0/src/sgis/geopandas_tools/buffer_dissolve_explode.py`

 * *Files 14% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         gdf: the GeoDataFrame that will be buffered, dissolved and exploded.
         distance: the distance (meters, degrees, depending on the crs) to buffer
             the geometry by
         resolution: The number of segments used to approximate a quarter circle.
             Here defaults to 50, as opposed to the default 16 in geopandas.
         index_parts: If False (default), the index after dissolve is respected. If
             True, an integer index level is added during explode.
-        copy: Whether to copy the GeoDataFrame before buffering.
+        copy: Whether to copy the GeoDataFrame before buffering. Defaults to True.
         **dissolve_kwargs: additional keyword arguments passed to geopandas' dissolve.
 
     Returns:
         A buffered GeoDataFrame where overlapping geometries are dissolved.
     """
     dissolve_kwargs, ignore_index = _decide_ignore_index(dissolve_kwargs)
 
@@ -93,15 +93,15 @@
     Args:
         gdf: the GeoDataFrame that will be
             buffered and dissolved.
         distance: the distance (meters, degrees, depending on the crs) to buffer
             the geometry by
         resolution: The number of segments used to approximate a quarter circle.
             Here defaults to 50, as opposed to the default 16 in geopandas.
-        copy: Whether to copy the GeoDataFrame before buffering.
+        copy: Whether to copy the GeoDataFrame before buffering. Defaults to True.
         **dissolve_kwargs: additional keyword arguments passed to geopandas' dissolve.
 
     Returns:
         A buffered GeoDataFrame where geometries are dissolved.
 
     Examples
     --------
@@ -166,15 +166,15 @@
     **dissolve_kwargs,
 ):
     """Dissolves overlapping geometries.
 
     It takes a GeoDataFrame and dissolves, fixes and explodes geometries.
 
     Args:
-        gdf: the GeoDataFrame that will be buffered, dissolved and exploded.
+        gdf: the GeoDataFrame that will be dissolved and exploded.
         index_parts: If False (default), the index after dissolve is respected. If
             True, an integer index level is added during explode.
         **dissolve_kwargs: additional keyword arguments passed to geopandas' dissolve.
 
     Returns:
         A GeoDataFrame where overlapping geometries are dissolved.
     """
@@ -187,37 +187,89 @@
     dissolved[geom_col] = dissolved.make_valid()
 
     return make_all_singlepart(
         dissolved, ignore_index=ignore_index, index_parts=index_parts
     )
 
 
-def dissexp_by_cluster(gdf: GeoDataFrame) -> GeoDataFrame:
-    return (
+def dissexp_by_cluster(gdf: GeoDataFrame, **dissolve_kwargs) -> GeoDataFrame:
+    """Dissolves overlapping geometries through clustering with sjoin and networkx.
+
+    Works exactly like dissexp, but, before dissolving, the geometries are divided
+    into clusters based on overlap (uses the function sgis.get_polygon_clusters).
+    The geometries are then dissolved based on this column (and optionally other
+    columns).
+
+    This might be many times faster than a regular dissexp, if there are many
+    non-overlapping geometries.
+
+    Args:
+        gdf: the GeoDataFrame that will be dissolved and exploded.
+        **dissolve_kwargs: Keyword arguments passed to geopandas' dissolve.
+
+    Returns:
+        A GeoDataFrame where overlapping geometries are dissolved.
+    """
+    by = dissolve_kwargs.pop("by", [])
+    if isinstance(by, str):
+        by = ["cluster_", by]
+    elif by is None:
+        by = ["cluster_"]
+    else:
+        by = ["cluster_"] + list(by)
+
+    dissolved = (
         gdf.explode(ignore_index=True)
-        .pipe(get_polygon_clusters, cluster_col="cluster")
-        .pipe(dissexp, by="cluster")
-        .reset_index(drop=True)
+        .explode(ignore_index=True)
+        .pipe(get_polygon_clusters, cluster_col="cluster_")
+        .pipe(dissexp, by=by, **dissolve_kwargs)
     )
 
+    if by == ["cluster_"]:
+        return dissolved.reset_index(drop=True)
+
+    if dissolve_kwargs.get("as_index", True):
+        dissolved.index = dissolved.index.droplevel(0)
+        return dissolved
+
+    return dissolved.drop("cluster_", axis=1)
+
 
 def buffdissexp_by_cluster(
     gdf: GeoDataFrame,
     distance: int | float,
     *,
     resolution: int = 50,
     copy: bool = True,
+    **dissolve_kwargs,
 ) -> GeoDataFrame:
-    return (
-        buff(gdf, distance, resolution=resolution, copy=copy)
-        .explode(ignore_index=True)
-        .pipe(get_polygon_clusters, cluster_col="cluster")
-        .pipe(dissexp, by="cluster")
-        .reset_index(drop=True)
-    )
+    """Buffers and dissolves overlapping geometries.
+
+    Works exactly like buffdissexp, but, before dissolving, the geometries are divided
+    into clusters based on overlap (uses the function sgis.get_polygon_clusters).
+    The geometries are then dissolved based on this column (and optionally other
+    columns).
+
+    This might be many times faster than a regular buffdissexp, if there are many
+    non-overlapping geometries.
+
+    Args:
+        gdf: the GeoDataFrame that will be buffered, dissolved and exploded.
+        distance: the distance (meters, degrees, depending on the crs) to buffer
+            the geometry by
+        resolution: The number of segments used to approximate a quarter circle.
+            Here defaults to 50, as opposed to the default 16 in geopandas.
+        copy: Whether to copy the GeoDataFrame before buffering. Defaults to True.
+        **dissolve_kwargs: additional keyword arguments passed to geopandas' dissolve.
+
+    Returns:
+        A buffered GeoDataFrame where overlapping geometries are dissolved.
+    """
+    buffered = buff(gdf, distance, resolution=resolution, copy=copy)
+    return dissexp_by_cluster(buffered, **dissolve_kwargs)
 
 
 def buff(
     gdf: GeoDataFrame | GeoSeries,
     distance: int | float,
     resolution: int = 50,
     copy: bool = True,
@@ -227,15 +279,15 @@
 
     Args:
         gdf: the GeoDataFrame that will be buffered, dissolved and exploded.
         distance: the distance (meters, degrees, depending on the crs) to buffer
             the geometry by
         resolution: The number of segments used to approximate a quarter circle.
             Here defaults to 50, as opposed to the default 16 in geopandas.
-        copy: Whether to copy the GeoDataFrame before buffering.
+        copy: Whether to copy the GeoDataFrame before buffering. Defaults to True.
         **buffer_kwargs: additional keyword arguments passed to geopandas' buffer.
 
     Returns:
         A buffered GeoDataFrame.
     """
 
     if isinstance(gdf, GeoSeries):
```

### Comparing `ssb_sgis-0.2.8/src/sgis/geopandas_tools/general.py` & `ssb_sgis-0.3.0/src/sgis/maps/maps.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,568 +1,459 @@
-import warnings
+"""Interactive and static mapping of multiple GeoDataFrames.
+
+The main function is 'explore', which displays one of more GeoDataFrames together in an
+interactive map with layers that can be toggled on and off. The 'samplemap' and
+'clipmap' functions do the same, but displays a random and chosen area respectfully.
+
+The 'qtm' function shows a simple static map of one or more GeoDataFrames.
+"""
+
+from numbers import Number
+from typing import Any
 
-import geopandas as gpd
-import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame, GeoSeries
-from geopandas.array import GeometryDtype
-from shapely import (
-    Geometry,
-    box,
-    extract_unique_points,
-    get_exterior_ring,
-    get_interior_ring,
-    get_num_interior_rings,
-    get_parts,
+from shapely import Geometry
+
+from ..geopandas_tools.general import (
+    address_to_coords,
+    address_to_gdf,
+    clean_clip,
+    is_wkt,
 )
-from shapely.geometry import LineString, Point, Polygon
-from shapely.ops import unary_union
+from ..geopandas_tools.geometry_types import get_geom_type
+from ..geopandas_tools.to_geodataframe import to_gdf
+from ..helpers import make_namedict
+from .explore import Explore
+from .map import Map
+from .thematicmap import ThematicMap
+
+
+def _get_mask(kwargs: dict, crs) -> tuple[GeoDataFrame | None, dict]:
+    masks = {
+        "bygdoy": (10.6976899, 59.9081695),
+        "kongsvinger": (12.0035242, 60.1875279),
+        "stavanger": (5.6960601, 58.8946196),
+        "volda": (6.0705987, 62.146643),
+    }
 
-from .geometry_types import make_all_singlepart, to_single_geom_type
-from .to_geodataframe import to_gdf
+    if "size" in kwargs and kwargs["size"] is not None:
+        size = kwargs["size"]
+    else:
+        size = 1000
 
+    for key, value in kwargs.items():
+        if key.lower() in masks:
+            mask = masks[key]
+            kwargs.pop(key)
+            if isinstance(value, Number) and value > 1:
+                size = value
+            the_mask = to_gdf([mask], crs=4326).to_crs(crs).buffer(size)
+            return the_mask, kwargs
+
+    return None, kwargs
+
+
+def explore(
+    *gdfs: GeoDataFrame,
+    column: str | None = None,
+    center: Any | None = None,
+    labels: tuple[str] | None = None,
+    max_zoom: int = 30,
+    browser: bool = False,
+    smooth_factor: int | float = 1.5,
+    size: int | None = None,
+    **kwargs,
+) -> None:
+    """Interactive map of GeoDataFrames with layers that can be toggled on/off.
 
-def coordinate_array(
-    gdf: GeoDataFrame | GeoSeries,
-) -> np.ndarray[np.ndarray[float], np.ndarray[float]]:
-    """Creates a 2d ndarray of coordinates from point geometries.
+    It takes all the given GeoDataFrames and displays them together in an
+    interactive map with a common legend. If 'column' is not specified, each
+    GeoDataFrame is given a unique color.
+
+    The 'center' parameter can be used to show only parts of large datasets.
+    'center' can be a string of a city or address, a coordinate tuple or a
+    geometry-like object.
 
     Args:
-        gdf: GeoDataFrame or GeoSeries of point geometries.
+        *gdfs: one or more GeoDataFrames.
+        column: The column to color the geometries by. Defaults to None, which means
+            each GeoDataFrame will get a unique color.
+        center: Either an address string to be geocoded or a geometry like object
+            (coordinate pair (x, y), GeoDataFrame, bbox, etc.).
+            The geometries will be clipped by a buffered circle around this point.
+            If 'size' is not given, 1000 will be used as the buffer distance.
+        labels: By default, the GeoDataFrames will be labeled by their object names.
+            Alternatively, labels can be specified as a tuple of strings with the same
+            length as the number of gdfs.
+        max_zoom: The maximum allowed level of zoom. Higher number means more zoom
+            allowed. Defaults to 30, which is higher than the geopandas default.
+        browser: If False (default), the maps will be shown in Jupyter.
+            If True the maps will be opened in a browser folder.
+        smooth_factor: How much to simplify the geometries. 1 is the minimum,
+            5 is quite a lot of simplification.
+        size: The buffer distance. Only used when center is given. It then defaults to
+            1000.
+        **kwargs: Keyword arguments to pass to geopandas.GeoDataFrame.explore, for
+            instance 'cmap' to change the colors, 'scheme' to change how the data
+            is grouped. This defaults to 'fisherjenkssampled' for numeric data.
 
-    Returns:
-        np.ndarray of np.ndarrays of coordinates.
+    See also
+    --------
+    samplemap: same functionality, but shows only a random area of a given size.
+    clipmap: same functionality, but shows only the areas clipped by a given mask.
 
     Examples
     --------
-    >>> from sgis import coordinate_array, random_points
-    >>> points = random_points(5)
-    >>> points
-                    geometry
-    0  POINT (0.59376 0.92577)
-    1  POINT (0.34075 0.91650)
-    2  POINT (0.74841 0.10627)
-    3  POINT (0.00966 0.87868)
-    4  POINT (0.38046 0.87879)
-    >>> coordinate_array(points)
-    array([[0.59376221, 0.92577159],
-        [0.34074678, 0.91650446],
-        [0.74840912, 0.10626954],
-        [0.00965935, 0.87867915],
-        [0.38045827, 0.87878816]])
-    >>> coordinate_array(points.geometry)
-    array([[0.59376221, 0.92577159],
-        [0.34074678, 0.91650446],
-        [0.74840912, 0.10626954],
-        [0.00965935, 0.87867915],
-        [0.38045827, 0.87878816]])
-    """
-    if isinstance(gdf, GeoDataFrame):
-        return np.array([(geom.x, geom.y) for geom in gdf.geometry])
-    else:
-        return np.array([(geom.x, geom.y) for geom in gdf])
+    >>> from sgis import read_parquet_url, explore
+    >>> roads = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_eidskog_2022.parquet")
+    >>> points = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_eidskog.parquet")
 
+    Simple explore of two GeoDataFrames.
 
-def _push_geom_col(gdf: GeoDataFrame) -> GeoDataFrame:
-    """Makes the geometry column the rightmost column in the GeoDataFrame.
+    >>> explore(roads, points)
 
-    Args:
-        gdf: GeoDataFrame.
+    With additional arguments.
 
-    Returns:
-        The GeoDataFrame with the geometry column pushed all the way to the right.
+    >>> roads["meters"] = roads.length
+    >>> points["meters"] = points.length
+    >>> explore(roads, points, column="meters", cmap="plasma", max_zoom=60)
     """
-    geom_col = gdf._geometry_column_name
-    return gdf.reindex(columns=[c for c in gdf.columns if c != geom_col] + [geom_col])
+    mask, kwargs = _get_mask(kwargs | {"size": size}, crs=gdfs[0].crs)
 
+    kwargs.pop("size", None)
 
-def drop_inactive_geometry_columns(gdf: GeoDataFrame) -> GeoDataFrame:
-    for col in gdf.columns:
-        if (
-            isinstance(gdf[col].dtype, GeometryDtype)
-            and col != gdf._geometry_column_name
-        ):
-            gdf = gdf.drop(col, axis=1)
-    return gdf
-
-
-def rename_geometry_if(gdf: GeoDataFrame) -> GeoDataFrame:
-    geom_col = gdf._geometry_column_name
-    if geom_col == "geometry" and geom_col in gdf.columns:
-        return gdf
-    elif geom_col in gdf.columns:
-        return gdf.rename_geometry("geometry")
+    if mask is not None:
+        return clipmap(
+            *gdfs,
+            column=column,
+            mask=mask,
+            labels=labels,
+            browser=browser,
+            max_zoom=max_zoom,
+            **kwargs,
+        )
 
-    geom_cols = list(
-        {col for col in gdf.columns if isinstance(gdf[col].dtype, GeometryDtype)}
-    )
-    if len(geom_cols) == 1:
-        gdf._geometry_column_name = geom_cols[0]
-        return gdf.rename_geometry("geometry")
+    if center is not None:
+        size = size or 1000
+        if isinstance(center, str) and not is_wkt(center):
+            mask = address_to_gdf(center, crs=gdfs[0].crs).buffer(size)
+        elif not isinstance(center, GeoDataFrame):
+            mask = to_gdf(center, crs=gdfs[0].crs).buffer(size)
+        elif get_geom_type(center) in ["point", "line"]:
+            mask = center.buffer(size)
+
+        return clipmap(
+            *gdfs,
+            column=column,
+            mask=mask,
+            labels=labels,
+            browser=browser,
+            max_zoom=max_zoom,
+            **kwargs,
+        )
 
-    raise ValueError(
-        "There are multiple geometry columns and none are the active geometry"
+    m = Explore(
+        *gdfs,
+        column=column,
+        labels=labels,
+        browser=browser,
+        max_zoom=max_zoom,
+        smooth_factor=smooth_factor,
+        **kwargs,
     )
+    m.explore()
+
 
+def samplemap(
+    *gdfs: GeoDataFrame,
+    column: str | None = None,
+    size: int = 1000,
+    sample_from_first: bool = True,
+    labels: tuple[str] | None = None,
+    max_zoom: int = 30,
+    smooth_factor: int = 1.5,
+    explore: bool = True,
+    browser: bool = False,
+    **kwargs,
+) -> None:
+    """Shows an interactive map of a random area of GeoDataFrames.
 
-def make_grid_from_bbox(
-    minx: int | float,
-    miny: int | float,
-    maxx: int | float,
-    maxy: int | float,
-    *_,
-    gridsize: int | float,
-    crs,
-) -> GeoDataFrame:
-    """Creates a polygon grid from a bounding box.
+    It takes all the GeoDataFrames specified, takes a random sample point from the
+    first, and shows all geometries within a given radius of this point. Otherwise
+    works like the explore function.
+
+    To re-use the sample area, use the line that is printed in this function,
+    containing the size and centerpoint. This line can be copypasted directly
+    into the explore or clipmap functions.
 
-    Creates a GeoDataFrame of grid cells of a given size within the given
-    maxumum and mimimum x and y values.
+    Note:
+        The maximum zoom level only works on the OpenStreetMap background map.
 
     Args:
-        minx: Minumum x coordinate.
-        miny: Minumum y coordinate.
-        maxx: Maximum x coordinate.
-        maxy: Maximum y coordinate.
-        gridsize: Length of the grid walls.
-        crs: Coordinate reference system.
+        *gdfs: one or more GeoDataFrames.
+        column: The column to color the geometries by. Defaults to None, which means
+            each GeoDataFrame will get a unique color.
+        size: the radius to buffer the sample point by before clipping with the data.
+            Defaults to 1000 (meters).
+        sample_from_first: If True (default), the sample point is taken form the
+            first specified GeoDataFrame. If False, all GeoDataFrames are considered.
+        labels: By default, the GeoDataFrames will be labeled by their object names.
+            Alternatively, labels can be specified as a tuple of strings the same
+            length as the number of gdfs.
+        max_zoom: The maximum allowed level of zoom. Higher number means more zoom
+            allowed. Defaults to 30, which is higher than the geopandas default.
+        smooth_factor: How much to simplify the geometries. 1 is the minimum,
+            5 is quite a lot of simplification.
+        explore: If True (default), an interactive map will be displayed. If False,
+            or not in Jupyter, a static plot will be shown.
+        browser: If False (default), the maps will be shown in Jupyter.
+            If True the maps will be opened in a browser folder.
+        **kwargs: Keyword arguments to pass to geopandas.GeoDataFrame.explore, for
+            instance 'cmap' to change the colors, 'scheme' to change how the data
+            is grouped. This defaults to 'fisherjenkssampled' for numeric data.
 
-    Returns:
-        GeoDataFrame with grid geometries.
-    """
-    grid_cells1 = []
-    grid_cells2 = []
-    grid_cells3 = []
-    grid_cells4 = []
-    for x0 in np.arange(minx, maxx + gridsize, gridsize):
-        for y0 in np.arange(miny, maxy + gridsize, gridsize):
-            x1 = x0 - gridsize
-            y1 = y0 + gridsize
-            grid_cells1.append(x0)
-            grid_cells2.append(y0)
-            grid_cells3.append(x1)
-            grid_cells4.append(y1)
-
-    grid_cells = box(grid_cells1, grid_cells2, grid_cells3, grid_cells4)
+    See also
+    --------
+    explore: Same functionality, but shows the entire area of the geometries.
+    clipmap: Same functionality, but shows only the areas clipped by a given mask.
 
-    return gpd.GeoDataFrame(grid_cells, columns=["geometry"], crs=crs)
+    Examples
+    --------
+    >>> from sgis import read_parquet_url, samplemap
+    >>> roads = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_eidskog_2022.parquet")
+    >>> points = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_eidskog.parquet")
 
+    With default sample size. To get a new sample area, simply re-run the line.
 
-def make_grid(gdf: GeoDataFrame, gridsize: int | float) -> GeoDataFrame:
-    """Create a polygon grid around a GeoDataFrame.
+    >>> samplemap(roads, points)
 
-    Creates a GeoDataFrame of grid cells of a given size within the bounds of
-    a given GeoDataFrame.
+    Sample area with a radius of 5 kilometers.
 
-    Args:
-        gdf: A GeoDataFrame.
-        gridsize: Length of the grid walls.
+    >>> samplemap(roads, points, size=5_000, column="meters")
 
-    Returns:
-        GeoDataFrame with grid polygons.
     """
-    minx, miny, maxx, maxy = gdf.total_bounds
-    return make_grid_from_bbox(minx, miny, maxx, maxy, gridsize=gridsize, crs=gdf.crs)
-
-
-def make_ssb_grid(gdf: GeoDataFrame, gridsize: int = 1000) -> GeoDataFrame:
-    """Creates a polygon grid around a GeoDataFrame with an SSB id column.
 
-    Creates a grid that follows the grids produced by Statistics Norway.
-    The GeoDataFrame must have 25833 as crs (UTM 33 N).
+    if isinstance(gdfs[-1], (float, int)):
+        *gdfs, size = gdfs
 
-    Courtesy https://gis.stackexchange.com/questions/269243/creating-polygon-grid-using-geopandas
+    mask, kwargs = _get_mask(kwargs | {"size": size}, crs=gdfs[0].crs)
+    kwargs.pop("size")
 
-    Args:
-        gdf: A GeoDataFrame.
-        gridsize: Size of the grid in meters.
-
-    Returns:
-        GeoDataFrame with grid geometries and a column 'SSBID'.
-
-    Raises:
-        ValueError: If the GeoDataFrame does not have 25833 as crs.
-    """
-    if not gdf.crs.equals(25833):
-        raise ValueError(
-            "Geodataframe must have crs = 25833. Use df.set_crs(25833) to set "
-            "projection or df.to_crs(25833) for transforming."
+    if mask is not None:
+        gdfs, column = Explore._separate_args(gdfs, column)
+        gdfs, kwargs = _prepare_clipmap(
+            *gdfs,
+            mask=mask,
+            labels=labels,
+            **kwargs,
         )
 
-    minx, miny, maxx, maxy = gdf.total_bounds
-
-    # Adjust for SSB-grid
-    minx = int(minx / int(gridsize)) * int(gridsize)
-    miny = int(miny / int(gridsize)) * int(gridsize)
-
-    cols = list(np.arange(minx, maxx + gridsize, gridsize))
-    rows = list(np.arange(miny, maxy + gridsize, gridsize))
-
-    polygons = []
-    for x in cols[:-1]:
-        for y in rows[:-1]:
-            polygons.append(
-                Polygon(
-                    [
-                        (x, y),
-                        (x + gridsize, y),
-                        (x + gridsize, y + gridsize),
-                        (x, y + gridsize),
-                    ]
-                )
-            )
-
-    grid = gpd.GeoDataFrame({"geometry": polygons}, crs=25833)
-
-    # Make SSB-id
-    grid["ostc"] = (
-        (np.floor((grid.geometry.centroid.x + 2000000) / gridsize) * gridsize).apply(
-            int
+    if explore:
+        m = Explore(
+            *gdfs,
+            column=column,
+            labels=labels,
+            browser=browser,
+            max_zoom=max_zoom,
+            smooth_factor=smooth_factor,
+            **kwargs,
         )
-    ).apply(str)
-    grid["nordc"] = (
-        (np.floor((grid.geometry.centroid.y) / gridsize) * gridsize).apply(int)
-    ).apply(str)
-    grid["SSBID"] = grid["ostc"] + grid["nordc"]
-    grid = grid.drop(columns=["ostc", "nordc"])
-    return grid
+        m.samplemap(size, sample_from_first=sample_from_first)
 
-
-def add_grid_id(
-    gdf: GeoDataFrame, gridsize: int, out_column: str = "SSBID"
-) -> GeoDataFrame:
-    """Adds a grid ID column to a GeoDataFrame of points.
-
-    The GeoDataFrame must have 25833 as crs (UTM 33 N).
-
-    Args:
-        gdf: A GeoDataFrame.
-        gridsize: Size of the grid in meters.
-
-    Returns:
-        The input GeoDataFrame with a new grid id column.
-
-    Raises:
-        ValueError: If the GeoDataFrame does not have 25833 as crs.
-    """
-    if gdf.crs != 25833:
-        raise ValueError(
-            "Geodataframe must have crs = 25833. Use df.set_crs(25833) to set "
-            "projection or df.to_crs(25833) for transforming."
+    else:
+        m = Map(
+            *gdfs,
+            column=column,
+            labels=labels,
+            **kwargs,
         )
-    midlrdf = gdf.copy()
-    midlrdf["ostc"] = (
-        (np.floor((midlrdf.geometry.x + 2000000) / gridsize) * gridsize).apply(int)
-    ).apply(str)
-    midlrdf["nordc"] = (
-        (np.floor((midlrdf.geometry.y) / gridsize) * gridsize).apply(int)
-    ).apply(str)
-    midlrdf[out_column] = midlrdf["ostc"] + midlrdf["nordc"]
-    midlrdf = midlrdf.drop(columns=["nordc", "ostc"])
-    return midlrdf
 
+        if sample_from_first:
+            sample = m._gdfs[0].sample(1)
+        else:
+            sample = m._gdf.sample(1)
 
-def bounds_to_polygon(gdf: GeoDataFrame) -> GeoDataFrame:
-    """Creates a box around the geometry in each row of a GeoDataFrame.
+        # convert lines to polygons
+        if get_geom_type(sample) == "line":
+            sample["geometry"] = sample.buffer(1)
 
-    Args:
-        gdf: The GeoDataFrame.
+        if get_geom_type(sample) == "polygon":
+            random_point = sample.sample_points(size=1)
 
-    Returns:
-        GeoDataFrame of box polygons with same length and index as 'gdf'.
-    """
-    bbox_each_row = [box(*arr) for arr in gdf.bounds.values]
-    return to_gdf(bbox_each_row, index=gdf.index, crs=gdf.crs)
+        # if point or mixed geometries
+        else:
+            random_point = sample.centroid
 
+        center = (random_point.geometry.iloc[0].x, random_point.geometry.iloc[0].y)
+        print(f"center={center}, size={size}")
 
-def bounds_to_points(gdf: GeoDataFrame) -> GeoDataFrame:
-    """Creates a 4-noded multipoint around the geometry in each row of a GeoDataFrame.
+        m._gdf = clean_clip(m._gdf, random_point.buffer(size))
 
-    Args:
-        gdf: The GeoDataFrame.
+        qtm(m._gdf, column=m.column, cmap=m._cmap, k=m.k)
 
-    Returns:
-        GeoDataFrame of multipoints with same length and index as 'gdf'.
-    """
-    gdf = bounds_to_polygon(gdf)
-    gdf["geometry"] = extract_unique_points(gdf)
-    return gdf
 
+def _prepare_clipmap(*gdfs, mask, labels, **kwargs):
+    if mask is None:
+        mask, kwargs = _get_mask(kwargs, crs=gdfs[0].crs)
+        if mask is None and len(gdfs) > 1:
+            *gdfs, mask = gdfs
+        elif mask is None:
+            raise ValueError("Must speficy mask.")
 
-def clean_geoms(
-    gdf: GeoDataFrame | GeoSeries, ignore_index: bool = False
-) -> GeoDataFrame | GeoSeries:
-    """Fixes geometries and removes invalid, empty, NaN and None geometries.
+    # storing object names in dict here, since the names disappear after clip
+    if not labels:
+        namedict = make_namedict(gdfs)
+        kwargs["namedict"] = namedict
 
-    Args:
-        gdf: GeoDataFrame or GeoSeries to be cleaned.
-        ignore_index: If True, the resulting axis will be labeled 0, 1, …, n - 1.
-            Defaults to False
-
-    Returns:
-        GeoDataFrame or GeoSeries with fixed geometries and only the rows with valid,
-        non-empty and not-NaN/-None geometries.
+    clipped: tuple[GeoDataFrame] = ()
 
-    Examples
-    --------
-    >>> from sgis import clean_geoms, to_gdf
-    >>> import pandas as pd
-    >>> from shapely import wkt
-    >>> gdf = to_gdf([
-    ...         "POINT (0 0)",
-    ...         "LINESTRING (1 1, 2 2)",
-    ...         "POLYGON ((3 3, 4 4, 3 4, 3 3))"
-    ...         ])
-    >>> gdf
-                                                geometry
-    0                            POINT (0.00000 0.00000)
-    1      LINESTRING (1.00000 1.00000, 2.00000 2.00000)
-    2  POLYGON ((3.00000 3.00000, 4.00000 4.00000, 3....
-
-    Removing None and empty geometries.
-
-    >>> missing = pd.DataFrame({"geometry": [None]})
-    >>> empty = to_gdf(wkt.loads("POINT (0 0)").buffer(0))
-    >>> gdf = pd.concat([gdf, missing, empty])
-    >>> gdf
-                                                geometry
-    0                            POINT (0.00000 0.00000)
-    1      LINESTRING (1.00000 1.00000, 2.00000 2.00000)
-    2  POLYGON ((3.00000 3.00000, 4.00000 4.00000, 3....
-    0                                               None
-    0                                      POLYGON EMPTY
-    >>> clean_geoms(gdf)
-                                                geometry
-    0                            POINT (0.00000 0.00000)
-    1      LINESTRING (1.00000 1.00000, 2.00000 2.00000)
-    2  POLYGON ((3.00000 3.00000, 4.00000 4.00000, 3....
-    """
-    warnings.filterwarnings("ignore", "GeoSeries.notna", UserWarning)
+    if mask is not None:
+        for gdf in gdfs:
+            clipped_ = clean_clip(gdf, mask)
+            clipped = clipped + (clipped_,)
 
-    if isinstance(gdf, GeoDataFrame):
-        geom_col = gdf._geometry_column_name
-        gdf[geom_col] = gdf.make_valid()
-        gdf = gdf.loc[
-            (gdf[geom_col].is_valid)
-            & (~gdf[geom_col].is_empty)
-            & (gdf[geom_col].notna())
-        ]
-    elif isinstance(gdf, GeoSeries):
-        gdf = gdf.make_valid()
-        gdf = gdf.loc[(gdf.is_valid) & (~gdf.is_empty) & (gdf.notna())]
     else:
-        raise TypeError(f"'gdf' should be GeoDataFrame or GeoSeries, got {type(gdf)}")
-
-    if ignore_index:
-        gdf = gdf.reset_index(drop=True)
+        for gdf in gdfs[:-1]:
+            clipped_ = clean_clip(gdf, gdfs[-1])
+            clipped = clipped + (clipped_,)
+
+    if not any(len(gdf) for gdf in clipped):
+        raise ValueError("None of the GeoDataFrames are within the mask extent.")
+
+    return clipped, kwargs
+
+
+def clipmap(
+    *gdfs: GeoDataFrame,
+    column: str | None = None,
+    mask: GeoDataFrame | GeoSeries | Geometry = None,
+    labels: tuple[str] | None = None,
+    explore: bool = True,
+    max_zoom: int = 30,
+    smooth_factor: int | float = 1.5,
+    browser: bool = False,
+    **kwargs,
+) -> None:
+    """Shows an interactive map of a of GeoDataFrames clipped to the mask extent.
 
-    return gdf
+    It takes all the GeoDataFrames specified, clips them to the extent of the mask,
+    and displays the resulting geometries in an interactive map with a common legends.
+    The layers can be toggled on and off.
 
+    For more info about the labeling and coloring of the map, see the explore function.
 
-def random_points(n: int, loc: float | int = 0.5) -> GeoDataFrame:
-    """Creates a GeoDataFrame with n random points.
+    Note:
+        The maximum zoom level only works on the OpenStreetMap background map.
 
     Args:
-        n: Number of points/rows to create.
-        loc: Mean ('centre') of the distribution.
-
-    Returns:
-        A GeoDataFrame of points with n rows.
+        *gdfs: one or more GeoDataFrames.
+        mask: the geometry to clip the data by.
+        column: The column to color the geometries by. Defaults to None, which means
+            each GeoDataFrame will get a unique color.
+        labels: By default, the GeoDataFrames will be labeled by their object names.
+            Alternatively, labels can be specified as a tuple of strings the same
+            length as the number of gdfs.
+        max_zoom: The maximum allowed level of zoom. Higher number means more zoom
+            allowed. Defaults to 30, which is higher than the geopandas default.
+        smooth_factor: How much to simplify the geometries. 1 is the minimum,
+            5 is quite a lot of simplification.
+        explore: If True (default), an interactive map will be displayed. If False,
+            or not in Jupyter, a static plot will be shown.
+        browser: If False (default), the maps will be shown in Jupyter.
+            If True the maps will be opened in a browser folder.
+        **kwargs: Keyword arguments to pass to geopandas.GeoDataFrame.explore, for
+            instance 'cmap' to change the colors, 'scheme' to change how the data
+            is grouped. This defaults to 'fisherjenkssampled' for numeric data.
 
-    Examples
+    See also
     --------
-    >>> from sgis import random_points
-    >>> points = random_points(10_000)
-    >>> points
-                         geometry
-    0     POINT (0.62044 0.22805)
-    1     POINT (0.31885 0.38109)
-    2     POINT (0.39632 0.61130)
-    3     POINT (0.99401 0.35732)
-    4     POINT (0.76403 0.73539)
-    ...                       ...
-    9995  POINT (0.90433 0.75080)
-    9996  POINT (0.10959 0.59785)
-    9997  POINT (0.00330 0.79168)
-    9998  POINT (0.90926 0.96215)
-    9999  POINT (0.01386 0.22935)
-    [10000 rows x 1 columns]
-
-    Values with a mean of 100.
-
-    >>> points = random_points(10_000, loc=100)
-    >>> points
-                         geometry
-    0      POINT (50.442 199.729)
-    1       POINT (26.450 83.367)
-    2     POINT (111.054 147.610)
-    3      POINT (93.141 141.456)
-    4       POINT (94.101 24.837)
-    ...                       ...
-    9995   POINT (174.344 91.772)
-    9996    POINT (95.375 11.391)
-    9997    POINT (45.694 60.843)
-    9998   POINT (73.261 101.881)
-    9999  POINT (134.503 168.155)
-    [10000 rows x 1 columns]
+    explore: same functionality, but shows the entire area of the geometries.
+    samplemap: same functionality, but shows only a random area of a given size.
     """
-    if isinstance(n, (str, float)):
-        n = int(n)
 
-    x = np.random.rand(n) * float(loc) * 2
-    y = np.random.rand(n) * float(loc) * 2
+    gdfs, column = Explore._separate_args(gdfs, column)
 
-    return GeoDataFrame(
-        (Point(x, y) for x, y in zip(x, y, strict=True)), columns=["geometry"]
+    clipped, kwargs = _prepare_clipmap(
+        *gdfs,
+        mask=mask,
+        labels=labels,
+        **kwargs,
     )
 
+    center = kwargs.pop("center", None)
+    size = kwargs.pop("size", None)
 
-def points_in_bounds(gdf: GeoDataFrame | GeoSeries, n2: int):
-    minx, miny, maxx, maxy = gdf.total_bounds
-    xs = np.linspace(minx, maxx, num=n2)
-    ys = np.linspace(miny, maxy, num=n2)
-    x_coords, y_coords = np.meshgrid(xs, ys, indexing="ij")
-    coords = np.concatenate((x_coords.reshape(-1, 1), y_coords.reshape(-1, 1)), axis=1)
-    return to_gdf(coords, crs=gdf.crs)
-
-
-def to_lines(*gdfs: GeoDataFrame, copy: bool = True) -> GeoDataFrame:
-    """Makes lines out of one or more GeoDataFrames and splits them at intersections.
-
-    The GeoDataFrames' geometries are converted to LineStrings, then unioned together
-    and made to singlepart. The lines are split at the intersections. Mimics
-    'feature to line' in ArcGIS.
-
-    Args:
-        *gdfs: one or more GeoDataFrames.
-        copy: whether to take a copy of the incoming GeoDataFrames. Defaults to True.
-
-    Returns:
-        A GeoDataFrame with singlepart line geometries and columns of all input
-            GeoDataFrames.
-
-    Note:
-        The index is preserved if only one GeoDataFrame is given, but otherwise
-        ignored. This is because the union overlay used if multiple GeoDataFrames
-        always ignores the index.
-
-    Examples
-    --------
-    Convert single polygon to linestring.
-
-    >>> import sgis as sg
-    >>> from shapely.geometry import Polygon
-    >>> poly1 = sg.to_gdf(Polygon([(0, 0), (0, 1), (1, 1), (1, 0)]))
-    >>> poly1["poly1"] = 1
-    >>> line = sg.to_lines(poly1)
-    >>> line
-                                                geometry  poly1
-    0  LINESTRING (0.00000 0.00000, 0.00000 1.00000, ...      1
-
-    Convert two overlapping polygons to linestrings.
-
-    >>> poly2 = sg.to_gdf(Polygon([(0.5, 0.5), (0.5, 1.5), (1.5, 1.5), (1.5, 0.5)]))
-    >>> poly2["poly2"] = 1
-    >>> lines = sg.to_lines(poly1, poly2)
-    >>> lines
-    poly1  poly2                                           geometry
-    0    1.0    NaN  LINESTRING (0.00000 0.00000, 0.00000 1.00000, ...
-    1    1.0    NaN  LINESTRING (0.50000 1.00000, 1.00000 1.00000, ...
-    2    1.0    NaN  LINESTRING (1.00000 0.50000, 1.00000 0.00000, ...
-    3    NaN    1.0      LINESTRING (0.50000 0.50000, 0.50000 1.00000)
-    4    NaN    1.0  LINESTRING (0.50000 1.00000, 0.50000 1.50000, ...
-    5    NaN    1.0      LINESTRING (1.00000 0.50000, 0.50000 0.50000)
-
-    Plot before and after.
-
-    >>> sg.qtm(poly1, poly2)
-    >>> lines["l"] = lines.length
-    >>> sg.qtm(lines, "l")
-    """
-
-    if any(any(gdf.geom_type.isin(["Point", "MultiPoint"])) for gdf in gdfs):
-        raise ValueError("Cannot convert points to lines.")
-
-    def _shapely_geometry_to_lines(geom):
-        if geom.area == 0:
-            return geom
-
-        singlepart = get_parts(geom)
-        lines = []
-        for part in singlepart:
-            exterior_ring = get_exterior_ring(part)
-            lines.append(exterior_ring)
-
-            n_interior_rings = get_num_interior_rings(part)
-            if not (n_interior_rings):
-                continue
-
-            interior_rings = [
-                LineString(get_interior_ring(part, n)) for n in range(n_interior_rings)
-            ]
-
-            lines = lines + interior_rings
-
-        return unary_union(lines)
-
-    lines = []
-    for gdf in gdfs:
-        if copy:
-            gdf = gdf.copy()
-
-        gdf[gdf._geometry_column_name] = gdf[gdf._geometry_column_name].map(
-            _shapely_geometry_to_lines
+    if explore:
+        m = Explore(
+            *clipped,
+            column=column,
+            labels=labels,
+            browser=browser,
+            max_zoom=max_zoom,
+            smooth_factor=smooth_factor,
+            **kwargs,
         )
+        m.explore(center=center, size=size)
+    else:
+        m = Map(
+            *gdfs,
+            column=column,
+            labels=labels,
+            **kwargs,
+        )
+        qtm(m._gdf, column=m.column, cmap=m._cmap, k=m.k)
 
-        gdf = to_single_geom_type(gdf, "line")
-
-        lines.append(gdf)
 
-    if len(lines) == 1:
-        return lines[0]
+def qtm(
+    *gdfs: GeoDataFrame,
+    column: str | None = None,
+    title: str | None = None,
+    black: bool = True,
+    size: int = 10,
+    legend: bool = True,
+    cmap: str | None = None,
+    k: int = 5,
+    **kwargs,
+) -> None:
+    """Quick, thematic map of one or more GeoDataFrames.
 
-    if len(lines[0]) and len(lines[1]):
-        unioned = lines[0].overlay(lines[1], how="union", keep_geom_type=True)
-    else:
-        unioned = pd.concat([lines[0], lines[1]], ignore_index=True)
+    Shows one or more GeoDataFrames in the same plot, with a common color scheme if
+    column is specified, otherwise with unique colors for each GeoDataFrame.
 
-    if len(lines) > 2:
-        for line_gdf in lines[2:]:
-            if len(line_gdf):
-                unioned = unioned.overlay(line_gdf, how="union", keep_geom_type=True)
-            else:
-                unioned = pd.concat([unioned, line_gdf], ignore_index=True)
+    The 'qtm' name is taken from the tmap package in R.
 
-    return make_all_singlepart(unioned, ignore_index=True)
+    Args:
+        *gdfs: One or more GeoDataFrames to plot.
+        column: The column to color the map by. Defaults to None, meaning each
+            GeoDataFrame is given a unique color.
+        title: Text to use as the map's heading.
+        black: If True (default), the background color will be black and the title
+            white. If False, it will be the opposite. The colormap will also be
+            'viridis' when black, and 'RdPu' when white.
+        size: Size of the plot. Defaults to 10.
+        title_fontsize: Size of the title.
+        cmap: Color palette of the map. See:
+            https://matplotlib.org/stable/tutorials/colors/colormaps.html
+        k: Number of color groups.
+        **kwargs: Additional keyword arguments taken by the geopandas plot method.
 
+    See also:
+        ThematicMap: Class with more options for customising the plot.
+    """
 
-def clean_clip(
-    gdf: GeoDataFrame | GeoSeries,
-    mask: GeoDataFrame | GeoSeries | Geometry,
-    **kwargs,
-) -> GeoDataFrame | GeoSeries:
-    """Clips geometries to the mask extent and cleans the geometries.
+    m = ThematicMap(*gdfs, column=column, size=size, black=black)
 
-    Geopandas.clip does a fast and durty clipping, with no guarantee for valid outputs.
-    Here, the clipped geometries are made valid, and then empty, NaN and invalid
-    geometries are removed.
+    m.title = title
 
-    Args:
-        gdf: GeoDataFrame or GeoSeries to be clipped
-        mask: the geometry to clip gdf
-        **kwargs: Additional keyword arguments passed to GeoDataFrame.clip
+    if k and len(m._unique_values) >= k:
+        m.k = k
 
-    Returns:
-        The cleanly clipped GeoDataFrame.
+    if cmap:
+        m.change_cmap(
+            cmap, start=kwargs.pop("cmap_start", 0), stop=kwargs.pop("cmap_stop", 256)
+        )
 
-    Raises:
-        TypeError: If gdf is not of type GeoDataFrame or GeoSeries.
-    """
-    if not isinstance(gdf, (GeoDataFrame, GeoSeries)):
-        raise TypeError(f"'gdf' should be GeoDataFrame or GeoSeries, got {type(gdf)}")
+    if not legend:
+        m.legend = None
 
-    try:
-        return gdf.clip(mask, **kwargs).pipe(clean_geoms)
-    except Exception:
-        gdf = clean_geoms(gdf)
-        mask = clean_geoms(mask)
-        return gdf.clip(mask, **kwargs).pipe(clean_geoms)
+    m.plot(**kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ssb_sgis-0.2.8/src/sgis/geopandas_tools/geometry_types.py` & `ssb_sgis-0.3.0/src/sgis/geopandas_tools/geometry_types.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.8/src/sgis/geopandas_tools/neighbors.py` & `ssb_sgis-0.3.0/src/sgis/geopandas_tools/neighbors.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.8/src/sgis/geopandas_tools/overlay.py` & `ssb_sgis-0.3.0/src/sgis/geopandas_tools/overlay.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.8/src/sgis/geopandas_tools/point_operations.py` & `ssb_sgis-0.3.0/src/sgis/geopandas_tools/point_operations.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.8/src/sgis/geopandas_tools/polygon_operations.py` & `ssb_sgis-0.3.0/src/sgis/geopandas_tools/polygon_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 """Functions for polygon geometries."""
-import functools
 import warnings
 
-import geopandas as gpd
 import networkx as nx
-import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame, GeoSeries
 from shapely import (
     area,
-    difference,
     get_exterior_ring,
     get_interior_ring,
     get_num_interior_rings,
     get_parts,
     polygons,
 )
 from shapely.ops import unary_union
 
 from .general import _push_geom_col, to_lines
 from .neighbors import get_neighbor_indices
 from .overlay import clean_overlay
 
 
+def get_centroid_ids(gdf: GeoDataFrame, groupby: str) -> pd.Series:
+    centerpoints = gdf.assign(geometry=lambda x: x.centroid)
+
+    grouped_centerpoints = centerpoints.dissolve(by=groupby).assign(
+        geometry=lambda x: x.centroid
+    )
+    xs = grouped_centerpoints.geometry.x
+    ys = grouped_centerpoints.geometry.y
+
+    grouped_centerpoints["wkt"] = [f"{int(x)}_{int(y)}" for x, y in zip(xs, ys)]
+
+    return gdf[groupby].map(grouped_centerpoints["wkt"])
+
+
 def get_polygon_clusters(
     *gdfs: GeoDataFrame | GeoSeries,
     cluster_col: str = "cluster",
     allow_multipart: bool = False,
+    wkt_col: bool = False,
 ) -> GeoDataFrame | tuple[GeoDataFrame]:
     """Find which polygons overlap without dissolving.
 
     Devides polygons into clusters in a fast and precice manner by using spatial join
     and networkx to find the connected components, i.e. overlapping geometries.
     If multiple GeoDataFrames are given, the clusters will be based on all
     combined.
@@ -41,14 +52,17 @@
     polygons overlap.
 
     Args:
         gdfs: One or more GeoDataFrames of polygons.
         cluster_col: Name of the resulting cluster column.
         allow_multipart: Whether to allow mutipart geometries in the gdfs.
             Defaults to False to avoid confusing results.
+        wkt_col: Whether to return the cluster column values as a string with x and y
+            coordinates. Convinient to always get unique ids.
+            Defaults to False because of speed.
 
     Returns:
         One or more GeoDataFrames (same amount as was given) with a new cluster column.
 
     Examples
     --------
 
@@ -105,16 +119,25 @@
     0        0  POLYGON ((0.99951 -0.03141, 0.99803 -0.06279, ...
     1        1  POLYGON ((4.99951 2.96859, 4.99803 2.93721, 4....
     2        2  POLYGON ((8.00000 7.00000, 7.99951 6.96859, 7....
     """
     if isinstance(gdfs[-1], str):
         *gdfs, cluster_col = gdfs
 
-    concated = pd.DataFrame()
+    concated = []
     orig_indices = ()
+
+    # take a copy only if there are gdfs with the same id
+    # To not get any overwriting in the for loop
+    if sum(df1 is df2 for df1 in gdfs for df2 in gdfs) > len(gdfs):
+        new_gdfs = ()
+        for gdf in gdfs:
+            new_gdfs = new_gdfs + (gdf.copy(),)
+        gdfs = new_gdfs
+
     for i, gdf in enumerate(gdfs):
         if isinstance(gdf, GeoSeries):
             gdf = gdf.to_frame()
 
         if not isinstance(gdf, GeoDataFrame):
             raise TypeError("'gdfs' should be GeoDataFrames or GeoSeries.")
 
@@ -125,15 +148,20 @@
                 "To allow multipart geometries, set allow_multipart=True"
             )
 
         orig_indices = orig_indices + (gdf.index,)
 
         gdf["i__"] = i
 
-        concated = pd.concat([concated, gdf], ignore_index=True)
+        concated.append(gdf)
+
+    concated = pd.concat(concated, ignore_index=True)
+
+    if not len(concated):
+        return concated.drop("i__", axis=1).assign(**{cluster_col: []})
 
     neighbors = get_neighbor_indices(concated, concated)
 
     edges = [(source, target) for source, target in neighbors.items()]
 
     graph = nx.Graph()
     graph.add_edges_from(edges)
@@ -142,14 +170,17 @@
         j: i
         for i, component in enumerate(nx.connected_components(graph))
         for j in component
     }
 
     concated[cluster_col] = component_mapper
 
+    if wkt_col:
+        concated[cluster_col] = get_centroid_ids(concated, groupby=cluster_col)
+
     concated = _push_geom_col(concated)
 
     n_gdfs = concated["i__"].unique()
 
     if len(n_gdfs) == 1:
         concated.index = orig_indices[0]
         return concated.drop(["i__"], axis=1)
```

### Comparing `ssb_sgis-0.2.8/src/sgis/geopandas_tools/to_geodataframe.py` & `ssb_sgis-0.3.0/src/sgis/geopandas_tools/to_geodataframe.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import numbers
 from collections.abc import Iterator, Sized
 
 import geopandas as gpd
+import numpy as np
 import pandas as pd
 import shapely
 from geopandas import GeoDataFrame, GeoSeries
 from pandas.api.types import is_array_like, is_dict_like, is_list_like
 from shapely import Geometry, box, wkb, wkt
 from shapely.geometry import Point
 from shapely.ops import unary_union
 
 
 def to_gdf(
-    geom: Geometry
+    obj: Geometry
     | str
     | bytes
     | list
     | tuple
     | dict
     | GeoSeries
     | pd.Series
@@ -27,32 +28,32 @@
     **kwargs,
 ) -> GeoDataFrame:
     """Converts geometry-like objects to a GeoDataFrame.
 
     Constructs a GeoDataFrame from any geometry-like object (coordinates, wkt, wkb),
     or any interable of such objects.
 
-    If geom is a DataFrame or dictionary, geometries can be in one column/key or 2-3
+    If obj is a DataFrame or dictionary, geometries can be in one column/key or 2-3
     if coordiantes are in x and x (and z) columns. The column/key "geometry" is used
     by default if it exists. The index and other columns/keys are preserved.
 
     Args:
-        geom: the object to be converted to a GeoDataFrame.
+        obj: the object to be converted to a GeoDataFrame.
         crs: if None (default), it uses the crs of the GeoSeries if GeoSeries
             is the input type. Otherwise, no crs is used.
-        geometry: Name of column(s) or key(s) in geom with geometry-like values.
+        geometry: Name of column(s) or key(s) in obj with geometry-like values.
             If not specified, the key/column 'geometry' will be used if it
             exists. If multiple columns, can be given as e.g. "xyz" or ["x", "y"].
         **kwargs: additional keyword arguments taken by the GeoDataFrame constructor.
 
     Returns:
         A GeoDataFrame with one column, the geometry column.
 
     Raises:
-        TypeError: If geom is a GeoDataFrame.
+        TypeError: If obj is a GeoDataFrame.
 
     Examples
     --------
     >>> from sgis import to_gdf
     >>> coords = (10, 60)
     >>> to_gdf(coords, crs=4326)
                         geometry
@@ -121,256 +122,291 @@
                              geometry
     0  POINT Z (82.000 88.000 82.000)
     1  POINT Z (70.000 92.000 20.000)
     2   POINT Z (91.000 34.000 3.000)
     3   POINT Z (1.000 50.000 77.000)
     4  POINT Z (58.000 49.000 46.000)
     """
-    if isinstance(geom, GeoDataFrame):
+    if isinstance(obj, GeoDataFrame):
         raise TypeError("'to_gdf' doesn't accept GeoDataFrames as input type.")
 
-    if isinstance(geom, GeoSeries):
-        geom_col = geometry if geometry else "geometry"
-        return _geoseries_to_gdf(geom, geom_col, crs, **kwargs)
-
-    geom_col = _find_geometry_column(geom, geometry)
-    index = kwargs.get("index", None)
-
-    if is_array_like(geom_col):
-        geometry = GeoSeries((_make_one_shapely_geom(g) for g in geometry), index=index)
-        return GeoDataFrame(geom, geometry=geometry, crs=crs, **kwargs)
-
-    # get done with the iterators that get consumed by 'all' statements
-    if isinstance(geom, Iterator) and not isinstance(geom, Sized):
-        geom = GeoSeries((_make_one_shapely_geom(g) for g in geom), index=index)
-        return GeoDataFrame({geom_col: geom}, geometry=geom_col, crs=crs, **kwargs)
-
-    if not is_dict_like(geom):
-        if not hasattr(geom, "__iter__") and hasattr(geom, "__dict__"):
-            if all(attr in geom.__dict__ for attr in ["minx", "miny", "maxx", "maxy"]):
-                geom = GeoSeries(
-                    shapely.box(*(geom.minx, geom.miny, geom.maxx, geom.maxy)),
-                    index=index,
-                )
-                return GeoDataFrame(
-                    {geom_col: geom}, geometry=geom_col, crs=crs, **kwargs
-                )
-        if hasattr(geom, "__iter__") and all(isinstance(g, dict) for g in geom):
-            crs = crs if crs else _get_crs(geom)
-            geom = pd.concat(GeoSeries(_from_json(g)) for g in geom)
+    if isinstance(obj, GeoSeries):
+        geom_col = geometry or "geometry"
+        return _geoseries_to_gdf(obj, geom_col, crs, **kwargs)
+
+    if is_array_like(geometry) and len(geometry) == len(obj):
+        geometry = GeoSeries(_make_one_shapely_geom(g) for g in geometry)
+        return GeoDataFrame(obj, geometry=geometry, crs=crs, **kwargs)
+
+    geom_col: str = find_geometry_column(obj, geometry)
+    index = kwargs.pop("index", None)
+
+    # get done with iterators that get consumed by 'all'
+    if isinstance(obj, Iterator) and not isinstance(obj, Sized):
+        obj = GeoSeries((_make_one_shapely_geom(g) for g in obj), index=index)
+        return GeoDataFrame({geom_col: obj}, geometry=geom_col, crs=crs, **kwargs)
+
+    crs = crs or get_crs_from_dict(obj)
+
+    if not is_dict_like(obj):
+        if is_boundingbox(obj):
+            obj = GeoSeries(shapely.box(*obj), index=index)
+            return GeoDataFrame({geom_col: obj}, geometry=geom_col, crs=crs, **kwargs)
+        if is_nested_geojson(obj):
+            # crs = crs or get_crs_from_dict(obj)
+            obj = pd.concat((GeoSeries(_from_json(g)) for g in obj), ignore_index=True)
             if index is not None:
-                geom.index = index
-            else:
-                geom = geom.reset_index(drop=True)
-            return GeoDataFrame({geom_col: geom}, geometry=geom_col, crs=crs, **kwargs)
+                obj.index = index
+            return GeoDataFrame({geom_col: obj}, geometry=geom_col, crs=crs, **kwargs)
+        # list etc.
         else:
-            geom = GeoSeries(_make_shapely_geoms(geom), index=index)
-            return GeoDataFrame({geom_col: geom}, geometry=geom_col, crs=crs, **kwargs)
+            obj = GeoSeries(make_shapely_geoms(obj), index=index)
+            return GeoDataFrame(
+                {geom_col: obj}, geometry=geom_col, index=index, crs=crs, **kwargs
+            )
 
     # now we have dict, Series or DataFrame
 
-    geom = geom.copy()
+    obj = obj.copy()
+
+    # preserve Series/DataFrame index
+    index = obj.index if hasattr(obj, "index") and index is None else index
 
-    # preserve Series/DataFrame index, overrides kwargs for now
-    index = geom.index if hasattr(geom, "index") else kwargs.get("index", None)
+    if geom_col in obj.keys():
+        if isinstance(obj, pd.DataFrame):
+            obj[geom_col] = GeoSeries(make_shapely_geoms(obj[geom_col]), index=index)
+            return GeoDataFrame(obj, geometry=geom_col, crs=crs, **kwargs)
+        if isinstance(obj[geom_col], Geometry):
+            return GeoDataFrame(
+                dict(obj), geometry=geom_col, crs=crs, index=[0], **kwargs
+            )
+        if not hasattr(obj[geom_col], "__iter__") or len(obj[geom_col]) == 1:
+            obj[geom_col] = make_shapely_geoms(obj[geom_col])
+            return GeoDataFrame(
+                dict(obj), geometry=geom_col, crs=crs, index=index, **kwargs
+            )
+        obj[geom_col] = GeoSeries(make_shapely_geoms(obj[geom_col]), index=index)
+        return GeoDataFrame(dict(obj), geometry=geom_col, crs=crs, **kwargs)
 
-    if geom_col in geom.keys():
-        geom[geom_col] = GeoSeries(_make_shapely_geoms(geom[geom_col]), index=index)
-        return GeoDataFrame(geom, geometry=geom_col, crs=crs, **kwargs)
-
-    if geometry and all(g in geom for g in geometry):
-        geom[geom_col] = _geoseries_from_xyz(geom, geometry, index=index)
-        return GeoDataFrame(geom, geometry=geom_col, crs=crs, **kwargs)
-
-    if len(geom.keys()) == 1:
-        key = list(geom.keys())[0]
-        if isinstance(geom, dict):
+    if geometry and all(g in obj for g in geometry):
+        obj[geom_col] = _geoseries_from_xyz(obj, geometry, index=index)
+        return GeoDataFrame(obj, geometry=geom_col, crs=crs, **kwargs)
+
+    if len(obj.keys()) == 1:
+        key = list(obj.keys())[0]
+        if isinstance(obj, dict):
             geoseries = GeoSeries(
-                _make_shapely_geoms(list(geom.values())[0]), index=index
+                make_shapely_geoms(list(obj.values())[0]), index=index
             )
-        elif isinstance(geom, pd.Series):
-            geoseries = GeoSeries(_make_shapely_geoms(geom), index=index)
+        elif isinstance(obj, pd.Series):
+            geoseries = GeoSeries(make_shapely_geoms(obj), index=index)
         else:
-            geoseries = GeoSeries(_make_shapely_geoms(geom.iloc[:, 0]), index=index)
+            geoseries = GeoSeries(make_shapely_geoms(obj.iloc[:, 0]), index=index)
         return GeoDataFrame({key: geoseries}, geometry=key, crs=crs, **kwargs)
 
-    if geometry and geom_col not in geom or isinstance(geom, pd.DataFrame):
+    if geometry and geom_col not in obj or isinstance(obj, pd.DataFrame):
         raise ValueError("Cannot find geometry column(s)", geometry)
 
     # geojson, __geo_interface__
     if (
-        isinstance(geom, dict)
-        and sum(key in geom for key in ["type", "coordinates", "features"]) >= 2
+        isinstance(obj, dict)
+        and sum(key in obj for key in ["type", "coordinates", "features"]) >= 2
     ):
-        if "geometry" in geom:
+        if "geometry" in obj:
             geometry = "geometry"
 
-        crs = crs if crs else _get_crs(geom)
-        print(crs)
-        geom = GeoSeries(_from_json(geom), index=index)
-        return GeoDataFrame({geom_col: geom}, geometry=geom_col, crs=crs, **kwargs)
+        # crs = crs or get_crs_from_dict(obj)
+        obj = GeoSeries(_from_json(obj), index=index)
+        return GeoDataFrame({geom_col: obj}, geometry=geom_col, crs=crs, **kwargs)
 
-    geoseries = _series_like_to_geoseries(geom, index=index)
+    geoseries = _series_like_to_geoseries(obj, index=index)
     return GeoDataFrame(geometry=geoseries, crs=crs, **kwargs)
 
 
-def _get_crs(geom):
-    if not is_dict_like(geom) and is_dict_like(geom[0]):
-        crss = list({_get_crs(g) for g in geom})
-        if len(crss) == 1:
-            return crss[0]
+def make_shapely_geoms(obj):
+    if _is_one_geometry(obj):
+        return _make_one_shapely_geom(obj)
+    if isinstance(obj, dict) and "coordinates" in obj:
+        return _from_json(obj)
+    return (_make_one_shapely_geom(g) for g in obj)
+
+
+def is_boundingbox(obj) -> bool:
+    if not hasattr(obj, "__iter__"):
+        return False
+
+    classname = obj.__class__.__name__.lower()
+    if "bounding" not in classname and "box" not in classname:
+        return False
+
+    if len(obj) == 4 and all(isinstance(x, numbers.Number) for x in obj):
+        return True
+
+    return False
+
+
+def is_nested_geojson(obj) -> bool:
+    if hasattr(obj, "__iter__") and all(isinstance(g, dict) for g in obj):
+        return True
+    return False
+
+
+def get_crs_from_dict(obj):
+    if (
+        not hasattr(obj, "__iter__")
+        or not is_dict_like(obj)
+        and not is_dict_like(obj[0])
+    ):
         return None
-    if "properties" in geom:
-        return _get_crs(geom["properties"])
-    if "crs" in geom:
-        geom = geom["crs"]
-        while is_dict_like(geom):
-            if "properties" in geom:
-                geom = geom["properties"]
-            elif "name" in geom:
-                geom = geom["name"]
+
+    if not is_dict_like(obj) and is_dict_like(obj[0]):
+        crss = list({get_crs_from_dict(g) for g in obj})
+        return crss[0] if len(crss) == 1 else None
+
+    if "properties" in obj:
+        return get_crs_from_dict(obj["properties"])
+
+    if "crs" in obj:
+        obj = obj["crs"]
+        while is_dict_like(obj):
+            if "properties" in obj:
+                obj = obj["properties"]
+            elif "name" in obj:
+                obj = obj["name"]
             else:
                 return None
-        return geom
+        return obj
+
     return None
 
 
-def _from_json(geom: dict):
-    if not isinstance(geom, dict) and isinstance(geom[0], dict):
-        return [_from_json(g) for g in geom]
-    if "geometry" in geom:
-        return _from_json(geom["geometry"])
-    if "features" in geom:
-        return _from_json(geom["features"])
-    coords = geom["coordinates"]
-    constructor = eval("shapely.geometry." + geom.get("type", Point))
+def _from_json(obj: dict):
+    if not isinstance(obj, dict) and isinstance(obj[0], dict):
+        return [_from_json(g) for g in obj]
+    if "geometry" in obj:
+        return _from_json(obj["geometry"])
+    if "features" in obj:
+        return _from_json(obj["features"])
+    coords = obj["coordinates"]
+    constructor = eval("shapely.geometry." + obj.get("type", Point))
     try:
         return constructor(coords)
     except TypeError:
         while len(coords) == 1:
             coords = coords[0]
         return constructor(coords)
 
 
-def _series_like_to_geoseries(geom, index):
+def _series_like_to_geoseries(obj, index):
     if index is None:
-        index = geom.keys()
-    if isinstance(geom, dict):
-        return GeoSeries(_make_shapely_geoms(list(geom.values())), index=index)
+        index = obj.keys()
+    if isinstance(obj, dict):
+        return GeoSeries(make_shapely_geoms(list(obj.values())), index=index)
     else:
-        return GeoSeries(_make_shapely_geoms(geom.values), index=index)
+        return GeoSeries(make_shapely_geoms(obj.values), index=index)
 
 
-def _geoseries_to_gdf(geom: GeoSeries, geometry, crs, **kwargs) -> GeoDataFrame:
+def _geoseries_to_gdf(obj: GeoSeries, geometry, crs, **kwargs) -> GeoDataFrame:
     if not crs:
-        crs = geom.crs
+        crs = obj.crs
     else:
-        geom = geom.to_crs(crs) if geom.crs else geom.set_crs(crs)
+        obj = obj.to_crs(crs) if obj.crs else obj.set_crs(crs)
 
-    return GeoDataFrame({geometry: geom}, geometry=geometry, crs=crs, **kwargs)
+    return GeoDataFrame({geometry: obj}, geometry=geometry, crs=crs, **kwargs)
 
 
-def _find_geometry_column(geom, geometry) -> str:
+def find_geometry_column(obj, geometry) -> str:
     if geometry is None:
         return "geometry"
 
-    if not is_list_like(geometry) and geometry in geom:
+    # dict key
+    if not is_list_like(geometry) and geometry in obj:
         return geometry
 
-    if len(geometry) == 1 and geometry[0] in geom:
+    # nested dict key
+    if len(geometry) == 1 and geometry[0] in obj:
         return geometry[0]
 
-    if len(geometry) == 2 or len(geometry) == 3:
+    if len(geometry) in {2, 3}:
         return "geometry"
 
-    if is_array_like(geometry) and len(geometry) == len(geom):
-        return geometry
-
     raise ValueError(
         "geometry should be a geometry column or x, y (z) coordinate columns."
     )
 
 
-def _geoseries_from_xyz(geom, geometry, index) -> GeoSeries:
+def _geoseries_from_xyz(obj, geometry, index) -> GeoSeries:
     """Make geoseries from the geometry column or columns (x y (z))."""
 
     if len(geometry) == 2:
         x, y = geometry
         z = None
 
     elif len(geometry) == 3:
         x, y, z = geometry
-        z = geom[z]
+        z = obj[z]
 
     else:
         raise ValueError(
             "geometry should be a geometry column or x, y (z) coordinate columns."
         )
 
-    return gpd.GeoSeries.from_xy(x=geom[x], y=geom[y], z=z, index=index)
+    return gpd.GeoSeries.from_xy(x=obj[x], y=obj[y], z=z, index=index)
 
 
-def _is_one_geometry(geom) -> bool:
+def _is_one_geometry(obj) -> bool:
     if (
-        isinstance(geom, (str, bytes, Geometry))
-        or all(isinstance(i, numbers.Number) for i in geom)
-        or not hasattr(geom, "__iter__")
+        isinstance(obj, (str, bytes, Geometry))
+        or all(isinstance(i, numbers.Number) for i in obj)
+        or not hasattr(obj, "__iter__")
     ):
         return True
     return False
 
 
-def _make_shapely_geoms(geom):
-    if _is_one_geometry(geom):
-        return _make_one_shapely_geom(geom)
-    if isinstance(geom, dict) and "coordinates" in geom:
-        return _from_json(geom)
-    return (_make_one_shapely_geom(g) for g in geom)
-
-
-def _make_one_shapely_geom(geom):
+def _make_one_shapely_geom(obj):
     """Create shapely geometry from wkt, wkb or coordinate tuple.
 
     Works recursively if the object is a nested iterable.
     """
-    if isinstance(geom, str):
-        return wkt.loads(geom)
+    if isinstance(obj, str):
+        return wkt.loads(obj)
 
-    if isinstance(geom, bytes):
-        return wkb.loads(geom)
+    if isinstance(obj, bytes):
+        return wkb.loads(obj)
 
-    if isinstance(geom, Geometry):
-        return geom
+    if isinstance(obj, Geometry):
+        return obj
 
-    if not hasattr(geom, "__iter__"):
+    if not hasattr(obj, "__iter__"):
         raise ValueError(
-            f"Couldn't create shapely geometry from {geom} of type {type(geom)}"
+            f"Couldn't create shapely geometry from {obj} of type {type(obj)}"
         )
 
-    if isinstance(geom, GeoSeries):
+    if isinstance(obj, GeoSeries):
         raise TypeError(
             "to_gdf doesn't accept iterable of GeoSeries. Instead use: "
-            "pd.concat(to_gdf(geom) for geom in geoseries_iterable)"
+            "pd.concat(to_gdf(obj) for obj in geoseries_iterable)"
         )
 
-    if not any(isinstance(g, numbers.Number) for g in geom):
+    if not any(isinstance(g, numbers.Number) for g in obj):
         # we're likely dealing with a nested iterable, so let's
         # recursively dig down to the coords/wkt/wkb
-        if len(geom) == 2 or len(geom) == 3:
+        if len(obj) == 2 or len(obj) == 3:
             try:
-                geom = [float(g) for g in geom]
-                return Point(geom)
+                obj = [float(g) for g in obj]
+                return Point(obj)
             except Exception:
                 pass
-        return unary_union([_make_one_shapely_geom(g) for g in geom])
+        return unary_union([_make_one_shapely_geom(g) for g in obj])
 
-    elif len(geom) == 2 or len(geom) == 3:
-        return Point(geom)
+    elif len(obj) == 2 or len(obj) == 3:
+        return Point(obj)
 
-    elif len(geom) == 4:
-        return box(*geom)
+    elif len(obj) == 4:
+        return box(*obj)
     else:
         raise ValueError(
             "If 'geom' is an iterable, each item should consist of "
             "wkt, wkb or (x, y (z) or bbox). Got ",
-            geom,
+            obj,
         )
```

### Comparing `ssb_sgis-0.2.8/src/sgis/helpers.py` & `ssb_sgis-0.3.0/src/sgis/helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,45 @@
 """Small helper functions."""
 import inspect
 import warnings
 
 from geopandas import GeoDataFrame
 
 
+def dict_zip_intersection(*dicts):
+    """From mCoding (YouTube)."""
+    if not dicts:
+        return
+
+    keys = set(dicts[0]).intersection(*dicts[1:])
+    for key in keys:
+        yield key, *(d[key] for d in dicts)
+
+
+def dict_zip(*dicts):
+    """From mCoding (YouTube)."""
+    if not dicts:
+        return
+
+    n = len(dicts[0])
+    if any(len(d) != n for d in dicts):
+        raise ValueError("arguments must have the same length")
+
+    for key, first_val in dicts[0].items():
+        yield key, first_val, *(other[key] for other in dicts[1:])
+
+
+def in_jupyter():
+    try:
+        get_ipython
+        return True
+    except NameError:
+        return False
+
+
 def return_two_vals(
     vals: tuple[str | None, str | None] | list[str] | str | int | float
 ) -> tuple[str | int | float, str | int | float | None]:
     """Return a two-length tuple from a str/int/float or list/tuple of length 1 or 2.
 
     Returns 'vals' as a 2-length tuple. If the input is a string, return
     a tuple of two strings. If the input is a list or tuple of two
```

### Comparing `ssb_sgis-0.2.8/src/sgis/maps/examine.py` & `ssb_sgis-0.3.0/src/sgis/maps/examine.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.8/src/sgis/maps/explore.py` & `ssb_sgis-0.3.0/src/sgis/maps/explore.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,32 +111,32 @@
             self.browser = kwargs.pop("in_browser")
 
         super().__init__(*gdfs, column=column, **kwargs)
 
         # remove columns not renerable by leaflet (list columns etc.)
         new_gdfs = []
         for gdf in self.gdfs:
-            cols_to_keep = [
-                col
-                for col in gdf.columns
-                if isinstance(gdf[col].iloc[0], (Number, str, Geometry))
-            ]
-            new_gdfs.append(gdf[cols_to_keep])
+            for col in gdf.columns:
+                if not len(gdf.loc[gdf[col].notna()]):
+                    continue
+                if not isinstance(
+                    gdf.loc[gdf[col].notna(), col].iloc[0], (Number, str, Geometry)
+                ):
+                    gdf = gdf.drop(col, axis=1)
+            new_gdfs.append(gdf)
         self._gdfs = new_gdfs
 
         self.popup = popup
         self.max_zoom = max_zoom
         self.smooth_factor = smooth_factor
         self.prefer_canvas = prefer_canvas
         self.measure_control = measure_control
         self.geocoder = geocoder
         self.save = save
 
-        self._to_single_geom_type()
-
         if self._is_categorical:
             if len(self.gdfs) == 1:
                 self._split_categories()
         else:
             if not self._cmap:
                 self._cmap = "viridis"
             self.cmap_start = kwargs.pop("cmap_start", 0)
@@ -164,15 +164,16 @@
             to_gdf(center, crs=self.crs)
             if not isinstance(center, GeoDataFrame)
             else center
         )
 
         gdfs: tuple[GeoDataFrame] = ()
         for gdf in self._gdfs:
-            gdf = gdf.clip(centerpoint.buffer(size))
+            keep_geom_type = False if get_geom_type(gdf) == "mixed" else True
+            gdf = gdf.clip(centerpoint.buffer(size), keep_geom_type=keep_geom_type)
             gdfs = gdfs + (gdf,)
         self._gdfs = gdfs
         self._gdf = pd.concat(gdfs, ignore_index=True)
 
         self._get_unique_values()
 
         self._explore(**kwargs)
@@ -267,55 +268,68 @@
             gdf = self.gdf.loc[self.gdf[self.column] == cat]
             new_gdfs.append(gdf)
             new_labels.append(cat)
         self._gdfs = new_gdfs
         self._gdf = pd.concat(new_gdfs, ignore_index=True)
         self.labels = new_labels
 
-    def _to_single_geom_type(self):
-        """Buffer gdf if mixed geometry types. Expode to singlepart.
+    def _to_single_geom_type(self, gdf) -> GeoDataFrame:
+        gdf = clean_geoms(gdf)
 
-        Because Folium does not handle mixed geometries well.
-        """
+        if get_geom_type(gdf) != "mixed":
+            return gdf
 
-        new_gdfs = []
-        for gdf in self._gdfs:
-            print(gdf)
-            if get_geom_type(gdf) == "mixed" and not unit_is_degrees(gdf):
-                gdf[gdf._geometry_column_name] = gdf.buffer(0.01)
+        geom_types = gdf.geom_type.str.lower()
+        mess = "Leaflet cannot render mixed geometry types well. "
+
+        if geom_types.str.contains("collection").any():
+            mess += "Exploding geometry collections. "
             gdf = make_all_singlepart(gdf)
-            new_gdfs.append(gdf)
-        self._gdfs = new_gdfs
-        self._gdf = pd.concat(new_gdfs, ignore_index=True)
-        self._nan_idx = self._gdf[self._column].isna()
+            geom_types = gdf.geom_type.str.lower()
+
+        if geom_types.str.contains("polygon").any():
+            mess += "Keeping only polygons."
+            gdf = to_single_geom_type(gdf, geom_type="polygon")
+
+        elif geom_types.str.contains("lin").any():
+            mess += "Keeping only lines."
+            gdf = to_single_geom_type(gdf, geom_type="line")
+
+        assert get_geom_type(gdf) != "mixed", gdf.geom_type.value_counts()
+
+        warnings.warn(mess)
+
+        return gdf
 
     def _update_column(self):
         self._is_categorical = self._check_if_categorical()
         self._fillna_if_col_is_missing()
         self._gdf = pd.concat(self._gdfs, ignore_index=True)
 
     def _create_categorical_map(self):
         self._get_categorical_colors()
 
         gdf = self._prepare_gdf_for_map(self._gdf)
         self.map = self._make_folium_map(
-            gdf,
+            bounds=gdf.total_bounds,
             max_zoom=self.max_zoom,
             popup=self.popup,
             prefer_canvas=self.prefer_canvas,
             **self.kwargs,
         )
 
         for gdf, label in zip(self._gdfs, self.labels, strict=True):
             if not len(gdf):
                 continue
 
             f = folium.FeatureGroup(name=label)
 
+            gdf = self._to_single_geom_type(gdf)
             gdf = self._prepare_gdf_for_map(gdf)
+
             gjs = self._make_geojson(
                 gdf,
                 color=gdf["color"],
                 tooltip=self._tooltip_cols(gdf),
                 popup=self.popup,
                 **{
                     key: value
@@ -345,15 +359,15 @@
             classified = self._classify_from_bins(self._gdf, bins=self.bins)
             classified_sequential = self._push_classification(classified)
             n_colors = len(np.unique(classified_sequential)) - any(self._nan_idx)
             unique_colors = self._get_continous_colors(n=n_colors)
 
         gdf = self._prepare_gdf_for_map(self._gdf)
         self.map = self._make_folium_map(
-            gdf,
+            bounds=gdf.total_bounds,
             max_zoom=self.max_zoom,
             popup=self.popup,
             prefer_canvas=self.prefer_canvas,
             **self.kwargs,
         )
 
         colorbar = bc.colormap.StepColormap(
@@ -365,18 +379,20 @@
         )
 
         for gdf, label in zip(self._gdfs, self.labels, strict=True):
             if not len(gdf):
                 continue
             f = folium.FeatureGroup(name=label)
 
+            gdf = self._to_single_geom_type(gdf)
+            gdf = self._prepare_gdf_for_map(gdf)
+
             classified = self._classify_from_bins(gdf, bins=self.bins)
             colorarray = unique_colors[classified]
 
-            gdf = self._prepare_gdf_for_map(gdf)
             gjs = self._make_geojson(
                 gdf,
                 color=colorarray,
                 tooltip=self._tooltip_cols(gdf),
                 popup=self.popup,
                 prefer_canvas=self.prefer_canvas,
                 **{
@@ -412,43 +428,30 @@
         if gdf.crs is not None and not gdf.crs.equals(4326):
             gdf = gdf.to_crs(4326)
 
         return gdf
 
     def _make_folium_map(
         self,
-        df,
+        bounds,
         attr=None,
         tiles="OpenStreetMap",
         width="100%",
         height="100%",
         control_scale=True,
-        map_kwds={},
+        map_kwds=None,
         **kwargs,
     ):
         import xyzservices
 
-        gdf = df.copy()
-
-        # convert LinearRing to LineString
-        rings_mask = gdf.geom_type == "LinearRing"
-        if rings_mask.any():
-            gdf.geometry[rings_mask] = gdf.geometry[rings_mask].apply(
-                lambda g: LineString(g)
-            )
-
-        if gdf.crs is None:
-            kwargs["crs"] = "Simple"
-            tiles = None
-        elif not gdf.crs.equals(4326):
-            gdf = gdf.to_crs(4326)
+        if not map_kwds:
+            map_kwds = {}
 
         # create folium.Map object
         # Get bounds to specify location and map extent
-        bounds = gdf.total_bounds
         location = kwargs.pop("location", None)
         if location is None:
             x = mean([bounds[0], bounds[2]])
             y = mean([bounds[1], bounds[3]])
             location = (y, x)
             if "zoom_start" in kwargs.keys():
                 fit = False
@@ -625,35 +628,14 @@
                 marker = folium.CircleMarker(**marker_kwds)
             else:
                 raise ValueError(
                     "Only 'marker', 'circle', and 'circle_marker' are "
                     "supported as marker values"
                 )
 
-        gdf = clean_geoms(gdf).pipe(make_all_singlepart)
-        if get_geom_type(gdf) == "mixed":
-            if gdf.geom_type.str.lower().str.contains("polygon").any():
-                warnings.warn(
-                    "GeoJsonTooltip is not configured to render for GeoJson "
-                    "GeometryCollection geometries. Keeping only polygons."
-                )
-                gdf = to_single_geom_type(gdf, geom_type="polygon")
-            elif gdf.geom_type.str.lower().str.contains("line").any():
-                warnings.warn(
-                    "GeoJsonTooltip is not configured to render for GeoJson "
-                    "GeometryCollection geometries. Keeping only lines."
-                )
-                gdf = to_single_geom_type(gdf, geom_type="line")
-            else:
-                warnings.warn(
-                    "GeoJsonTooltip is not configured to render for GeoJson "
-                    "GeometryCollection geometries. Keeping only points."
-                )
-                gdf = to_single_geom_type(gdf, geom_type="point")
-
         # prepare tooltip and popup
         if isinstance(gdf, GeoDataFrame):
             # add named index to the tooltip
             if gdf.index.name is not None:
                 gdf = gdf.reset_index()
             # specify fields to show in the tooltip
             tooltip = _tooltip_popup("tooltip", tooltip, gdf, **tooltip_kwds)
```

### Comparing `ssb_sgis-0.2.8/src/sgis/maps/httpserver.py` & `ssb_sgis-0.3.0/src/sgis/maps/httpserver.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.8/src/sgis/maps/legend.py` & `ssb_sgis-0.3.0/src/sgis/maps/legend.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from matplotlib.lines import Line2D
 from pandas import Series
 
-from ..geopandas_tools.general import points_in_bounds
+from ..geopandas_tools.bounds import points_in_bounds
 
 
 # the geopandas._explore raises a deprication warning. Ignoring for now.
 warnings.filterwarnings(
     action="ignore", category=matplotlib.MatplotlibDeprecationWarning
 )
 pd.options.mode.chained_assignment = None
```

### Comparing `ssb_sgis-0.2.8/src/sgis/maps/map.py` & `ssb_sgis-0.3.0/src/sgis/maps/map.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,16 @@
     7: "#00ffee",
     8: "#36d19b",
     9: "#94006b",
     10: "#750000",
     11: "#1c6b00",
 }
 
+DEFAULT_SCHEME = "quantiles"
+
 
 class Map:
     """Base class that prepares one or more GeoDataFrames for mapping.
 
     The class has no public methods.
     """
 
@@ -55,15 +57,15 @@
         *gdfs: GeoDataFrame,
         column: str | None = None,
         labels: tuple[str] | None = None,
         k: int = 5,
         bins: tuple[float] | None = None,
         nan_label: str = "Missing",
         nan_color="#c2c2c2",
-        scheme="fisherjenks",
+        scheme: str = DEFAULT_SCHEME,
         **kwargs,
     ):
         if not all(isinstance(gdf, GeoDataFrame) for gdf in gdfs):
             gdfs, column = self._separate_args(gdfs, column)
 
         self._column = column
         self.bins = bins
@@ -98,17 +100,20 @@
 
         self._gdfs = self._to_common_crs_and_one_geom_col(self._gdfs)
         self._is_categorical = self._check_if_categorical()
 
         if self._column:
             self._fillna_if_col_is_missing()
         else:
+            gdfs = []
             for gdf, label in zip(self._gdfs, self.labels, strict=True):
                 gdf["label"] = label
+                gdfs.append(gdf)
             self._column = "label"
+            self._gdfs = gdfs
 
         self._gdf = pd.concat(self._gdfs, ignore_index=True)
 
         self._nan_idx = self._gdf[self._column].isna()
         self._get_unique_values()
 
     def _get_unique_values(self):
@@ -245,26 +250,28 @@
             self._unique_values = self.nan_label
             self._k = 1
 
     def _get_labels(self, gdfs: tuple[GeoDataFrame]) -> None:
         """Putting the labels/names in a list before copying the gdfs."""
         self.labels: list[str] = []
         for i, gdf in enumerate(gdfs):
-            if hasattr(gdf, "name"):
+            if hasattr(gdf, "name") and isinstance(gdf.name, str):
                 name = gdf.name
             else:
                 name = get_name(gdf)
-                if not name:
-                    name = str(i)
+                name = name or str(i)
             self.labels.append(name)
 
     def _set_labels(self) -> None:
         """Setting the labels after copying the gdfs."""
+        gdfs = []
         for i, gdf in enumerate(self._gdfs):
             gdf["label"] = self.labels[i]
+            gdfs.append(gdf)
+        self._gdfs = gdfs
 
     def _to_common_crs_and_one_geom_col(self, gdfs: list[GeoDataFrame]):
         """Need common crs and max one geometry column."""
         crs_list = list({gdf.crs for gdf in gdfs if gdf.crs is not None})
         if crs_list:
             self.crs = crs_list[0]
         new_gdfs = []
@@ -394,15 +401,21 @@
             self._k = self._k - 1
 
         if self._k > len(self._unique_values):
             self._k = len(self._unique_values)
             n_classes = len(self._unique_values)
 
         if self.scheme == "jenks":
-            bins = jenks_breaks(gdf.loc[~self._nan_idx, column], n_classes=n_classes)
+            try:
+                bins = jenks_breaks(
+                    gdf.loc[~self._nan_idx, column], n_classes=n_classes
+                )
+                bins = self._add_minmax_to_bins(bins)
+            except Exception:
+                pass
         else:
             binning = classify(
                 np.asarray(gdf.loc[~self._nan_idx, column]),
                 scheme=self.scheme,
                 k=self._k,
             )
             bins = binning.bins
@@ -463,16 +476,29 @@
         else:
             if len(bins) == self._k + 1:
                 bins = bins[1:]
 
             if gdf[self._column].isna().all():
                 return np.repeat(len(bins), len(gdf))
 
-            # need numpy.nan instead of pd.NA as of now
+            # need numpy.nan instead of pd.NA
             gdf[self._column] = gdf[self._column].fillna(np.nan)
+
+            # also, fillna doesn't always work. So doing it manually
+            def proper_fillna(val):
+                try:
+                    if "NAType" in val.__class__.__name__:
+                        return np.nan
+                except Exception:
+                    return val
+
+                return val
+
+            gdf[self._column] = gdf[self._column].apply(proper_fillna)
+
             classified = np.searchsorted(bins, gdf[self._column])
 
         return classified
 
     def _push_classification(self, classified: np.ndarray) -> np.ndarray:
         """Push classes downwards if gaps in classification sequence.
```

### Comparing `ssb_sgis-0.2.8/src/sgis/maps/thematicmap.py` & `ssb_sgis-0.3.0/src/sgis/maps/thematicmap.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.8/src/sgis/networkanalysis/_get_route.py` & `ssb_sgis-0.3.0/src/sgis/networkanalysis/_get_route.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.8/src/sgis/networkanalysis/_od_cost_matrix.py` & `ssb_sgis-0.3.0/src/sgis/networkanalysis/_od_cost_matrix.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.8/src/sgis/networkanalysis/_points.py` & `ssb_sgis-0.3.0/src/sgis/networkanalysis/_points.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.8/src/sgis/networkanalysis/_service_area.py` & `ssb_sgis-0.3.0/src/sgis/networkanalysis/_service_area.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.8/src/sgis/networkanalysis/closing_network_holes.py` & `ssb_sgis-0.3.0/src/sgis/networkanalysis/closing_network_holes.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.8/src/sgis/networkanalysis/cutting_lines.py` & `ssb_sgis-0.3.0/src/sgis/networkanalysis/cutting_lines.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.8/src/sgis/networkanalysis/directednetwork.py` & `ssb_sgis-0.3.0/src/sgis/networkanalysis/directednetwork.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,23 +5,30 @@
 import pandas as pd
 from geopandas import GeoDataFrame
 from shapely.constructive import reverse
 
 from ..helpers import return_two_vals, unit_is_meters
 
 
-def make_directed_network_norway(gdf: GeoDataFrame) -> GeoDataFrame:
+def make_directed_network_norway(gdf: GeoDataFrame, dropnegative: bool) -> GeoDataFrame:
     """Runs the method make_directed_network for Norwegian road data.
 
     The parameters in make_directed_network are set to the correct values for
     Norwegian road data as of 2023.
 
     The data can be downloaded here:
     https://kartkatalog.geonorge.no/metadata/nvdb-ruteplan-nettverksdatasett/8d0f9066-34f9-4423-be12-8e8523089313
 
+    Args:
+        gdf: Road GeoDataFrame.
+        dropnegative: Whether to keep rows with negative minute values in both directions.
+            These are mostly circles with no impact on the analyses, but there might be
+            exceptions. Keeping negative values will cause an error when building the
+            network graph. Recode these rows to a non-negative values to keep them.
+
     Examples
     --------
     2022 data for the municipalities of Oslo and Eidskog can be read directly like this:
 
     >>> import sgis as sg
     >>> roads = sg.read_parquet_url(
     ...     "https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet"
@@ -55,41 +62,56 @@
     175620  0.007564  MULTILINESTRING Z ((268641.225 6651871.624 111...
     175621  0.020246  MULTILINESTRING Z ((268669.748 6651890.291 110...
     175622  0.036810  MULTILINESTRING Z ((268681.757 6651886.457 110...
     175623  0.003019  MULTILINESTRING Z ((268682.748 6651886.162 110...
     175624  0.036975  MULTILINESTRING Z ((268694.594 6651881.688 111...
     [175541 rows x 45 columns]
     """
-    gdf = gdf.loc[~((gdf.drivetime_fw == -1) & (gdf.drivetime_bw == -1))]
+    if gdf["drivetime_fw"].isna().any():
+        raise ValueError("Missing values in the columns 'drivetime_fw'")
+    if gdf["drivetime_bw"].isna().any():
+        raise ValueError("Missing values in the columns 'drivetime_bw'")
+
     return make_directed_network(
         gdf,
         direction_col="oneway",
         direction_vals_bft=("B", "FT", "TF"),
         minute_cols=("drivetime_fw", "drivetime_bw"),
+        dropnegative=dropnegative,
+        dropna=False,
     )
 
 
 def make_directed_network(
     gdf: GeoDataFrame,
     direction_col: str,
     direction_vals_bft: tuple[str, str, str],
+    dropna: bool | None = None,
+    dropnegative: bool | None = None,
     minute_cols: tuple[str, str] | str | None = None,
     speed_col_kmh: str | None = None,
     flat_speed_kmh: int | None = None,
     reverse_tofrom: bool = True,
 ) -> GeoDataFrame:
     """Flips the line geometries of roads going backwards and in both directions.
 
     Args:
         gdf: GeoDataFrame of line geometries.
         direction_col: name of column specifying the direction of the line
             geometry.
         direction_vals_bft: tuple or list with the values of the direction
             column. Must be in the order 'both directions', 'from', 'to'.
             E.g. ('B', 'F', 'T').
+        dropna: When minutes_cols is set, whether to drop rows with missing values
+            in both columns. Alternatively, set these rows to a positive value before
+            making the directed network.
+        dropnegative: When minutes_cols is set, whether to drop rows with negative values
+            in both columns. Not dropping them will cause an error when building a
+            network graph. Alternatively, set these rows to a positive value before
+            making the directed network.
         minute_cols (optional): column or columns containing the number of minutes
             it takes to traverse the line. If one column name is given, this will
             be used for both directions. If tuple/list with two column names,
             the first column will be used as the minute column for the forward
             direction, and the second column for roads going backwards.
         speed_col_kmh (optional): name of column with the road speed limit.
         flat_speed_kmh (optional): Speed in kilometers per hour to use as the speed for
@@ -106,41 +128,57 @@
     Raises:
         ValueError: If 'flat_speed_kmh' or 'speed_col_kmh' is specified and the unit of
             the coordinate reference system is not 'metre'.
     """
     _validate_minute_args(minute_cols, speed_col_kmh, flat_speed_kmh)
     _validate_direction_args(gdf, direction_col, direction_vals_bft)
 
+    if minute_cols is not None and any(x is None for x in [dropnegative, dropna]):
+        raise ValueError(
+            "Must specify 'dropna' and 'dropnegative' when 'minute_cols' is given."
+        )
+
+    if speed_col_kmh is not None and any(x is None for x in [dropnegative, dropna]):
+        raise ValueError(
+            "Must specify 'dropna' and 'dropnegative' when 'speed_col_kmh' is given."
+        )
+
     if (flat_speed_kmh or speed_col_kmh) and not unit_is_meters(gdf):
         raise ValueError(
             "The crs must have 'metre' as units when calculating minutes."
             "Change crs or calculate minutes manually."
         )
 
     b, f, t = direction_vals_bft
 
     if minute_cols and minute_cols != "minutes" and minute_cols[0] != "minutes":
         gdf = gdf.drop("minutes", axis=1, errors="ignore")
 
-    # select the directional and bidirectional rows.
-    ft = gdf.loc[gdf[direction_col] == f]
-    tf = gdf.loc[gdf[direction_col] == t]
-    both_ways = gdf.loc[gdf[direction_col] == b]
-    both_ways2 = both_ways.copy()
-
     if minute_cols:
         try:
             min_f, min_t = return_two_vals(minute_cols)
         except ValueError as e:
             raise ValueError(
                 "'minute_cols' should be column name (string) or tuple/list with "
                 "values of directions forwards and backwards, in that order."
             ) from e
 
-        # rename the two minute cols
+        if dropna:
+            gdf = gdf.loc[~((gdf[min_f].isna()) & (gdf[min_t].isna()))]
+        if dropnegative:
+            gdf = gdf.loc[~((gdf[min_f] < 0) & (gdf[min_t] < 0))]
+
+    # select the directional and bidirectional rows.
+    ft = gdf.loc[gdf[direction_col] == f]
+    tf = gdf.loc[gdf[direction_col] == t]
+    both_ways = gdf.loc[gdf[direction_col] == b]
+    both_ways2 = both_ways.copy()
+
+    if minute_cols:
+        # to single minute column
         both_ways = both_ways.rename(columns={min_f: "minutes"}, errors="raise")
         both_ways2 = both_ways2.rename(columns={min_t: "minutes"}, errors="raise")
 
         ft = ft.rename(columns={min_f: "minutes"}, errors="raise")
         tf = tf.rename(columns={min_t: "minutes"}, errors="raise")
 
     both_ways2.geometry = reverse(both_ways2.geometry)
```

### Comparing `ssb_sgis-0.2.8/src/sgis/networkanalysis/finding_isolated_networks.py` & `ssb_sgis-0.3.0/src/sgis/networkanalysis/finding_isolated_networks.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.8/src/sgis/networkanalysis/network.py` & `ssb_sgis-0.3.0/src/sgis/networkanalysis/network.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.8/src/sgis/networkanalysis/networkanalysis.py` & `ssb_sgis-0.3.0/src/sgis/networkanalysis/networkanalysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,16 +127,22 @@
 
     def _check_if_holes_are_nan(self):
         HOLES_ARE_NAN = (
             "Network holes have been filled by straigt lines, but the rows have "
             f"NaN values in the {self.rules.weight!r} column. Either remove NaNs "
             "or fill these values with a numeric value (e.g. 0)."
         )
-        if hasattr(self.network.gdf, "hole") and all(
-            self.network.gdf[self.network.gdf["hole"] == 1, self.rules.weight].isna()
+        if (
+            hasattr(self.network.gdf, "hole")
+            and len(self.network.gdf.loc[lambda x: x["hole"] == 1])
+            and (
+                self.network.gdf.loc[lambda x: x["hole"] == 1, self.rules.weight]
+                .isna()
+                .all()
+            )
         ):
             raise ValueError(HOLES_ARE_NAN)
 
     def od_cost_matrix(
         self,
         origins: GeoDataFrame,
         destinations: GeoDataFrame,
```

### Comparing `ssb_sgis-0.2.8/src/sgis/networkanalysis/networkanalysisrules.py` & `ssb_sgis-0.3.0/src/sgis/networkanalysis/networkanalysisrules.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.8/src/sgis/networkanalysis/nodes.py` & `ssb_sgis-0.3.0/src/sgis/networkanalysis/nodes.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.8/src/sgis/read_parquet.py` & `ssb_sgis-0.3.0/src/sgis/io/read_parquet.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.8/PKG-INFO` & `ssb_sgis-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: ssb-sgis
-Version: 0.2.8
+Version: 0.3.0
 Summary: GIS functions used at Statistics Norway.
 Home-page: https://github.com/statisticsnorway/ssb-sgis
 License: MIT
 Author: Statistics Norway
 Author-email: ort@ssb.no
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Dist: branca (>=0.6.0)
 Requires-Dist: folium (>=0.14.0)
+Requires-Dist: geocoder (>=1.38.1,<2.0.0)
 Requires-Dist: geopandas (>=0.13.0)
 Requires-Dist: igraph (>=0.10.4)
 Requires-Dist: ipython (>=8.13.2)
 Requires-Dist: jenkspy (>=0.3.2)
 Requires-Dist: mapclassify (>=2.5.0)
 Requires-Dist: matplotlib (>=3.7.0)
 Requires-Dist: networkx (>=3.0)
 Requires-Dist: numpy (>=1.24.2)
 Requires-Dist: pandas (>=1.5.3)
 Requires-Dist: pyarrow (>=11.0.0)
+Requires-Dist: rasterio (>=1.3.8,<2.0.0)
 Requires-Dist: requests (>=2.28.2)
+Requires-Dist: rtree (>=1.0.1,<2.0.0)
 Requires-Dist: scikit-learn (>=1.2.1)
 Requires-Dist: shapely (>=2.0.1)
 Requires-Dist: xyzservices (>=2023.2.0)
 Project-URL: Changelog, https://github.com/statisticsnorway/ssb-sgis/releases
 Project-URL: Repository, https://github.com/statisticsnorway/ssb-sgis
 Description-Content-Type: text/markdown
```

