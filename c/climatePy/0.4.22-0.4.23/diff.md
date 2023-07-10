# Comparing `tmp/climatePy-0.4.22.tar.gz` & `tmp/climatePy-0.4.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climatePy-0.4.22.tar", last modified: Thu Jul  6 22:05:41 2023, max compression
+gzip compressed data, was "climatePy-0.4.23.tar", last modified: Mon Jul 10 20:36:02 2023, max compression
```

## Comparing `climatePy-0.4.22.tar` & `climatePy-0.4.23.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:05:41.195930 climatePy-0.4.22/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-06 22:05:38.000000 climatePy-0.4.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-06 22:05:41.195930 climatePy-0.4.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-06 22:05:38.000000 climatePy-0.4.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:05:41.155930 climatePy-0.4.22/climatePy/
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-06 22:05:38.000000 climatePy-0.4.22/climatePy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-07-06 22:05:38.000000 climatePy-0.4.22/climatePy/_climatepy_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    59354 2023-07-06 22:05:38.000000 climatePy-0.4.22/climatePy/_dap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-06 22:05:38.000000 climatePy-0.4.22/climatePy/_netrc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-07-06 22:05:38.000000 climatePy-0.4.22/climatePy/_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    26691 2023-07-06 22:05:38.000000 climatePy-0.4.22/climatePy/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:05:41.155930 climatePy-0.4.22/climatePy/data/
--rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-06 22:05:38.000000 climatePy-0.4.22/climatePy/data/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:05:41.155930 climatePy-0.4.22/climatePy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-06 22:05:41.000000 climatePy-0.4.22/climatePy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-06 22:05:41.000000 climatePy-0.4.22/climatePy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 22:05:41.000000 climatePy-0.4.22/climatePy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-06 22:05:41.000000 climatePy-0.4.22/climatePy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 22:05:41.000000 climatePy-0.4.22/climatePy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 22:05:41.195930 climatePy-0.4.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-06 22:05:40.000000 climatePy-0.4.22/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:05:41.195930 climatePy-0.4.22/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 22:05:38.000000 climatePy-0.4.22/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43883 2023-07-06 22:05:38.000000 climatePy-0.4.22/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-06 22:05:38.000000 climatePy-0.4.22/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:36:02.712463 climatePy-0.4.23/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-10 20:35:59.000000 climatePy-0.4.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-10 20:36:02.712463 climatePy-0.4.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-10 20:35:59.000000 climatePy-0.4.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:36:02.656463 climatePy-0.4.23/climatePy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-10 20:35:59.000000 climatePy-0.4.23/climatePy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-07-10 20:35:59.000000 climatePy-0.4.23/climatePy/_climatepy_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59427 2023-07-10 20:35:59.000000 climatePy-0.4.23/climatePy/_dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-10 20:35:59.000000 climatePy-0.4.23/climatePy/_netrc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32764 2023-07-10 20:35:59.000000 climatePy-0.4.23/climatePy/_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26690 2023-07-10 20:35:59.000000 climatePy-0.4.23/climatePy/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:36:02.656463 climatePy-0.4.23/climatePy/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-10 20:35:59.000000 climatePy-0.4.23/climatePy/data/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:36:02.656463 climatePy-0.4.23/climatePy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-10 20:36:02.000000 climatePy-0.4.23/climatePy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-10 20:36:02.000000 climatePy-0.4.23/climatePy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:36:02.000000 climatePy-0.4.23/climatePy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 20:36:02.000000 climatePy-0.4.23/climatePy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 20:36:02.000000 climatePy-0.4.23/climatePy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 20:36:02.712463 climatePy-0.4.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-10 20:36:01.000000 climatePy-0.4.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:36:02.712463 climatePy-0.4.23/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:35:59.000000 climatePy-0.4.23/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-10 20:35:59.000000 climatePy-0.4.23/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-10 20:35:59.000000 climatePy-0.4.23/tests/test_utils.py
```

### Comparing `climatePy-0.4.22/LICENSE` & `climatePy-0.4.23/LICENSE`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.22/PKG-INFO` & `climatePy-0.4.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.22
+Version: 0.4.23
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.22/README.md` & `climatePy-0.4.23/README.md`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.22/climatePy/__init__.py` & `climatePy-0.4.23/climatePy/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,17 +17,14 @@
 from ._climatepy_filter import climatepy_filter
 from ._dap import dap, dap_crop, dap_get
 from ._shortcuts import getTerraClim, getTerraClimNormals, getGridMET, getMACA, \
     get3DEP, getLOCA, getPRISM, getPolaris, \
     getBCCA, getLivneh, getLivneh_fluxes, getISRIC_soils, getDaymet, \
     getVIC, getNASADEM, getWorldClim, getCHIRPS, getLCMAP, getNLDAS
 
-# can i do this and get the __all__ to grab all the functions from ._shortcuts.py ?
-# from ._shortcuts import *
-
 __all__ = [
     'climatepy_filter',
     'dap',
     'dap_crop',
     'dap_get',
     'getTerraClim',
     'getTerraClimNormals', 
@@ -48,15 +45,15 @@
     'getCHIRPS', 
     'getLCMAP',
     'getNLDAS',
     'params'
 ]
 
 ##############################
-# Old method
+# # Old method
 # import pandas as pd
 # import pkg_resources
 
 # def params():
 #     data_file = pkg_resources.resource_filename('climatePy', 'data/catalog.csv')
 #     # data_file = pkg_resources.resource_filename('src', 'data/catalog.csv')
 #     data = pd.read_csv(data_file)
```

### Comparing `climatePy-0.4.22/climatePy/_climatepy_filter.py` & `climatePy-0.4.23/climatePy/_climatepy_filter.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.22/climatePy/_dap.py` & `climatePy-0.4.23/climatePy/_dap.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,30 +24,32 @@
 # library for parallel processing
 from joblib import Parallel, delayed
 
 # import climatePy modules
 from . import _utils as utils
 from . import _climatepy_filter as climatepy_filter
 
+# from climatePy import _utils as utils
+# from climatePy import _climatepy_filter as climatepy_filter
+
 # warnings lib
 import warnings
 
 # suppress warnings
 warnings.filterwarnings('ignore', category=Warning)
 
 # from src.climatePy import climatepy_filter, utils
 # from climatePy import climatepy_filter, utils
 # import utils from src.climatePy
 # from climatePy import _utils, climatepy_filter
 # from climatePy import _utils, climatepy_filter
 # from climatePy import _utils, climatepy_filter
-# import ._utils as utils
-# import ._climatepy_filter as climatepy_filter
-# import _utils as utils
-# import _climatepy_filter as climatepy_filter
+
+######################################################
+######################################################
 
 def dap_crop(
     URL       = None,
     catalog   = None,
     AOI       = None, 
     startDate = None, 
     endDate   = None,
@@ -285,14 +287,15 @@
         end         = None,
         toptobottom = False,
         dopar       = True,
         verbose     = False
         ):
         
         """Get data from a DAP server"""
+    
 
         if not isinstance(toptobottom, bool):
 
             # print("Checking if all toptobottom values are Nan...")
 
             # convert to float to check for nan
             nan_chk = toptobottom.astype(float)
```

### Comparing `climatePy-0.4.22/climatePy/_netrc_utils.py` & `climatePy-0.4.23/climatePy/_netrc_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.22/climatePy/_shortcuts.py` & `climatePy-0.4.23/climatePy/_shortcuts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Data manipulation tools
 import pandas as pd
 import geopandas as gpd
 import xarray as xr
 import shapely
 from shapely.geometry import Point
-# import matplotlib.pyplot as plt
 
 # import climatePy modules
 from . import _utils as utils
 from . import _dap as dap
 from . import _climatepy_filter as climatepy_filter
 
 # import climatePy._utils as utils
@@ -21,15 +20,15 @@
 
 # suppress warnings
 warnings.filterwarnings('ignore', category=Warning)
 
 
 # test data
 # AOI    = gpd.read_file('climatePy/data/san_luis_obispo_county.gpkg')
-AOI    = gpd.read_file('climatePy/data/boulder_county.gpkg')
+# AOI    = gpd.read_file('climatePy/data/boulder_county.gpkg')
 
 # ----------------------
 # ---- getTerraClim ----
 # ----------------------
 
 def getTerraClim(
         AOI       = None,
```

### Comparing `climatePy-0.4.22/climatePy/_utils.py` & `climatePy-0.4.23/climatePy/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # data wrangling and manipulation
 import numpy as np
 import pandas as pd
 
 # warnings lib
 import warnings
 
-
 # suppress warnings
 warnings.filterwarnings('ignore', category=Warning)
 
 def getExtension(x):
     """Extract the file extension from a string"""
 
     dot_pos = x.rfind('.')
```

### Comparing `climatePy-0.4.22/climatePy/data/catalog.csv` & `climatePy-0.4.23/climatePy/data/catalog.csv`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.22/climatePy.egg-info/PKG-INFO` & `climatePy-0.4.23/climatePy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.22
+Version: 0.4.23
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.22/setup.py` & `climatePy-0.4.23/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="climatePy",                         # pkg name
     # version="0.0.4.24",                        # version
-    version='0.4.22',
+    version='0.4.23',
     author="Angus Watters, Mike Johnson",     # authors
     description="A Python package for getting point and gridded climate data by AOI",
     long_description=long_description,      # long description is read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # python modules to install
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `climatePy-0.4.22/tests/test_shortcuts.py` & `climatePy-0.4.23/tests/test_shortcuts.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 # from .climatePy import shortcuts
 # from src.climatePy import shortcuts
 # from src.climatePy import dap
 # from src.climatePy import climatepy_filter
 # from src.climatePy import utils
 
 # AOI    = gpd.read_file('climatePy/data/boulder_county.gpkg')
+
+# climatePy.getGridMET(AOI, "pr", "2000-01-01", "2000-01-01", verbose=True)
 # AOI    = gpd.read_file('climatePy/data/san_luis_obispo_county.gpkg')
 
 # @pytest.fixture(params=['miami_dade_county', 'san_luis_obispo_county', 
 #                         'litchfield_county', 'tuscaloosa_county', 
 #                         'boulder_county', 'king_county'])
 
 @pytest.fixture(params=['san_luis_obispo_county', 'boulder_county'])
```

### Comparing `climatePy-0.4.22/tests/test_utils.py` & `climatePy-0.4.23/tests/test_utils.py`

 * *Files identical despite different names*

