# Comparing `tmp/vallarisStreaming-0.0.2.tar.gz` & `tmp/vallarisStreaming-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vallarisStreaming-0.0.2.tar", last modified: Mon Jul 10 09:57:53 2023, max compression
+gzip compressed data, was "vallarisStreaming-0.0.3.tar", last modified: Mon Jul 10 10:08:24 2023, max compression
```

## Comparing `vallarisStreaming-0.0.2.tar` & `vallarisStreaming-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:57:53.017422 vallarisStreaming-0.0.2/
--rw-r--r--   0 root         (0) root         (0)     1776 2023-07-10 09:57:53.010786 vallarisStreaming-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1125 2022-02-28 05:06:07.000000 vallarisStreaming-0.0.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 09:57:53.021012 vallarisStreaming-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      887 2023-07-10 09:57:32.000000 vallarisStreaming-0.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:57:52.901412 vallarisStreaming-0.0.2/vallarisStreaming/
--rw-r--r--   0 root         (0) root         (0)       59 2022-11-14 09:26:26.000000 vallarisStreaming-0.0.2/vallarisStreaming/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10176 2023-07-10 09:56:46.000000 vallarisStreaming-0.0.2/vallarisStreaming/perform.py
--rw-r--r--   0 root         (0) root         (0)    15092 2023-02-04 10:04:36.000000 vallarisStreaming-0.0.2/vallarisStreaming/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:57:52.994224 vallarisStreaming-0.0.2/vallarisStreaming.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1776 2023-07-10 09:57:52.000000 vallarisStreaming-0.0.2/vallarisStreaming.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      308 2023-07-10 09:57:52.000000 vallarisStreaming-0.0.2/vallarisStreaming.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 09:57:52.000000 vallarisStreaming-0.0.2/vallarisStreaming.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-07-10 09:57:52.000000 vallarisStreaming-0.0.2/vallarisStreaming.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-10 09:57:52.000000 vallarisStreaming-0.0.2/vallarisStreaming.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:08:24.975976 vallarisStreaming-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1776 2023-07-10 10:08:24.970134 vallarisStreaming-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1125 2022-02-28 05:06:07.000000 vallarisStreaming-0.0.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 10:08:24.979050 vallarisStreaming-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      887 2023-07-10 10:08:22.000000 vallarisStreaming-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:08:24.871245 vallarisStreaming-0.0.3/vallarisStreaming/
+-rw-r--r--   0 root         (0) root         (0)       77 2023-07-10 10:07:41.000000 vallarisStreaming-0.0.3/vallarisStreaming/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10185 2023-07-10 10:07:18.000000 vallarisStreaming-0.0.3/vallarisStreaming/perform.py
+-rw-r--r--   0 root         (0) root         (0)    15092 2023-02-04 10:04:36.000000 vallarisStreaming-0.0.3/vallarisStreaming/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 10:08:24.954263 vallarisStreaming-0.0.3/vallarisStreaming.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1776 2023-07-10 10:08:24.000000 vallarisStreaming-0.0.3/vallarisStreaming.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      308 2023-07-10 10:08:24.000000 vallarisStreaming-0.0.3/vallarisStreaming.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 10:08:24.000000 vallarisStreaming-0.0.3/vallarisStreaming.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-07-10 10:08:24.000000 vallarisStreaming-0.0.3/vallarisStreaming.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-10 10:08:24.000000 vallarisStreaming-0.0.3/vallarisStreaming.egg-info/top_level.txt
```

### Comparing `vallarisStreaming-0.0.2/PKG-INFO` & `vallarisStreaming-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vallarisStreaming
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to processing Vallaris Maps
 Home-page: https://v2k.vallarismaps.com
 Author: Sattawat Arab
 Author-email: support@vallarismaps.com
 License: UNKNOWN
 Description: # Vallaris library
         A package to made for support Vallaris Maps
```

### Comparing `vallarisStreaming-0.0.2/README.md` & `vallarisStreaming-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `vallarisStreaming-0.0.2/setup.py` & `vallarisStreaming-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="vallarisStreaming", # Replace with your own username
-    version="0.0.2",
+    version="0.0.3",
     author="Sattawat Arab",
     author_email="support@vallarismaps.com",
     description="A package to processing Vallaris Maps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://v2k.vallarismaps.com",
     packages=setuptools.find_packages(),
```

### Comparing `vallarisStreaming-0.0.2/vallarisStreaming/perform.py` & `vallarisStreaming-0.0.3/vallarisStreaming/perform.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import requests
 import tarfile
 from geopandas import GeoSeries
 from shapely.geometry import Polygon
 import geopandas as gpd
 import pandas as pd
 from shapely.geometry import Polygon
-from vallaris.utils import *
+from vallarisStreaming.utils import *
 from IPython.display import display, Javascript, Markdown as md, HTML
 from urllib.parse import urlencode
 import zipfile
 from IPython.display import IFrame
 import rasterio
 from rasterio.plot import show
 import numpy as np
```

### Comparing `vallarisStreaming-0.0.2/vallarisStreaming/utils.py` & `vallarisStreaming-0.0.3/vallarisStreaming/utils.py`

 * *Files identical despite different names*

### Comparing `vallarisStreaming-0.0.2/vallarisStreaming.egg-info/PKG-INFO` & `vallarisStreaming-0.0.3/vallarisStreaming.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vallarisStreaming
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to processing Vallaris Maps
 Home-page: https://v2k.vallarismaps.com
 Author: Sattawat Arab
 Author-email: support@vallarismaps.com
 License: UNKNOWN
 Description: # Vallaris library
         A package to made for support Vallaris Maps
```

