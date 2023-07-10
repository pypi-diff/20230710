# Comparing `tmp/tsdb-0.0.8.tar.gz` & `tmp/tsdb-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsdb-0.0.8.tar", last modified: Sun Mar 19 13:48:43 2023, max compression
+gzip compressed data, was "tsdb-0.0.9.tar", last modified: Mon Jul 10 16:48:21 2023, max compression
```

## Comparing `tsdb-0.0.8.tar` & `tsdb-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 13:48:43.843323 tsdb-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-03-19 13:48:33.000000 tsdb-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-03-19 13:48:43.843323 tsdb-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-03-19 13:48:33.000000 tsdb-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 13:48:43.843323 tsdb-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-19 13:48:33.000000 tsdb-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 13:48:43.839323 tsdb-0.0.8/tsdb/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-19 13:48:33.000000 tsdb-0.0.8/tsdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-19 13:48:33.000000 tsdb-0.0.8/tsdb/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 13:48:43.843323 tsdb-0.0.8/tsdb/data_loading_funcs/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-19 13:48:33.000000 tsdb-0.0.8/tsdb/data_loading_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-03-19 13:48:33.000000 tsdb-0.0.8/tsdb/data_loading_funcs/beijing_multisite_air_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-03-19 13:48:33.000000 tsdb-0.0.8/tsdb/data_loading_funcs/electricity_load_diagrams.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-03-19 13:48:33.000000 tsdb-0.0.8/tsdb/data_loading_funcs/physionet_2012.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-03-19 13:48:33.000000 tsdb-0.0.8/tsdb/data_loading_funcs/physionet_2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-03-19 13:48:33.000000 tsdb-0.0.8/tsdb/data_loading_funcs/ucr_uea_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9674 2023-03-19 13:48:33.000000 tsdb-0.0.8/tsdb/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-03-19 13:48:33.000000 tsdb-0.0.8/tsdb/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 13:48:43.843323 tsdb-0.0.8/tsdb/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-19 13:48:33.000000 tsdb-0.0.8/tsdb/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-03-19 13:48:33.000000 tsdb-0.0.8/tsdb/tests/test_tsdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 13:48:43.839323 tsdb-0.0.8/tsdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-03-19 13:48:43.000000 tsdb-0.0.8/tsdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-03-19 13:48:43.000000 tsdb-0.0.8/tsdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 13:48:43.000000 tsdb-0.0.8/tsdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-19 13:48:43.000000 tsdb-0.0.8/tsdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-19 13:48:43.000000 tsdb-0.0.8/tsdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:48:21.903931 tsdb-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-10 16:48:07.000000 tsdb-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-10 16:48:21.903931 tsdb-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-10 16:48:07.000000 tsdb-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-10 16:48:21.903931 tsdb-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-10 16:48:07.000000 tsdb-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:48:21.899931 tsdb-0.0.9/tsdb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:48:21.903931 tsdb-0.0.9/tsdb/data_loading_funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/data_loading_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/data_loading_funcs/beijing_multisite_air_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/data_loading_funcs/electricity_load_diagrams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/data_loading_funcs/physionet_2012.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/data_loading_funcs/physionet_2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/data_loading_funcs/ucr_uea_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/data_loading_funcs/vessel_ais.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:48:21.903931 tsdb-0.0.9/tsdb/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/tests/test_tsdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:48:21.899931 tsdb-0.0.9/tsdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-10 16:48:21.000000 tsdb-0.0.9/tsdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-10 16:48:21.000000 tsdb-0.0.9/tsdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:48:21.000000 tsdb-0.0.9/tsdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-10 16:48:21.000000 tsdb-0.0.9/tsdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 16:48:21.000000 tsdb-0.0.9/tsdb.egg-info/top_level.txt
```

### Comparing `tsdb-0.0.8/LICENSE` & `tsdb-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tsdb-0.0.8/tsdb/data_loading_funcs/beijing_multisite_air_quality.py` & `tsdb-0.0.9/tsdb/data_loading_funcs/beijing_multisite_air_quality.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,34 +10,34 @@
 
 import os
 
 import pandas as pd
 
 
 def load_beijing_air_quality(local_path):
-    """ Load dataset Beijing Multi-site Air Quality.
+    """Load dataset Beijing Multi-site Air Quality.
 
     Parameters
     ----------
     local_path : str,
         The local path of dir saving the raw data of Beijing Multi-site Air Quality.
 
     Returns
     -------
     data : dict
         A dictionary contains X:
             X : pandas.DataFrame
                 The time-series data of Beijing Multi-site Air Quality.
     """
-    dir_path = os.path.join(local_path, 'PRSA_Data_20130301-20170228')
+    dir_path = os.path.join(local_path, "PRSA_Data_20130301-20170228")
     df_collector = []
     file_list = os.listdir(dir_path)
     for filename in file_list:
         file_path = os.path.join(dir_path, filename)
         current_df = pd.read_csv(file_path)
         df_collector.append(current_df)
-        print(f'Reading {file_path}, data shape {current_df.shape}')
+        print(f"Reading {file_path}, data shape {current_df.shape}")
     df = pd.concat(df_collector, axis=0)
     data = {
-        'X': df,
+        "X": df,
     }
     return data
```

### Comparing `tsdb-0.0.8/tsdb/data_loading_funcs/electricity_load_diagrams.py` & `tsdb-0.0.9/tsdb/data_loading_funcs/electricity_load_diagrams.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 
 import os
 
 import pandas as pd
 
 
 def load_electricity(local_path):
-    """ Load dataset Electricity Load Diagrams.
+    """Load dataset Electricity Load Diagrams.
 
     Parameters
     ----------
     local_path : str,
         The local path of dir saving the raw data of Electricity Load Diagrams.
 
     Returns
     -------
     data : dict
         A dictionary contains X:
             X : pandas.DataFrame
                 The time-series data of Electricity Load Diagrams.
     """
-    file_path = os.path.join(local_path, 'LD2011_2014.txt')
-    df = pd.read_csv(file_path, index_col=0, sep=';', decimal=',')
+    file_path = os.path.join(local_path, "LD2011_2014.txt")
+    df = pd.read_csv(file_path, index_col=0, sep=";", decimal=",")
     df.index = pd.to_datetime(df.index)
     # feature_names = df.columns.tolist()
     # feature_num = len(feature_names)
-    df['datetime'] = pd.to_datetime(df.index)
+    df["datetime"] = pd.to_datetime(df.index)
     data = {
-        'X': df,
+        "X": df,
     }
     return data
```

### Comparing `tsdb-0.0.8/tsdb/data_loading_funcs/physionet_2012.py` & `tsdb-0.0.9/tsdb/data_loading_funcs/physionet_2012.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import os
 
 import pandas as pd
 
 
 def load_physionet2012(local_path):
-    """ Load dataset PhysioNet Challenge 2012, which is a time-series classification dataset.
+    """Load dataset PhysioNet Challenge 2012, which is a time-series classification dataset.
 
     Parameters
     ----------
     local_path : str,
         The local path of dir saving the raw data of PhysioNet Challenge 2012.
 
     Returns
@@ -37,52 +37,52 @@
     All samples contain 48 time steps. Truncated if the sample has more than 48 steps. Padded if
     the sample has less than 48 steps. Static features such as 'Age', 'Gender', 'ICUType', 'Height',
     are removed. Column 'Time' also gets removed. Following 12 samples are dropped because of containing
     no time-series information at all: 147514, 142731, 145611, 140501, 155655, 143656, 156254, 150309,
     140936, 141264, 150649, 142998.
     """
 
-    time_series_measurements_dir = ['set-a', 'set-b', 'set-c']
-    outcome_files = ['Outcomes-a.txt', 'Outcomes-b.txt', 'Outcomes-c.txt']
+    time_series_measurements_dir = ["set-a", "set-b", "set-c"]
+    outcome_files = ["Outcomes-a.txt", "Outcomes-b.txt", "Outcomes-c.txt"]
 
     outcome_collector = []
     for o_ in outcome_files:
         outcome_file_path = os.path.join(local_path, o_)
-        with open(outcome_file_path, 'r') as f:
-            outcome = pd.read_csv(f)[['In-hospital_death', 'RecordID']]
-        outcome['RecordID'] = outcome['RecordID'].astype(int)  # ensure RecordID's type is int
-        outcome = outcome.set_index('RecordID')
+        with open(outcome_file_path, "r") as f:
+            outcome = pd.read_csv(f)[["In-hospital_death", "RecordID"]]
+        outcome["RecordID"] = outcome["RecordID"].astype(
+            int
+        )  # ensure RecordID's type is int
+        outcome = outcome.set_index("RecordID")
         outcome_collector.append(outcome)
     y = pd.concat(outcome_collector)
 
     df_collector = []
 
     # iterate over all samples
     for m_ in time_series_measurements_dir:
         raw_data_dir = os.path.join(local_path, m_)
         for filename in os.listdir(raw_data_dir):
-            recordID = int(filename.split('.txt')[0])
-            with open(os.path.join(raw_data_dir, filename), 'r') as f:
+            recordID = int(filename.split(".txt")[0])
+            with open(os.path.join(raw_data_dir, filename), "r") as f:
                 df_temp = pd.read_csv(f)
-            df_temp['Time'] = df_temp['Time'].apply(lambda x: int(x.split(':')[0]))
-            df_temp = df_temp.pivot_table('Value', 'Time', 'Parameter')
+            df_temp["Time"] = df_temp["Time"].apply(lambda x: int(x.split(":")[0]))
+            df_temp = df_temp.pivot_table("Value", "Time", "Parameter")
             df_temp = df_temp.reset_index()  # take Time from index as a col
             if len(df_temp) == 1:
-                print(f'Ignore {recordID}, because its len==1, having no time series data')
+                print(
+                    f"Ignore {recordID}, because its len==1, having no time series data"
+                )
                 continue
 
-            df_temp['RecordID'] = recordID
-            df_temp['Age'] = df_temp.loc[0, 'Age']
-            df_temp['Height'] = df_temp.loc[0, 'Height']
+            df_temp["RecordID"] = recordID
+            df_temp["Age"] = df_temp.loc[0, "Age"]
+            df_temp["Height"] = df_temp.loc[0, "Height"]
             df_collector.append(df_temp)
 
     df = pd.concat(df_collector, sort=True)
     X = df.reset_index(drop=True)
-    unique_ids = df['RecordID'].unique()
+    unique_ids = df["RecordID"].unique()
     y = y.loc[unique_ids]
 
-    data = {
-        'X': X,
-        'y': y,
-        'static_features': ['Age', 'Gender', 'ICUType', 'Height']
-    }
+    data = {"X": X, "y": y, "static_features": ["Age", "Gender", "ICUType", "Height"]}
     return data
```

### Comparing `tsdb-0.0.8/tsdb/data_loading_funcs/ucr_uea_datasets.py` & `tsdb-0.0.9/tsdb/data_loading_funcs/ucr_uea_datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,16 @@
 import warnings
 
 import numpy
 from sklearn.utils.estimator_checks import _NotAnArray as NotAnArray
 
 try:
     from scipy.io import arff
-
     HAS_ARFF = True
-
-except:
+except Exception:
     HAS_ARFF = False
 
 
 def load_ucr_uea_dataset(local_path, dataset_name):
     try:
         # if both TXT and ARFF files are provided, the TXT versions are
         # used
@@ -39,33 +37,38 @@
             X_train, y_train = _load_arff_uea(
                 os.path.join(local_path, dataset_name + "_TRAIN.arff")
             )
             X_test, y_test = _load_arff_uea(
                 os.path.join(local_path, dataset_name + "_TEST.arff")
             )
         else:
-            warnings.warn("dataset \"%s\" is not provided in either TXT "
-                          "or ARFF format and thus could not be loaded"
-                          % dataset_name,
-                          category=RuntimeWarning, stacklevel=2)
+            warnings.warn(
+                'dataset "%s" is not provided in either TXT '
+                "or ARFF format and thus could not be loaded" % dataset_name,
+                category=RuntimeWarning,
+                stacklevel=2,
+            )
             return None
 
         data = {
-            'X_train': X_train,
-            'y_train': y_train,
-            'X_test': X_test,
-            'y_test': y_test
+            "X_train": X_train,
+            "y_train": y_train,
+            "X_test": X_test,
+            "y_test": y_test,
         }
 
         return data
 
     except Exception as exception:
-        warnings.warn("dataset \"%s\" could be downloaded but not "
-                      "parsed: %s" % (dataset_name, str(exception)),
-                      category=RuntimeWarning, stacklevel=2)
+        warnings.warn(
+            'dataset "%s" could be downloaded but not '
+            "parsed: %s" % (dataset_name, str(exception)),
+            category=RuntimeWarning,
+            stacklevel=2,
+        )
 
 
 def _has_files(data_dir, dataset_name, ext):
     """Determines whether some downloaded and unzipped dataset provides
     both training and test data in the given format.
 
     Parameters
@@ -80,16 +83,17 @@
     Returns
     -------
     bool
         if there are both training and test files with the specified
         file extension
     """
     basename = os.path.join(data_dir, dataset_name)
-    return (os.path.exists(basename + "_TRAIN.%s" % ext) and
-            os.path.exists(basename + "_TEST.%s" % ext))
+    return os.path.exists(basename + "_TRAIN.%s" % ext) and os.path.exists(
+        basename + "_TEST.%s" % ext
+    )
 
 
 def ts_size(ts):
     """Returns actual time series size.
 
     Final timesteps that have `NaN` values for all dimensions will be removed
     from the count. Infinity and negative infinity ar considered valid time
@@ -166,15 +170,15 @@
     """
     ts_out = numpy.array(ts, copy=True)
     if ts_out.ndim <= 1:
         ts_out = ts_out.reshape((-1, 1))
     if ts_out.dtype != float:
         ts_out = ts_out.astype(float)
     if remove_nans:
-        ts_out = ts_out[:ts_size(ts_out)]
+        ts_out = ts_out[: ts_size(ts_out)]
     return ts_out
 
 
 def to_time_series_dataset(dataset, dtype=float):
     """Transforms a time series dataset so that it fits the format used in
     ``tslearn`` models.
 
@@ -212,32 +216,32 @@
 
     See Also
     --------
     to_time_series : Transforms a single time series
     """
     try:
         import pandas as pd
+
         if isinstance(dataset, pd.DataFrame):
             return to_time_series_dataset(numpy.array(dataset))
     except ImportError:
         pass
     if isinstance(dataset, NotAnArray):  # Patch to pass sklearn tests
         return to_time_series_dataset(numpy.array(dataset))
     if len(dataset) == 0:
         return numpy.zeros((0, 0, 0))
     if numpy.array(dataset[0]).ndim == 0:
         dataset = [dataset]
     n_ts = len(dataset)
-    max_sz = max([ts_size(to_time_series(ts, remove_nans=True))
-                  for ts in dataset])
+    max_sz = max([ts_size(to_time_series(ts, remove_nans=True)) for ts in dataset])
     d = to_time_series(dataset[0]).shape[1]
     dataset_out = numpy.zeros((n_ts, max_sz, d), dtype=dtype) + numpy.nan
     for i in range(n_ts):
         ts = to_time_series(dataset[i], remove_nans=True)
-        dataset_out[i, :ts.shape[0]] = ts
+        dataset_out[i, : ts.shape[0]] = ts
     return dataset_out.astype(dtype)
 
 
 def _load_arff_uea(dataset_path):
     """Load arff file for uni/multi variate dataset
 
     Parameters
@@ -255,16 +259,18 @@
     Raises
     ------
     ImportError: if the version of *Scipy* is too old (pre 1.3.0)
     Exception: on any failure, e.g. if the given file does not exist or is
                corrupted
     """
     if not HAS_ARFF:
-        raise ImportError("scipy 1.3.0 or newer is required to load "
-                          "time series datasets from arff format.")
+        raise ImportError(
+            "scipy 1.3.0 or newer is required to load "
+            "time series datasets from arff format."
+        )
     data, meta = arff.loadarff(dataset_path)
     names = meta.names()  # ["input", "class"] for multi-variate
 
     # firstly get y_train
     y_ = data[names[-1]]  # data["class"]
     y = numpy.array(y_).astype("str")
```

### Comparing `tsdb-0.0.8/tsdb/data_processing.py` & `tsdb-0.0.9/tsdb/data_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,22 @@
 import sys
 import tempfile
 import urllib.request
 import warnings
 
 import numpy
 
-from tsdb.data_loading_funcs import *
+from tsdb.data_loading_funcs import (
+    load_physionet2012,
+    load_physionet2019,
+    load_electricity,
+    load_beijing_air_quality,
+    load_ucr_uea_dataset,
+    load_ais,
+)
 from tsdb.database import DATABASE, AVAILABLE_DATASETS
 
 CACHED_DATASET_DIR = os.path.join(os.path.expanduser("~"), ".tsdb_cached_datasets")
 
 
 def window_truncate(feature_vectors, seq_len):
     """Generate time series samples, truncating windows from time-series data with a given sequence length.
@@ -35,15 +42,15 @@
     -------
     array,
         Truncated time series with given sequence length.
     """
     start_indices = numpy.asarray(range(feature_vectors.shape[0] // seq_len)) * seq_len
     sample_collector = []
     for idx in start_indices:
-        sample_collector.append(feature_vectors[idx: idx + seq_len])
+        sample_collector.append(feature_vectors[idx : idx + seq_len])
 
     return numpy.asarray(sample_collector).astype("float32")
 
 
 def _download_and_extract(url, saving_path):
     """Download dataset from the given url and extract to the given saving path.
 
@@ -86,15 +93,15 @@
     except Exception as e:
         shutil.rmtree(saving_path, ignore_errors=True)
         print(f"Exception: {e}\n" f"Download failed. Aborting.")
         sys.exit()
     print(f"Successfully downloaded data to {raw_data_saving_path}.")
 
     if (
-            suffix in supported_compression_format
+        suffix in supported_compression_format
     ):  # if the file is compressed, then unpack it
         try:
             os.makedirs(saving_path, exist_ok=True)
             shutil.unpack_archive(raw_data_saving_path, saving_path)
             print(f"Successfully extracted data to {saving_path}")
         except shutil.Error:
             warnings.warn(
@@ -152,15 +159,15 @@
     # if CACHED_DATASET_DIR does not exist, abort
     if not os.path.exists(CACHED_DATASET_DIR):
         print("No cached data. Operation aborted.")
         sys.exit()
     # if CACHED_DATASET_DIR exists, then purge
     if dataset_name is not None:
         assert (
-                dataset_name in AVAILABLE_DATASETS
+            dataset_name in AVAILABLE_DATASETS
         ), f"{dataset_name} is not available in TSDB, so it has no cache. Please check your dataset name."
         dir_to_delete = os.path.join(CACHED_DATASET_DIR, dataset_name)
         if not os.path.exists(dir_to_delete):
             print(f"Dataset {dataset_name} is not cached. Operation aborted.")
             sys.exit()
         print(f"Purging cached dataset {dataset_name} under {dir_to_delete}...")
     else:
@@ -259,21 +266,22 @@
         Whether to use cache (including data downloading and processing)
 
     Returns
     -------
     pandas.DataFrame,
         Loaded dataset.
     """
-    assert dataset_name in AVAILABLE_DATASETS, \
-        f'The given dataset name "{dataset_name}" is not in the database. ' \
-        f'Please fetch the full list of the available datasets with tsdb.list_available_datasets()'
+    assert dataset_name in AVAILABLE_DATASETS, (
+        f'The given dataset name "{dataset_name}" is not in the database. '
+        f"Please fetch the full list of the available datasets with tsdb.list_available_datasets()"
+    )
 
     dataset_saving_path = os.path.join(CACHED_DATASET_DIR, dataset_name)
     if not os.path.exists(
-            dataset_saving_path
+        dataset_saving_path
     ):  # if the dataset is not cached, then download it
         download_and_extract(dataset_name, dataset_saving_path)
     else:
         if use_cache:
             print(
                 f"Dataset {dataset_name} has already been downloaded. Processing directly..."
             )
@@ -295,14 +303,16 @@
                 result = load_physionet2012(dataset_saving_path)
             if dataset_name == "physionet_2019":
                 result = load_physionet2019(dataset_saving_path)
             elif dataset_name == "electricity_load_diagrams":
                 result = load_electricity(dataset_saving_path)
             elif dataset_name == "beijing_multisite_air_quality":
                 result = load_beijing_air_quality(dataset_saving_path)
+            elif dataset_name == "vessel_AIS":
+                result = load_ais(dataset_saving_path)
             elif "UCR_UEA_" in dataset_name:
                 actual_dataset_name = dataset_name.replace(
                     "UCR_UEA_", ""
                 )  # delete 'UCR_UEA_' in the name
                 result = load_ucr_uea_dataset(dataset_saving_path, actual_dataset_name)
 
         except FileExistsError:
```

### Comparing `tsdb-0.0.8/tsdb/tests/test_tsdb.py` & `tsdb-0.0.9/tsdb/tests/test_tsdb.py`

 * *Files identical despite different names*

### Comparing `tsdb-0.0.8/tsdb.egg-info/SOURCES.txt` & `tsdb-0.0.9/tsdb.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 LICENSE
 README.md
+setup.cfg
 setup.py
 tsdb/__init__.py
-tsdb/__version__.py
 tsdb/data_processing.py
 tsdb/database.py
 tsdb.egg-info/PKG-INFO
 tsdb.egg-info/SOURCES.txt
 tsdb.egg-info/dependency_links.txt
 tsdb.egg-info/requires.txt
 tsdb.egg-info/top_level.txt
 tsdb/data_loading_funcs/__init__.py
 tsdb/data_loading_funcs/beijing_multisite_air_quality.py
 tsdb/data_loading_funcs/electricity_load_diagrams.py
 tsdb/data_loading_funcs/physionet_2012.py
 tsdb/data_loading_funcs/physionet_2019.py
 tsdb/data_loading_funcs/ucr_uea_datasets.py
+tsdb/data_loading_funcs/vessel_ais.py
 tsdb/tests/__init__.py
 tsdb/tests/test_tsdb.py
```

