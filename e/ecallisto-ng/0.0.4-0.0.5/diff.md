# Comparing `tmp/ecallisto_ng-0.0.4.tar.gz` & `tmp/ecallisto_ng-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecallisto_ng-0.0.4.tar", last modified: Mon Jul 10 17:33:35 2023, max compression
+gzip compressed data, was "ecallisto_ng-0.0.5.tar", last modified: Mon Jul 10 17:53:26 2023, max compression
```

## Comparing `ecallisto_ng-0.0.4.tar` & `ecallisto_ng-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:33:35.758959 ecallisto_ng-0.0.4/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.0.4/LICENSE
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1615 2023-07-10 17:33:35.758959 ecallisto_ng-0.0.4/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1035 2023-07-10 17:29:49.000000 ecallisto_ng-0.0.4/README.md
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      836 2023-07-10 17:27:25.000000 ecallisto_ng-0.0.4/pyproject.toml
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-10 17:33:35.758959 ecallisto_ng-0.0.4/setup.cfg
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:33:35.758959 ecallisto_ng-0.0.4/src/
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:33:35.758959 ecallisto_ng-0.0.4/src/ecallisto_ng/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.0.4/src/ecallisto_ng/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:33:35.758959 ecallisto_ng-0.0.4/src/ecallisto_ng/data_fetching/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3096 2023-07-10 16:52:06.000000 ecallisto_ng-0.0.4/src/ecallisto_ng/data_fetching/get_data.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:33:35.758959 ecallisto_ng-0.0.4/src/ecallisto_ng/data_processing/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     4716 2023-07-10 17:16:31.000000 ecallisto_ng-0.0.4/src/ecallisto_ng/data_processing/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:33:35.758959 ecallisto_ng-0.0.4/src/ecallisto_ng/plotting/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2392 2023-07-10 17:23:39.000000 ecallisto_ng-0.0.4/src/ecallisto_ng/plotting/plotting_utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:33:35.758959 ecallisto_ng-0.0.4/src/ecallisto_ng.egg-info/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1615 2023-07-10 17:33:35.000000 ecallisto_ng-0.0.4/src/ecallisto_ng.egg-info/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      389 2023-07-10 17:33:35.000000 ecallisto_ng-0.0.4/src/ecallisto_ng.egg-info/SOURCES.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-10 17:33:35.000000 ecallisto_ng-0.0.4/src/ecallisto_ng.egg-info/dependency_links.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      113 2023-07-10 17:33:35.000000 ecallisto_ng-0.0.4/src/ecallisto_ng.egg-info/requires.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-10 17:33:35.000000 ecallisto_ng-0.0.4/src/ecallisto_ng.egg-info/top_level.txt
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:53:26.753817 ecallisto_ng-0.0.5/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.0.5/LICENSE
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2773 2023-07-10 17:53:26.753817 ecallisto_ng-0.0.5/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2192 2023-07-10 17:46:34.000000 ecallisto_ng-0.0.5/README.md
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      836 2023-07-10 17:53:01.000000 ecallisto_ng-0.0.5/pyproject.toml
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-10 17:53:26.753817 ecallisto_ng-0.0.5/setup.cfg
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:53:26.742983 ecallisto_ng-0.0.5/src/
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:53:26.753817 ecallisto_ng-0.0.5/src/ecallisto_ng/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.0.5/src/ecallisto_ng/__init__.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:53:26.753817 ecallisto_ng-0.0.5/src/ecallisto_ng/data_fetching/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3096 2023-07-10 16:52:06.000000 ecallisto_ng-0.0.5/src/ecallisto_ng/data_fetching/get_data.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:53:26.753817 ecallisto_ng-0.0.5/src/ecallisto_ng/data_processing/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     4716 2023-07-10 17:16:31.000000 ecallisto_ng-0.0.5/src/ecallisto_ng/data_processing/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:53:26.753817 ecallisto_ng-0.0.5/src/ecallisto_ng/plotting/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2392 2023-07-10 17:23:39.000000 ecallisto_ng-0.0.5/src/ecallisto_ng/plotting/plotting_utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:53:26.753817 ecallisto_ng-0.0.5/src/ecallisto_ng.egg-info/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2773 2023-07-10 17:53:26.000000 ecallisto_ng-0.0.5/src/ecallisto_ng.egg-info/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      389 2023-07-10 17:53:26.000000 ecallisto_ng-0.0.5/src/ecallisto_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-10 17:53:26.000000 ecallisto_ng-0.0.5/src/ecallisto_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      113 2023-07-10 17:53:26.000000 ecallisto_ng-0.0.5/src/ecallisto_ng.egg-info/requires.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-10 17:53:26.000000 ecallisto_ng-0.0.5/src/ecallisto_ng.egg-info/top_level.txt
```

### Comparing `ecallisto_ng-0.0.4/LICENSE` & `ecallisto_ng-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.0.4/PKG-INFO` & `ecallisto_ng-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,66 @@
 Metadata-Version: 2.1
 Name: ecallisto_ng
-Version: 0.0.4
+Version: 0.0.5
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
-## Ecallisto NG is a very basic and simple package to access the Ecallisto API. 
-## It is written in Python 3.9 and uses the requests library and accesses the Ecallisto API at https://v000792.fhnw.ch/api/data
+Ecallisto NG is a compact yet effective Python package designed to facilitate seamless interaction with the Ecallisto API. 
+The package is constructed in Python 3.9 and utilizes the `requests` library to directly access the Ecallisto API via the link: [https://v000792.fhnw.ch/api/data](https://v000792.fhnw.ch/api/data).
 
 ## Installation
-Clone this repository and install it with pip
+To install this package, clone this repository and use pip for installation. Execute the following command in your terminal:
 ```pip install -e .```
-## PYPI
-This package is also available on PYPI: https://pypi.org/project/ecallisto-ng/
+
+## PyPI
+Ecallisto NG is conveniently available on PyPI as well. To download, visit the following link: [https://pypi.org/project/ecallisto-ng/](https://pypi.org/project/ecallisto-ng/)
+
 ## Usage
-### Data fetching
+Here's a guide on how to use the different features of Ecallisto NG:
+
+### Data Fetching
+Fetching data is easy using the `get_data` function, housed under the `ecallisto_ng.data_fetching.get_data` module. Here's an example:
+
 ```python
 from ecallisto_ng.data_fetching.get_data import get_data
+
 parameters = {
     "instrument_name": "austria_unigraz_01",
     "start_datetime": "2021-03-01 06:30:00",
     "end_datetime": "2021-03-07 23:30:00",
     "timebucket": "15m",
     "agg_function": "MAX",
 }
 
 df = get_data(parameters)
 ```
 
 ### Plotting 
-We offer some basic plotting functions. 
+Ecallisto NG provides basic plotting capabilities. Here's an example of how to generate a spectogram:
 ```python
 from ecallisto_ng.plotting.plot import fill_missing_timesteps_with_nan, plot_spectogram
 
 df = fill_missing_timesteps_with_nan(df)
 plot_spectogram(df,  parameters["instrument_name"], parameters["start_datetime"], parameters["end_datetime"])
 ```
+
+### Spectogram editing
+We also provide some basic functionalities to edit the spectogram. Here's how you can do it:
+```python
+from ecallisto_ng.data_processing.utils import elimwrongchannels, subtract_constant_background, subtract_rolling_background
+
+df = elimwrongchannels(df)
+df = subtract_constant_background(df)
+df = subtract_rolling_background(df)
+
+plot_spectogram(df,  parameters["instrument_name"], parameters["start_datetime"], parameters["end_datetime"])
+```
+These simple commands allow you to easily manipulate spectogram data, enabling effective use of the Ecallisto API for your needs.
```

### Comparing `ecallisto_ng-0.0.4/pyproject.toml` & `ecallisto_ng-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ecallisto_ng"
-version = "0.0.4"
+version = "0.0.5"
 authors = [{name = "Vincenzo Timmel", email = "vincenzo.timmel@fhnw.ch"}]
 description = "A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API."
 readme = "README.md"
 
 requires-python = ">=3.9"
 
 classifiers = [
```

### Comparing `ecallisto_ng-0.0.4/src/ecallisto_ng/data_fetching/get_data.py` & `ecallisto_ng-0.0.5/src/ecallisto_ng/data_fetching/get_data.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.0.4/src/ecallisto_ng/data_processing/utils.py` & `ecallisto_ng-0.0.5/src/ecallisto_ng/data_processing/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.0.4/src/ecallisto_ng/plotting/plotting_utils.py` & `ecallisto_ng-0.0.5/src/ecallisto_ng/plotting/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.0.4/src/ecallisto_ng.egg-info/PKG-INFO` & `ecallisto_ng-0.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,52 @@
-Metadata-Version: 2.1
-Name: ecallisto-ng
-Version: 0.0.4
-Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
-Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
-Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
-Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Ecallisto NG 
-## Ecallisto NG is a very basic and simple package to access the Ecallisto API. 
-## It is written in Python 3.9 and uses the requests library and accesses the Ecallisto API at https://v000792.fhnw.ch/api/data
+Ecallisto NG is a compact yet effective Python package designed to facilitate seamless interaction with the Ecallisto API. 
+The package is constructed in Python 3.9 and utilizes the `requests` library to directly access the Ecallisto API via the link: [https://v000792.fhnw.ch/api/data](https://v000792.fhnw.ch/api/data).
 
 ## Installation
-Clone this repository and install it with pip
+To install this package, clone this repository and use pip for installation. Execute the following command in your terminal:
 ```pip install -e .```
-## PYPI
-This package is also available on PYPI: https://pypi.org/project/ecallisto-ng/
+
+## PyPI
+Ecallisto NG is conveniently available on PyPI as well. To download, visit the following link: [https://pypi.org/project/ecallisto-ng/](https://pypi.org/project/ecallisto-ng/)
+
 ## Usage
-### Data fetching
+Here's a guide on how to use the different features of Ecallisto NG:
+
+### Data Fetching
+Fetching data is easy using the `get_data` function, housed under the `ecallisto_ng.data_fetching.get_data` module. Here's an example:
+
 ```python
 from ecallisto_ng.data_fetching.get_data import get_data
+
 parameters = {
     "instrument_name": "austria_unigraz_01",
     "start_datetime": "2021-03-01 06:30:00",
     "end_datetime": "2021-03-07 23:30:00",
     "timebucket": "15m",
     "agg_function": "MAX",
 }
 
 df = get_data(parameters)
 ```
 
 ### Plotting 
-We offer some basic plotting functions. 
+Ecallisto NG provides basic plotting capabilities. Here's an example of how to generate a spectogram:
 ```python
 from ecallisto_ng.plotting.plot import fill_missing_timesteps_with_nan, plot_spectogram
 
 df = fill_missing_timesteps_with_nan(df)
 plot_spectogram(df,  parameters["instrument_name"], parameters["start_datetime"], parameters["end_datetime"])
 ```
+
+### Spectogram editing
+We also provide some basic functionalities to edit the spectogram. Here's how you can do it:
+```python
+from ecallisto_ng.data_processing.utils import elimwrongchannels, subtract_constant_background, subtract_rolling_background
+
+df = elimwrongchannels(df)
+df = subtract_constant_background(df)
+df = subtract_rolling_background(df)
+
+plot_spectogram(df,  parameters["instrument_name"], parameters["start_datetime"], parameters["end_datetime"])
+```
+These simple commands allow you to easily manipulate spectogram data, enabling effective use of the Ecallisto API for your needs.
```

