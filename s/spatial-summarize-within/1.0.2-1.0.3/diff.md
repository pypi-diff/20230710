# Comparing `tmp/spatial_summarize_within-1.0.2.tar.gz` & `tmp/spatial_summarize_within-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatial_summarize_within-1.0.2.tar", last modified: Fri Jun 16 23:36:36 2023, max compression
+gzip compressed data, was "spatial_summarize_within-1.0.3.tar", last modified: Mon Jul 10 03:55:41 2023, max compression
```

## Comparing `spatial_summarize_within-1.0.2.tar` & `spatial_summarize_within-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-06-16 23:36:36.043167 spatial_summarize_within-1.0.2/
--rw-r--r--   0 Kenne      (501) staff       (20)     1076 2023-05-06 22:57:53.000000 spatial_summarize_within-1.0.2/LICENSE
--rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-06-16 23:36:36.043056 spatial_summarize_within-1.0.2/PKG-INFO
--rw-r--r--   0 Kenne      (501) staff       (20)     6664 2023-05-28 20:50:21.000000 spatial_summarize_within-1.0.2/README.md
--rw-r--r--   0 Kenne      (501) staff       (20)       38 2023-06-16 23:36:36.043202 spatial_summarize_within-1.0.2/setup.cfg
--rw-r--r--   0 Kenne      (501) staff       (20)      329 2023-06-16 23:29:51.000000 spatial_summarize_within-1.0.2/setup.py
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-06-16 23:36:36.042360 spatial_summarize_within-1.0.2/spatial_summarize_within/
--rw-r--r--   0 Kenne      (501) staff       (20)      141 2023-05-12 03:23:32.000000 spatial_summarize_within-1.0.2/spatial_summarize_within/__init__.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2348 2023-06-16 23:34:36.000000 spatial_summarize_within-1.0.2/spatial_summarize_within/max_within.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2376 2023-06-16 23:34:08.000000 spatial_summarize_within-1.0.2/spatial_summarize_within/mean_within.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2348 2023-06-16 23:35:44.000000 spatial_summarize_within-1.0.2/spatial_summarize_within/min_within.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2335 2023-06-16 23:35:44.000000 spatial_summarize_within-1.0.2/spatial_summarize_within/sum_within.py
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-06-16 23:36:36.042901 spatial_summarize_within-1.0.2/spatial_summarize_within.egg-info/
--rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-06-16 23:36:36.000000 spatial_summarize_within-1.0.2/spatial_summarize_within.egg-info/PKG-INFO
--rw-r--r--   0 Kenne      (501) staff       (20)      459 2023-06-16 23:36:36.000000 spatial_summarize_within-1.0.2/spatial_summarize_within.egg-info/SOURCES.txt
--rw-r--r--   0 Kenne      (501) staff       (20)        1 2023-06-16 23:36:36.000000 spatial_summarize_within-1.0.2/spatial_summarize_within.egg-info/dependency_links.txt
--rw-r--r--   0 Kenne      (501) staff       (20)       37 2023-06-16 23:36:36.000000 spatial_summarize_within-1.0.2/spatial_summarize_within.egg-info/requires.txt
--rw-r--r--   0 Kenne      (501) staff       (20)       25 2023-06-16 23:36:36.000000 spatial_summarize_within-1.0.2/spatial_summarize_within.egg-info/top_level.txt
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-07-10 03:55:41.059357 spatial_summarize_within-1.0.3/
+-rw-r--r--   0 Kenne      (501) staff       (20)     1076 2023-05-06 22:57:53.000000 spatial_summarize_within-1.0.3/LICENSE
+-rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-07-10 03:55:41.059238 spatial_summarize_within-1.0.3/PKG-INFO
+-rw-r--r--   0 Kenne      (501) staff       (20)     6819 2023-06-16 23:38:22.000000 spatial_summarize_within-1.0.3/README.md
+-rw-r--r--   0 Kenne      (501) staff       (20)       38 2023-07-10 03:55:41.059396 spatial_summarize_within-1.0.3/setup.cfg
+-rw-r--r--   0 Kenne      (501) staff       (20)      329 2023-07-10 03:52:47.000000 spatial_summarize_within-1.0.3/setup.py
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-07-10 03:55:41.058505 spatial_summarize_within-1.0.3/spatial_summarize_within/
+-rw-r--r--   0 Kenne      (501) staff       (20)      141 2023-05-12 03:23:32.000000 spatial_summarize_within-1.0.3/spatial_summarize_within/__init__.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2370 2023-07-10 03:53:06.000000 spatial_summarize_within-1.0.3/spatial_summarize_within/max_within.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2398 2023-07-10 03:53:06.000000 spatial_summarize_within-1.0.3/spatial_summarize_within/mean_within.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2370 2023-07-10 03:53:06.000000 spatial_summarize_within-1.0.3/spatial_summarize_within/min_within.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2357 2023-07-10 03:53:06.000000 spatial_summarize_within-1.0.3/spatial_summarize_within/sum_within.py
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-07-10 03:55:41.059068 spatial_summarize_within-1.0.3/spatial_summarize_within.egg-info/
+-rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-07-10 03:55:41.000000 spatial_summarize_within-1.0.3/spatial_summarize_within.egg-info/PKG-INFO
+-rw-r--r--   0 Kenne      (501) staff       (20)      459 2023-07-10 03:55:41.000000 spatial_summarize_within-1.0.3/spatial_summarize_within.egg-info/SOURCES.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)        1 2023-07-10 03:55:41.000000 spatial_summarize_within-1.0.3/spatial_summarize_within.egg-info/dependency_links.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)       37 2023-07-10 03:55:41.000000 spatial_summarize_within-1.0.3/spatial_summarize_within.egg-info/requires.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)       25 2023-07-10 03:55:41.000000 spatial_summarize_within-1.0.3/spatial_summarize_within.egg-info/top_level.txt
```

### Comparing `spatial_summarize_within-1.0.2/LICENSE` & `spatial_summarize_within-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spatial_summarize_within-1.0.2/README.md` & `spatial_summarize_within-1.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Spatial Summarize Within
 Spatial Summarize Within is a Python package that simplifies the process of summarizing attribute data within overlapping geometries in shapefiles. Given two shapefiles, it calculates the weighted values of specified attributes based on the overlap percentages between the input shapefile and the overlay shapefile. The statistics are calculated using only the proportion of the area that is within the boundary.
+## Usage
+Full [Tutorial](https://github.com/LandonWall/summarize_within_example/blob/master/notebooks/Summarize%20Precinct%20Data%20Within%20Cities.ipynb)
 
 ## Installation
 
 You can install Spatial Summarize Within using pip:
 
 ```bash
 pip install spatial_summarize_within
```

### Comparing `spatial_summarize_within-1.0.2/spatial_summarize_within/max_within.py` & `spatial_summarize_within-1.0.3/spatial_summarize_within/max_within.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     # Check if key exists in both dataframes
     if key in input_shapefile.columns and key in input_summary_features.columns:
         # Append suffix to key in input_summary_features
         input_summary_features = input_summary_features.rename(columns={key: key+"_summary"})
     # Add area column to input geodataframe
     input_summary_features["area"] = input_summary_features.geometry.area
     # Intersect the input geodataframe with the entire overlay shapefile
-    intersected = gpd.overlay(input_summary_features, input_shapefile, how='intersection')
+    intersected = gpd.overlay(input_summary_features, input_shapefile, how='intersection', keep_geom_type=False)
     # Calculate the area of each polygon in intersect dataframe
     intersected["intersect_area"] = intersected.area
     # Calculate the percentage overlap of each polygon
     intersected["overlap_pct"] = intersected["intersect_area"] / intersected["area"]
     # Create an empty geodataframe to store the results
     result_gdf = gpd.GeoDataFrame()
```

### Comparing `spatial_summarize_within-1.0.2/spatial_summarize_within/mean_within.py` & `spatial_summarize_within-1.0.3/spatial_summarize_within/mean_within.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     # Check if key exists in both dataframes
     if key in input_shapefile.columns and key in input_summary_features.columns:
         # Append suffix to key in input_summary_features
         input_summary_features = input_summary_features.rename(columns={key: key+"_summary"})
     # Add area column to input geodataframe
     input_summary_features["area"] = input_summary_features.geometry.area
     # Intersect the input geodataframe with the entire overlay shapefile
-    intersected = gpd.overlay(input_summary_features, input_shapefile, how='intersection')
+    intersected = gpd.overlay(input_summary_features, input_shapefile, how='intersection', keep_geom_type=False)
     # Calculate the area of each polygon in intersect dataframe
     intersected["intersect_area"] = intersected.area
     # Calculate the percentage overlap of each polygon
     intersected["overlap_pct"] = intersected["intersect_area"] / intersected["area"]
     # Create an empty geodataframe to store the results
     result_gdf = gpd.GeoDataFrame()
```

### Comparing `spatial_summarize_within-1.0.2/spatial_summarize_within/min_within.py` & `spatial_summarize_within-1.0.3/spatial_summarize_within/sum_within.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,45 +3,44 @@
 import shapely
 from shapely import wkt
 import shapely.ops
 from shapely.geometry import Polygon, MultiPolygon, shape, Point
 import geopandas as gpd
 import mapclassify
 
-# Function
-def min_within(input_shapefile, input_summary_features, columns, key, join_type='inner'):
+# function
+def sum_within(input_shapefile, input_summary_features, columns, key, join_type='inner'):
     # Check if key exists in both dataframes
     if key in input_shapefile.columns and key in input_summary_features.columns:
         # Append suffix to key in input_summary_features
         input_summary_features = input_summary_features.rename(columns={key: key+"_summary"})
     # Add area column to input geodataframe
     input_summary_features["area"] = input_summary_features.geometry.area
     # Intersect the input geodataframe with the entire overlay shapefile
-    intersected = gpd.overlay(input_summary_features, input_shapefile, how='intersection')
+    intersected = gpd.overlay(input_summary_features, input_shapefile, how='intersection', keep_geom_type=False)
     # Calculate the area of each polygon in intersect dataframe
     intersected["intersect_area"] = intersected.area
     # Calculate the percentage overlap of each polygon
     intersected["overlap_pct"] = intersected["intersect_area"] / intersected["area"]
     # Create an empty geodataframe to store the results
     result_gdf = gpd.GeoDataFrame()
 
     # Loop through each polygon in the overlay geodataframe
     for polygon in input_shapefile.itertuples():
-        # Select intersected parts that belong to the current polygon
+        # Select intersected parts that belong to current polygon
         temp_intersect = intersected.loc[intersected[key] == getattr(polygon, key)]
-        # Calculate the weighted value for each column
+        # Calculate the weighted sum
         for column in columns:
-            temp_intersect[column] = (temp_intersect[column] * temp_intersect["overlap_pct"]).min()
+            temp_intersect.loc[:, column] = (temp_intersect[column] * temp_intersect["overlap_pct"]).round(0)
         # Keep only the relevant columns in the temp_intersect dataframe
         temp_intersect = temp_intersect[[key] + columns + ['intersect_area', 'overlap_pct']]
         # Group the results
-        temp_result = temp_intersect.groupby(key).min(numeric_only=True).reset_index()
+        temp_result = temp_intersect.groupby(key).sum(numeric_only=True).reset_index()
         # Append the results to the result gdf
         result_gdf = pd.concat([result_gdf, temp_result], ignore_index=True)
 
     # Merge the result with the overlay geodataframe
     result_gdf = input_shapefile.merge(result_gdf, on=key, how=join_type)
-
     # Remove the area column from input geodataframe
     input_summary_features = input_summary_features.drop("area", axis=1)
 
     return result_gdf
```

### Comparing `spatial_summarize_within-1.0.2/spatial_summarize_within/sum_within.py` & `spatial_summarize_within-1.0.3/spatial_summarize_within/min_within.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,44 +3,45 @@
 import shapely
 from shapely import wkt
 import shapely.ops
 from shapely.geometry import Polygon, MultiPolygon, shape, Point
 import geopandas as gpd
 import mapclassify
 
-# function
-def sum_within(input_shapefile, input_summary_features, columns, key, join_type='inner'):
+# Function
+def min_within(input_shapefile, input_summary_features, columns, key, join_type='inner'):
     # Check if key exists in both dataframes
     if key in input_shapefile.columns and key in input_summary_features.columns:
         # Append suffix to key in input_summary_features
         input_summary_features = input_summary_features.rename(columns={key: key+"_summary"})
     # Add area column to input geodataframe
     input_summary_features["area"] = input_summary_features.geometry.area
     # Intersect the input geodataframe with the entire overlay shapefile
-    intersected = gpd.overlay(input_summary_features, input_shapefile, how='intersection')
+    intersected = gpd.overlay(input_summary_features, input_shapefile, how='intersection', keep_geom_type=False)
     # Calculate the area of each polygon in intersect dataframe
     intersected["intersect_area"] = intersected.area
     # Calculate the percentage overlap of each polygon
     intersected["overlap_pct"] = intersected["intersect_area"] / intersected["area"]
     # Create an empty geodataframe to store the results
     result_gdf = gpd.GeoDataFrame()
 
     # Loop through each polygon in the overlay geodataframe
     for polygon in input_shapefile.itertuples():
-        # Select intersected parts that belong to current polygon
+        # Select intersected parts that belong to the current polygon
         temp_intersect = intersected.loc[intersected[key] == getattr(polygon, key)]
-        # Calculate the weighted sum
+        # Calculate the weighted value for each column
         for column in columns:
-            temp_intersect.loc[:, column] = (temp_intersect[column] * temp_intersect["overlap_pct"]).round(0)
+            temp_intersect[column] = (temp_intersect[column] * temp_intersect["overlap_pct"]).min()
         # Keep only the relevant columns in the temp_intersect dataframe
         temp_intersect = temp_intersect[[key] + columns + ['intersect_area', 'overlap_pct']]
         # Group the results
-        temp_result = temp_intersect.groupby(key).sum(numeric_only=True).reset_index()
+        temp_result = temp_intersect.groupby(key).min(numeric_only=True).reset_index()
         # Append the results to the result gdf
         result_gdf = pd.concat([result_gdf, temp_result], ignore_index=True)
 
     # Merge the result with the overlay geodataframe
     result_gdf = input_shapefile.merge(result_gdf, on=key, how=join_type)
+
     # Remove the area column from input geodataframe
     input_summary_features = input_summary_features.drop("area", axis=1)
 
     return result_gdf
```

