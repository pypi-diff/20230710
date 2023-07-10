# Comparing `tmp/sliderule-3.5.0.tar.gz` & `tmp/sliderule-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliderule-3.5.0.tar", last modified: Fri Jun  9 17:43:39 2023, max compression
+gzip compressed data, was "sliderule-3.6.0.tar", last modified: Mon Jul 10 20:01:50 2023, max compression
```

## Comparing `sliderule-3.5.0.tar` & `sliderule-3.6.0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 17:43:39.936906 sliderule-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-06-09 17:43:27.000000 sliderule-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-06-09 17:43:27.000000 sliderule-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      584 2023-06-09 17:43:39.936906 sliderule-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-06-09 17:43:27.000000 sliderule-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-09 17:43:27.000000 sliderule-3.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 17:43:39.936906 sliderule-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-06-09 17:43:27.000000 sliderule-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 17:43:39.936906 sliderule-3.5.0/sliderule/
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    30629 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/earthdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    17363 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/gedi.py
--rw-r--r--   0 runner    (1001) docker     (122)     9808 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/h5.py
--rw-r--r--   0 runner    (1001) docker     (122)    34802 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/icesat2.py
--rw-r--r--   0 runner    (1001) docker     (122)    38844 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/io.py
--rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/ipxapi.py
--rw-r--r--   0 runner    (1001) docker     (122)    85029 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/ipysliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)     6249 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/raster.py
--rw-r--r--   0 runner    (1001) docker     (122)    45769 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/sliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)    12772 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/swot.py
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-09 17:43:27.000000 sliderule-3.5.0/sliderule/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 17:43:39.936906 sliderule-3.5.0/sliderule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      584 2023-06-09 17:43:39.000000 sliderule-3.5.0/sliderule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      997 2023-06-09 17:43:39.000000 sliderule-3.5.0/sliderule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 17:43:39.000000 sliderule-3.5.0/sliderule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-09 17:43:39.000000 sliderule-3.5.0/sliderule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-09 17:43:39.000000 sliderule-3.5.0/sliderule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 17:43:39.936906 sliderule-3.5.0/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/big_query.py
--rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/build_3dep_DEM_geojson.py
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/build_arctic_dem_mosaics_index.py
--rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/build_arctic_dem_mosaics_vrt_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/build_arctic_dem_strips_vrt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/extract_h5_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/icepyx_region.py
--rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/lpdaac_download.py
--rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)      922 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/query_cmr.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/query_elevations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/query_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/query_photons.py
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/query_stac.py
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/query_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/region_of_interest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/results_to_s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/stac.py
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/stream_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/tail_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     6260 2023-06-09 17:43:27.000000 sliderule-3.5.0/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-09 17:43:27.000000 sliderule-3.5.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 20:01:50.114854 sliderule-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-07-10 20:01:35.000000 sliderule-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-07-10 20:01:35.000000 sliderule-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-07-10 20:01:50.114854 sliderule-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-10 20:01:35.000000 sliderule-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-07-10 20:01:35.000000 sliderule-3.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-10 20:01:50.114854 sliderule-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-07-10 20:01:35.000000 sliderule-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 20:01:50.110854 sliderule-3.6.0/sliderule/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30636 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/earthdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17363 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/gedi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9808 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/h5.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34802 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/icesat2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38844 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/ipxapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    85029 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/ipysliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6578 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/raster.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45770 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/sliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12772 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/swot.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 20:01:50.114854 sliderule-3.6.0/sliderule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-07-10 20:01:50.000000 sliderule-3.6.0/sliderule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-07-10 20:01:50.000000 sliderule-3.6.0/sliderule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 20:01:50.000000 sliderule-3.6.0/sliderule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-10 20:01:50.000000 sliderule-3.6.0/sliderule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-10 20:01:50.000000 sliderule-3.6.0/sliderule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 20:01:50.114854 sliderule-3.6.0/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/big_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/build_3dep_DEM_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/build_arctic_dem_mosaics_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/build_arctic_dem_mosaics_vrt_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/build_arctic_dem_strips_vrt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/extract_h5_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/icepyx_region.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/lpdaac_download.py
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/lpdaac_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/query_cmr.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/query_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/query_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/query_photons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/query_stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/query_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/region_of_interest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/results_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/stream_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/tail_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6260 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-10 20:01:35.000000 sliderule-3.6.0/version.txt
```

### Comparing `sliderule-3.5.0/LICENSE` & `sliderule-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/PKG-INFO` & `sliderule-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.5.0
+Version: 3.6.0
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.5.0/README.md` & `sliderule-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/setup.py` & `sliderule-3.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/sliderule/earthdata.py` & `sliderule-3.6.0/sliderule/earthdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
             # non-datapool links, we should be able to do this in a non-hack way
             continue
         filename = link['href'].split('/')[-1]
         if filename in unique_filenames:
             # Exclude links with duplicate filenames (they would overwrite)
             continue
         unique_filenames.add(filename)
-        if any([extension in link['href'] for extension in data_formats]):
+        if any([link['href'].endswith(extension) for extension in data_formats]):
             resource = link['href'].split("/")[-1]
             urls.append(resource)
     # return filtered urls
     return urls
 
 def __cmr_granule_metadata(search_results):
     """Get the metadata for CMR returned granules"""
```

### Comparing `sliderule-3.5.0/sliderule/gedi.py` & `sliderule-3.6.0/sliderule/gedi.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/sliderule/h5.py` & `sliderule-3.6.0/sliderule/h5.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/sliderule/icesat2.py` & `sliderule-3.6.0/sliderule/icesat2.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,15 +392,15 @@
         asset:          str
                         data source asset (see `Assets </web/rtd/user_guide/ICESat-2.html#assets>`_)
         version:        str
                         the version of the ATL03 data to use for processing
         callbacks:      dictionary
                         a callback function that is called for each result record
         resources:      list
-                        a list of granules to process (e.g. ["ATL03_20181019065445_03150111_004_01.h5", ...])
+                        a list of granules to process (e.g. ["ATL03_20181019065445_03150111_005_01.h5", ...])
         keep_id:        bool
                         whether to retain the "extent_id" column in the GeoDataFrame for future merges
         as_numpy_array: bool
                         whether to provide all sampled values as numpy arrays even if there is only a single value
 
     Returns
     -------
@@ -505,15 +505,15 @@
         asset:          str
                         data source asset (see `Assets </web/rtd/user_guide/ICESat-2.html#assets>`_)
         version:        str
                         the version of the ATL03 data to return
         callbacks:      dictionary
                         a callback function that is called for each result record
         resources:      list
-                        a list of granules to process (e.g. ["ATL03_20181019065445_03150111_004_01.h5", ...])
+                        a list of granules to process (e.g. ["ATL03_20181019065445_03150111_005_01.h5", ...])
         keep_id:        bool
                         whether to retain the "extent_id" column in the GeoDataFrame for future merges
 
     Returns
     -------
     GeoDataFrame
         ATL03 segments (see `Photon Segments </web/rtd/user_guide/ICESat-2.html#photon-segments>`_)
@@ -714,15 +714,15 @@
         asset:          str
                         data source asset (see `Assets </web/rtd/user_guide/ICESat-2.html#assets>`_)
         version:        str
                         the version of the ATL03 data to use for processing
         callbacks:      dictionary
                         a callback function that is called for each result record
         resources:      list
-                        a list of granules to process (e.g. ["ATL03_20181019065445_03150111_004_01.h5", ...])
+                        a list of granules to process (e.g. ["ATL03_20181019065445_03150111_005_01.h5", ...])
         keep_id:        bool
                         whether to retain the "extent_id" column in the GeoDataFrame for future merges
         as_numpy_array: bool
                         whether to provide all sampled values as numpy arrays even if there is only a single value
 
     Returns
     -------
```

### Comparing `sliderule-3.5.0/sliderule/io.py` & `sliderule-3.6.0/sliderule/io.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/sliderule/ipxapi.py` & `sliderule-3.6.0/sliderule/ipxapi.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/sliderule/ipysliderule.py` & `sliderule-3.6.0/sliderule/ipysliderule.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/sliderule/raster.py` & `sliderule-3.6.0/sliderule/raster.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,27 @@
 ###############################################################################
 
 logger = logging.getLogger(__name__)
 
 profiles = {}
 
 ###############################################################################
+# UTILITIES
+###############################################################################
+
+#
+# poly2bbox
+#
+def poly2bbox(poly):
+    lats = [p["lat"] for p in poly]
+    lons = [p["lon"] for p in poly]
+    bbox = [ min(lons), min(lats), max(lons), max(lats) ]
+    return bbox
+
+###############################################################################
 # APIs
 ###############################################################################
 
 #
 # Sample
 #
 def sample(asset, coordinates, parms={}):
@@ -59,32 +72,32 @@
     parms:          dict
                     dictionary of samping parameters
 
     Returns
     -------
     GeoDataFrame
         geolocated sampled values along with metadata
-    
+
     Examples
     --------
         >>> import sliderule
         >>> gdf = sliderule.sample("arctidcem-mosaic", [[-178.0,51.7]])
     '''
     # Massage Arguments
     if type(coordinates[0]) != list:
         coorindates = [coorindates]
-    
+
     # Perform Request
     rqst = {"samples": {"asset": asset, **parms}, "coordinates": coordinates}
     rsps = sliderule.source("samples", rqst)
-    
+
     # Sanity Check Response
     if len(rsps) <= 0:
         return sliderule.emptyframe()
-    
+
     # Count Records
     num_records = 0
     for input_coord_response in rsps["samples"]:
         for raster_sample in input_coord_response:
             num_records += 1
 
     # Get Types
@@ -96,34 +109,34 @@
     mean_nptype     = sliderule.get_definition("zsrec.sample", "mean")['nptype']
     median_nptype   = sliderule.get_definition("zsrec.sample", "median")['nptype']
     stdev_nptype    = sliderule.get_definition("zsrec.sample", "stdev")['nptype']
     mad_nptype      = sliderule.get_definition("zsrec.sample", "mad")['nptype']
 
     # Build Initial Columns
     columns = {
-        'time': numpy.empty(num_records, numpy.int64), 
-        'latitude': numpy.empty(num_records, numpy.double), 
-        'longitude': numpy.empty(num_records, numpy.double), 
-        'file': [], 
+        'time': numpy.empty(num_records, numpy.int64),
+        'latitude': numpy.empty(num_records, numpy.double),
+        'longitude': numpy.empty(num_records, numpy.double),
+        'file': [],
         'value': numpy.empty(num_records, value_nptype)
     }
     if 'with_flags' in parms:
         columns = {
-            'flags': numpy.empty(num_records, flags_nptype), 
+            'flags': numpy.empty(num_records, flags_nptype),
             **columns
         }
     if 'zonal_stats' in parms:
         columns = {
-            'count': numpy.empty(num_records, count_nptype), 
-            'min': numpy.empty(num_records, min_nptype), 
-            'max': numpy.empty(num_records, max_nptype), 
-            'mean': numpy.empty(num_records, mean_nptype), 
-            'median': numpy.empty(num_records, median_nptype), 
-            'stdev': numpy.empty(num_records, stdev_nptype), 
-            'mad': numpy.empty(num_records, mad_nptype), 
+            'count': numpy.empty(num_records, count_nptype),
+            'min': numpy.empty(num_records, min_nptype),
+            'max': numpy.empty(num_records, max_nptype),
+            'mean': numpy.empty(num_records, mean_nptype),
+            'median': numpy.empty(num_records, median_nptype),
+            'stdev': numpy.empty(num_records, stdev_nptype),
+            'mad': numpy.empty(num_records, mad_nptype),
             **columns
         }
 
     # Populate Columns
     i = 0
     per_coord_index = 0
     for input_coord_response in rsps["samples"]:
```

### Comparing `sliderule-3.5.0/sliderule/sliderule.py` & `sliderule-3.6.0/sliderule/sliderule.py`

 * *Files 0% similar despite different names*

```diff
@@ -863,15 +863,15 @@
         try:
             host = "https://ps." + service_url + "/api/org_num_nodes/" + service_org + "/"
             rsps = session.get(host, headers=headers, timeout=request_timeout)
             rsps_body = rsps.json()
             rsps.raise_for_status()
             requested_nodes = max(min(desired_nodes, rsps_body["max_nodes"]), rsps_body["min_nodes"])
             if requested_nodes != desired_nodes:
-                logger.info("Provisioning system desired nodes truncated to {}".format(requested_nodes))
+                logger.info("Provisioning system desired nodes overridden to {}".format(requested_nodes))
         except requests.exceptions.HTTPError as e:
             logger.info('{}'.format(e))
             logger.info('Provisioning system status request returned error => {}'.format(rsps_body["error_msg"]))
 
         # Request number of nodes in cluster
         try:
             if type(time_to_live) == int:
```

### Comparing `sliderule-3.5.0/sliderule/swot.py` & `sliderule-3.6.0/sliderule/swot.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/sliderule.egg-info/PKG-INFO` & `sliderule-3.6.0/sliderule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.5.0
+Version: 3.6.0
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.5.0/sliderule.egg-info/SOURCES.txt` & `sliderule-3.6.0/sliderule.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 utils/build_3dep_DEM_geojson.py
 utils/build_arctic_dem_mosaics_index.py
 utils/build_arctic_dem_mosaics_vrt_list.py
 utils/build_arctic_dem_strips_vrt.py
 utils/extract_h5_dataset.py
 utils/icepyx_region.py
 utils/lpdaac_download.py
+utils/lpdaac_list.py
 utils/monitor.py
 utils/query_cmr.py
 utils/query_elevations.py
 utils/query_metrics.py
 utils/query_photons.py
 utils/query_stac.py
 utils/query_version.py
```

### Comparing `sliderule-3.5.0/utils/big_query.py` & `sliderule-3.6.0/utils/big_query.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/utils/build_3dep_DEM_geojson.py` & `sliderule-3.6.0/utils/build_3dep_DEM_geojson.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/utils/build_arctic_dem_mosaics_index.py` & `sliderule-3.6.0/utils/build_arctic_dem_mosaics_index.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/utils/build_arctic_dem_mosaics_vrt_list.py` & `sliderule-3.6.0/utils/build_arctic_dem_mosaics_vrt_list.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/utils/build_arctic_dem_strips_vrt.py` & `sliderule-3.6.0/utils/build_arctic_dem_strips_vrt.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/utils/extract_h5_dataset.py` & `sliderule-3.6.0/utils/extract_h5_dataset.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/utils/icepyx_region.py` & `sliderule-3.6.0/utils/icepyx_region.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/utils/lpdaac_download.py` & `sliderule-3.6.0/utils/lpdaac_download.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/utils/monitor.py` & `sliderule-3.6.0/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/utils/query_cmr.py` & `sliderule-3.6.0/utils/query_cmr.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/utils/query_elevations.py` & `sliderule-3.6.0/utils/query_elevations.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/utils/query_metrics.py` & `sliderule-3.6.0/utils/query_metrics.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/utils/query_photons.py` & `sliderule-3.6.0/utils/query_photons.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/utils/query_stac.py` & `sliderule-3.6.0/utils/query_stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/utils/query_version.py` & `sliderule-3.6.0/utils/query_version.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/utils/region_of_interest.py` & `sliderule-3.6.0/utils/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/utils/results_to_s3.py` & `sliderule-3.6.0/utils/results_to_s3.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/utils/stac.py` & `sliderule-3.6.0/utils/stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/utils/stream_events.py` & `sliderule-3.6.0/utils/stream_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/utils/tail_events.py` & `sliderule-3.6.0/utils/tail_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.5.0/utils/utils.py` & `sliderule-3.6.0/utils/utils.py`

 * *Files identical despite different names*

