# Comparing `tmp/vallarisStreaming-0.0.1.tar.gz` & `tmp/vallarisStreaming-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vallarisStreaming-0.0.1.tar", last modified: Mon Jul 10 09:48:34 2023, max compression
+gzip compressed data, was "vallarisStreaming-0.0.2.tar", last modified: Mon Jul 10 09:57:53 2023, max compression
```

## Comparing `vallarisStreaming-0.0.1.tar` & `vallarisStreaming-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:48:34.636435 vallarisStreaming-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1776 2023-07-10 09:48:34.631215 vallarisStreaming-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1125 2022-02-28 05:06:07.000000 vallarisStreaming-0.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 09:48:34.638824 vallarisStreaming-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      875 2023-07-10 08:46:16.000000 vallarisStreaming-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:48:34.526895 vallarisStreaming-0.0.1/vallarisStreaming/
--rw-r--r--   0 root         (0) root         (0)       59 2022-11-14 09:26:26.000000 vallarisStreaming-0.0.1/vallarisStreaming/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10176 2023-07-10 09:42:12.000000 vallarisStreaming-0.0.1/vallarisStreaming/perform.py
--rw-r--r--   0 root         (0) root         (0)    15092 2023-02-04 10:04:36.000000 vallarisStreaming-0.0.1/vallarisStreaming/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:48:34.617118 vallarisStreaming-0.0.1/vallarisStreaming.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1776 2023-07-10 09:48:34.000000 vallarisStreaming-0.0.1/vallarisStreaming.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      308 2023-07-10 09:48:34.000000 vallarisStreaming-0.0.1/vallarisStreaming.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 09:48:34.000000 vallarisStreaming-0.0.1/vallarisStreaming.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      125 2023-07-10 09:48:34.000000 vallarisStreaming-0.0.1/vallarisStreaming.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-10 09:48:34.000000 vallarisStreaming-0.0.1/vallarisStreaming.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:57:53.017422 vallarisStreaming-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1776 2023-07-10 09:57:53.010786 vallarisStreaming-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1125 2022-02-28 05:06:07.000000 vallarisStreaming-0.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 09:57:53.021012 vallarisStreaming-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      887 2023-07-10 09:57:32.000000 vallarisStreaming-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:57:52.901412 vallarisStreaming-0.0.2/vallarisStreaming/
+-rw-r--r--   0 root         (0) root         (0)       59 2022-11-14 09:26:26.000000 vallarisStreaming-0.0.2/vallarisStreaming/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10176 2023-07-10 09:56:46.000000 vallarisStreaming-0.0.2/vallarisStreaming/perform.py
+-rw-r--r--   0 root         (0) root         (0)    15092 2023-02-04 10:04:36.000000 vallarisStreaming-0.0.2/vallarisStreaming/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:57:52.994224 vallarisStreaming-0.0.2/vallarisStreaming.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1776 2023-07-10 09:57:52.000000 vallarisStreaming-0.0.2/vallarisStreaming.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      308 2023-07-10 09:57:52.000000 vallarisStreaming-0.0.2/vallarisStreaming.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 09:57:52.000000 vallarisStreaming-0.0.2/vallarisStreaming.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-07-10 09:57:52.000000 vallarisStreaming-0.0.2/vallarisStreaming.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-10 09:57:52.000000 vallarisStreaming-0.0.2/vallarisStreaming.egg-info/top_level.txt
```

### Comparing `vallarisStreaming-0.0.1/PKG-INFO` & `vallarisStreaming-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vallarisStreaming
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to processing Vallaris Maps
 Home-page: https://v2k.vallarismaps.com
 Author: Sattawat Arab
 Author-email: support@vallarismaps.com
 License: UNKNOWN
 Description: # Vallaris library
         A package to made for support Vallaris Maps
```

### Comparing `vallarisStreaming-0.0.1/README.md` & `vallarisStreaming-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vallarisStreaming-0.0.1/setup.py` & `vallarisStreaming-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="vallarisStreaming", # Replace with your own username
-    version="0.0.1",
+    version="0.0.2",
     author="Sattawat Arab",
     author_email="support@vallarismaps.com",
     description="A package to processing Vallaris Maps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://v2k.vallarismaps.com",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires= ['xmltodict','jsonschema','ndjson','geojson','requests','geopandas','pandas', 'rtree', 'numpy','shapely','tqdm', 'python-dotenv', 'matplotlib', 'earthpy', 'uuid'],
+    install_requires= ['xmltodict','jsonschema','ndjson','geojson','requests','geopandas','pandas', 'rtree', 'numpy','shapely','tqdm', 'python-dotenv', 'matplotlib', 'earthpy', 'uuid', 'rasterio'],
     python_requires='>=3.6',
 )
```

### Comparing `vallarisStreaming-0.0.1/vallarisStreaming/perform.py` & `vallarisStreaming-0.0.2/vallarisStreaming/perform.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     except:
         Api_Key = os.environ["APIKey"]
         VallarisServer = os.environ["VallarisServer"]
 
     return [Api_Key, VallarisServer]
 
 
-def ConnectData(property):
+def connectData(property):
 
     try :
         get_data = property
         host = os.environ["VallarisServer"]
         APIKey = os.environ["APIKey"]
         # print(host)
         # get Properties
@@ -229,15 +229,15 @@
         return gdf
     
     except Exception as e:
         # print(e)
         msg = "Perform step Connect Data KeyError: " + str(e)
         return msg
 
-def FetchData(PARAMETER, *args, **kwargs):
+def fetchData(PARAMETER, *args, **kwargs):
     AGRITRONIC_API_URL = kwargs.get('AGRITRONIC_API_URL', False)
     AGRITRONIC_APP_KEY = kwargs.get('AGRITRONIC_APP_KEY', False)
     VALALRIS_API_URL = kwargs.get('VALALRIS_API_URL', False)
     VALALRIS_API_KEY = kwargs.get('VALALRIS_API_KEY', False)
     STATION_ID = kwargs.get('STATION_ID', False)
     DATA_DATE = kwargs.get('DATA_DATE', False)
```

### Comparing `vallarisStreaming-0.0.1/vallarisStreaming/utils.py` & `vallarisStreaming-0.0.2/vallarisStreaming/utils.py`

 * *Files identical despite different names*

### Comparing `vallarisStreaming-0.0.1/vallarisStreaming.egg-info/PKG-INFO` & `vallarisStreaming-0.0.2/vallarisStreaming.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vallarisStreaming
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to processing Vallaris Maps
 Home-page: https://v2k.vallarismaps.com
 Author: Sattawat Arab
 Author-email: support@vallarismaps.com
 License: UNKNOWN
 Description: # Vallaris library
         A package to made for support Vallaris Maps
```

