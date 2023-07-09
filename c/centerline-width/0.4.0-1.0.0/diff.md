# Comparing `tmp/centerline-width-0.4.0.tar.gz` & `tmp/centerline-width-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/centerline-width-0.4.0.tar", last modified: Tue Jun 27 20:55:34 2023, max compression
+gzip compressed data, was "dist/centerline-width-1.0.0.tar", last modified: Sun Jul  9 22:03:56 2023, max compression
```

## Comparing `centerline-width-0.4.0.tar` & `centerline-width-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-27 20:55:34.398051 centerline-width-0.4.0/
--rw-rw-r--   0 user      (1000) user      (1000)    42076 2023-06-27 20:55:34.398051 centerline-width-0.4.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    36442 2023-06-27 20:52:49.000000 centerline-width-0.4.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-27 20:55:34.394050 centerline-width-0.4.0/centerline_width/
--rw-rw-r--   0 user      (1000) user      (1000)     1632 2023-06-23 06:05:21.000000 centerline-width-0.4.0/centerline_width/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    26135 2023-06-26 21:50:27.000000 centerline-width-0.4.0/centerline_width/centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)    16829 2023-06-26 21:48:17.000000 centerline-width-0.4.0/centerline_width/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-0.4.0/centerline_width/getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)     8526 2023-06-24 01:42:25.000000 centerline-width-0.4.0/centerline_width/plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     6759 2023-06-01 21:17:09.000000 centerline-width-0.4.0/centerline_width/preprocessing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-27 20:55:34.394050 centerline-width-0.4.0/centerline_width/pytests/
--rw-rw-r--   0 user      (1000) user      (1000)    13693 2023-06-26 21:49:08.000000 centerline-width-0.4.0/centerline_width/pytests/test_centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-0.4.0/centerline_width/pytests/test_getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)    12990 2023-06-24 07:23:37.000000 centerline-width-0.4.0/centerline_width/pytests/test_plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-0.4.0/centerline_width/pytests/test_preprocessing.py
--rw-rw-r--   0 user      (1000) user      (1000)     5105 2023-06-24 07:13:29.000000 centerline-width-0.4.0/centerline_width/pytests/test_riverCenterlineClass.py
--rw-rw-r--   0 user      (1000) user      (1000)     6510 2023-06-26 21:49:56.000000 centerline-width-0.4.0/centerline_width/riverCenterlineClass.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-27 20:55:34.394050 centerline-width-0.4.0/centerline_width.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    42076 2023-06-27 20:55:34.000000 centerline-width-0.4.0/centerline_width.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      700 2023-06-27 20:55:34.000000 centerline-width-0.4.0/centerline_width.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-27 20:55:34.000000 centerline-width-0.4.0/centerline_width.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      160 2023-06-27 20:55:34.000000 centerline-width-0.4.0/centerline_width.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2023-06-27 20:55:34.000000 centerline-width-0.4.0/centerline_width.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-27 20:55:34.398051 centerline-width-0.4.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1850 2023-06-27 20:52:28.000000 centerline-width-0.4.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-09 22:03:56.576991 centerline-width-1.0.0/
+-rw-rw-r--   0 user      (1000) user      (1000)    42692 2023-07-09 22:03:56.572991 centerline-width-1.0.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    37006 2023-07-09 08:39:47.000000 centerline-width-1.0.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-09 22:03:56.552991 centerline-width-1.0.0/centerline_width/
+-rw-rw-r--   0 user      (1000) user      (1000)     1632 2023-06-23 06:05:21.000000 centerline-width-1.0.0/centerline_width/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    26135 2023-06-26 21:50:27.000000 centerline-width-1.0.0/centerline_width/centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16829 2023-06-26 21:48:17.000000 centerline-width-1.0.0/centerline_width/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-1.0.0/centerline_width/getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9280 2023-06-28 04:14:39.000000 centerline-width-1.0.0/centerline_width/plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6759 2023-06-01 21:17:09.000000 centerline-width-1.0.0/centerline_width/preprocessing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-09 22:03:56.572991 centerline-width-1.0.0/centerline_width/pytests/
+-rw-rw-r--   0 user      (1000) user      (1000)    13693 2023-06-26 21:49:08.000000 centerline-width-1.0.0/centerline_width/pytests/test_centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-1.0.0/centerline_width/pytests/test_getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12990 2023-06-24 07:23:37.000000 centerline-width-1.0.0/centerline_width/pytests/test_plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-1.0.0/centerline_width/pytests/test_preprocessing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5105 2023-06-24 07:13:29.000000 centerline-width-1.0.0/centerline_width/pytests/test_riverCenterlineClass.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6510 2023-06-26 21:49:56.000000 centerline-width-1.0.0/centerline_width/riverCenterlineClass.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-09 22:03:56.556991 centerline-width-1.0.0/centerline_width.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    42692 2023-07-09 22:03:56.000000 centerline-width-1.0.0/centerline_width.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      700 2023-07-09 22:03:56.000000 centerline-width-1.0.0/centerline_width.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-09 22:03:56.000000 centerline-width-1.0.0/centerline_width.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      160 2023-07-09 22:03:56.000000 centerline-width-1.0.0/centerline_width.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-07-09 22:03:56.000000 centerline-width-1.0.0/centerline_width.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-09 22:03:56.576991 centerline-width-1.0.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1846 2023-07-09 22:02:40.000000 centerline-width-1.0.0/setup.py
```

### Comparing `centerline-width-0.4.0/PKG-INFO` & `centerline-width-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 0.4.0
+Version: 1.0.0
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.4.0.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.0.0.tar.gz
 Description: # Centerline-Width
          <p align="center">
           <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
         </p>
         
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
         [![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
+        ![PyPi-Versions](https://img.shields.io/pypi/pyversions/centerline-width)
         [![pytests](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml/badge.svg)](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml)
         
         Find the centerline and width of rivers based on the latitude and longitude positions from the right and left bank 
         
         * **Convert raw data from Google Earth Pro to CSV**
         	* extractPointsToTextFile()
         	* convertColumnsToCSV()
@@ -171,19 +172,19 @@
         				interpolate_n=5,
         				interpolate_n_centerpoints=None,
         				equal_distance=10,
         				ellipsoid="WGS84")
         ```
         * **[REQUIRED]** csv_data (string): File location of the text file to convert
         * [OPTIONAL] optional_cutoff (int): Include only the first x number of the data to chart (useful for debugging)
-        * [OPTIONAL] interpolate_data (bool): Interpolate between existing data by adding additional points
+        * [OPTIONAL] interpolate_data (boolean): Interpolate between existing data by adding additional points
         * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
         * [OPTIONAL] interpolate_n_centerpoints (int): Number of points used to interpolate the Voronoi centerline, defaults to the the length of the data frame (df_len)
         * [OPTIONAL] equal_distance (int): Equal distance between points (in meters) used to interpolate the Voronoi centerline, defaults 10 meters
-        * [OPTIONAL] ellipsoid (string): Ellipsoid definition of Earth to provide size and shape for built-in functions to convert degrees to meters, options include (is sensitive to case): ["GRS80", "airy", "bessel", "clrk66", "intl", "WGS60", "WGS66", "WGS72", "WGS84", "sphere"] for more details: ["Built-in ellpsoid defintions"](https://proj.org/en/9.2/usage/ellipsoids.html#built-in-ellipsoid-definitions), defaults to "WGS84"
+        * [OPTIONAL] ellipsoid (string): Ellipsoid definition of Earth to provide size and shape for built-in functions to convert degrees to meters, options include (is sensitive to case): ["GRS80", "airy", "bessel", "clrk66", "intl", "WGS60", "WGS66", "WGS72", "WGS84", "sphere"] for more details: ["Built-in ellipsoid defintions"](https://proj.org/en/9.2/usage/ellipsoids.html#built-in-ellipsoid-definitions), defaults to "WGS84"
         
         **Solutions for sparse data:**
         
         `interpolate_data` is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps due to the combination of sparse data and a narrow river (See: Debugging, Error Handling, and Edge Cases - Fix Gaps and Jagged Centerlines). By default, `interpolate_data=True` will add 5 additional points between each existing point but can be increased or decreased by modifying the `interpolate_n` option
         
         `interpolate_n_centerpoints` is an option that can be used to increase the resolution (number of points) of the centerline found by the Voronoi vertices. By default, will evenly space out to the size of the dataframe. Can artificially increase the amount of width lines generated by increasing the number of center points. When `interpolate_n_centerpoints` increases, the number of width lines generated will increase (and visa versa)
         
@@ -197,32 +198,32 @@
         * centerlineEqualDistance (list of tuples): List of the latitude and longitude coordinates of the centerline generated by equal distances between coordinates from the Voronoi diagrams
         * centerlineEvenlySpaced (list of tuples): List of the latitude and longitude coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
         * centerlineSmoothed (list of tuples): List of the latitude and longitude coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
         * centerlineLength (float): Length of the centerline of the river (in km)
         * rightBankLength (float): Length of the right bank of the river (in km)
         * leftBankLength (float): Length of the left bank of the river (in km)
         
-        **Object (class) additional atttributes:**
+        **Object (class) additional attributes:**
         
         * river_name (string): name of object, set to the csv_data string
         * left_bank_coordinates (list of tuples): list of coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
         * right_bank_coordinates (list of tuples) list of coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
         * df_len (int): Length of the data frame of the csv data (spliced by the optional_cutoff)
         * equal_distance (int): Distance between points (in meters) used in centerlineEqualDistance, defaults to points every 10 meters
-        * ellipsoid (string): Built-in ellipsoid defintion of Earth to determine how degrees are converted to meters used by centerlineEqualDistance, defaults to "WGS84"
-        * bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate river bank (used to define an inside and an outside of the river)
+        * ellipsoid (string): Built-in ellipsoid definition of Earth to determine how degrees are converted to meters used by centerlineEqualDistance, defaults to "WGS84"
+        * bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate riverbank (used to define an inside and an outside of the river)
         * top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon
         * bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
         * starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
         * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
         * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
         * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
         * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
-        * interpolate_data (bool): if interpolating between existing data, defaults to False
-        * interpolate_n (int): specifies how many additional points will be added between points along the river bank when interpolating data, defaults to 5
+        * interpolate_data (boolean): if interpolating between existing data, defaults to False
+        * interpolate_n (int): specifies how many additional points will be added between points along the riverbank when interpolating data, defaults to 5
         * interpolate_n_centerpoints (int): specifies how many points will be used to interpolate the Voronoi centerline, defaults to the length of the data frame (df_len)
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         ```
         
@@ -284,14 +285,16 @@
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
         ```
         Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
         
+        Note: it is best practice to plot the centerline with `plotCenterline()` to ensure that the results saved are as expected
+        
         ### Save Centerline Coordinates to a .MAT File
         Save the centerline coordinates to a .mat file with columns for latitude and longitude
         
         ```
         saveCenterlineMAT(save_to_mat=None, centerline_type="Voronoi")
         ```
         * **[REQUIRED]** save_to_mat (string): MAT filename, requires a .mat extension
@@ -302,14 +305,16 @@
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.saveCenterlineMAT(save_to_mat="centerline_coordinates.mat", centerline_type="Smoothed")
         ```
         Returns a .mat file with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed_Centerline_Latitude_(Deg), Smoothed_Centerline_Longitude_(Deg)`
         
+        Note: it is best practice to plot the centerline with `plotCenterline()` to ensure that the results saved are as expected
+        
         ### Return Length of Centerline
         Return the length of the centerline found between the left and right bank generated by the Voronoi diagram
         ```
         river_object.centerlineLength
         ```
         Length returned in kilometers
         ```python
@@ -361,38 +366,38 @@
         		flag_intersections=True,
         		remove_intersections=False)
         ```
         * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
         * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
         * [OPTIONAL] display_true_centerline (boolean): Display generated true centerline based on Voronoi diagrams
         * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
-        * [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
-        * [OPTIONAL] flag_intersections (bool): Display intersecting width lines as red in graph, defaults to True
-        * [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to False
+        * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
+        * [OPTIONAL] flag_intersections (boolean): Display intersecting width lines as red in graph, defaults to True
+        * [OPTIONAL] remove_intersections (boolean): Remove intersecting lines (but maintain the most width lines as possible) and only return non-intersecting width lines, defaults to False
         
         **apply_smoothing**
         
         apply_smoothing applies a spline to smooth the centerline points created by the Voronoi vertices. This reduces the noise of the slopes and can create width lines that are less susceptible to small changes in the bank
         
         | apply_smoothing=False | apply_smoothing=True |
         | ------------- | ------------- |
         | ![river_without_smoothing+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_without_smoothing.png) | ![river_with_smoothing+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_with_smoothing.png) |
         
         **transect_span_distance**
         
-        Transect span describes the number of points that are averaged to generated a width line (example: transect_span_distance=3, average of three slopes)
+        Transect span describes the number of points that are averaged to generate a width line (example: transect_span_distance=3, average of three slopes)
         
         ![transect_span_distance](https://user-images.githubusercontent.com/22159116/227870492-69d105b2-0d3e-4d50-90d9-e938400a58fb.png)
         | transect_span_distance=6 | transect_span_distance=30 |
         | ------------- | ------------- |
         | ![river_transect_6+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_transect_6.png) | ![river_transect_30+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_transect_30.png) |
         
         **remove_intersections**
         
-        remove_intersections will remove the width lines that intersect other lines (that could be creating unrepresentative long width lines). Intersections are removed first in order from most to least (to ensure that the most width lines as possible are kept) and then, based on the longer of two intersecting lines
+        remove_intersections will remove the width lines that intersect other lines (that could be creating unrepresentative long width lines). Intersections are removed first in order from most to least number of intersections and then based on the longer of two intersecting lines. This ensures that the most width lines as possible are kept
         
         Intersecting lines are flagged in red by default (flag_intersections=True)
         
         | remove_intersections=False | remove_intersections=True |
         | ------------- | ------------- |
         | ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
         
@@ -410,29 +415,31 @@
         ```
         riverWidthFromCenterline(transect_span_distance=3,
         			apply_smoothing=True,
         			remove_intersections=False,
         			save_to_csv=None)
         ```
         * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
-        * [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
-        * [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to True
+        * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
+        * [OPTIONAL] remove_intersections (boolean): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to True
         * [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (<units specified>)`)
         
         Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordinates may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_width_dict = river_object.riverWidthFromCenterline(transect_span_distance=3,
         							apply_smoothing=True,
         							remove_intersections=True)
         ```
         Width dictionary = `{(-92.86792084788995, 30.037769672351182): 0.10969163557087018, (-92.86795038641004, 30.03769867854198): 0.10794219579997719}`
         
+        Note: it is best practice to plot the centerline and width with same arguments in `plotCenterlineWidth()` to ensure that the results when `save_to_csv=True` are as expected
+        
         ## Documentation and Algorithm to Determine Centerline
         
         The centerline is defined by the greatest distance from the right and left bank, created from a Voronoi Diagram. The remaining paths within the river are filtered through Dijkstra's algorithm to find the shortest path that is the centerline
         
         ### Right and Left bank points are plotted (X-Axis for Latitude, Y-Axis for Longitude)
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example1.png)
         
@@ -447,15 +454,15 @@
         
         ### Filter out any point pairs that only have one connection to filter out the short dead end paths and find the starting and ending node based on distance from the top and bottom of polygon
         With the vertices removed, it is possible to form multiple unconnected graphs within the polygon. The largest subgraph is assumed to contain the centerline and the other subgraphs are filtered out
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example6.png)
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example7.png)
         
         ### Find the shortest path from the starting node to the ending node ([Dijkstra's Algorithm](https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.shortest_paths.generic.shortest_path.html#networkx.algorithms.shortest_paths.generic.shortest_path))
-        | Points on River Bank | NetworkX Graph of Points on River Bank |
+        | Points on Riverbank | NetworkX Graph of Points on Riverbank |
         | ------------- | ------------- |
         | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example10.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example9.png) |
         
         ### Display the centerline found by connecting the starting/ending node with the shortest path
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example8.png)
         
         This is an attempt at a more robust algorithm working from raw data to ensure that all dead ends are removed, and no gaps exist in the centerline
@@ -468,15 +475,15 @@
         **Vertices that have at least two connections (that would create gaps):**
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example5.png)
         
         ## Debugging, Error Handling, and Edge Cases
         ### Wide Start/End of River
         If the data starts or ends with a large width, it is possible for the starting/ending nodes to end up in the wrong position
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example3.png)
-        Currently, the starting node is determined by the closest node to the top of the bank (in green) and the ending node is determined by the closest node to the bottom of the bank (in red) that sits along the longest path
+        Currently, the starting node is determined by the closest node on the path to the top of the bank (in green) and the ending node is determined by the closest node on the path to the bottom of the bank (in red) that sits along the longest path
         
         ### Invalid Polygon
         A polygon is formed to encapsulate the river with the given data (to determine the inside and outside of the river). The top and bottom are connected by a straight line from the start/end of the available data. As a result, it is possible for this straight line to overlap and create an invalid polygon.
         
         A polygon is invalid if it overlaps within itself:
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example1.png)
         In this example, the polygon is invalid, but with such a small overlap it is still able to find a valid path
@@ -487,15 +494,15 @@
         ### Invalid Centerline
         If the data is too small, a centerline and its coordinates cannot not be found (since only a single Voronoi vertex exists within the polygon and after dead ends are filtered)
         
         `CRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set displayVoronoi=True to view vertices. Can typically be fixed by adding more data to expand range.`
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example2.png)
         Can be fixed by expanding the data until the polygon is large enough to contain at least two different vertex points
         
-        ### Invalid Top and Bottom Bank Postions (flipBankDirection = True)
+        ### Invalid Top and Bottom Bank Positions (flipBankDirection = True)
         Error: `WARNING: Invalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flipBankDirection=True (or reset to default 'False' if currently set to flipBankDirection=True)`
         
         If the data for the left and right riverbanks are generated in reverse order, they will be read in the incorrect order and the graph will find the invalid top and bottom of the bank
         
         If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
         
         This can be fixed by using the flipBankDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
@@ -552,15 +559,15 @@
         
         ## Bug and Feature Request
         
         Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/cyschneck/centerline-width/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
         
 Keywords: geophysics,python,voronoi,networkx,centerline,centerline-extraction,centerline-detection,rivers,river-bank-length,river-bank,limnology,hydrology
 Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Education
```

### Comparing `centerline-width-0.4.0/README.md` & `centerline-width-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
  <p align="center">
   <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
 </p>
 
 ![PyPi](https://img.shields.io/pypi/v/centerline-width)
 ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
 [![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
+![PyPi-Versions](https://img.shields.io/pypi/pyversions/centerline-width)
 [![pytests](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml/badge.svg)](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml)
 
 Find the centerline and width of rivers based on the latitude and longitude positions from the right and left bank 
 
 * **Convert raw data from Google Earth Pro to CSV**
 	* extractPointsToTextFile()
 	* convertColumnsToCSV()
@@ -163,19 +164,19 @@
 				interpolate_n=5,
 				interpolate_n_centerpoints=None,
 				equal_distance=10,
 				ellipsoid="WGS84")
 ```
 * **[REQUIRED]** csv_data (string): File location of the text file to convert
 * [OPTIONAL] optional_cutoff (int): Include only the first x number of the data to chart (useful for debugging)
-* [OPTIONAL] interpolate_data (bool): Interpolate between existing data by adding additional points
+* [OPTIONAL] interpolate_data (boolean): Interpolate between existing data by adding additional points
 * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
 * [OPTIONAL] interpolate_n_centerpoints (int): Number of points used to interpolate the Voronoi centerline, defaults to the the length of the data frame (df_len)
 * [OPTIONAL] equal_distance (int): Equal distance between points (in meters) used to interpolate the Voronoi centerline, defaults 10 meters
-* [OPTIONAL] ellipsoid (string): Ellipsoid definition of Earth to provide size and shape for built-in functions to convert degrees to meters, options include (is sensitive to case): ["GRS80", "airy", "bessel", "clrk66", "intl", "WGS60", "WGS66", "WGS72", "WGS84", "sphere"] for more details: ["Built-in ellpsoid defintions"](https://proj.org/en/9.2/usage/ellipsoids.html#built-in-ellipsoid-definitions), defaults to "WGS84"
+* [OPTIONAL] ellipsoid (string): Ellipsoid definition of Earth to provide size and shape for built-in functions to convert degrees to meters, options include (is sensitive to case): ["GRS80", "airy", "bessel", "clrk66", "intl", "WGS60", "WGS66", "WGS72", "WGS84", "sphere"] for more details: ["Built-in ellipsoid defintions"](https://proj.org/en/9.2/usage/ellipsoids.html#built-in-ellipsoid-definitions), defaults to "WGS84"
 
 **Solutions for sparse data:**
 
 `interpolate_data` is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps due to the combination of sparse data and a narrow river (See: Debugging, Error Handling, and Edge Cases - Fix Gaps and Jagged Centerlines). By default, `interpolate_data=True` will add 5 additional points between each existing point but can be increased or decreased by modifying the `interpolate_n` option
 
 `interpolate_n_centerpoints` is an option that can be used to increase the resolution (number of points) of the centerline found by the Voronoi vertices. By default, will evenly space out to the size of the dataframe. Can artificially increase the amount of width lines generated by increasing the number of center points. When `interpolate_n_centerpoints` increases, the number of width lines generated will increase (and visa versa)
 
@@ -189,32 +190,32 @@
 * centerlineEqualDistance (list of tuples): List of the latitude and longitude coordinates of the centerline generated by equal distances between coordinates from the Voronoi diagrams
 * centerlineEvenlySpaced (list of tuples): List of the latitude and longitude coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
 * centerlineSmoothed (list of tuples): List of the latitude and longitude coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
 * centerlineLength (float): Length of the centerline of the river (in km)
 * rightBankLength (float): Length of the right bank of the river (in km)
 * leftBankLength (float): Length of the left bank of the river (in km)
 
-**Object (class) additional atttributes:**
+**Object (class) additional attributes:**
 
 * river_name (string): name of object, set to the csv_data string
 * left_bank_coordinates (list of tuples): list of coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
 * right_bank_coordinates (list of tuples) list of coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
 * df_len (int): Length of the data frame of the csv data (spliced by the optional_cutoff)
 * equal_distance (int): Distance between points (in meters) used in centerlineEqualDistance, defaults to points every 10 meters
-* ellipsoid (string): Built-in ellipsoid defintion of Earth to determine how degrees are converted to meters used by centerlineEqualDistance, defaults to "WGS84"
-* bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate river bank (used to define an inside and an outside of the river)
+* ellipsoid (string): Built-in ellipsoid definition of Earth to determine how degrees are converted to meters used by centerlineEqualDistance, defaults to "WGS84"
+* bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate riverbank (used to define an inside and an outside of the river)
 * top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon
 * bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
 * starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
 * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
 * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
 * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
 * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
-* interpolate_data (bool): if interpolating between existing data, defaults to False
-* interpolate_n (int): specifies how many additional points will be added between points along the river bank when interpolating data, defaults to 5
+* interpolate_data (boolean): if interpolating between existing data, defaults to False
+* interpolate_n (int): specifies how many additional points will be added between points along the riverbank when interpolating data, defaults to 5
 * interpolate_n_centerpoints (int): specifies how many points will be used to interpolate the Voronoi centerline, defaults to the length of the data frame (df_len)
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 ```
 
@@ -276,14 +277,16 @@
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
 ```
 Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
 
+Note: it is best practice to plot the centerline with `plotCenterline()` to ensure that the results saved are as expected
+
 ### Save Centerline Coordinates to a .MAT File
 Save the centerline coordinates to a .mat file with columns for latitude and longitude
 
 ```
 saveCenterlineMAT(save_to_mat=None, centerline_type="Voronoi")
 ```
 * **[REQUIRED]** save_to_mat (string): MAT filename, requires a .mat extension
@@ -294,14 +297,16 @@
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_object.saveCenterlineMAT(save_to_mat="centerline_coordinates.mat", centerline_type="Smoothed")
 ```
 Returns a .mat file with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed_Centerline_Latitude_(Deg), Smoothed_Centerline_Longitude_(Deg)`
 
+Note: it is best practice to plot the centerline with `plotCenterline()` to ensure that the results saved are as expected
+
 ### Return Length of Centerline
 Return the length of the centerline found between the left and right bank generated by the Voronoi diagram
 ```
 river_object.centerlineLength
 ```
 Length returned in kilometers
 ```python
@@ -353,38 +358,38 @@
 		flag_intersections=True,
 		remove_intersections=False)
 ```
 * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
 * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
 * [OPTIONAL] display_true_centerline (boolean): Display generated true centerline based on Voronoi diagrams
 * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
-* [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
-* [OPTIONAL] flag_intersections (bool): Display intersecting width lines as red in graph, defaults to True
-* [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to False
+* [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
+* [OPTIONAL] flag_intersections (boolean): Display intersecting width lines as red in graph, defaults to True
+* [OPTIONAL] remove_intersections (boolean): Remove intersecting lines (but maintain the most width lines as possible) and only return non-intersecting width lines, defaults to False
 
 **apply_smoothing**
 
 apply_smoothing applies a spline to smooth the centerline points created by the Voronoi vertices. This reduces the noise of the slopes and can create width lines that are less susceptible to small changes in the bank
 
 | apply_smoothing=False | apply_smoothing=True |
 | ------------- | ------------- |
 | ![river_without_smoothing+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_without_smoothing.png) | ![river_with_smoothing+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_with_smoothing.png) |
 
 **transect_span_distance**
 
-Transect span describes the number of points that are averaged to generated a width line (example: transect_span_distance=3, average of three slopes)
+Transect span describes the number of points that are averaged to generate a width line (example: transect_span_distance=3, average of three slopes)
 
 ![transect_span_distance](https://user-images.githubusercontent.com/22159116/227870492-69d105b2-0d3e-4d50-90d9-e938400a58fb.png)
 | transect_span_distance=6 | transect_span_distance=30 |
 | ------------- | ------------- |
 | ![river_transect_6+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_transect_6.png) | ![river_transect_30+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_transect_30.png) |
 
 **remove_intersections**
 
-remove_intersections will remove the width lines that intersect other lines (that could be creating unrepresentative long width lines). Intersections are removed first in order from most to least (to ensure that the most width lines as possible are kept) and then, based on the longer of two intersecting lines
+remove_intersections will remove the width lines that intersect other lines (that could be creating unrepresentative long width lines). Intersections are removed first in order from most to least number of intersections and then based on the longer of two intersecting lines. This ensures that the most width lines as possible are kept
 
 Intersecting lines are flagged in red by default (flag_intersections=True)
 
 | remove_intersections=False | remove_intersections=True |
 | ------------- | ------------- |
 | ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
 
@@ -402,29 +407,31 @@
 ```
 riverWidthFromCenterline(transect_span_distance=3,
 			apply_smoothing=True,
 			remove_intersections=False,
 			save_to_csv=None)
 ```
 * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
-* [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
-* [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to True
+* [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
+* [OPTIONAL] remove_intersections (boolean): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to True
 * [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (<units specified>)`)
 
 Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordinates may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_width_dict = river_object.riverWidthFromCenterline(transect_span_distance=3,
 							apply_smoothing=True,
 							remove_intersections=True)
 ```
 Width dictionary = `{(-92.86792084788995, 30.037769672351182): 0.10969163557087018, (-92.86795038641004, 30.03769867854198): 0.10794219579997719}`
 
+Note: it is best practice to plot the centerline and width with same arguments in `plotCenterlineWidth()` to ensure that the results when `save_to_csv=True` are as expected
+
 ## Documentation and Algorithm to Determine Centerline
 
 The centerline is defined by the greatest distance from the right and left bank, created from a Voronoi Diagram. The remaining paths within the river are filtered through Dijkstra's algorithm to find the shortest path that is the centerline
 
 ### Right and Left bank points are plotted (X-Axis for Latitude, Y-Axis for Longitude)
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example1.png)
 
@@ -439,15 +446,15 @@
 
 ### Filter out any point pairs that only have one connection to filter out the short dead end paths and find the starting and ending node based on distance from the top and bottom of polygon
 With the vertices removed, it is possible to form multiple unconnected graphs within the polygon. The largest subgraph is assumed to contain the centerline and the other subgraphs are filtered out
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example6.png)
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example7.png)
 
 ### Find the shortest path from the starting node to the ending node ([Dijkstra's Algorithm](https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.shortest_paths.generic.shortest_path.html#networkx.algorithms.shortest_paths.generic.shortest_path))
-| Points on River Bank | NetworkX Graph of Points on River Bank |
+| Points on Riverbank | NetworkX Graph of Points on Riverbank |
 | ------------- | ------------- |
 | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example10.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example9.png) |
 
 ### Display the centerline found by connecting the starting/ending node with the shortest path
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example8.png)
 
 This is an attempt at a more robust algorithm working from raw data to ensure that all dead ends are removed, and no gaps exist in the centerline
@@ -460,15 +467,15 @@
 **Vertices that have at least two connections (that would create gaps):**
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example5.png)
 
 ## Debugging, Error Handling, and Edge Cases
 ### Wide Start/End of River
 If the data starts or ends with a large width, it is possible for the starting/ending nodes to end up in the wrong position
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example3.png)
-Currently, the starting node is determined by the closest node to the top of the bank (in green) and the ending node is determined by the closest node to the bottom of the bank (in red) that sits along the longest path
+Currently, the starting node is determined by the closest node on the path to the top of the bank (in green) and the ending node is determined by the closest node on the path to the bottom of the bank (in red) that sits along the longest path
 
 ### Invalid Polygon
 A polygon is formed to encapsulate the river with the given data (to determine the inside and outside of the river). The top and bottom are connected by a straight line from the start/end of the available data. As a result, it is possible for this straight line to overlap and create an invalid polygon.
 
 A polygon is invalid if it overlaps within itself:
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example1.png)
 In this example, the polygon is invalid, but with such a small overlap it is still able to find a valid path
@@ -479,15 +486,15 @@
 ### Invalid Centerline
 If the data is too small, a centerline and its coordinates cannot not be found (since only a single Voronoi vertex exists within the polygon and after dead ends are filtered)
 
 `CRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set displayVoronoi=True to view vertices. Can typically be fixed by adding more data to expand range.`
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example2.png)
 Can be fixed by expanding the data until the polygon is large enough to contain at least two different vertex points
 
-### Invalid Top and Bottom Bank Postions (flipBankDirection = True)
+### Invalid Top and Bottom Bank Positions (flipBankDirection = True)
 Error: `WARNING: Invalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flipBankDirection=True (or reset to default 'False' if currently set to flipBankDirection=True)`
 
 If the data for the left and right riverbanks are generated in reverse order, they will be read in the incorrect order and the graph will find the invalid top and bottom of the bank
 
 If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
 
 This can be fixed by using the flipBankDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
```

### Comparing `centerline-width-0.4.0/centerline_width/__init__.py` & `centerline-width-1.0.0/centerline_width/__init__.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.4.0/centerline_width/centerline.py` & `centerline-width-1.0.0/centerline_width/centerline.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.4.0/centerline_width/error_handling.py` & `centerline-width-1.0.0/centerline_width/error_handling.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.4.0/centerline_width/getCoordinatesKML.py` & `centerline-width-1.0.0/centerline_width/getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.4.0/centerline_width/plotDiagrams.py` & `centerline-width-1.0.0/centerline_width/plotDiagrams.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,26 +171,41 @@
 			else:
 				# recreate the centerline with evenly spaced points
 				right_width_coordinates, left_width_coordinates, num_intersection_coordinates = centerline_width.riverWidthFromCenterlineCoordinates(river_object=river_object, 
 																														centerline_coordinates=river_object.centerlineEvenlySpaced,
 																														transect_span_distance=transect_span_distance,
 																														remove_intersections=remove_intersections)
 
+			invalid_label_added = False # prevent legend for width lines from being generated more than once (because is inside a loop)
+			valid_label_added = False  # prevent legend for width lines from being generated more than once (because is inside a loop)
+			# plot width lines
 			for center_coord, edge_coord in right_width_coordinates.items():
 				x_points = (right_width_coordinates[center_coord][0], left_width_coordinates[center_coord][0])
 				y_points = (right_width_coordinates[center_coord][1], left_width_coordinates[center_coord][1])
 				if flag_intersections:
 					if num_intersection_coordinates[center_coord] > 0:
 						if remove_intersections:
 							logger.error("\nERROR: Unable to completely resolve all intersections lines to be removed")
-						plt.plot(x_points, y_points, 'red', linewidth=1)
+						if not invalid_label_added: 
+							plt.plot(x_points, y_points, 'red', label="Intersecting Width", linewidth=1)
+							invalid_label_added = True
+						else:
+							plt.plot(x_points, y_points, 'red', linewidth=1)
 					else:
-						plt.plot(x_points, y_points, 'green', linewidth=1)
+						if not valid_label_added:
+							plt.plot(x_points, y_points, 'green', label="Non-Intersecting Width", linewidth=1)
+							valid_label_added = True
+						else:
+							plt.plot(x_points, y_points, 'green', linewidth=1)
 				else:
-					plt.plot(x_points, y_points, 'green', linewidth=1)
+					if not valid_label_added:
+						plt.plot(x_points, y_points, 'green', label="Width", linewidth=1)
+						valid_label_added = True
+					else:
+						plt.plot(x_points, y_points, 'green', linewidth=1)
 
 	# Plot Title, Legends, and Axis Labels
 	if not plot_title:
 		plt.title("River Width Coordinates: Valid Centerline = {0}, Valid Polygon = {1}{2}, Interpolated = {3}".format(valid_path_through, river_object.bank_polygon.is_valid, number_of_evenly_spaced_points, river_object.interpolate_data))
 	else:
 		plt.title(plot_title)
 	plt.xlabel("Longitude (°)")
```

### Comparing `centerline-width-0.4.0/centerline_width/preprocessing.py` & `centerline-width-1.0.0/centerline_width/preprocessing.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.4.0/centerline_width/pytests/test_centerline.py` & `centerline-width-1.0.0/centerline_width/pytests/test_centerline.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.4.0/centerline_width/pytests/test_getCoordinatesKML.py` & `centerline-width-1.0.0/centerline_width/pytests/test_getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.4.0/centerline_width/pytests/test_plotDiagrams.py` & `centerline-width-1.0.0/centerline_width/pytests/test_plotDiagrams.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.4.0/centerline_width/pytests/test_preprocessing.py` & `centerline-width-1.0.0/centerline_width/pytests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.4.0/centerline_width/pytests/test_riverCenterlineClass.py` & `centerline-width-1.0.0/centerline_width/pytests/test_riverCenterlineClass.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.4.0/centerline_width/riverCenterlineClass.py` & `centerline-width-1.0.0/centerline_width/riverCenterlineClass.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.4.0/centerline_width.egg-info/PKG-INFO` & `centerline-width-1.0.0/centerline_width.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 0.4.0
+Version: 1.0.0
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.4.0.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.0.0.tar.gz
 Description: # Centerline-Width
          <p align="center">
           <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
         </p>
         
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
         [![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
+        ![PyPi-Versions](https://img.shields.io/pypi/pyversions/centerline-width)
         [![pytests](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml/badge.svg)](https://github.com/cyschneck/centerline-width/actions/workflows/pytests.yml)
         
         Find the centerline and width of rivers based on the latitude and longitude positions from the right and left bank 
         
         * **Convert raw data from Google Earth Pro to CSV**
         	* extractPointsToTextFile()
         	* convertColumnsToCSV()
@@ -171,19 +172,19 @@
         				interpolate_n=5,
         				interpolate_n_centerpoints=None,
         				equal_distance=10,
         				ellipsoid="WGS84")
         ```
         * **[REQUIRED]** csv_data (string): File location of the text file to convert
         * [OPTIONAL] optional_cutoff (int): Include only the first x number of the data to chart (useful for debugging)
-        * [OPTIONAL] interpolate_data (bool): Interpolate between existing data by adding additional points
+        * [OPTIONAL] interpolate_data (boolean): Interpolate between existing data by adding additional points
         * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
         * [OPTIONAL] interpolate_n_centerpoints (int): Number of points used to interpolate the Voronoi centerline, defaults to the the length of the data frame (df_len)
         * [OPTIONAL] equal_distance (int): Equal distance between points (in meters) used to interpolate the Voronoi centerline, defaults 10 meters
-        * [OPTIONAL] ellipsoid (string): Ellipsoid definition of Earth to provide size and shape for built-in functions to convert degrees to meters, options include (is sensitive to case): ["GRS80", "airy", "bessel", "clrk66", "intl", "WGS60", "WGS66", "WGS72", "WGS84", "sphere"] for more details: ["Built-in ellpsoid defintions"](https://proj.org/en/9.2/usage/ellipsoids.html#built-in-ellipsoid-definitions), defaults to "WGS84"
+        * [OPTIONAL] ellipsoid (string): Ellipsoid definition of Earth to provide size and shape for built-in functions to convert degrees to meters, options include (is sensitive to case): ["GRS80", "airy", "bessel", "clrk66", "intl", "WGS60", "WGS66", "WGS72", "WGS84", "sphere"] for more details: ["Built-in ellipsoid defintions"](https://proj.org/en/9.2/usage/ellipsoids.html#built-in-ellipsoid-definitions), defaults to "WGS84"
         
         **Solutions for sparse data:**
         
         `interpolate_data` is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps due to the combination of sparse data and a narrow river (See: Debugging, Error Handling, and Edge Cases - Fix Gaps and Jagged Centerlines). By default, `interpolate_data=True` will add 5 additional points between each existing point but can be increased or decreased by modifying the `interpolate_n` option
         
         `interpolate_n_centerpoints` is an option that can be used to increase the resolution (number of points) of the centerline found by the Voronoi vertices. By default, will evenly space out to the size of the dataframe. Can artificially increase the amount of width lines generated by increasing the number of center points. When `interpolate_n_centerpoints` increases, the number of width lines generated will increase (and visa versa)
         
@@ -197,32 +198,32 @@
         * centerlineEqualDistance (list of tuples): List of the latitude and longitude coordinates of the centerline generated by equal distances between coordinates from the Voronoi diagrams
         * centerlineEvenlySpaced (list of tuples): List of the latitude and longitude coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
         * centerlineSmoothed (list of tuples): List of the latitude and longitude coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
         * centerlineLength (float): Length of the centerline of the river (in km)
         * rightBankLength (float): Length of the right bank of the river (in km)
         * leftBankLength (float): Length of the left bank of the river (in km)
         
-        **Object (class) additional atttributes:**
+        **Object (class) additional attributes:**
         
         * river_name (string): name of object, set to the csv_data string
         * left_bank_coordinates (list of tuples): list of coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
         * right_bank_coordinates (list of tuples) list of coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
         * df_len (int): Length of the data frame of the csv data (spliced by the optional_cutoff)
         * equal_distance (int): Distance between points (in meters) used in centerlineEqualDistance, defaults to points every 10 meters
-        * ellipsoid (string): Built-in ellipsoid defintion of Earth to determine how degrees are converted to meters used by centerlineEqualDistance, defaults to "WGS84"
-        * bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate river bank (used to define an inside and an outside of the river)
+        * ellipsoid (string): Built-in ellipsoid definition of Earth to determine how degrees are converted to meters used by centerlineEqualDistance, defaults to "WGS84"
+        * bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate riverbank (used to define an inside and an outside of the river)
         * top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon
         * bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
         * starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
         * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
         * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
         * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
         * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
-        * interpolate_data (bool): if interpolating between existing data, defaults to False
-        * interpolate_n (int): specifies how many additional points will be added between points along the river bank when interpolating data, defaults to 5
+        * interpolate_data (boolean): if interpolating between existing data, defaults to False
+        * interpolate_n (int): specifies how many additional points will be added between points along the riverbank when interpolating data, defaults to 5
         * interpolate_n_centerpoints (int): specifies how many points will be used to interpolate the Voronoi centerline, defaults to the length of the data frame (df_len)
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         ```
         
@@ -284,14 +285,16 @@
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
         ```
         Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
         
+        Note: it is best practice to plot the centerline with `plotCenterline()` to ensure that the results saved are as expected
+        
         ### Save Centerline Coordinates to a .MAT File
         Save the centerline coordinates to a .mat file with columns for latitude and longitude
         
         ```
         saveCenterlineMAT(save_to_mat=None, centerline_type="Voronoi")
         ```
         * **[REQUIRED]** save_to_mat (string): MAT filename, requires a .mat extension
@@ -302,14 +305,16 @@
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.saveCenterlineMAT(save_to_mat="centerline_coordinates.mat", centerline_type="Smoothed")
         ```
         Returns a .mat file with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed_Centerline_Latitude_(Deg), Smoothed_Centerline_Longitude_(Deg)`
         
+        Note: it is best practice to plot the centerline with `plotCenterline()` to ensure that the results saved are as expected
+        
         ### Return Length of Centerline
         Return the length of the centerline found between the left and right bank generated by the Voronoi diagram
         ```
         river_object.centerlineLength
         ```
         Length returned in kilometers
         ```python
@@ -361,38 +366,38 @@
         		flag_intersections=True,
         		remove_intersections=False)
         ```
         * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
         * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
         * [OPTIONAL] display_true_centerline (boolean): Display generated true centerline based on Voronoi diagrams
         * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
-        * [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
-        * [OPTIONAL] flag_intersections (bool): Display intersecting width lines as red in graph, defaults to True
-        * [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to False
+        * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
+        * [OPTIONAL] flag_intersections (boolean): Display intersecting width lines as red in graph, defaults to True
+        * [OPTIONAL] remove_intersections (boolean): Remove intersecting lines (but maintain the most width lines as possible) and only return non-intersecting width lines, defaults to False
         
         **apply_smoothing**
         
         apply_smoothing applies a spline to smooth the centerline points created by the Voronoi vertices. This reduces the noise of the slopes and can create width lines that are less susceptible to small changes in the bank
         
         | apply_smoothing=False | apply_smoothing=True |
         | ------------- | ------------- |
         | ![river_without_smoothing+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_without_smoothing.png) | ![river_with_smoothing+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_with_smoothing.png) |
         
         **transect_span_distance**
         
-        Transect span describes the number of points that are averaged to generated a width line (example: transect_span_distance=3, average of three slopes)
+        Transect span describes the number of points that are averaged to generate a width line (example: transect_span_distance=3, average of three slopes)
         
         ![transect_span_distance](https://user-images.githubusercontent.com/22159116/227870492-69d105b2-0d3e-4d50-90d9-e938400a58fb.png)
         | transect_span_distance=6 | transect_span_distance=30 |
         | ------------- | ------------- |
         | ![river_transect_6+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_transect_6.png) | ![river_transect_30+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_transect_30.png) |
         
         **remove_intersections**
         
-        remove_intersections will remove the width lines that intersect other lines (that could be creating unrepresentative long width lines). Intersections are removed first in order from most to least (to ensure that the most width lines as possible are kept) and then, based on the longer of two intersecting lines
+        remove_intersections will remove the width lines that intersect other lines (that could be creating unrepresentative long width lines). Intersections are removed first in order from most to least number of intersections and then based on the longer of two intersecting lines. This ensures that the most width lines as possible are kept
         
         Intersecting lines are flagged in red by default (flag_intersections=True)
         
         | remove_intersections=False | remove_intersections=True |
         | ------------- | ------------- |
         | ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
         
@@ -410,29 +415,31 @@
         ```
         riverWidthFromCenterline(transect_span_distance=3,
         			apply_smoothing=True,
         			remove_intersections=False,
         			save_to_csv=None)
         ```
         * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
-        * [OPTIONAL] apply_smoothing (bool): Apply a B-spline smoothing to centerline
-        * [OPTIONAL] remove_intersections (bool): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to True
+        * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
+        * [OPTIONAL] remove_intersections (boolean): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to True
         * [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (<units specified>)`)
         
         Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordinates may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_width_dict = river_object.riverWidthFromCenterline(transect_span_distance=3,
         							apply_smoothing=True,
         							remove_intersections=True)
         ```
         Width dictionary = `{(-92.86792084788995, 30.037769672351182): 0.10969163557087018, (-92.86795038641004, 30.03769867854198): 0.10794219579997719}`
         
+        Note: it is best practice to plot the centerline and width with same arguments in `plotCenterlineWidth()` to ensure that the results when `save_to_csv=True` are as expected
+        
         ## Documentation and Algorithm to Determine Centerline
         
         The centerline is defined by the greatest distance from the right and left bank, created from a Voronoi Diagram. The remaining paths within the river are filtered through Dijkstra's algorithm to find the shortest path that is the centerline
         
         ### Right and Left bank points are plotted (X-Axis for Latitude, Y-Axis for Longitude)
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example1.png)
         
@@ -447,15 +454,15 @@
         
         ### Filter out any point pairs that only have one connection to filter out the short dead end paths and find the starting and ending node based on distance from the top and bottom of polygon
         With the vertices removed, it is possible to form multiple unconnected graphs within the polygon. The largest subgraph is assumed to contain the centerline and the other subgraphs are filtered out
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example6.png)
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example7.png)
         
         ### Find the shortest path from the starting node to the ending node ([Dijkstra's Algorithm](https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.shortest_paths.generic.shortest_path.html#networkx.algorithms.shortest_paths.generic.shortest_path))
-        | Points on River Bank | NetworkX Graph of Points on River Bank |
+        | Points on Riverbank | NetworkX Graph of Points on Riverbank |
         | ------------- | ------------- |
         | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example10.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example9.png) |
         
         ### Display the centerline found by connecting the starting/ending node with the shortest path
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example8.png)
         
         This is an attempt at a more robust algorithm working from raw data to ensure that all dead ends are removed, and no gaps exist in the centerline
@@ -468,15 +475,15 @@
         **Vertices that have at least two connections (that would create gaps):**
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example5.png)
         
         ## Debugging, Error Handling, and Edge Cases
         ### Wide Start/End of River
         If the data starts or ends with a large width, it is possible for the starting/ending nodes to end up in the wrong position
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example3.png)
-        Currently, the starting node is determined by the closest node to the top of the bank (in green) and the ending node is determined by the closest node to the bottom of the bank (in red) that sits along the longest path
+        Currently, the starting node is determined by the closest node on the path to the top of the bank (in green) and the ending node is determined by the closest node on the path to the bottom of the bank (in red) that sits along the longest path
         
         ### Invalid Polygon
         A polygon is formed to encapsulate the river with the given data (to determine the inside and outside of the river). The top and bottom are connected by a straight line from the start/end of the available data. As a result, it is possible for this straight line to overlap and create an invalid polygon.
         
         A polygon is invalid if it overlaps within itself:
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example1.png)
         In this example, the polygon is invalid, but with such a small overlap it is still able to find a valid path
@@ -487,15 +494,15 @@
         ### Invalid Centerline
         If the data is too small, a centerline and its coordinates cannot not be found (since only a single Voronoi vertex exists within the polygon and after dead ends are filtered)
         
         `CRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set displayVoronoi=True to view vertices. Can typically be fixed by adding more data to expand range.`
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_example2.png)
         Can be fixed by expanding the data until the polygon is large enough to contain at least two different vertex points
         
-        ### Invalid Top and Bottom Bank Postions (flipBankDirection = True)
+        ### Invalid Top and Bottom Bank Positions (flipBankDirection = True)
         Error: `WARNING: Invalid Polygon Due to Flipped Banks, fix recommendation: rerun convertColumnsToCSV() and set flipBankDirection=True (or reset to default 'False' if currently set to flipBankDirection=True)`
         
         If the data for the left and right riverbanks are generated in reverse order, they will be read in the incorrect order and the graph will find the invalid top and bottom of the bank
         
         If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
         
         This can be fixed by using the flipBankDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
@@ -552,15 +559,15 @@
         
         ## Bug and Feature Request
         
         Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/cyschneck/centerline-width/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
         
 Keywords: geophysics,python,voronoi,networkx,centerline,centerline-extraction,centerline-detection,rivers,river-bank-length,river-bank,limnology,hydrology
 Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Education
```

### Comparing `centerline-width-0.4.0/centerline_width.egg-info/SOURCES.txt` & `centerline-width-1.0.0/centerline_width.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `centerline-width-0.4.0/setup.py` & `centerline-width-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 # Python Package Setup
 from setuptools import setup, find_namespace_packages
 
-VERSION="0.4.0"
+VERSION="1.0.0"
 DESCRIPTION="A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank"
 
 with open("README.md", "r") as f:
 	long_description_readme = f.read()
 
 setup(
 	name="centerline-width",
@@ -17,15 +17,15 @@
 	long_description_content_type='text/markdown',
 	url="https://github.com/cyschneck/centerline-width",
 	download_url="https://github.com/cyschneck/centerline-width/archive/refs/tags/v{0}.tar.gz".format(VERSION),
 	author="Una Schneck (unaschneck), Cora Schneck (cyschneck)",
 	keywords=["geophysics", "python", "voronoi", "networkx", "centerline", "centerline-extraction", "centerline-detection", "rivers", "river-bank-length", "river-bank", "limnology", "hydrology"],
 	license="MIT",
 	classifiers=[
-		"Development Status :: 2 - Pre-Alpha",
+		"Development Status :: 3 - Alpha",
 		"Intended Audience :: Developers",
 		"Intended Audience :: Education",
 		"Intended Audience :: Science/Research",
 		"License :: OSI Approved :: MIT License",
 		"Programming Language :: Python",
 		"Programming Language :: Python :: 3.9",
 		"Intended Audience :: Education",
```

