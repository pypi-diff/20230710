# Comparing `tmp/ecallisto_ng-0.0.5.tar.gz` & `tmp/ecallisto_ng-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecallisto_ng-0.0.5.tar", last modified: Mon Jul 10 17:53:26 2023, max compression
+gzip compressed data, was "ecallisto_ng-0.0.6.tar", last modified: Mon Jul 10 17:56:58 2023, max compression
```

## Comparing `ecallisto_ng-0.0.5.tar` & `ecallisto_ng-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:53:26.753817 ecallisto_ng-0.0.5/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.0.5/LICENSE
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2773 2023-07-10 17:53:26.753817 ecallisto_ng-0.0.5/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2192 2023-07-10 17:46:34.000000 ecallisto_ng-0.0.5/README.md
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      836 2023-07-10 17:53:01.000000 ecallisto_ng-0.0.5/pyproject.toml
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-10 17:53:26.753817 ecallisto_ng-0.0.5/setup.cfg
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:53:26.742983 ecallisto_ng-0.0.5/src/
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:53:26.753817 ecallisto_ng-0.0.5/src/ecallisto_ng/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.0.5/src/ecallisto_ng/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:53:26.753817 ecallisto_ng-0.0.5/src/ecallisto_ng/data_fetching/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3096 2023-07-10 16:52:06.000000 ecallisto_ng-0.0.5/src/ecallisto_ng/data_fetching/get_data.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:53:26.753817 ecallisto_ng-0.0.5/src/ecallisto_ng/data_processing/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     4716 2023-07-10 17:16:31.000000 ecallisto_ng-0.0.5/src/ecallisto_ng/data_processing/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:53:26.753817 ecallisto_ng-0.0.5/src/ecallisto_ng/plotting/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2392 2023-07-10 17:23:39.000000 ecallisto_ng-0.0.5/src/ecallisto_ng/plotting/plotting_utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:53:26.753817 ecallisto_ng-0.0.5/src/ecallisto_ng.egg-info/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2773 2023-07-10 17:53:26.000000 ecallisto_ng-0.0.5/src/ecallisto_ng.egg-info/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      389 2023-07-10 17:53:26.000000 ecallisto_ng-0.0.5/src/ecallisto_ng.egg-info/SOURCES.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-10 17:53:26.000000 ecallisto_ng-0.0.5/src/ecallisto_ng.egg-info/dependency_links.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      113 2023-07-10 17:53:26.000000 ecallisto_ng-0.0.5/src/ecallisto_ng.egg-info/requires.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-10 17:53:26.000000 ecallisto_ng-0.0.5/src/ecallisto_ng.egg-info/top_level.txt
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:56:58.697126 ecallisto_ng-0.0.6/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.0.6/LICENSE
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2773 2023-07-10 17:56:58.697126 ecallisto_ng-0.0.6/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2192 2023-07-10 17:46:34.000000 ecallisto_ng-0.0.6/README.md
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      836 2023-07-10 17:56:50.000000 ecallisto_ng-0.0.6/pyproject.toml
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-10 17:56:58.697126 ecallisto_ng-0.0.6/setup.cfg
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:56:58.697126 ecallisto_ng-0.0.6/src/
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:56:58.697126 ecallisto_ng-0.0.6/src/ecallisto_ng/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.0.6/src/ecallisto_ng/__init__.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:56:58.697126 ecallisto_ng-0.0.6/src/ecallisto_ng/data_fetching/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3096 2023-07-10 16:52:06.000000 ecallisto_ng-0.0.6/src/ecallisto_ng/data_fetching/get_data.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:56:58.697126 ecallisto_ng-0.0.6/src/ecallisto_ng/data_processing/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     4716 2023-07-10 17:16:31.000000 ecallisto_ng-0.0.6/src/ecallisto_ng/data_processing/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:56:58.697126 ecallisto_ng-0.0.6/src/ecallisto_ng/plotting/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2425 2023-07-10 17:56:33.000000 ecallisto_ng-0.0.6/src/ecallisto_ng/plotting/plotting_utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:56:58.697126 ecallisto_ng-0.0.6/src/ecallisto_ng.egg-info/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2773 2023-07-10 17:56:58.000000 ecallisto_ng-0.0.6/src/ecallisto_ng.egg-info/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      389 2023-07-10 17:56:58.000000 ecallisto_ng-0.0.6/src/ecallisto_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-10 17:56:58.000000 ecallisto_ng-0.0.6/src/ecallisto_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      113 2023-07-10 17:56:58.000000 ecallisto_ng-0.0.6/src/ecallisto_ng.egg-info/requires.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-10 17:56:58.000000 ecallisto_ng-0.0.6/src/ecallisto_ng.egg-info/top_level.txt
```

### Comparing `ecallisto_ng-0.0.5/LICENSE` & `ecallisto_ng-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.0.5/PKG-INFO` & `ecallisto_ng-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecallisto_ng
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecallisto_ng-0.0.5/README.md` & `ecallisto_ng-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.0.5/pyproject.toml` & `ecallisto_ng-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ecallisto_ng"
-version = "0.0.5"
+version = "0.0.6"
 authors = [{name = "Vincenzo Timmel", email = "vincenzo.timmel@fhnw.ch"}]
 description = "A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API."
 readme = "README.md"
 
 requires-python = ">=3.9"
 
 classifiers = [
```

### Comparing `ecallisto_ng-0.0.5/src/ecallisto_ng/data_fetching/get_data.py` & `ecallisto_ng-0.0.6/src/ecallisto_ng/data_fetching/get_data.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.0.5/src/ecallisto_ng/data_processing/utils.py` & `ecallisto_ng-0.0.6/src/ecallisto_ng/data_processing/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.0.5/src/ecallisto_ng/plotting/plotting_utils.py` & `ecallisto_ng-0.0.6/src/ecallisto_ng/plotting/plotting_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 
     Examples
     --------
     >>> dates = pd.date_range('2023-02-19 01:00', '2023-02-19 05:00', freq='2H')
     >>> freqs = ['10M', '20M', '30M']
     >>> data = np.random.randn(len(dates), len(freqs))
     >>> df = pd.DataFrame(data, index=dates, columns=freqs)
+    >>> df = df.drop(df.index[1])
     >>> df = fill_missing_timesteps_with_nan(df)
     >>> print(df)
-
                             10M       20M       30M
     2023-02-19 01:00:00 -0.349636  0.004947  0.546848
     2023-02-19 03:00:00       NaN       NaN       NaN
     2023-02-19 05:00:00 -0.576182  1.222293 -0.416526
     """
     # Change index to datetime, if it's not already
     df.index = pd.to_datetime(df.index)
```

### Comparing `ecallisto_ng-0.0.5/src/ecallisto_ng.egg-info/PKG-INFO` & `ecallisto_ng-0.0.6/src/ecallisto_ng.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecallisto-ng
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

