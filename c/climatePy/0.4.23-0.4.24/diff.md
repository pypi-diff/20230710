# Comparing `tmp/climatePy-0.4.23.tar.gz` & `tmp/climatePy-0.4.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climatePy-0.4.23.tar", last modified: Mon Jul 10 20:36:02 2023, max compression
+gzip compressed data, was "climatePy-0.4.24.tar", last modified: Mon Jul 10 21:04:48 2023, max compression
```

## Comparing `climatePy-0.4.23.tar` & `climatePy-0.4.24.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:36:02.712463 climatePy-0.4.23/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-10 20:35:59.000000 climatePy-0.4.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-10 20:36:02.712463 climatePy-0.4.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-10 20:35:59.000000 climatePy-0.4.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:36:02.656463 climatePy-0.4.23/climatePy/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-10 20:35:59.000000 climatePy-0.4.23/climatePy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-07-10 20:35:59.000000 climatePy-0.4.23/climatePy/_climatepy_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    59427 2023-07-10 20:35:59.000000 climatePy-0.4.23/climatePy/_dap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-10 20:35:59.000000 climatePy-0.4.23/climatePy/_netrc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    32764 2023-07-10 20:35:59.000000 climatePy-0.4.23/climatePy/_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    26690 2023-07-10 20:35:59.000000 climatePy-0.4.23/climatePy/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:36:02.656463 climatePy-0.4.23/climatePy/data/
--rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-10 20:35:59.000000 climatePy-0.4.23/climatePy/data/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:36:02.656463 climatePy-0.4.23/climatePy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-10 20:36:02.000000 climatePy-0.4.23/climatePy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-10 20:36:02.000000 climatePy-0.4.23/climatePy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:36:02.000000 climatePy-0.4.23/climatePy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 20:36:02.000000 climatePy-0.4.23/climatePy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 20:36:02.000000 climatePy-0.4.23/climatePy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 20:36:02.712463 climatePy-0.4.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-10 20:36:01.000000 climatePy-0.4.23/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:36:02.712463 climatePy-0.4.23/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:35:59.000000 climatePy-0.4.23/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-10 20:35:59.000000 climatePy-0.4.23/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-10 20:35:59.000000 climatePy-0.4.23/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:04:48.205310 climatePy-0.4.24/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-10 21:04:45.000000 climatePy-0.4.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-10 21:04:48.205310 climatePy-0.4.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-10 21:04:45.000000 climatePy-0.4.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:04:48.161309 climatePy-0.4.24/climatePy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-10 21:04:45.000000 climatePy-0.4.24/climatePy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20016 2023-07-10 21:04:45.000000 climatePy-0.4.24/climatePy/_climatepy_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59427 2023-07-10 21:04:45.000000 climatePy-0.4.24/climatePy/_dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-10 21:04:45.000000 climatePy-0.4.24/climatePy/_netrc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32764 2023-07-10 21:04:45.000000 climatePy-0.4.24/climatePy/_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26690 2023-07-10 21:04:45.000000 climatePy-0.4.24/climatePy/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:04:48.161309 climatePy-0.4.24/climatePy/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-10 21:04:45.000000 climatePy-0.4.24/climatePy/data/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:04:48.161309 climatePy-0.4.24/climatePy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-10 21:04:48.000000 climatePy-0.4.24/climatePy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-10 21:04:48.000000 climatePy-0.4.24/climatePy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 21:04:48.000000 climatePy-0.4.24/climatePy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 21:04:48.000000 climatePy-0.4.24/climatePy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 21:04:48.000000 climatePy-0.4.24/climatePy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 21:04:48.205310 climatePy-0.4.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-10 21:04:47.000000 climatePy-0.4.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:04:48.205310 climatePy-0.4.24/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:04:45.000000 climatePy-0.4.24/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-10 21:04:45.000000 climatePy-0.4.24/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-10 21:04:45.000000 climatePy-0.4.24/tests/test_utils.py
```

### Comparing `climatePy-0.4.23/LICENSE` & `climatePy-0.4.24/LICENSE`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.23/PKG-INFO` & `climatePy-0.4.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.23
+Version: 0.4.24
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.23/README.md` & `climatePy-0.4.24/README.md`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.23/climatePy/__init__.py` & `climatePy-0.4.24/climatePy/__init__.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.23/climatePy/_climatepy_filter.py` & `climatePy-0.4.24/climatePy/_climatepy_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,15 +303,15 @@
             shapely.geometry.polygon.Polygon, 
             shapely.geometry.multipolygon.MultiPolygon)):
         
         # convert shapely geometry to geopandas dataframe
         AOI = shapely_to_gpd(AOI)
 
     # 5. AOI filter
-    if AOI is None:
+    if AOI is not None:
         catalog = find_intersects(
             catalog = catalog,
             AOI     = AOI
             )
         
     # remove duplicates
     catalog = catalog[~catalog.drop(['URL'], axis=1).duplicated()]
```

### Comparing `climatePy-0.4.23/climatePy/_dap.py` & `climatePy-0.4.24/climatePy/_dap.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.23/climatePy/_netrc_utils.py` & `climatePy-0.4.24/climatePy/_netrc_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.23/climatePy/_shortcuts.py` & `climatePy-0.4.24/climatePy/_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.23/climatePy/_utils.py` & `climatePy-0.4.24/climatePy/_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.23/climatePy/data/catalog.csv` & `climatePy-0.4.24/climatePy/data/catalog.csv`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.23/climatePy.egg-info/PKG-INFO` & `climatePy-0.4.24/climatePy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.23
+Version: 0.4.24
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.23/setup.py` & `climatePy-0.4.24/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="climatePy",                         # pkg name
     # version="0.0.4.24",                        # version
-    version='0.4.23',
+    version='0.4.24',
     author="Angus Watters, Mike Johnson",     # authors
     description="A Python package for getting point and gridded climate data by AOI",
     long_description=long_description,      # long description is read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # python modules to install
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `climatePy-0.4.23/tests/test_shortcuts.py` & `climatePy-0.4.24/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.23/tests/test_utils.py` & `climatePy-0.4.24/tests/test_utils.py`

 * *Files identical despite different names*

