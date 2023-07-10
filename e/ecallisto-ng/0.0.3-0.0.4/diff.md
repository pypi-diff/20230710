# Comparing `tmp/ecallisto_ng-0.0.3.tar.gz` & `tmp/ecallisto_ng-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecallisto_ng-0.0.3.tar", last modified: Thu Jul  6 22:30:47 2023, max compression
+gzip compressed data, was "ecallisto_ng-0.0.4.tar", last modified: Mon Jul 10 17:33:35 2023, max compression
```

## Comparing `ecallisto_ng-0.0.3.tar` & `ecallisto_ng-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 22:30:47.207938 ecallisto_ng-0.0.3/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.0.3/LICENSE
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1615 2023-07-06 22:30:47.207938 ecallisto_ng-0.0.3/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1035 2023-07-06 20:56:31.000000 ecallisto_ng-0.0.3/README.md
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      808 2023-07-06 22:30:39.000000 ecallisto_ng-0.0.3/pyproject.toml
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-06 22:30:47.207938 ecallisto_ng-0.0.3/setup.cfg
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 22:30:47.207938 ecallisto_ng-0.0.3/src/
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 22:30:47.207938 ecallisto_ng-0.0.3/src/ecallisto_ng/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.0.3/src/ecallisto_ng/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 22:30:47.207938 ecallisto_ng-0.0.3/src/ecallisto_ng/data_fetching/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2966 2023-07-06 22:28:49.000000 ecallisto_ng-0.0.3/src/ecallisto_ng/data_fetching/get_data.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 22:30:47.207938 ecallisto_ng-0.0.3/src/ecallisto_ng/plotting/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2172 2023-07-06 18:11:00.000000 ecallisto_ng-0.0.3/src/ecallisto_ng/plotting/plotting_utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 22:30:47.207938 ecallisto_ng-0.0.3/src/ecallisto_ng.egg-info/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1615 2023-07-06 22:30:47.000000 ecallisto_ng-0.0.3/src/ecallisto_ng.egg-info/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      347 2023-07-06 22:30:47.000000 ecallisto_ng-0.0.3/src/ecallisto_ng.egg-info/SOURCES.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-06 22:30:47.000000 ecallisto_ng-0.0.3/src/ecallisto_ng.egg-info/dependency_links.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       92 2023-07-06 22:30:47.000000 ecallisto_ng-0.0.3/src/ecallisto_ng.egg-info/requires.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-06 22:30:47.000000 ecallisto_ng-0.0.3/src/ecallisto_ng.egg-info/top_level.txt
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:33:35.758959 ecallisto_ng-0.0.4/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.0.4/LICENSE
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1615 2023-07-10 17:33:35.758959 ecallisto_ng-0.0.4/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1035 2023-07-10 17:29:49.000000 ecallisto_ng-0.0.4/README.md
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      836 2023-07-10 17:27:25.000000 ecallisto_ng-0.0.4/pyproject.toml
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-10 17:33:35.758959 ecallisto_ng-0.0.4/setup.cfg
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:33:35.758959 ecallisto_ng-0.0.4/src/
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:33:35.758959 ecallisto_ng-0.0.4/src/ecallisto_ng/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.0.4/src/ecallisto_ng/__init__.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:33:35.758959 ecallisto_ng-0.0.4/src/ecallisto_ng/data_fetching/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3096 2023-07-10 16:52:06.000000 ecallisto_ng-0.0.4/src/ecallisto_ng/data_fetching/get_data.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:33:35.758959 ecallisto_ng-0.0.4/src/ecallisto_ng/data_processing/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     4716 2023-07-10 17:16:31.000000 ecallisto_ng-0.0.4/src/ecallisto_ng/data_processing/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:33:35.758959 ecallisto_ng-0.0.4/src/ecallisto_ng/plotting/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2392 2023-07-10 17:23:39.000000 ecallisto_ng-0.0.4/src/ecallisto_ng/plotting/plotting_utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:33:35.758959 ecallisto_ng-0.0.4/src/ecallisto_ng.egg-info/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1615 2023-07-10 17:33:35.000000 ecallisto_ng-0.0.4/src/ecallisto_ng.egg-info/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      389 2023-07-10 17:33:35.000000 ecallisto_ng-0.0.4/src/ecallisto_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-10 17:33:35.000000 ecallisto_ng-0.0.4/src/ecallisto_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      113 2023-07-10 17:33:35.000000 ecallisto_ng-0.0.4/src/ecallisto_ng.egg-info/requires.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-10 17:33:35.000000 ecallisto_ng-0.0.4/src/ecallisto_ng.egg-info/top_level.txt
```

### Comparing `ecallisto_ng-0.0.3/LICENSE` & `ecallisto_ng-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.0.3/PKG-INFO` & `ecallisto_ng-0.0.4/src/ecallisto_ng.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
-Name: ecallisto_ng
-Version: 0.0.3
+Name: ecallisto-ng
+Version: 0.0.4
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ecallisto NG 
 ## Ecallisto NG is a very basic and simple package to access the Ecallisto API. 
-## It is written in Python 3.7 and uses the requests library and accesses the Ecallisto API at https://v000792.fhnw.ch/api/data
+## It is written in Python 3.9 and uses the requests library and accesses the Ecallisto API at https://v000792.fhnw.ch/api/data
 
 ## Installation
-Clone this repository and install it with pip:
+Clone this repository and install it with pip
 ```pip install -e .```
 ## PYPI
 This package is also available on PYPI: https://pypi.org/project/ecallisto-ng/
 ## Usage
 ### Data fetching
 ```python
 from ecallisto_ng.data_fetching.get_data import get_data
@@ -31,14 +31,15 @@
     "end_datetime": "2021-03-07 23:30:00",
     "timebucket": "15m",
     "agg_function": "MAX",
 }
 
 df = get_data(parameters)
 ```
+
 ### Plotting 
 We offer some basic plotting functions. 
 ```python
 from ecallisto_ng.plotting.plot import fill_missing_timesteps_with_nan, plot_spectogram
 
 df = fill_missing_timesteps_with_nan(df)
 plot_spectogram(df,  parameters["instrument_name"], parameters["start_datetime"], parameters["end_datetime"])
```

### Comparing `ecallisto_ng-0.0.3/README.md` & `ecallisto_ng-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Ecallisto NG 
 ## Ecallisto NG is a very basic and simple package to access the Ecallisto API. 
-## It is written in Python 3.7 and uses the requests library and accesses the Ecallisto API at https://v000792.fhnw.ch/api/data
+## It is written in Python 3.9 and uses the requests library and accesses the Ecallisto API at https://v000792.fhnw.ch/api/data
 
 ## Installation
-Clone this repository and install it with pip:
+Clone this repository and install it with pip
 ```pip install -e .```
 ## PYPI
 This package is also available on PYPI: https://pypi.org/project/ecallisto-ng/
 ## Usage
 ### Data fetching
 ```python
 from ecallisto_ng.data_fetching.get_data import get_data
@@ -17,14 +17,15 @@
     "end_datetime": "2021-03-07 23:30:00",
     "timebucket": "15m",
     "agg_function": "MAX",
 }
 
 df = get_data(parameters)
 ```
+
 ### Plotting 
 We offer some basic plotting functions. 
 ```python
 from ecallisto_ng.plotting.plot import fill_missing_timesteps_with_nan, plot_spectogram
 
 df = fill_missing_timesteps_with_nan(df)
 plot_spectogram(df,  parameters["instrument_name"], parameters["start_datetime"], parameters["end_datetime"])
```

### Comparing `ecallisto_ng-0.0.3/pyproject.toml` & `ecallisto_ng-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ecallisto_ng"
-version = "0.0.3"
+version = "0.0.4"
 authors = [{name = "Vincenzo Timmel", email = "vincenzo.timmel@fhnw.ch"}]
 description = "A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API."
 readme = "README.md"
 
 requires-python = ">=3.9"
 
 classifiers = [
@@ -15,14 +15,15 @@
 dependencies = [
     'ipython>=8.14.0',
     'nbformat>=5.9.0',
     'numpy>=1.25.0',
     'pandas>=2.0.3',
     'plotly>=5.15.0',
     'requests>=2.31.0',
+    'scikit-image>=0.21.0',
 
 ]
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `ecallisto_ng-0.0.3/src/ecallisto_ng/data_fetching/get_data.py` & `ecallisto_ng-0.0.4/src/ecallisto_ng/data_fetching/get_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,26 @@
 
 import pandas as pd
 import requests
 
 BASE_URL = "https://v000792.fhnw.ch"
 
 
-def get_data(instrument_name, start_datetime, end_datetime, timebucket=None, agg_function=None, return_type='json', verbose=False):
+def get_data(
+    instrument_name,
+    start_datetime,
+    end_datetime,
+    timebucket=None,
+    agg_function=None,
+    return_type="json",
+    verbose=False,
+):
     """
     Get data from the eCallisto API. See: https://v000792.fhnw.ch/api/redoc
-    Of course, this is just a wrapper around the requests.post function. 
+    Of course, this is just a wrapper around the requests.post function.
     Depending on the size, the request can take a while. For example, two
     weeks of data, aggregated in a specific way, can take around 20 seconds.
 
     Parameters
     ----------
     instrument_name : str
         The name of the instrument to get data from.
@@ -39,37 +47,43 @@
     """
     data = {
         "instrument_name": instrument_name,
         "start_datetime": start_datetime,
         "end_datetime": end_datetime,
         "timebucket": timebucket,
         "agg_function": agg_function,
-        "return_type": return_type
+        "return_type": return_type,
     }
 
     response = requests.post(BASE_URL + "/api/data", json=data, timeout=180)
 
     if response.status_code == 200:
-        url = response.json()['json_url'] if return_type=='json' else response.json()['fits_url']
+        url = (
+            response.json()["json_url"]
+            if return_type == "json"
+            else response.json()["fits_url"]
+        )
         url = BASE_URL + url
         while True:
             # Sleep for a short period of time to allow the data to be fetched
             time.sleep(5)
             # Check if the file is available yet
             file_response = requests.get(url)
             if file_response.status_code == 200:
                 # If the file is available, return the data
-                if return_type == 'json':
+                if return_type == "json":
                     df = pd.DataFrame(file_response.json())
                     return df
                 else:
-                    fits_path = f'{instrument_name}_{start_datetime}_{end_datetime}.fits'
-                    with open(fits_path, 'wb') as f:
+                    fits_path = (
+                        f"{instrument_name}_{start_datetime}_{end_datetime}.fits"
+                    )
+                    with open(fits_path, "wb") as f:
                         f.write(file_response.content)
                     return fits_path
             elif file_response.status_code == 404:
                 # If the file is not found, continue waiting
                 continue
             else:
                 raise ValueError(f"Error getting file from API: {file_response.text}")
     else:
-        raise ValueError(f"Error getting data from API: {response.text}")
+        raise ValueError(f"Error getting data from API: {response.text}")
```

### Comparing `ecallisto_ng-0.0.3/src/ecallisto_ng/plotting/plotting_utils.py` & `ecallisto_ng-0.0.4/src/ecallisto_ng/plotting/plotting_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import numpy as np
 import pandas as pd
 import plotly.express as px
 
 
-def plot_spectogram(df, instrument_name, start_datetime, end_datetime, size=18):
-    fig = px.imshow(df.T)
+def plot_spectogram(df, instrument_name, start_datetime, end_datetime, size=18, round_precision=2):
+    # Create a new dataframe with rounded column names
+    df_rounded = df.copy()
+    df_rounded.columns = [f"{float(col):.{round_precision}f}" for col in df.columns]
+
+    fig = px.imshow(df_rounded.T)
     fig.update_layout(
         title=f"Spectogram of {instrument_name} from {start_datetime} to {end_datetime}",
         xaxis_title="Datetime",
         yaxis_title="Frequency",
         font=dict(family="Courier New, monospace", size=size, color="#7f7f7f"),
     )
     return fig
 
-
 def fill_missing_timesteps_with_nan(df):
     """
-    Fill missing timesteps in a pandas DataFrame with NaN values.
+    Fill missing timesteps in a pandas DataFrame with NaN values. Only needed for plotting.
 
     Parameters
     ----------
     df : pandas.DataFrame
         The DataFrame to fill missing timesteps in.
 
     Returns
```

### Comparing `ecallisto_ng-0.0.3/src/ecallisto_ng.egg-info/PKG-INFO` & `ecallisto_ng-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
-Name: ecallisto-ng
-Version: 0.0.3
+Name: ecallisto_ng
+Version: 0.0.4
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ecallisto NG 
 ## Ecallisto NG is a very basic and simple package to access the Ecallisto API. 
-## It is written in Python 3.7 and uses the requests library and accesses the Ecallisto API at https://v000792.fhnw.ch/api/data
+## It is written in Python 3.9 and uses the requests library and accesses the Ecallisto API at https://v000792.fhnw.ch/api/data
 
 ## Installation
-Clone this repository and install it with pip:
+Clone this repository and install it with pip
 ```pip install -e .```
 ## PYPI
 This package is also available on PYPI: https://pypi.org/project/ecallisto-ng/
 ## Usage
 ### Data fetching
 ```python
 from ecallisto_ng.data_fetching.get_data import get_data
@@ -31,14 +31,15 @@
     "end_datetime": "2021-03-07 23:30:00",
     "timebucket": "15m",
     "agg_function": "MAX",
 }
 
 df = get_data(parameters)
 ```
+
 ### Plotting 
 We offer some basic plotting functions. 
 ```python
 from ecallisto_ng.plotting.plot import fill_missing_timesteps_with_nan, plot_spectogram
 
 df = fill_missing_timesteps_with_nan(df)
 plot_spectogram(df,  parameters["instrument_name"], parameters["start_datetime"], parameters["end_datetime"])
```

