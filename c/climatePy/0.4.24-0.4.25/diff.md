# Comparing `tmp/climatePy-0.4.24.tar.gz` & `tmp/climatePy-0.4.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climatePy-0.4.24.tar", last modified: Mon Jul 10 21:04:48 2023, max compression
+gzip compressed data, was "climatePy-0.4.25.tar", last modified: Mon Jul 10 21:24:10 2023, max compression
```

## Comparing `climatePy-0.4.24.tar` & `climatePy-0.4.25.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:04:48.205310 climatePy-0.4.24/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-10 21:04:45.000000 climatePy-0.4.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-10 21:04:48.205310 climatePy-0.4.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-10 21:04:45.000000 climatePy-0.4.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:04:48.161309 climatePy-0.4.24/climatePy/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-10 21:04:45.000000 climatePy-0.4.24/climatePy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20016 2023-07-10 21:04:45.000000 climatePy-0.4.24/climatePy/_climatepy_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    59427 2023-07-10 21:04:45.000000 climatePy-0.4.24/climatePy/_dap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-10 21:04:45.000000 climatePy-0.4.24/climatePy/_netrc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    32764 2023-07-10 21:04:45.000000 climatePy-0.4.24/climatePy/_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    26690 2023-07-10 21:04:45.000000 climatePy-0.4.24/climatePy/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:04:48.161309 climatePy-0.4.24/climatePy/data/
--rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-10 21:04:45.000000 climatePy-0.4.24/climatePy/data/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:04:48.161309 climatePy-0.4.24/climatePy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-10 21:04:48.000000 climatePy-0.4.24/climatePy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-10 21:04:48.000000 climatePy-0.4.24/climatePy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 21:04:48.000000 climatePy-0.4.24/climatePy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 21:04:48.000000 climatePy-0.4.24/climatePy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 21:04:48.000000 climatePy-0.4.24/climatePy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 21:04:48.205310 climatePy-0.4.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-10 21:04:47.000000 climatePy-0.4.24/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:04:48.205310 climatePy-0.4.24/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:04:45.000000 climatePy-0.4.24/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-10 21:04:45.000000 climatePy-0.4.24/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-10 21:04:45.000000 climatePy-0.4.24/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:24:10.049995 climatePy-0.4.25/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-10 21:24:07.000000 climatePy-0.4.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-10 21:24:10.049995 climatePy-0.4.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-10 21:24:07.000000 climatePy-0.4.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:24:10.009995 climatePy-0.4.25/climatePy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-10 21:24:07.000000 climatePy-0.4.25/climatePy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20034 2023-07-10 21:24:07.000000 climatePy-0.4.25/climatePy/_climatepy_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59218 2023-07-10 21:24:07.000000 climatePy-0.4.25/climatePy/_dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-10 21:24:07.000000 climatePy-0.4.25/climatePy/_netrc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32764 2023-07-10 21:24:07.000000 climatePy-0.4.25/climatePy/_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26690 2023-07-10 21:24:07.000000 climatePy-0.4.25/climatePy/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:24:10.009995 climatePy-0.4.25/climatePy/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-10 21:24:07.000000 climatePy-0.4.25/climatePy/data/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:24:10.009995 climatePy-0.4.25/climatePy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-10 21:24:09.000000 climatePy-0.4.25/climatePy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-10 21:24:10.000000 climatePy-0.4.25/climatePy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 21:24:09.000000 climatePy-0.4.25/climatePy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 21:24:09.000000 climatePy-0.4.25/climatePy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 21:24:09.000000 climatePy-0.4.25/climatePy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 21:24:10.049995 climatePy-0.4.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-10 21:24:09.000000 climatePy-0.4.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:24:10.049995 climatePy-0.4.25/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:24:07.000000 climatePy-0.4.25/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-10 21:24:07.000000 climatePy-0.4.25/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-10 21:24:07.000000 climatePy-0.4.25/tests/test_utils.py
```

### Comparing `climatePy-0.4.24/LICENSE` & `climatePy-0.4.25/LICENSE`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.24/PKG-INFO` & `climatePy-0.4.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.24
+Version: 0.4.25
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.24/README.md` & `climatePy-0.4.25/README.md`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.24/climatePy/__init__.py` & `climatePy-0.4.25/climatePy/__init__.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.24/climatePy/_climatepy_filter.py` & `climatePy-0.4.25/climatePy/_climatepy_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,24 +291,24 @@
 
         if scenario is not None:
             if isinstance(scenario, str):
                 catalog = catalog[catalog['scenario'].str.contains(scenario)]
             elif isinstance(scenario, list):
                 catalog = catalog[catalog['scenario'].str.contains('|'.join(scenario))]
 
-    # If AOI is a shapely geometry, convert AOI into GeoPandas dataframe 
-    if isinstance(AOI, (shapely.geometry.point.Point, 
-            shapely.geometry.multipoint.MultiPoint,
-            shapely.geometry.linestring.LineString, 
-            shapely.geometry.multilinestring.MultiLineString, 
-            shapely.geometry.polygon.Polygon, 
-            shapely.geometry.multipolygon.MultiPolygon)):
+    # # If AOI is a shapely geometry, convert AOI into GeoPandas dataframe 
+    # if isinstance(AOI, (shapely.geometry.point.Point, 
+    #         shapely.geometry.multipoint.MultiPoint,
+    #         shapely.geometry.linestring.LineString, 
+    #         shapely.geometry.multilinestring.MultiLineString, 
+    #         shapely.geometry.polygon.Polygon, 
+    #         shapely.geometry.multipolygon.MultiPolygon)):
         
-        # convert shapely geometry to geopandas dataframe
-        AOI = shapely_to_gpd(AOI)
+    #     # convert shapely geometry to geopandas dataframe
+    #     AOI = shapely_to_gpd(AOI)
 
     # 5. AOI filter
     if AOI is not None:
         catalog = find_intersects(
             catalog = catalog,
             AOI     = AOI
             )
```

### Comparing `climatePy-0.4.24/climatePy/_dap.py` & `climatePy-0.4.25/climatePy/_dap.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,29 +375,29 @@
             dap_data = dap_crop(
                 URL       = URL,
                 catalog   = catalog,
                 AOI       = AOI,
                 startDate = startDate,
                 endDate   = endDate,
                 varname   = varname,
-                verbose   = False
+                verbose   = verbose
                 )
             
             # if dopar:
             #     if verbose:
             #         print("Getting DAP data in parallel")
             # else:
             #     if verbose:
             #         print("Getting DAP data in serial")
 
             # get dap data
             dap_data = dap_get(
                 dap_data = dap_data,
                 dopar    = dopar,
-                verbose  = False
+                verbose  = verbose
                 )
             
             return dap_data
         
 def match_args(func, *args, **kwargs):
 
     """Match default arguments for a function.
@@ -1309,15 +1309,15 @@
 #     """
 
     if URL is None:
         URL = catalog.URL.to_list()
 
     if verbose:
         print("Opening VRT from URL: ", URL)
- 
+
     # Area of interest
     vrts = crop_vrt(urls = URL, AOI = AOI, verbose = verbose)
 
     # vrts2 = Parallel(n_jobs=-1)(delayed(crop_vrt) (urls = [i],
     #                                     AOI  = AOI,
     #                                     verbose = False
     #                                     ) for i in URL)
@@ -1355,75 +1355,75 @@
 
     # create dictionary of DataArrays
     vrts = dict(zip(catalog['variable'], vrts))
 
     return vrts
 
 def parse_date(duration, interval):
-        """Parse the date range based on the duration and interval.
+    """Parse the date range based on the duration and interval.
 
-        Args:
-            duration (str): The duration string in the format "start_date/end_date".
-            interval (str): The interval string specifying the time unit.
-        
-        Returns:
-            pd.DatetimeIndex: A pandas DatetimeIndex representing the parsed date range.
-        """
-        
-        # split duration string
-        d = duration.split("/")
-        
-        # if end date is "..", set it to today's date
-        if d[1] == "..":
-                d[1] = datetime.now().strftime("%Y-%m-%d")
-
-        # if interval in ["1 month", "1 months"]:
-        if any(keyword in interval for keyword in ["1 month", "1 months", "monthly"]):
-        # if any(keyword in interval for keyword in ["1 month", "1 months", "31 days", "monthly"]):
-                d[0] = datetime.strptime(d[0], "%Y-%m-%d").strftime("%Y-%m-01")
-
-        # if interval in ["hour", "hours"]:
-        if any(keyword in interval for keyword in ["hour", "hours"]):
-                d[0] = datetime.strptime(d[0], "%Y-%m-%d").strftime("%Y-%m-%d %H:%M:%S")
-                d[1] = datetime.strptime(d[1], "%Y-%m-%d").strftime("%Y-%m-%d %H:%M:%S")
-
-        # if interval is 31 days, change to 1 month
-        if interval in ["31 days","31.5 days"]:
-            interval = "1 month"
-
-        # if interval is 365, 365.5 days, change to 1 year
-        if interval in ["365 days","365.5 days"]:
-            interval = "1 year"
-
-        interval_map = {
-            "hour": "H",
-            "hours": "H",
-            "minute": "min",
-            "minutes": "min",
-            "second": "S",
-            "seconds": "S",
-            "month": "MS",  # Month Start
-            "months": "MS"  # Month Start
-            }
-        
-        # split interval string
-        interval_type = interval.split(" ")[-1]
+    Args:
+        duration (str): The duration string in the format "start_date/end_date".
+        interval (str): The interval string specifying the time unit.
+    
+    Returns:
+        pd.DatetimeIndex: A pandas DatetimeIndex representing the parsed date range.
+    """
+    
+    # split duration string
+    d = duration.split("/")
+    
+    # if end date is "..", set it to today's date
+    if d[1] == "..":
+            d[1] = datetime.now().strftime("%Y-%m-%d")
+
+    # if interval in ["1 month", "1 months"]:
+    if any(keyword in interval for keyword in ["1 month", "1 months", "monthly"]):
+    # if any(keyword in interval for keyword in ["1 month", "1 months", "31 days", "monthly"]):
+            d[0] = datetime.strptime(d[0], "%Y-%m-%d").strftime("%Y-%m-01")
+
+    # if interval in ["hour", "hours"]:
+    if any(keyword in interval for keyword in ["hour", "hours"]):
+            d[0] = datetime.strptime(d[0], "%Y-%m-%d").strftime("%Y-%m-%d %H:%M:%S")
+            d[1] = datetime.strptime(d[1], "%Y-%m-%d").strftime("%Y-%m-%d %H:%M:%S")
+
+    # if interval is 31 days, change to 1 month
+    if interval in ["31 days","31.5 days"]:
+        interval = "1 month"
+
+    # if interval is 365, 365.5 days, change to 1 year
+    if interval in ["365 days","365.5 days"]:
+        interval = "1 year"
+
+    interval_map = {
+        "hour": "H",
+        "hours": "H",
+        "minute": "min",
+        "minutes": "min",
+        "second": "S",
+        "seconds": "S",
+        "month": "MS",  # Month Start
+        "months": "MS"  # Month Start
+        }
+    
+    # split interval string
+    interval_type = interval.split(" ")[-1]
 
-        # get frequency from interval_map
-        freq = interval_map.get(interval_type, interval_type[0])
-        
-        # # convert start_date and end_date to pandas Timestamp objects
-        # start_date = pd.Timestamp(d[0])
-        # end_date = pd.Timestamp(d[1])
-        # # calculate the number of days between start and end dates
-        # delta = (end_date - start_date) / (nT - 1)
-        # # generate the date range
-        # date_range = pd.date_range(start=start_date, end=end_date, freq=str(int(delta.days))+'D')
+    # get frequency from interval_map
+    freq = interval_map.get(interval_type, interval_type[0])
+    
+    # # convert start_date and end_date to pandas Timestamp objects
+    # start_date = pd.Timestamp(d[0])
+    # end_date = pd.Timestamp(d[1])
+    # # calculate the number of days between start and end dates
+    # delta = (end_date - start_date) / (nT - 1)
+    # # generate the date range
+    # date_range = pd.date_range(start=start_date, end=end_date, freq=str(int(delta.days))+'D')
 
-        return pd.date_range(start=d[0], end=d[1], freq=freq)
+    return pd.date_range(start=d[0], end=d[1], freq=freq)
 
 # def parse_date2(duration, nT):
     # duration = catalog["duration"].iloc[i]
     # interval = catalog["interval"].iloc[i]
     # nT = catalog["nT"].iloc[i]
 #     d = duration.split("/")
 #     if d[1] == "..":
```

### Comparing `climatePy-0.4.24/climatePy/_netrc_utils.py` & `climatePy-0.4.25/climatePy/_netrc_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.24/climatePy/_shortcuts.py` & `climatePy-0.4.25/climatePy/_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.24/climatePy/_utils.py` & `climatePy-0.4.25/climatePy/_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.24/climatePy/data/catalog.csv` & `climatePy-0.4.25/climatePy/data/catalog.csv`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.24/climatePy.egg-info/PKG-INFO` & `climatePy-0.4.25/climatePy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.24
+Version: 0.4.25
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.24/setup.py` & `climatePy-0.4.25/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="climatePy",                         # pkg name
     # version="0.0.4.24",                        # version
-    version='0.4.24',
+    version='0.4.25',
     author="Angus Watters, Mike Johnson",     # authors
     description="A Python package for getting point and gridded climate data by AOI",
     long_description=long_description,      # long description is read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # python modules to install
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `climatePy-0.4.24/tests/test_shortcuts.py` & `climatePy-0.4.25/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.24/tests/test_utils.py` & `climatePy-0.4.25/tests/test_utils.py`

 * *Files identical despite different names*

