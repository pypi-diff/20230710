# Comparing `tmp/tubular-0.3.7.tar.gz` & `tmp/tubular-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tubular-0.3.7.tar", last modified: Wed Jul  5 14:01:24 2023, max compression
+gzip compressed data, was "tubular-0.3.8.tar", last modified: Mon Jul 10 16:13:10 2023, max compression
```

## Comparing `tubular-0.3.7.tar` & `tubular-0.3.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-05 14:01:24.760365 tubular-0.3.7/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1550 2023-07-05 13:47:51.000000 tubular-0.3.7/LICENSE
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4335 2023-07-05 14:01:24.760365 tubular-0.3.7/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3706 2023-07-05 13:47:51.000000 tubular-0.3.7/README.md
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2023-07-05 14:01:24.760365 tubular-0.3.7/setup.cfg
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1457 2023-07-05 13:47:51.000000 tubular-0.3.7/setup.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-05 14:01:24.748365 tubular-0.3.7/tests/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2023-07-05 13:47:51.000000 tubular-0.3.7/tests/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14672 2023-07-05 13:47:51.000000 tubular-0.3.7/tests/test_data.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4876 2023-07-05 13:47:51.000000 tubular-0.3.7/tests/test_transformers.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-05 14:01:24.756365 tubular-0.3.7/tubular/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      286 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       22 2023-07-05 14:00:40.000000 tubular-0.3.7/tubular/_version.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14927 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/base.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    20028 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/capping.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1985 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/comparison.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    41786 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/dates.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    13464 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/imputers.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    17192 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/mapping.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2002 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/misc.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    42271 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/nominal.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    30363 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/numeric.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6024 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/strings.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-05 14:01:24.756365 tubular-0.3.7/tubular.egg-info/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4335 2023-07-05 14:01:24.000000 tubular-0.3.7/tubular.egg-info/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      470 2023-07-05 14:01:24.000000 tubular-0.3.7/tubular.egg-info/SOURCES.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2023-07-05 14:01:24.000000 tubular-0.3.7/tubular.egg-info/dependency_links.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       40 2023-07-05 14:01:24.000000 tubular-0.3.7/tubular.egg-info/requires.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       14 2023-07-05 14:01:24.000000 tubular-0.3.7/tubular.egg-info/top_level.txt
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-10 16:13:10.090562 tubular-0.3.8/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1550 2023-07-10 16:08:48.000000 tubular-0.3.8/LICENSE
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4336 2023-07-10 16:13:10.086562 tubular-0.3.8/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3707 2023-07-10 16:08:48.000000 tubular-0.3.8/README.md
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2023-07-10 16:13:10.090562 tubular-0.3.8/setup.cfg
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1519 2023-07-10 16:08:48.000000 tubular-0.3.8/setup.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-10 16:13:10.074562 tubular-0.3.8/tests/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2023-07-10 16:08:48.000000 tubular-0.3.8/tests/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14382 2023-07-10 16:08:48.000000 tubular-0.3.8/tests/test_data.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4983 2023-07-10 16:08:48.000000 tubular-0.3.8/tests/test_transformers.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-10 16:13:10.082563 tubular-0.3.8/tubular/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      175 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       22 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/_version.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    15066 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/base.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    20018 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/capping.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2063 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/comparison.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    41318 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/dates.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    13415 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/imputers.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    17169 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/mapping.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2003 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/misc.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    42320 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/nominal.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    29859 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/numeric.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5981 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/strings.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-10 16:13:10.086562 tubular-0.3.8/tubular.egg-info/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4336 2023-07-10 16:13:09.000000 tubular-0.3.8/tubular.egg-info/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      470 2023-07-10 16:13:09.000000 tubular-0.3.8/tubular.egg-info/SOURCES.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2023-07-10 16:13:09.000000 tubular-0.3.8/tubular.egg-info/dependency_links.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       40 2023-07-10 16:13:09.000000 tubular-0.3.8/tubular.egg-info/requires.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       14 2023-07-10 16:13:09.000000 tubular-0.3.8/tubular.egg-info/top_level.txt
```

### Comparing `tubular-0.3.7/LICENSE` & `tubular-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tubular-0.3.7/PKG-INFO` & `tubular-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tubular
-Version: 0.3.7
+Version: 0.3.8
 Summary: Package to perform pre processing steps for machine learning models
 Author: LV GI Data Science Team
 Author-email: #DataSciencePackages@lv.co.uk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -109,8 +109,8 @@
 pytest
 ```
 
 ## Contribute
 
 `tubular` is under active development, we're super excited if you're interested in contributing! 
 
-See the [CONTRIBUTING](https://github.com/lvgig/tubular/blob/main/CONTRIBUTING.md) file for the full details of our working practices.
+See the [CONTRIBUTING](https://github.com/lvgig/tubular/blob/main/CONTRIBUTING.rst) file for the full details of our working practices.
```

### Comparing `tubular-0.3.7/README.md` & `tubular-0.3.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -92,8 +92,8 @@
 pytest
 ```
 
 ## Contribute
 
 `tubular` is under active development, we're super excited if you're interested in contributing! 
 
-See the [CONTRIBUTING](https://github.com/lvgig/tubular/blob/main/CONTRIBUTING.md) file for the full details of our working practices.
+See the [CONTRIBUTING](https://github.com/lvgig/tubular/blob/main/CONTRIBUTING.rst) file for the full details of our working practices.
```

### Comparing `tubular-0.3.7/setup.py` & `tubular-0.3.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-import setuptools
 import re
 
-with open("README.md", "r") as fh:
+import setuptools
+
+with open("README.md") as fh:
     long_description = fh.read()
 
 # get version from _version.py file, from below
 # https://stackoverflow.com/questions/458550/standard-way-to-embed-version-into-python-package
 VERSION_FILE = "tubular/_version.py"
-version_file_str = open(VERSION_FILE, "rt").read()
 VERSION_STR_RE = r"^__version__ = ['\"]([^'\"]*)['\"]"
-mo = re.search(VERSION_STR_RE, version_file_str, re.M)
-if mo:
-    version = mo.group(1)
-else:
-    raise RuntimeError("Unable to find version string in %s." % (VERSION_FILE,))
+with open(VERSION_FILE) as version_file:
+    version_file_str = version_file.read()
+    mo = re.search(VERSION_STR_RE, version_file_str, re.M)
+    if mo:
+        version = mo.group(1)
+    else:
+        msg = f"Unable to find version string in {VERSION_FILE}."
+        raise RuntimeError(msg)
 
 
 def list_reqs(fname="requirements.txt"):
     with open(fname) as fd:
         return fd.read().splitlines()
```

### Comparing `tubular-0.3.7/tests/test_data.py` & `tubular-0.3.8/tests/test_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,164 +1,143 @@
 """This module contains functions that create simple datasets that are used in the tests."""
 
 import datetime
-import pandas as pd
+
 import numpy as np
+import pandas as pd
 
 
 def create_series_1(n=6):
     """Create simple series of [0:n-1]."""
-
-    df = pd.Series(np.arange(n))
-
-    return df
+    return pd.Series(np.arange(n))
 
 
 def create_1_int_column_df(n=6):
     """Create single column DataFrame of [0:n-1]."""
-
-    df = pd.DataFrame({"a": np.arange(n)})
-
-    return df
+    return pd.DataFrame({"a": np.arange(n)})
 
 
 def create_zeros_array(shape=(10, 3)):
     """Create simple 2d numpy array of zeros of given shape."""
-
-    arr = np.zeros(shape)
-
-    return arr
+    return np.zeros(shape)
 
 
 def create_numeric_df_1():
-    """Example with numeric dataframe"""
-    df = pd.DataFrame(
+    """Example with numeric dataframe."""
+    return pd.DataFrame(
         {
             "a": [34.48, 21.71, 32.83, 1.08, 32.93, 4.74, 2.76, 75.7, 14.08, 61.31],
             "b": [12.03, 20.32, 24.12, 24.18, 68.99, 0.0, 0.0, 59.46, 11.02, 60.68],
             "c": [17.06, 12.25, 19.15, 29.73, 1.98, 8.23, 15.22, 20.59, 3.82, 39.73],
             "d": [25.94, 70.22, 72.94, 64.55, 0.41, 13.62, 30.22, 4.6, 67.13, 10.38],
             "e": [94.3, 4.18, 51.7, 16.63, 2.6, 16.57, 3.51, 30.79, 66.19, 25.44],
-        }
+        },
     )
-    return df
 
 
 def create_df_1():
     """Create simple DataFrame with the following...
 
     6 rows
     2 columns;
     - a integer 1:6
     - b object a:f
     no nulls
     """
-
-    df = pd.DataFrame({"a": [1, 2, 3, 4, 5, 6], "b": ["a", "b", "c", "d", "e", "f"]})
-
-    return df
+    return pd.DataFrame({"a": [1, 2, 3, 4, 5, 6], "b": ["a", "b", "c", "d", "e", "f"]})
 
 
 def create_df_2():
-    """Create simple DataFrame to use in other tests"""
-
+    """Create simple DataFrame to use in other tests."""
     df = pd.DataFrame(
         {
             "a": [1, 2, 3, 4, 5, 6, np.NaN],
             "b": ["a", "b", "c", "d", "e", "f", np.NaN],
             "c": ["a", "b", "c", "d", "e", "f", np.NaN],
-        }
+        },
     )
 
     df["c"] = df["c"].astype("category")
 
     return df
 
 
 def create_df_4():
-    """Create simple DataFrame to use in other tests"""
-
+    """Create simple DataFrame to use in other tests."""
     df = pd.DataFrame(
         {
             "a": [1, 2, 3, 4, 5, 6, 7, np.NaN],
             "b": ["a", "b", "c", "d", "e", "f", "g", np.NaN],
             "c": ["a", "b", "c", "d", "e", "f", "g", np.NaN],
-        }
+        },
     )
 
     df["c"] = df["c"].astype("category")
 
     return df
 
 
 def create_df_3():
-    """Create simple DataFrame to use in other tests"""
-
-    df = pd.DataFrame(
+    """Create simple DataFrame to use in other tests."""
+    return pd.DataFrame(
         {
             "a": [1, 2, 3, 4, 5, 6, np.NaN],
             "b": [1, 2, 3, np.NaN, 7, 8, 9],
             "c": [np.NaN, 1, 2, 3, -4, -5, -6],
-        }
+        },
     )
 
-    return df
-
 
 def create_df_5():
-    """Create simple DataFrame to use in other tests"""
-
+    """Create simple DataFrame to use in other tests."""
     df = pd.DataFrame(
         {
             "a": [1, 2, 3, 4, 5, 6, 7, 8, 9, np.NaN],
             "b": ["a", "a", "a", "d", "e", "f", "g", np.NaN, np.NaN, np.NaN],
             "c": ["a", "a", "c", "c", "e", "e", "f", "g", "h", np.NaN],
-        }
+        },
     )
 
     df["c"] = df["c"].astype("category")
 
     return df
 
 
 def create_df_6():
-    """Nulls in different positions to check summing weights by col with nulls"""
-
+    """Nulls in different positions to check summing weights by col with nulls."""
     df = pd.DataFrame(
         {
             "a": [2, 2, 2, 2, np.NaN, 2, 2, 2, 3, 3],
             "b": ["a", "a", "a", "d", "e", "f", "g", np.NaN, np.NaN, np.NaN],
             "c": ["a", "b", "c", "d", "f", "f", "f", "g", "g", np.NaN],
-        }
+        },
     )
 
     df["c"] = df["c"].astype("category")
 
     return df
 
 
 def create_df_7():
-    """Create simple DataFrame to use in other tests"""
-
+    """Create simple DataFrame to use in other tests."""
     df = pd.DataFrame(
         {
             "a": [4, 2, 2, 1, 3],
             "b": ["x", "z", "y", "x", "x"],
             "c": ["c", "a", "a", "c", "b"],
-        }
+        },
     )
 
     df["c"] = df["c"].astype("category")
 
     return df
 
 
 def create_df_8():
-    """Create simple DataFrame to use in other tests"""
-
+    """Create simple DataFrame to use in other tests."""
     df = pd.DataFrame(
         {
             "a": [1, 5, 2, 3, 3],
             "b": ["w", "w", "z", "y", "x"],
             "c": ["a", "a", "c", "b", "a"],
         },
         index=[10, 15, 200, 251, 59],
@@ -166,53 +145,44 @@
 
     df["c"] = df["c"].astype("category")
 
     return df
 
 
 def create_df_9():
-    """Create simple DataFrame to use in other tests"""
-
-    df = pd.DataFrame(
+    """Create simple DataFrame to use in other tests."""
+    return pd.DataFrame(
         {
             "a": [1, 2, np.nan, 4, np.nan, 6],
             "b": [np.nan, 5, 4, 3, 2, 1],
             "c": [3, 2, 1, 4, 5, 6],
-        }
+        },
     )
 
-    return df
-
 
 def create_df_10():
-    """Create simple DataFrame to use in other tests"""
-
-    df = pd.DataFrame(
+    """Create simple DataFrame to use in other tests."""
+    return pd.DataFrame(
         {
             "a": [1, 2, 3, 4, 5, 6, 7, 8, 9, np.NaN],
             "b": ["a", "a", "a", "d", "e", "f", "g", np.NaN, np.NaN, np.NaN],
             "c": [1, 1, 3, 4, 5, 6, 5, 8, 9, 50],
-        }
+        },
     )
 
-    return df
-
 
 def create_df_11():
-    """Create simple DataFrame to use in other tests"""
-
-    df = pd.DataFrame(
+    """Create simple DataFrame to use in other tests."""
+    return pd.DataFrame(
         {
             "a": [1, 2, 3],
             "b": [4, 5, 6],
-        }
+        },
     )
 
-    return df
-
 
 def create_large_null_df(n_col=1000):
     """Create large single row df with all null values.
 
     Parameters
     ----------
     n_col : int
@@ -220,24 +190,20 @@
 
     Returns
     -------
     data_df : pd.DataFrame
         Single row dataframe with n_col columns; entirely populated with null values.
 
     """
-
     data_dict = {}
 
     for i in range(n_col):
-
         data_dict["col_" + str(i)] = np.NaN
 
-    data_df = pd.DataFrame(data_dict, index=[0])
-
-    return data_df
+    return pd.DataFrame(data_dict, index=[0])
 
 
 def create_large_half_null_df(n_col=1000):
     """Create large 2 row df with all null values in 1 row and all 1s in the other.
 
     Parameters
     ----------
@@ -247,56 +213,48 @@
     Returns
     -------
     data_df : pd.DataFrame
         Two row dataframe with n_col columns; the first row taking entirely values of 1 and the
         second taking entirely null values.
 
     """
-
     data_dict = {}
 
     col_values = [1.0, np.NaN]
 
     for i in range(n_col):
-
         data_dict["col_" + str(i)] = col_values
 
-    data_df = pd.DataFrame(data_dict, index=[0, 1])
-
-    return data_df
+    return pd.DataFrame(data_dict, index=[0, 1])
 
 
 def create_weighted_imputers_test_df():
-    """Create DataFrame to use imputer tests that correct values are imputed for weighted dataframes
+    """Create DataFrame to use imputer tests that correct values are imputed for weighted dataframes.
 
     weight column contains the weights between 0 and 1
     """
-
-    df = pd.DataFrame(
+    return pd.DataFrame(
         {
             "a": [1.0, 1.0, 1.0, 3.0, 5.0, 5.0],
             "b": ["a", "a", "a", "d", "e", "e"],
             "c": ["a", "a", np.nan, np.nan, np.nan, "f"],
             "d": [1.0, 5.0, 3.0, np.nan, np.nan, 1.0],
             "response": [0, 1, 0, 1, 1, 1],
             "weight": [0.1, 0.1, 0.8, 0.5, 0.9, 0.8],
-        }
+        },
     )
 
-    return df
-
 
 def create_MeanResponseTransformer_test_df():
-    """Create DataFrame to use MeanResponseTransformer tests that correct values are
+    """Create DataFrame to use MeanResponseTransformer tests that correct values are.
 
     DataFrame column a is the response, the other columns are categorical columns
     of types; object, category, int, float, bool.
 
     """
-
     df = pd.DataFrame(
         {
             "a": [1.0, 2.0, 3.0, 4.0, 5.0, 6.0],
             "b": ["a", "b", "c", "d", "e", "f"],
             "c": ["a", "b", "c", "d", "e", "f"],
             "d": [1, 2, 3, 4, 5, 6],
             "e": [1, 2, 3, 4, 5, 6.0],
@@ -305,15 +263,15 @@
                 "blue",
                 "blue",
                 "yellow",
                 "yellow",
                 "green",
                 "green",
             ],
-        }
+        },
     )
 
     df["c"] = df["c"].astype("category")
 
     return df
 
 
@@ -338,83 +296,75 @@
                 "yellow",
                 "yellow",
                 "green",
                 "green",
                 "yellow",
                 "blue",
             ],
-        }
+        },
     )
 
     df["c"] = df["c"].astype("category")
 
     return df
 
 
 def create_OrdinalEncoderTransformer_test_df():
-    """Create DataFrame to use OrdinalEncoderTransformer tests that correct values are
+    """Create DataFrame to use OrdinalEncoderTransformer tests that correct values are.
 
     DataFrame column a is the response, the other columns are categorical columns
     of types; object, category, int, float, bool.
 
     """
-
     df = pd.DataFrame(
         {
             "a": [1, 2, 3, 4, 5, 6],
             "b": ["a", "b", "c", "d", "e", "f"],
             "c": ["a", "b", "c", "d", "e", "f"],
             "d": [1, 2, 3, 4, 5, 6],
             "e": [3, 4, 5, 6, 7, 8.0],
             "f": [False, False, False, True, True, True],
-        }
+        },
     )
 
     df["c"] = df["c"].astype("category")
 
     return df
 
 
 def create_NearestMeanResponseImputer_test_df():
     """Create DataFrame to use in NearestMeanResponseImputer tests.
 
     DataFrame column c is the response, the other columns are numerical columns containing null entries.
 
     """
-
-    df = pd.DataFrame(
+    return pd.DataFrame(
         {
             "a": [1, 1, 2, 3, 3, np.nan],
             "b": [np.nan, np.nan, 1, 3, 3, 4],
             "c": [2, 3, 2, 1, 4, 1],
-        }
+        },
     )
 
-    return df
-
 
 def create_values_map(df):
-
     value_map = {}
 
     for i in df.columns:
-
         value_map[i] = {}
 
         for j in df[i].unique():
-
             value_map[i][j] = j
 
     return value_map
 
 
 def create_date_test_df():
     """Create DataFrame for DateDiffLeapYearTransformer tests."""
-
-    df = pd.DataFrame(
+    return pd.DataFrame(
         {
             "a": [
                 datetime.date(1993, 9, 27),
                 datetime.date(2000, 3, 19),
                 datetime.date(2018, 11, 10),
                 datetime.date(2018, 10, 10),
                 datetime.date(2018, 10, 10),
@@ -428,42 +378,36 @@
                 datetime.date(2018, 11, 10),
                 datetime.date(2018, 11, 10),
                 datetime.date(2018, 9, 10),
                 datetime.date(2015, 11, 10),
                 datetime.date(2015, 11, 10),
                 datetime.date(2015, 7, 23),
             ],
-        }
+        },
     )
 
-    return df
-
 
 def create_date_test_nulls_df():
     """Create DataFrame with nulls only for DateDiffLeapYearTransformer, DateDifferenceTransformer tests."""
-
-    df = pd.DataFrame(
+    return pd.DataFrame(
         {
             "a": [
                 np.NaN,
             ],
             "b": [
                 np.NaN,
             ],
         },
         index=[0],
     )
 
-    return df
-
 
 def create_datediff_test_df():
     """Create DataFrame for DateDifferenceTransformer tests."""
-
-    df = pd.DataFrame(
+    return pd.DataFrame(
         {
             "a": [
                 datetime.datetime(1993, 9, 27, 11, 58, 58),
                 datetime.datetime(2000, 3, 19, 12, 59, 59),
                 datetime.datetime(2018, 11, 10, 11, 59, 59),
                 datetime.datetime(2018, 10, 10, 11, 59, 59),
                 datetime.datetime(2018, 10, 10, 11, 59, 59),
@@ -477,68 +421,56 @@
                 datetime.datetime(2018, 11, 10, 11, 59, 59),
                 datetime.datetime(2018, 11, 10, 11, 59, 59),
                 datetime.datetime(2018, 9, 10, 9, 59, 59),
                 datetime.datetime(2015, 11, 10, 11, 59, 59),
                 datetime.datetime(2015, 11, 10, 12, 59, 59),
                 datetime.datetime(2015, 7, 23, 11, 59, 59),
             ],
-        }
+        },
     )
 
-    return df
-
 
 def create_datediff_test_nulls_df():
     """Create DataFrame with nulls only for DateDifferenceTransformer tests."""
-
-    df = pd.DataFrame(
+    return pd.DataFrame(
         {
             "a": [
                 datetime.datetime(1993, 9, 27, 11, 58, 58),
                 np.NaN,
             ],
             "b": [
                 np.NaN,
                 datetime.datetime(2019, 12, 25, 11, 58, 58),
             ],
         },
         index=[0, 1],
     )
 
-    return df
-
 
 def create_to_datetime_test_df():
     """Create DataFrame to be used in the ToDatetimeTransformer tests."""
-
-    df = pd.DataFrame(
-        {"a": [1950, 1960, 2000, 2001, np.NaN, 2010], "b": [1, 2, 3, 4, 5, np.NaN]}
+    return pd.DataFrame(
+        {"a": [1950, 1960, 2000, 2001, np.NaN, 2010], "b": [1, 2, 3, 4, 5, np.NaN]},
     )
 
-    return df
-
 
 def create_is_between_dates_df_1():
     """Create df to use in IsBetweenDates tests. Contains 3 columns of 2 datatime values."""
-
-    df = pd.DataFrame(
+    return pd.DataFrame(
         {
             "a": pd.date_range(start="1/1/2016", end="27/02/2017", periods=2),
             "b": pd.date_range(start="1/2/2016", end="27/09/2017", periods=2),
             "c": pd.date_range(start="1/3/2016", end="27/04/2017", periods=2),
-        }
+        },
     )
 
-    return df
-
 
 def create_is_between_dates_df_2():
     """Create df to use in IsBetweenDates tests. Contains 3 columns of 5 datatime values, covers edge cases."""
-
-    df = pd.DataFrame(
+    return pd.DataFrame(
         {
             "a": [
                 datetime.datetime(1990, 2, 1),
                 datetime.datetime(1990, 2, 1),
                 datetime.datetime(1990, 2, 1),
                 datetime.datetime(1990, 2, 1),
                 datetime.datetime(1990, 2, 1),
@@ -556,24 +488,20 @@
                 datetime.datetime(1990, 3, 1),
                 datetime.datetime(1990, 3, 1),
                 datetime.datetime(1990, 3, 1),
                 datetime.datetime(1990, 3, 1),
                 datetime.datetime(1990, 3, 1),
                 datetime.datetime(1990, 3, 1),
             ],
-        }
+        },
     )
 
-    return df
-
 
 # Example DataFrame for downcasting dtypes tests
 def create_downcast_df():
     """Create a dataframe with mixed dtypes to use in downcasting tests."""
-    df = pd.DataFrame(
+    return pd.DataFrame(
         {
             "a": [1, 2, 3, 4, 5],
             "b": [1.0, 2.0, 3.0, 4.0, 5.0],
-        }
+        },
     )
-
-    return df
```

### Comparing `tubular-0.3.7/tests/test_transformers.py` & `tubular-0.3.8/tests/test_transformers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,56 @@
 # tests to apply to all transformers
 import pytest
+import sklearn.base as b
+
 import tubular.base as base
 import tubular.capping as capping
 import tubular.comparison as comparison
 import tubular.dates as dates
 import tubular.imputers as imputers
 import tubular.mapping as mapping
 import tubular.misc as misc
 import tubular.nominal as nominal
 import tubular.numeric as numeric
 import tubular.strings as strings
-import sklearn.base as b
 
 
-class TestInit(object):
+class TestInit:
     """Tests for transformer.init()."""
 
     def ListOfTransformers():
         """List of transformers in tubular to be used in subsequent tests."""
-
-        list_of_transformers = [
+        return [
             base.BaseTransformer(columns=["a"]),
             base.DataFrameMethodTransformer(
-                new_column_name="a", pd_method_name="sum", columns="b"
+                new_column_name="a",
+                pd_method_name="sum",
+                columns="b",
             ),
             capping.CappingTransformer(capping_values={"a": [0.1, 0.2]}),
             capping.OutOfRangeNullTransformer(capping_values={"a": [0.1, 0.2]}),
             comparison.EqualityChecker(columns=["a", "b"], new_col_name="c"),
             dates.DateDiffLeapYearTransformer(
-                column_lower="a", column_upper="b", new_column_name="c", drop_cols=True
+                column_lower="a",
+                column_upper="b",
+                new_column_name="c",
+                drop_cols=True,
             ),
             dates.DateDifferenceTransformer(
-                column_lower="a", column_upper="b", new_column_name="c", units="D"
+                column_lower="a",
+                column_upper="b",
+                new_column_name="c",
+                units="D",
             ),
             dates.ToDatetimeTransformer(column="a", new_column_name="b"),
             dates.DatetimeInfoExtractor(columns="a"),
             dates.SeriesDtMethodTransformer(
-                new_column_name="a", pd_method_name="month", column="b"
+                new_column_name="a",
+                pd_method_name="month",
+                column="b",
             ),
             dates.BetweenDatesTransformer(
                 column_lower="a",
                 column_upper="b",
                 column_between="c",
                 new_column_name="c",
             ),
@@ -57,21 +67,24 @@
             imputers.ModeImputer(columns="a"),
             imputers.NearestMeanResponseImputer(columns="a"),
             imputers.NullIndicator(columns="a"),
             mapping.BaseMappingTransformer(mappings={"a": {1: 2, 3: 4}}),
             mapping.BaseMappingTransformMixin(),
             mapping.MappingTransformer(mappings={"a": {1: 2, 3: 4}}),
             mapping.CrossColumnMappingTransformer(
-                adjust_column="b", mappings={"a": {1: 2, 3: 4}}
+                adjust_column="b",
+                mappings={"a": {1: 2, 3: 4}},
             ),
             mapping.CrossColumnMultiplyTransformer(
-                adjust_column="b", mappings={"a": {1: 2, 3: 4}}
+                adjust_column="b",
+                mappings={"a": {1: 2, 3: 4}},
             ),
             mapping.CrossColumnAddTransformer(
-                adjust_column="b", mappings={"a": {1: 2, 3: 4}}
+                adjust_column="b",
+                mappings={"a": {1: 2, 3: 4}},
             ),
             misc.SetValueTransformer(columns="a", value=1),
             misc.SetColumnDtype(columns="a", dtype=str),
             nominal.BaseNominalTransformer(),
             nominal.NominalToIntegerTransformer(columns="a"),
             nominal.GroupRareLevelsTransformer(columns="a"),
             nominal.MeanResponseTransformer(columns="a"),
@@ -89,34 +102,25 @@
                 new_column_name="a",
                 pd_method_name="find",
                 columns="b",
                 pd_method_kwargs={"sub": "a"},
             ),
             strings.StringConcatenator(columns=["a", "b"], new_column="c"),
         ]
-        return list_of_transformers
 
     @pytest.mark.parametrize("transformer", ListOfTransformers())
     def test_print(self, transformer):
-        """
-        Test that transformer can be printed.
+        """Test that transformer can be printed.
         If an error is raised in this test it will not prevent the transformer from working correctly,
         but will stop other unit tests passing.
         """
-
         print(transformer)
 
     @pytest.mark.parametrize("transformer", ListOfTransformers())
     def test_clone(self, transformer):
-        """
-        Test that transformer can be used in sklearn.base.clone function.
-        """
-
+        """Test that transformer can be used in sklearn.base.clone function."""
         b.clone(transformer)
 
     @pytest.mark.parametrize("transformer", ListOfTransformers())
     def test_unexpected_kwarg(self, transformer):
-        """
-        Test that transformer can be used in sklearn.base.clone function.
-        """
-
+        """Test that transformer can be used in sklearn.base.clone function."""
         b.clone(transformer)
```

### Comparing `tubular-0.3.7/tubular/base.py` & `tubular-0.3.8/tubular/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-"""
-This module contains transformers that other transformers in the package inherit
+"""This module contains transformers that other transformers in the package inherit
 from. These transformers contain key checks to be applied in all cases.
 """
 
-import pandas as pd
 import warnings
+
+import pandas as pd
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import check_is_fitted
 
-
 from tubular._version import __version__
 
 
 class BaseTransformer(TransformerMixin, BaseEstimator):
     """Base tranformer class which all other transformers in the package inherit from.
 
     Provides fit and transform methods (required by sklearn transformers), simple input checking
@@ -44,73 +43,58 @@
 
     version_ : str
         Version number (__version__ attribute from _version.py).
 
     """
 
     def classname(self):
-        """Method that returns the name of the current class when called"""
+        """Method that returns the name of the current class when called."""
         return type(self).__name__
 
-    def __init__(self, columns=None, copy=True, verbose=False):
-
+    def __init__(self, columns=None, copy=True, verbose=False) -> None:
         self.version_ = __version__
 
         if not isinstance(verbose, bool):
+            msg = f"{self.classname()}: verbose must be a bool"
+            raise TypeError(msg)
 
-            raise TypeError(f"{self.classname()}: verbose must be a bool")
-
-        else:
-
-            self.verbose = verbose
+        self.verbose = verbose
 
         if self.verbose:
-
             print("BaseTransformer.__init__() called")
 
         if columns is None:
-
             self.columns = None
 
         else:
-
             # make sure columns is a single str or list of strs
             if isinstance(columns, str):
-
                 self.columns = [columns]
 
             elif isinstance(columns, list):
-
                 if not len(columns) > 0:
-
-                    raise ValueError(f"{self.classname()}: columns has no values")
+                    msg = f"{self.classname()}: columns has no values"
+                    raise ValueError(msg)
 
                 for c in columns:
-
                     if not isinstance(c, str):
-
-                        raise TypeError(
-                            f"{self.classname()}: each element of columns should be a single (string) column name"
-                        )
+                        msg = f"{self.classname()}: each element of columns should be a single (string) column name"
+                        raise TypeError(msg)
 
                 self.columns = columns
 
             else:
-
-                raise TypeError(
-                    f"{self.classname()}: columns must be a string or list with the columns to be pre-processed (if specified)"
-                )
+                msg = f"{self.classname()}: columns must be a string or list with the columns to be pre-processed (if specified)"
+                raise TypeError(msg)
 
         if not isinstance(copy, bool):
+            msg = f"{self.classname()}: copy must be a bool"
+            raise TypeError(msg)
 
-            raise TypeError(f"{self.classname()}: copy must be a bool")
-
-        else:
-
-            self.copy = copy
+        self.copy = copy
 
     def fit(self, X, y=None):
         """Base transformer fit method, checks X and y types. Currently only pandas DataFrames are allowed for X
         and DataFrames or Series for y.
 
         Fit calls the columns_set_or_check method which will set the columns attribute to all columns in X, if it
         is None.
@@ -120,36 +104,33 @@
         X : pd.DataFrame
             Data to fit the transformer on.
 
         y : None or pd.DataFrame or pd.Series, default = None
             Optional argument only required for the transformer to work with sklearn pipelines.
 
         """
-
         if self.verbose:
-
             print("BaseTransformer.fit() called")
 
         self.columns_set_or_check(X)
 
         if not X.shape[0] > 0:
-
-            raise ValueError(f"{self.classname()}: X has no rows; {X.shape}")
+            msg = f"{self.classname()}: X has no rows; {X.shape}"
+            raise ValueError(msg)
 
         if y is not None:
-
             if not isinstance(y, pd.Series):
-
-                raise TypeError(
+                msg = (
                     f"{self.classname()}: unexpected type for y, should be a pd.Series"
                 )
+                raise TypeError(msg)
 
             if not y.shape[0] > 0:
-
-                raise ValueError(f"{self.classname()}: y is empty; {y.shape}")
+                msg = f"{self.classname()}: y is empty; {y.shape}"
+                raise ValueError(msg)
 
         return self
 
     def _combine_X_y(self, X, y):
         """Combine X and y by adding a new column with the values of y to a copy of X.
 
         The new column response column will be called `_temporary_response`.
@@ -162,36 +143,32 @@
         X : pd.DataFrame
             Data containing explanatory variables.
 
         y : pd.Series
             Response variable.
 
         """
-
         if not isinstance(X, pd.DataFrame):
-
-            raise TypeError(f"{self.classname()}: X should be a pd.DataFrame")
+            msg = f"{self.classname()}: X should be a pd.DataFrame"
+            raise TypeError(msg)
 
         if not isinstance(y, pd.Series):
-
-            raise TypeError(f"{self.classname()}: y should be a pd.Series")
+            msg = f"{self.classname()}: y should be a pd.Series"
+            raise TypeError(msg)
 
         if X.shape[0] != y.shape[0]:
-
-            raise ValueError(
-                f"{self.classname()}: X and y have different numbers of rows ({X.shape[0]} vs {y.shape[0]})"
-            )
+            msg = f"{self.classname()}: X and y have different numbers of rows ({X.shape[0]} vs {y.shape[0]})"
+            raise ValueError(msg)
 
         if not (X.index == y.index).all():
-
             warnings.warn(f"{self.classname()}: X and y do not have equal indexes")
 
         X_y = X.copy()
 
-        X_y["_temporary_response"] = y.values
+        X_y["_temporary_response"] = y.to_numpy()
 
         return X_y
 
     def transform(self, X):
         """Base transformer transform method; checks X type (pandas DataFrame only) and copies data if requested.
 
         Transform calls the columns_check method which will check columns in columns attribute are in X.
@@ -203,28 +180,25 @@
 
         Returns
         -------
         X : pd.DataFrame
             Input X, copied if specified by user.
 
         """
-
         self.columns_check(X)
 
         if self.verbose:
-
             print("BaseTransformer.transform() called")
 
         if self.copy:
-
             X = X.copy()
 
         if not X.shape[0] > 0:
-
-            raise ValueError(f"{self.classname()}: X has no rows; {X.shape}")
+            msg = f"{self.classname()}: X has no rows; {X.shape}"
+            raise ValueError(msg)
 
         return X
 
     def check_is_fitted(self, attribute):
         """Check if particular attributes are on the object. This is useful to do before running transform to avoid
         trying to transform data without first running the fit method.
 
@@ -232,102 +206,94 @@
 
         Parameters
         ----------
         attributes : List
             List of str values giving names of attribute to check exist on self.
 
         """
-
         check_is_fitted(self, attribute)
 
     def columns_check(self, X):
         """Method to check that the columns attribute is set and all values are present in X.
 
         Parameters
         ----------
         X : pd.DataFrame
             Data to check columns are in.
 
         """
-
         if not isinstance(X, pd.DataFrame):
-
-            raise TypeError(f"{self.classname()}: X should be a pd.DataFrame")
+            msg = f"{self.classname()}: X should be a pd.DataFrame"
+            raise TypeError(msg)
 
         if self.columns is None:
-
-            raise ValueError(f"{self.classname()}: columns not set")
+            msg = f"{self.classname()}: columns not set"
+            raise ValueError(msg)
 
         if not isinstance(self.columns, list):
-
-            raise TypeError(f"{self.classname()}: self.columns should be a list")
+            msg = f"{self.classname()}: self.columns should be a list"
+            raise TypeError(msg)
 
         for c in self.columns:
-
-            if c not in X.columns.values:
-
+            if c not in X.columns.to_numpy():
                 raise ValueError(f"{self.classname()}: variable " + c + " is not in X")
 
     def columns_set_or_check(self, X):
         """Function to check or set columns attribute.
 
         If the columns attribute is None then set it to all columns in X. Otherwise run the columns_check method.
 
         Parameters
         ----------
         X : pd.DataFrame
             Data to check columns are in.
 
         """
-
         if not isinstance(X, pd.DataFrame):
-
-            raise TypeError(f"{self.classname()}: X should be a pd.DataFrame")
+            msg = f"{self.classname()}: X should be a pd.DataFrame"
+            raise TypeError(msg)
 
         if self.columns is None:
-
             self.columns = list(X.columns.values)
 
         else:
-
             self.columns_check(X)
 
     @staticmethod
     def check_weights_column(X, weights_column):
-        """Helper method for validating weights column in dataframe
+        """Helper method for validating weights column in dataframe.
 
         Args:
+        ----
             X (pd.DataFrame): df containing weight column
             weights_column (str): name of weight column
 
         """
-
         if weights_column is not None:
-
             # check if given weight is in columns
             if weights_column not in X.columns:
-
-                raise ValueError(
-                    f"weight col ({weights_column}) is not present in columns of data"
-                )
+                msg = f"weight col ({weights_column}) is not present in columns of data"
+                raise ValueError(msg)
 
             # check weight is numeric
-            elif not pd.api.types.is_numeric_dtype(X[weights_column]):
 
-                raise ValueError("weight column must be numeric.")
+            if not pd.api.types.is_numeric_dtype(X[weights_column]):
+                msg = "weight column must be numeric."
+                raise ValueError(msg)
 
             # check weight is positive
-            elif not (X[weights_column] < 0).sum() == 0:
 
-                raise ValueError("weight column must be positive")
+            if (X[weights_column] < 0).sum() != 0:
+                msg = "weight column must be positive"
+                raise ValueError(msg)
 
             # check weight non-null
-            elif not (X[weights_column].isnull()).sum() == 0:
-
-                raise ValueError("weight column must be non-null")
+            if X[weights_column].isna().sum() != 0:
+                msg = "weight column must be non-null"
+                raise ValueError(msg)
 
 
 class ReturnKeyDict(dict):
     """Dict class that implements __missing__ method to return the key if it is not present in the dict
     when looked up.
 
     This is intended to be used in combination with the pd.Series.map function so that it does not
@@ -343,15 +309,14 @@
             key to lookup from dict
 
         Returns
         -------
         key : input key
 
         """
-
         return key
 
 
 class DataFrameMethodTransformer(BaseTransformer):
     """Tranformer that applies a pandas.DataFrame method.
 
     Transformer assigns the output of the method to a new column or columns. It is possible to
@@ -403,77 +368,56 @@
         self,
         new_column_name,
         pd_method_name,
         columns,
         pd_method_kwargs={},
         drop_original=False,
         **kwargs,
-    ):
-
+    ) -> None:
         super().__init__(columns=columns, **kwargs)
 
         if type(new_column_name) is list:
-
             for i, item in enumerate(new_column_name):
-
-                if not type(item) is str:
-
-                    raise TypeError(
-                        f"{self.classname()}: if new_column_name is a list, all elements must be strings but got {type(item)} in position {i}"
-                    )
-
-        elif not type(new_column_name) is str:
-
-            raise TypeError(
-                f"{self.classname()}: unexpected type ({type(new_column_name)}) for new_column_name, must be str or list of strings"
-            )
-
-        if not type(pd_method_name) is str:
-
-            raise TypeError(
-                f"{self.classname()}: unexpected type ({type(pd_method_name)}) for pd_method_name, expecting str"
-            )
-
-        if not type(pd_method_kwargs) is dict:
-
-            raise TypeError(
-                f"{self.classname()}: pd_method_kwargs should be a dict but got type {type(pd_method_kwargs)}"
-            )
-
-        else:
-
-            for i, k in enumerate(pd_method_kwargs.keys()):
-
-                if not type(k) is str:
-
-                    raise TypeError(
-                        f"{self.classname()}: unexpected type ({type(k)}) for pd_method_kwargs key in position {i}, must be str"
-                    )
-
-        if not type(drop_original) is bool:
-
-            raise TypeError(
-                f"{self.classname()}: unexpected type ({type(drop_original)}) for drop_original, expecting bool"
-            )
+                if type(item) is not str:
+                    msg = f"{self.classname()}: if new_column_name is a list, all elements must be strings but got {type(item)} in position {i}"
+                    raise TypeError(msg)
+
+        elif type(new_column_name) is not str:
+            msg = f"{self.classname()}: unexpected type ({type(new_column_name)}) for new_column_name, must be str or list of strings"
+            raise TypeError(msg)
+
+        if type(pd_method_name) is not str:
+            msg = f"{self.classname()}: unexpected type ({type(pd_method_name)}) for pd_method_name, expecting str"
+            raise TypeError(msg)
+
+        if type(pd_method_kwargs) is not dict:
+            msg = f"{self.classname()}: pd_method_kwargs should be a dict but got type {type(pd_method_kwargs)}"
+            raise TypeError(msg)
+
+        for i, k in enumerate(pd_method_kwargs.keys()):
+            if type(k) is not str:
+                msg = f"{self.classname()}: unexpected type ({type(k)}) for pd_method_kwargs key in position {i}, must be str"
+                raise TypeError(msg)
+
+        if type(drop_original) is not bool:
+            msg = f"{self.classname()}: unexpected type ({type(drop_original)}) for drop_original, expecting bool"
+            raise TypeError(msg)
 
         self.new_column_name = new_column_name
         self.pd_method_name = pd_method_name
         self.pd_method_kwargs = pd_method_kwargs
         self.drop_original = drop_original
 
         try:
-
             df = pd.DataFrame()
             getattr(df, pd_method_name)
 
         except Exception as err:
-
-            raise AttributeError(
-                f"""{self.classname()}: error accessing "{pd_method_name}" method on pd.DataFrame object - pd_method_name should be a pd.DataFrame method"""
-            ) from err
+            msg = f'{self.classname()}: error accessing "{pd_method_name}" method on pd.DataFrame object - pd_method_name should be a pd.DataFrame method'
+            raise AttributeError(msg) from err
 
     def transform(self, X):
         """Transform input pandas DataFrame (X) using the given pandas.DataFrame method and assign the output
         back to column or columns in X.
 
         Any keyword arguments set in the pd_method_kwargs attribute are passed onto the pandas DataFrame method when calling it.
 
@@ -485,19 +429,17 @@
         Returns
         -------
         X : pd.DataFrame
             Input X with additional column or columns (self.new_column_name) added. These contain the output of
             running the pandas DataFrame method.
 
         """
-
         X = super().transform(X)
 
         X[self.new_column_name] = getattr(X[self.columns], self.pd_method_name)(
-            **self.pd_method_kwargs
+            **self.pd_method_kwargs,
         )
 
         if self.drop_original:
-
-            X.drop(self.columns, axis=1, inplace=True)
+            X = X.drop(self.columns, axis=1)
 
         return X
```

### Comparing `tubular-0.3.7/tubular/capping.py` & `tubular-0.3.8/tubular/capping.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-"""
-This module contains a transformer that applies capping to numeric columns.
-"""
+"""This module contains a transformer that applies capping to numeric columns."""
 
-import pandas as pd
-import numpy as np
-import warnings
 import copy
+import warnings
+
+import numpy as np
+import pandas as pd
 
 from tubular.base import BaseTransformer
 
 
 class CappingTransformer(BaseTransformer):
     """Transformer to cap numeric values at both or either minimum and maximum values.
 
@@ -57,120 +56,92 @@
 
     _replacement_values : dict
         Replacement values when capping is applied. Will be a copy of capping_values.
 
     """
 
     def __init__(
-        self, capping_values=None, quantiles=None, weights_column=None, **kwargs
-    ):
-
+        self,
+        capping_values=None,
+        quantiles=None,
+        weights_column=None,
+        **kwargs,
+    ) -> None:
         if capping_values is None and quantiles is None:
-
-            raise ValueError(
-                f"{self.classname()}: both capping_values and quantiles are None, either supply capping values in the "
-                "capping_values argument or supply quantiles that can be learnt in the fit method"
-            )
+            msg = f"{self.classname()}: both capping_values and quantiles are None, either supply capping values in the capping_values argument or supply quantiles that can be learnt in the fit method"
+            raise ValueError(msg)
 
         if capping_values is not None and quantiles is not None:
-
-            raise ValueError(
-                f"{self.classname()}: both capping_values and quantiles are not None, supply one or the other"
-            )
+            msg = f"{self.classname()}: both capping_values and quantiles are not None, supply one or the other"
+            raise ValueError(msg)
 
         if capping_values is not None:
-
             self.check_capping_values_dict(capping_values, "capping_values")
 
             self.capping_values = capping_values
 
             super().__init__(columns=list(capping_values.keys()), **kwargs)
 
         if quantiles is not None:
-
             self.check_capping_values_dict(quantiles, "quantiles")
 
             for k, quantile_values in quantiles.items():
-
                 for quantile_value in quantile_values:
-
-                    if quantile_value is not None:
-
-                        if quantile_value < 0 or quantile_value > 1:
-
-                            raise ValueError(
-                                f"{self.classname()}: quantile values must be in the range [0, 1] but got {quantile_value} for key {k}"
-                            )
+                    if (quantile_value is not None) and (
+                        quantile_value < 0 or quantile_value > 1
+                    ):
+                        msg = f"{self.classname()}: quantile values must be in the range [0, 1] but got {quantile_value} for key {k}"
+                        raise ValueError(msg)
 
             self.capping_values = {}
 
             super().__init__(columns=list(quantiles.keys()), **kwargs)
 
         self.quantiles = quantiles
         self.weights_column = weights_column
         self._replacement_values = copy.deepcopy(self.capping_values)
 
     def check_capping_values_dict(self, capping_values_dict, dict_name):
         """Performs checks on a dictionary passed to ."""
-
         if type(capping_values_dict) is not dict:
-
-            raise TypeError(
-                f"{self.classname()}: {dict_name} should be dict of columns and capping values"
-            )
+            msg = f"{self.classname()}: {dict_name} should be dict of columns and capping values"
+            raise TypeError(msg)
 
         for k, cap_values in capping_values_dict.items():
-
             if type(k) is not str:
-
-                raise TypeError(
-                    f"{self.classname()}: all keys in {dict_name} should be str, but got {type(k)}"
-                )
+                msg = f"{self.classname()}: all keys in {dict_name} should be str, but got {type(k)}"
+                raise TypeError(msg)
 
             if type(cap_values) is not list:
-
-                raise TypeError(
-                    f"{self.classname()}: each item in {dict_name} should be a list, but got {type(cap_values)} for key {k}"
-                )
+                msg = f"{self.classname()}: each item in {dict_name} should be a list, but got {type(cap_values)} for key {k}"
+                raise TypeError(msg)
 
             if len(cap_values) != 2:
-
-                raise ValueError(
-                    f"{self.classname()}: each item in {dict_name} should be length 2, but got {len(cap_values)} for key {k}"
-                )
+                msg = f"{self.classname()}: each item in {dict_name} should be length 2, but got {len(cap_values)} for key {k}"
+                raise ValueError(msg)
 
             for cap_value in cap_values:
-
                 if cap_value is not None:
-
                     if type(cap_value) not in [int, float]:
-
-                        raise TypeError(
-                            f"{self.classname()}: each item in {dict_name} lists must contain numeric values or None, got {type(cap_value)} for key {k}"
-                        )
+                        msg = f"{self.classname()}: each item in {dict_name} lists must contain numeric values or None, got {type(cap_value)} for key {k}"
+                        raise TypeError(msg)
 
                     if np.isnan(cap_value) or np.isinf(cap_value):
+                        msg = f"{self.classname()}: item in {dict_name} lists contains numpy NaN or Inf values"
+                        raise ValueError(msg)
 
-                        raise ValueError(
-                            f"{self.classname()}: item in {dict_name} lists contains numpy NaN or Inf values"
-                        )
-
-            if all([cap_value is not None for cap_value in cap_values]):
-
-                if cap_values[0] >= cap_values[1]:
-
-                    raise ValueError(
-                        f"{self.classname()}: lower value is greater than or equal to upper value for key {k}"
-                    )
-
-            if all([cap_value is None for cap_value in cap_values]):
-
-                raise ValueError(
-                    f"{self.classname()}: both values are None for key {k}"
-                )
+            if all(cap_value is not None for cap_value in cap_values) and (
+                cap_values[0] >= cap_values[1]
+            ):
+                msg = f"{self.classname()}: lower value is greater than or equal to upper value for key {k}"
+                raise ValueError(msg)
+
+            if all(cap_value is None for cap_value in cap_values):
+                msg = f"{self.classname()}: both values are None for key {k}"
+                raise ValueError(msg)
 
     def fit(self, X, y=None):
         """Learn capping values from input data X.
 
         Calculates the quantiles to cap at given the quantiles dictionary supplied
         when initialising the transformer. Saves learnt values in the capping_values
         attribute.
@@ -180,39 +151,37 @@
         X : pd.DataFrame
             A dataframe with required columns to be capped.
 
         y : None
             Required for pipeline.
 
         """
-
         super().fit(X, y)
 
         if self.quantiles is not None:
-
             for col in self.columns:
-
                 if self.weights_column is None:
-
                     cap_values = self.prepare_quantiles(
-                        X[col], self.quantiles[col], self.weights_column
+                        X[col],
+                        self.quantiles[col],
+                        self.weights_column,
                     )
 
                 else:
-
                     cap_values = self.prepare_quantiles(
-                        X[col], self.quantiles[col], X[self.weights_column]
+                        X[col],
+                        self.quantiles[col],
+                        X[self.weights_column],
                     )
 
                 self.capping_values[col] = cap_values
 
         else:
-
             warnings.warn(
-                f"{self.classname()}: quantiles not set so no fitting done in CappingTransformer"
+                f"{self.classname()}: quantiles not set so no fitting done in CappingTransformer",
             )
 
         self._replacement_values = copy.deepcopy(self.capping_values)
 
         return self
 
     def prepare_quantiles(self, values, quantiles, sample_weight=None):
@@ -237,33 +206,29 @@
 
         Returns
         -------
         interp_quantiles : list
             List containing computed quantiles.
 
         """
-
         if quantiles[0] is None:
-
             quantiles = np.array([quantiles[1]])
 
             results_no_none = self.weighted_quantile(values, quantiles, sample_weight)
 
             results = [None] + results_no_none
 
         elif quantiles[1] is None:
-
             quantiles = np.array([quantiles[0]])
 
             results_no_none = self.weighted_quantile(values, quantiles, sample_weight)
 
             results = results_no_none + [None]
 
         else:
-
             results = self.weighted_quantile(values, quantiles, sample_weight)
 
         return results
 
     def weighted_quantile(self, values, quantiles, sample_weight=None):
         """Method to calculate weighted quantiles.
 
@@ -317,33 +282,34 @@
         [1.0, 1.0, 1.0, 1.5, 2.0, 2.5, 3.0, 3.5, 4.0, 4.5, 5.0]
         >>>
         >>> computed_quantiles = x.weighted_quantile(values = [1, 2, 3, 4, 5], sample_weight = [1, 0, 1, 0, 1], quantiles = [0, 0.5, 1.0])
         >>> [round(q, 1) for q in computed_quantiles]
         [1.0, 2.0, 5.0]
 
         """
-
         if sample_weight is None:
             sample_weight = np.ones(len(values))
         else:
             sample_weight = np.array(sample_weight)
 
         if np.isnan(sample_weight).sum() > 0:
-            raise ValueError(f"{self.classname()}: null values in sample weights")
+            msg = f"{self.classname()}: null values in sample weights"
+            raise ValueError(msg)
 
         if np.isinf(sample_weight).sum() > 0:
-            raise ValueError(f"{self.classname()}: infinite values in sample weights")
+            msg = f"{self.classname()}: infinite values in sample weights"
+            raise ValueError(msg)
 
         if (sample_weight < 0).sum() > 0:
-            raise ValueError(f"{self.classname()}: negative weights in sample weights")
+            msg = f"{self.classname()}: negative weights in sample weights"
+            raise ValueError(msg)
 
         if sample_weight.sum() <= 0:
-            raise ValueError(
-                f"{self.classname()}: total sample weights are not greater than 0"
-            )
+            msg = f"{self.classname()}: total sample weights are not greater than 0"
+            raise ValueError(msg)
 
         values = np.array(values)
         quantiles = np.array(quantiles)
 
         nan_filter = ~np.isnan(values)
         values = values[nan_filter]
         sample_weight = sample_weight[nan_filter]
@@ -355,17 +321,15 @@
         sorter = np.argsort(values, kind="stable")
         values = values[sorter]
         sample_weight = sample_weight[sorter]
 
         weighted_quantiles = np.cumsum(sample_weight)
         weighted_quantiles = weighted_quantiles / np.sum(sample_weight)
 
-        interp_quantiles = list(np.interp(quantiles, weighted_quantiles, values))
-
-        return interp_quantiles
+        return list(np.interp(quantiles, weighted_quantiles, values))
 
     def transform(self, X):
         """Apply capping to columns in X.
 
         If cap_value_max is set, any values above cap_value_max will be set to cap_value_max. If cap_value_min
         is set any values below cap_value_min will be set to cap_value_min. Only works or numeric columns.
 
@@ -376,60 +340,51 @@
 
         Returns
         -------
         X : pd.DataFrame
             Transformed input X with min and max capping applied to the specified columns.
 
         """
-
         self.check_is_fitted(["capping_values"])
         self.check_is_fitted(["_replacement_values"])
 
         if self.capping_values == {}:
-
-            raise ValueError(
-                f"{self.classname()}: capping_values attribute is an empty dict - perhaps the fit method has not been run yet"
-            )
+            msg = f"{self.classname()}: capping_values attribute is an empty dict - perhaps the fit method has not been run yet"
+            raise ValueError(msg)
 
         if self._replacement_values == {}:
-
-            raise ValueError(
-                f"{self.classname()}: _replacement_values attribute is an empty dict - perhaps the fit method has not been run yet"
-            )
+            msg = f"{self.classname()}: _replacement_values attribute is an empty dict - perhaps the fit method has not been run yet"
+            raise ValueError(msg)
 
         X = super().transform(X)
 
         numeric_column_types = X[self.columns].apply(
-            pd.api.types.is_numeric_dtype, axis=0
+            pd.api.types.is_numeric_dtype,
+            axis=0,
         )
 
         if not numeric_column_types.all():
-
             non_numeric_columns = list(
-                numeric_column_types.loc[~numeric_column_types].index
+                numeric_column_types.loc[~numeric_column_types].index,
             )
 
-            raise TypeError(
-                f"{self.classname()}: The following columns are not numeric in X; {non_numeric_columns}"
-            )
+            msg = f"{self.classname()}: The following columns are not numeric in X; {non_numeric_columns}"
+            raise TypeError(msg)
 
         for col in self.columns:
-
             cap_value_min = self.capping_values[col][0]
             cap_value_max = self.capping_values[col][1]
 
             replacement_min = self._replacement_values[col][0]
             replacement_max = self._replacement_values[col][1]
 
             if cap_value_min is not None:
-
                 X.loc[X[col] < cap_value_min, col] = replacement_min
 
             if cap_value_max is not None:
-
                 X.loc[X[col] > cap_value_max, col] = replacement_max
 
         return X
 
 
 class OutOfRangeNullTransformer(CappingTransformer):
     """Transformer to set values outside of a range to null.
@@ -479,17 +434,20 @@
 
     _replacement_values : dict
         Replacement values when capping is applied. This will contain nulls for each column.
 
     """
 
     def __init__(
-        self, capping_values=None, quantiles=None, weights_column=None, **kwargs
-    ):
-
+        self,
+        capping_values=None,
+        quantiles=None,
+        weights_column=None,
+        **kwargs,
+    ) -> None:
         super().__init__(
             capping_values=capping_values,
             quantiles=quantiles,
             weights_column=weights_column,
             **kwargs,
         )
 
@@ -497,17 +455,15 @@
 
     def set_replacement_values(self):
         """Method to set the _replacement_values to have all null values.
 
         Keeps the existing keys in the _replacement_values dict and sets all values (except None) in the lists to np.NaN. Any None
         values remain in place.
         """
-
         for k, replacements_list in self._replacement_values.items():
-
             null_replacements_list = [
                 np.NaN if replace_value is not None else None
                 for replace_value in replacements_list
             ]
 
             self._replacement_values[k] = null_replacements_list
 
@@ -523,13 +479,12 @@
         X : pd.DataFrame
             A dataframe with required columns to be capped.
 
         y : None
             Required for pipeline.
 
         """
-
         super().fit(X=X, y=y)
 
         self.set_replacement_values()
 
         return self
```

### Comparing `tubular-0.3.7/tubular/comparison.py` & `tubular-0.3.8/tubular/comparison.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from tubular.base import BaseTransformer
 import pandas as pd
 
+from tubular.base import BaseTransformer
+
 
 class EqualityChecker(BaseTransformer):
-
     """Transformer to check if two columns are equal.
 
     Parameters
     ----------
     columns: list
         List containing names of the two columns to check.
 
@@ -19,38 +19,42 @@
 
     **kwargs:
         Arbitrary keyword arguments passed onto BaseTransformer.init method.
 
     """
 
     def __init__(
-        self, columns: list, new_col_name: str, drop_original: bool = False, **kwargs
+        self,
+        columns: list,
+        new_col_name: str,
+        drop_original: bool = False,
+        **kwargs,
     ) -> None:
-
         super().__init__(columns=columns, **kwargs)
 
         if not (isinstance(columns, list)):
-            raise TypeError(f"{self.classname()}: columns should be list")
+            msg = f"{self.classname()}: columns should be list"
+            raise TypeError(msg)
 
         if len(columns) != 2:
-            raise ValueError(
-                f"{self.classname()}: This transformer works with two columns only"
-            )
+            msg = f"{self.classname()}: This transformer works with two columns only"
+            raise ValueError(msg)
 
         if not (isinstance(new_col_name, str)):
-            raise TypeError(f"{self.classname()}: new_col_name should be str")
+            msg = f"{self.classname()}: new_col_name should be str"
+            raise TypeError(msg)
 
         if not (isinstance(drop_original, bool)):
-            raise TypeError(f"{self.classname()}: drop_original should be bool")
+            msg = f"{self.classname()}: drop_original should be bool"
+            raise TypeError(msg)
 
         self.new_col_name = new_col_name
         self.drop_original = drop_original
 
     def transform(self, X: pd.DataFrame) -> pd.DataFrame:
-
         """Create a column which is populated by the boolean
         matching between two columns iterated over rows.
 
         Parameters
         ----------
         X : pd.DataFrame
             Data to apply mappings to.
@@ -62,11 +66,10 @@
 
         """
         X = super().transform(X)
 
         X[self.new_col_name] = X[self.columns[0]] == X[self.columns[1]]
 
         if self.drop_original:
-
-            X.drop(self.columns, axis=1, inplace=True)
+            X = X.drop(self.columns, axis=1)
 
         return X
```

### Comparing `tubular-0.3.7/tubular/dates.py` & `tubular-0.3.8/tubular/dates.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-"""
-This module contains a transformer that applies capping to numeric columns.
-"""
+"""This module contains a transformer that applies capping to numeric columns."""
 
 import datetime
 import warnings
+from typing import List, Union
+
 import numpy as np
 import pandas as pd
 
-from typing import Union, List
-
 from tubular.base import BaseTransformer
 
 
 class DateDiffLeapYearTransformer(BaseTransformer):
     """Transformer to calculate the number of years between two dates.
 
     Parameters
@@ -61,32 +59,36 @@
         self,
         column_lower,
         column_upper,
         new_column_name,
         drop_cols,
         missing_replacement=None,
         **kwargs,
-    ):
+    ) -> None:
         if not isinstance(column_lower, str):
-            raise TypeError(f"{self.classname()}: column_lower should be a str")
+            msg = f"{self.classname()}: column_lower should be a str"
+            raise TypeError(msg)
 
         if not isinstance(column_upper, str):
-            raise TypeError(f"{self.classname()}: column_upper should be a str")
+            msg = f"{self.classname()}: column_upper should be a str"
+            raise TypeError(msg)
 
         if not isinstance(new_column_name, str):
-            raise TypeError(f"{self.classname()}: new_column_name should be a str")
+            msg = f"{self.classname()}: new_column_name should be a str"
+            raise TypeError(msg)
 
         if not isinstance(drop_cols, bool):
-            raise TypeError(f"{self.classname()}: drop_cols should be a bool")
+            msg = f"{self.classname()}: drop_cols should be a bool"
+            raise TypeError(msg)
 
-        if missing_replacement:
-            if not type(missing_replacement) in [int, float, str]:
-                raise TypeError(
-                    f"{self.classname()}: if not None, missing_replacement should be an int, float or string"
-                )
+        if (missing_replacement) and (
+            type(missing_replacement) not in [int, float, str]
+        ):
+            msg = f"{self.classname()}: if not None, missing_replacement should be an int, float or string"
+            raise TypeError(msg)
 
         super().__init__(columns=[column_lower, column_upper], **kwargs)
 
         self.new_column_name = new_column_name
         self.drop_cols = drop_cols
         self.missing_replacement = missing_replacement
 
@@ -108,48 +110,44 @@
 
         Returns
         -------
         age : int
             Year gap between the upper and lower date values passes.
 
         """
-
         if not isinstance(row, pd.Series):
-            raise TypeError(f"{self.classname()}: row should be a pd.Series")
+            msg = f"{self.classname()}: row should be a pd.Series"
+            raise TypeError(msg)
 
-        if (pd.isnull(row[self.columns[0]])) or (pd.isnull(row[self.columns[1]])):
+        if (pd.isna(row[self.columns[0]])) or (pd.isna(row[self.columns[1]])):
             return self.missing_replacement
 
-        else:
-            if not type(row[self.columns[1]]) in [datetime.date, datetime.datetime]:
-                raise TypeError(
-                    f"{self.classname()}: upper column values should be datetime.datetime or datetime.date objects"
-                )
-
-            if not type(row[self.columns[0]]) in [datetime.date, datetime.datetime]:
-                raise TypeError(
-                    f"{self.classname()}: lower column values should be datetime.datetime or datetime.date objects"
-                )
-
-            age = row[self.columns[1]].year - row[self.columns[0]].year
-
-            if age > 0:
-                if (row[self.columns[1]].month, row[self.columns[1]].day) < (
-                    row[self.columns[0]].month,
-                    row[self.columns[0]].day,
-                ):
-                    age += -1
-            elif age < 0:
-                if (row[self.columns[1]].month, row[self.columns[1]].day) > (
-                    row[self.columns[0]].month,
-                    row[self.columns[0]].day,
-                ):
-                    age += 1
+        if type(row[self.columns[1]]) not in [datetime.date, datetime.datetime]:
+            msg = f"{self.classname()}: upper column values should be datetime.datetime or datetime.date objects"
+            raise TypeError(msg)
+
+        if type(row[self.columns[0]]) not in [datetime.date, datetime.datetime]:
+            msg = f"{self.classname()}: lower column values should be datetime.datetime or datetime.date objects"
+            raise TypeError(msg)
+
+        age = row[self.columns[1]].year - row[self.columns[0]].year
+
+        if age > 0:
+            if (row[self.columns[1]].month, row[self.columns[1]].day) < (
+                row[self.columns[0]].month,
+                row[self.columns[0]].day,
+            ):
+                age += -1
+        elif age < 0 and (row[self.columns[1]].month, row[self.columns[1]].day) > (
+            row[self.columns[0]].month,
+            row[self.columns[0]].day,
+        ):
+            age += 1
 
-            return age
+        return age
 
     def transform(self, X):
         """Calculate year gap between the two provided columns.
 
         New column is created under the 'new_column_name', and optionally removes the
         old date columns.
 
@@ -160,21 +158,20 @@
 
         Returns
         -------
         X : pd.DataFrame
             Transformed data with new_column_name column.
 
         """
-
         X = super().transform(X)
 
         X[self.new_column_name] = X.apply(lambda x: self.calculate_age(x), axis=1)
 
         if self.drop_cols:
-            X.drop(self.columns, axis=1, inplace=True)
+            X = X.drop(self.columns, axis=1)
 
         return X
 
 
 class DateDifferenceTransformer(BaseTransformer):
     """Class to transform calculate the difference between 2 date fields in specified units.
 
@@ -198,49 +195,52 @@
         self,
         column_lower,
         column_upper,
         new_column_name=None,
         units="D",
         copy=True,
         verbose=False,
-    ):
-        if not type(column_lower) is str:
-            raise TypeError(f"{self.classname()}: column_lower must be a str")
+    ) -> None:
+        if type(column_lower) is not str:
+            msg = f"{self.classname()}: column_lower must be a str"
+            raise TypeError(msg)
 
-        if not type(column_upper) is str:
-            raise TypeError(f"{self.classname()}: column_upper must be a str")
+        if type(column_upper) is not str:
+            msg = f"{self.classname()}: column_upper must be a str"
+            raise TypeError(msg)
 
         columns = [column_lower, column_upper]
 
         accepted_values_units = [
             "Y",
             "M",
             "D",
             "h",
             "m",
             "s",
         ]
 
-        if not type(units) is str:
-            raise TypeError(f"{self.classname()}: units must be a str")
+        if type(units) is not str:
+            msg = f"{self.classname()}: units must be a str"
+            raise TypeError(msg)
 
         if units not in accepted_values_units:
-            raise ValueError(
-                f"{self.classname()}: units must be one of {accepted_values_units}, got {units}"
-            )
+            msg = f"{self.classname()}: units must be one of {accepted_values_units}, got {units}"
+            raise ValueError(msg)
         if units in ["Y", "M"]:
             warnings.warn(
-                f"{self.classname()}: Y/M units will be changed or deprecated in a future version, consider using DateDiffLeapYearTransformer or D units instead"
+                f"{self.classname()}: Y/M units will be changed or deprecated in a future version, consider using DateDiffLeapYearTransformer or D units instead",
             )
 
         self.units = units
 
         if new_column_name is not None:
-            if not type(new_column_name) is str:
-                raise TypeError(f"{self.classname()}: new_column_name must be a str")
+            if type(new_column_name) is not str:
+                msg = f"{self.classname()}: new_column_name must be a str"
+                raise TypeError(msg)
 
             self.new_column_name = new_column_name
 
         else:
             self.new_column_name = f"{column_upper}_{column_lower}_datediff_{units}"
 
         super().__init__(columns=columns, copy=copy, verbose=verbose)
@@ -255,15 +255,14 @@
 
         Parameters
         ----------
         X : pd.DataFrame
             Data to transform.
 
         """
-
         X = super().transform(X)
 
         X[self.new_column_name] = (
             X[self.columns[1]] - X[self.columns[0]]
         ) / np.timedelta64(1, self.units)
 
         return X
@@ -286,34 +285,37 @@
         A dictionary of keyword arguments to be passed to the pd.to_datetime method when it is called in transform.
 
     **kwargs
         Arbitrary keyword arguments passed onto pd.to_datetime().
 
     """
 
-    def __init__(self, column, new_column_name, to_datetime_kwargs={}, **kwargs):
-        if not type(column) is str:
-            raise TypeError(
-                f"{self.classname()}: column should be a single str giving the column to transform to datetime"
-            )
-
-        if not type(new_column_name) is str:
-            raise TypeError(f"{self.classname()}: new_column_name must be a str")
+    def __init__(
+        self,
+        column,
+        new_column_name,
+        to_datetime_kwargs={},
+        **kwargs,
+    ) -> None:
+        if type(column) is not str:
+            msg = f"{self.classname()}: column should be a single str giving the column to transform to datetime"
+            raise TypeError(msg)
 
-        if not type(to_datetime_kwargs) is dict:
-            raise TypeError(
-                f"{self.classname()}: to_datetime_kwargs should be a dict but got type {type(to_datetime_kwargs)}"
-            )
+        if type(new_column_name) is not str:
+            msg = f"{self.classname()}: new_column_name must be a str"
+            raise TypeError(msg)
 
-        else:
-            for i, k in enumerate(to_datetime_kwargs.keys()):
-                if not type(k) is str:
-                    raise TypeError(
-                        f"{self.classname()}: unexpected type ({type(k)}) for to_datetime_kwargs key in position {i}, must be str"
-                    )
+        if type(to_datetime_kwargs) is not dict:
+            msg = f"{self.classname()}: to_datetime_kwargs should be a dict but got type {type(to_datetime_kwargs)}"
+            raise TypeError(msg)
+
+        for i, k in enumerate(to_datetime_kwargs.keys()):
+            if type(k) is not str:
+                msg = f"{self.classname()}: unexpected type ({type(k)}) for to_datetime_kwargs key in position {i}, must be str"
+                raise TypeError(msg)
 
         self.to_datetime_kwargs = to_datetime_kwargs
         self.new_column_name = new_column_name
 
         # This attribute is not for use in any method, use 'columns' instead.
         # Here only as a fix to allow string representation of transformer.
         self.column = column
@@ -325,19 +327,19 @@
 
         Parameters
         ----------
         X : pd.DataFrame
             Data with column to transform.
 
         """
-
         X = super().transform(X)
 
         X[self.new_column_name] = pd.to_datetime(
-            X[self.columns[0]], **self.to_datetime_kwargs
+            X[self.columns[0]],
+            **self.to_datetime_kwargs,
         )
 
         return X
 
 
 class SeriesDtMethodTransformer(BaseTransformer):
     """Tranformer that applies a pandas.Series.dt method.
@@ -390,57 +392,55 @@
 
     pd_method_kwargs : dict
         Dictionary of keyword arguments to call the pd.Series.dt method with.
 
     """
 
     def __init__(
-        self, new_column_name, pd_method_name, column, pd_method_kwargs={}, **kwargs
-    ):
+        self,
+        new_column_name,
+        pd_method_name,
+        column,
+        pd_method_kwargs={},
+        **kwargs,
+    ) -> None:
         if type(column) is not str:
-            raise TypeError(
-                f"{self.classname()}: column should be a str but got {type(column)}"
-            )
+            msg = f"{self.classname()}: column should be a str but got {type(column)}"
+            raise TypeError(msg)
 
         super().__init__(columns=column, **kwargs)
 
         if type(new_column_name) is not str:
-            raise TypeError(
-                f"{self.classname()}: unexpected type ({type(new_column_name)}) for new_column_name, must be str"
-            )
+            msg = f"{self.classname()}: unexpected type ({type(new_column_name)}) for new_column_name, must be str"
+            raise TypeError(msg)
 
         if type(pd_method_name) is not str:
-            raise TypeError(
-                f"{self.classname()}: unexpected type ({type(pd_method_name)}) for pd_method_name, expecting str"
-            )
+            msg = f"{self.classname()}: unexpected type ({type(pd_method_name)}) for pd_method_name, expecting str"
+            raise TypeError(msg)
 
         if type(pd_method_kwargs) is not dict:
-            raise TypeError(
-                f"{self.classname()}: pd_method_kwargs should be a dict but got type {type(pd_method_kwargs)}"
-            )
+            msg = f"{self.classname()}: pd_method_kwargs should be a dict but got type {type(pd_method_kwargs)}"
+            raise TypeError(msg)
 
-        else:
-            for i, k in enumerate(pd_method_kwargs.keys()):
-                if not type(k) is str:
-                    raise TypeError(
-                        f"{self.classname()}: unexpected type ({type(k)}) for pd_method_kwargs key in position {i}, must be str"
-                    )
+        for i, k in enumerate(pd_method_kwargs.keys()):
+            if type(k) is not str:
+                msg = f"{self.classname()}: unexpected type ({type(k)}) for pd_method_kwargs key in position {i}, must be str"
+                raise TypeError(msg)
 
         self.new_column_name = new_column_name
         self.pd_method_name = pd_method_name
         self.pd_method_kwargs = pd_method_kwargs
 
         try:
             ser = pd.Series([datetime.datetime(2020, 12, 21)])
             getattr(ser.dt, pd_method_name)
 
         except Exception as err:
-            raise AttributeError(
-                f"""{self.classname()}: error accessing "dt.{pd_method_name}" method on pd.Series object - pd_method_name should be a pd.Series.dt method"""
-            ) from err
+            msg = f'{self.classname()}: error accessing "dt.{pd_method_name}" method on pd.Series object - pd_method_name should be a pd.Series.dt method'
+            raise AttributeError(msg) from err
 
         if callable(getattr(ser.dt, pd_method_name)):
             self._callable = True
 
         else:
             self._callable = False
 
@@ -463,25 +463,26 @@
         Returns
         -------
         X : pd.DataFrame
             Input X with additional column (self.new_column_name) added. These contain the output of
             running the pd.Series.dt method.
 
         """
-
         X = super().transform(X)
 
         if self._callable:
             X[self.new_column_name] = getattr(
-                X[self.columns[0]].dt, self.pd_method_name
+                X[self.columns[0]].dt,
+                self.pd_method_name,
             )(**self.pd_method_kwargs)
 
         else:
             X[self.new_column_name] = getattr(
-                X[self.columns[0]].dt, self.pd_method_name
+                X[self.columns[0]].dt,
+                self.pd_method_name,
             )
 
         return X
 
 
 class BetweenDatesTransformer(BaseTransformer):
     """Transformer to generate a boolean column indicating if one date is between two others.
@@ -548,47 +549,53 @@
         column_lower,
         column_between,
         column_upper,
         new_column_name,
         lower_inclusive=True,
         upper_inclusive=True,
         **kwargs,
-    ):
+    ) -> None:
         if type(column_lower) is not str:
-            raise TypeError(f"{self.classname()}: column_lower should be str")
+            msg = f"{self.classname()}: column_lower should be str"
+            raise TypeError(msg)
 
         if type(column_between) is not str:
-            raise TypeError(f"{self.classname()}: column_between should be str")
+            msg = f"{self.classname()}: column_between should be str"
+            raise TypeError(msg)
 
         if type(column_upper) is not str:
-            raise TypeError(f"{self.classname()}: column_upper should be str")
+            msg = f"{self.classname()}: column_upper should be str"
+            raise TypeError(msg)
 
         if type(new_column_name) is not str:
-            raise TypeError(f"{self.classname()}: new_column_name should be str")
+            msg = f"{self.classname()}: new_column_name should be str"
+            raise TypeError(msg)
 
         if type(lower_inclusive) is not bool:
-            raise TypeError(f"{self.classname()}: lower_inclusive should be a bool")
+            msg = f"{self.classname()}: lower_inclusive should be a bool"
+            raise TypeError(msg)
 
         if type(upper_inclusive) is not bool:
-            raise TypeError(f"{self.classname()}: upper_inclusive should be a bool")
+            msg = f"{self.classname()}: upper_inclusive should be a bool"
+            raise TypeError(msg)
 
         self.new_column_name = new_column_name
         self.lower_inclusive = lower_inclusive
         self.upper_inclusive = upper_inclusive
 
         super().__init__(columns=[column_lower, column_between, column_upper], **kwargs)
 
         # This attribute is not for use in any method, use 'columns' instead.
         # Here only as a fix to allow string representation of transformer.
         self.column_lower = column_lower
         self.column_upper = column_upper
         self.column_between = column_between
 
     def transform(self, X):
-        """Transform - creates column indicating if middle date is between the other two
+        """Transform - creates column indicating if middle date is between the other two.
 
         If not all column_lower values are less than or equal to column_upper when transform is run
         then a warning will be raised.
 
         Parameters
         ----------
         X : pd.DataFrame
@@ -597,26 +604,24 @@
         Returns
         -------
         X : pd.DataFrame
             Input X with additional column (self.new_column_name) added. This column is
             boolean and indicates if the middle column is between the other 2.
 
         """
-
         X = super().transform(X)
 
         for col in self.columns:
             if not pd.api.types.is_datetime64_dtype(X[col]):
-                raise TypeError(
-                    f"{self.classname()}: {col} should be datetime64[ns] type but got {X[col].dtype}"
-                )
+                msg = f"{self.classname()}: {col} should be datetime64[ns] type but got {X[col].dtype}"
+                raise TypeError(msg)
 
         if not (X[self.columns[0]] <= X[self.columns[2]]).all():
             warnings.warn(
-                f"{self.classname()}: not all {self.columns[2]} are greater than or equal to {self.columns[0]}"
+                f"{self.classname()}: not all {self.columns[2]} are greater than or equal to {self.columns[0]}",
             )
 
         if self.lower_inclusive:
             lower_comparison = X[self.columns[0]] <= X[self.columns[1]]
 
         else:
             lower_comparison = X[self.columns[0]] < X[self.columns[1]]
@@ -629,15 +634,15 @@
 
         X[self.new_column_name] = lower_comparison & upper_comparison
 
         return X
 
 
 class DatetimeInfoExtractor(BaseTransformer):
-    """Transformer to extract various features from datetime var
+    """Transformer to extract various features from datetime var.
 
     Parameters
     ----------
     columns : str or list
         datetime columns to extract information from
 
     include : list of str, default = ["timeofday", "timeofmonth", "timeofyear", "dayofweek"]
@@ -703,44 +708,43 @@
 
     def __init__(
         self,
         columns,
         include=["timeofday", "timeofmonth", "timeofyear", "dayofweek"],
         datetime_mappings={},
         **kwargs,
-    ):
-        if not type(include) is list:
-            raise TypeError(f"{self.classname()}: include should be List")
-
-        if not type(datetime_mappings) is dict:
-            raise TypeError(f"{self.classname()}: datetime_mappings should be Dict")
+    ) -> None:
+        if type(include) is not list:
+            msg = f"{self.classname()}: include should be List"
+            raise TypeError(msg)
+
+        if type(datetime_mappings) is not dict:
+            msg = f"{self.classname()}: datetime_mappings should be Dict"
+            raise TypeError(msg)
 
         super().__init__(columns=columns, **kwargs)
 
         for var in include:
             if var not in [
                 "timeofday",
                 "timeofmonth",
                 "timeofyear",
                 "dayofweek",
             ]:
-                raise ValueError(
-                    f'{self.classname()}: elements in include should be in ["timeofday", "timeofmonth", "timeofyear", "dayofweek"]'
-                )
+                msg = f'{self.classname()}: elements in include should be in ["timeofday", "timeofmonth", "timeofyear", "dayofweek"]'
+                raise ValueError(msg)
 
         if datetime_mappings != {}:
             for key, mapping in datetime_mappings.items():
-                if not type(mapping) is dict:
-                    raise TypeError(
-                        f"{self.classname()}: values in datetime_mappings should be dict"
-                    )
+                if type(mapping) is not dict:
+                    msg = f"{self.classname()}: values in datetime_mappings should be dict"
+                    raise TypeError(msg)
                 if key not in include:
-                    raise ValueError(
-                        f"{self.classname()}: keys in datetime_mappings should be in include"
-                    )
+                    msg = f"{self.classname()}: keys in datetime_mappings should be in include"
+                    raise ValueError(msg)
 
         self.include = include
         self.datetime_mappings = datetime_mappings
         self.mappings_provided = self.datetime_mappings.keys()
 
         # Select correct mapping either from default or user input
 
@@ -789,69 +793,55 @@
         # Invert dictionaries for quicker lookup
 
         if "timeofday" in include:
             self.timeofday_mapping = {
                 vi: k for k, v in timeofday_mapping.items() for vi in v
             }
             if set(self.timeofday_mapping.keys()) != set(range(24)):
-                raise ValueError(
-                    "{}: timeofday mapping dictionary should contain mapping for all hours between 0-23. {} are missing".format(
-                        self.classname(),
-                        set(range(24)) - set(self.timeofday_mapping.keys()),
-                    )
-                )
+                msg = f"{self.classname()}: timeofday mapping dictionary should contain mapping for all hours between 0-23. {set(range(24)) - set(self.timeofday_mapping.keys())} are missing"
+                raise ValueError(msg)
+
             # Check if all hours in dictionary
         else:
             self.timeofday_mapping = {}
 
         if "timeofmonth" in include:
             self.timeofmonth_mapping = {
                 vi: k for k, v in timeofmonth_mapping.items() for vi in v
             }
             if set(self.timeofmonth_mapping.keys()) != set(range(32)):
-                raise ValueError(
-                    "{}: timeofmonth mapping dictionary should contain mapping for all days between 1-31. {} are missing".format(
-                        self.classname(),
-                        set(range(1, 32)) - set(self.timeofmonth_mapping.keys()),
-                    )
-                )
+                msg = f"{self.classname()}: timeofmonth mapping dictionary should contain mapping for all days between 1-31. {set(range(1, 32)) - set(self.timeofmonth_mapping.keys())} are missing"
+                raise ValueError(msg)
         else:
             self.timeofmonth_mapping = {}
 
         if "timeofyear" in include:
             self.timeofyear_mapping = {
                 vi: k for k, v in timeofyear_mapping.items() for vi in v
             }
             if set(self.timeofyear_mapping.keys()) != set(range(1, 13)):
-                raise ValueError(
-                    "{}: timeofyear mapping dictionary should contain mapping for all months between 1-12. {} are missing".format(
-                        self.classname(),
-                        set(range(1, 13)) - set(self.timeofyear_mapping.keys()),
-                    )
-                )
+                msg = f"{self.classname()}: timeofyear mapping dictionary should contain mapping for all months between 1-12. {set(range(1, 13)) - set(self.timeofyear_mapping.keys())} are missing"
+                raise ValueError(msg)
+
         else:
             self.timeofyear_mapping = {}
 
         if "dayofweek" in include:
             self.dayofweek_mapping = {
                 vi: k for k, v in dayofweek_mapping.items() for vi in v
             }
             if set(self.dayofweek_mapping.keys()) != set(range(7)):
-                raise ValueError(
-                    "{}: dayofweek mapping dictionary should contain mapping for all days between 0-6. {} are missing".format(
-                        self.classname(),
-                        set(range(7)) - set(self.dayofweek_mapping.keys()),
-                    )
-                )
+                msg = f"{self.classname()}: dayofweek mapping dictionary should contain mapping for all days between 0-6. {set(range(7)) - set(self.dayofweek_mapping.keys())} are missing"
+                raise ValueError(msg)
+
         else:
             self.dayofweek_mapping = {}
 
     def _map_values(self, value, interval: str):
-        """
-        Method to apply mappings for a specified interval ("timeofday", "timeofmonth", "timeofyear" or "dayofweek")
+        """Method to apply mappings for a specified interval ("timeofday", "timeofmonth", "timeofyear" or "dayofweek")
         from corresponding mapping attribute to a single value.
 
         Parameters
         ----------
         interval : str
             the time period to map "timeofday", "timeofmonth", "timeofyear" or "dayofweek"
 
@@ -860,18 +850,17 @@
 
 
         Returns
         -------
         str : str
             Mapped value
         """
-
-        if not type(value) is float:
-            if not type(value) is int:
-                raise TypeError(f"{self.classname()}: value should be float or int")
+        if type(value) is not float and type(value) is not int:
+            msg = f"{self.classname()}: value should be float or int"
+            raise TypeError(msg)
 
         errors = {
             "timeofday": "0-23",
             "dayofweek": "0-6",
             "timeofmonth": "1-31",
             "timeofyear": "1-12",
         }
@@ -884,78 +873,78 @@
         mappings = {
             "timeofday": self.timeofday_mapping,
             "dayofweek": self.dayofweek_mapping,
             "timeofmonth": self.timeofmonth_mapping,
             "timeofyear": self.timeofyear_mapping,
         }
 
-        if not np.isnan(value):
-            if value not in np.arange(*ranges[interval]):
-                raise ValueError(
-                    f"{self.classname()}: value for {interval} mapping  in self._map_values should be an integer value in {errors[interval]}"
-                )
+        if (not np.isnan(value)) and (value not in np.arange(*ranges[interval])):
+            msg = f"{self.classname()}: value for {interval} mapping  in self._map_values should be an integer value in {errors[interval]}"
+            raise ValueError(msg)
 
         if np.isnan(value):
             return np.nan
-        else:
-            return mappings[interval][value]
+
+        return mappings[interval][value]
 
     def transform(self, X):
-        """Transform - Extracts new features from datetime variables
+        """Transform - Extracts new features from datetime variables.
 
         Parameters
         ----------
         X : pd.DataFrame
             Data with columns to extract info from.
 
         Returns
         -------
         X : pd.DataFrame
             Transformed input X with added columns of extracted information.
         """
-
         X = super().transform(X)
 
         for col in self.columns:
-            if not X[col].dtype.name == "datetime64[ns]":
+            if X[col].dtype.name != "datetime64[ns]":
                 try:
                     X[col] = X[col].dt.tz_localize(None)
                 except AttributeError:
-                    raise TypeError(
+                    msg = (
                         f"{self.classname()}: values in {col} should be datetime64[ns]"
                     )
+                    raise TypeError(msg)
 
         for col in self.columns:
             if "timeofday" in self.include:
                 X[col + "_timeofday"] = X[col].dt.hour.apply(
-                    self._map_values, interval="timeofday"
+                    self._map_values,
+                    interval="timeofday",
                 )
 
             if "timeofmonth" in self.include:
                 X[col + "_timeofmonth"] = X[col].dt.day.apply(
-                    self._map_values, interval="timeofmonth"
+                    self._map_values,
+                    interval="timeofmonth",
                 )
 
             if "timeofyear" in self.include:
                 X[col + "_timeofyear"] = X[col].dt.month.apply(
-                    self._map_values, interval="timeofyear"
+                    self._map_values,
+                    interval="timeofyear",
                 )
 
             if "dayofweek" in self.include:
                 X[col + "_dayofweek"] = X[col].dt.weekday.apply(
-                    self._map_values, interval="dayofweek"
+                    self._map_values,
+                    interval="dayofweek",
                 )
 
         return X
 
 
 class DatetimeSinusoidCalculator(BaseTransformer):
-
-    """
-    Transformer to derive a feature in a dataframe by calculating the
+    """Transformer to derive a feature in a dataframe by calculating the
     sine or cosine of a datetime column in a given unit (e.g hour), with the option to scale
     period of the sine or cosine to match the natural period of the unit (e.g. 24).
 
     Parameters
     ----------
     columns : str or list
         Columns to take the sine or cosine of. Must be a datetime[64] column.
@@ -969,15 +958,15 @@
         name and units to be used for that column.
 
     period : int, float or dict, default = 2*np.pi
         The period of the output in the units specified above. To leave the period of the sinusoid output as 2 pi, specify 2*np.pi (or leave as default).
         Can be a string or a dict containing key-value pairs of column name and period to be used for that column.
 
     Attributes
-    -----------
+    ----------
     columns : str or list
         Columns to take the sine or cosine of.
 
     method : str or list
         The function to be calculated; either sin, cos or a list containing both.
 
     units : str or dict
@@ -992,132 +981,123 @@
 
     def __init__(
         self,
         columns: Union[str, List[str]],
         method: Union[str, List[str]],
         units: Union[str, dict],
         period: Union[int, float, dict, dict] = 2 * np.pi,
-    ):
+    ) -> None:
         super().__init__(columns, copy=True)
 
         if not isinstance(method, str) and not isinstance(method, list):
-            raise TypeError(
-                "{}: method must be a string or list but got {}".format(
-                    self.classname(), type(method)
-                )
+            msg = "{}: method must be a string or list but got {}".format(
+                self.classname(),
+                type(method),
             )
+            raise TypeError(msg)
 
         if not isinstance(units, str) and not isinstance(units, dict):
-            raise TypeError(
-                "{}: units must be a string or dict but got {}".format(
-                    self.classname(), type(units)
-                )
+            msg = "{}: units must be a string or dict but got {}".format(
+                self.classname(),
+                type(units),
             )
+            raise TypeError(msg)
 
         if (
             (not isinstance(period, int))
             and (not isinstance(period, float))
             and (not isinstance(period, dict))
             or (isinstance(period, bool))
         ):
-            raise TypeError(
-                "{}: period must be an int, float or dict but got {}".format(
-                    self.classname(), type(period)
-                )
+            msg = "{}: period must be an int, float or dict but got {}".format(
+                self.classname(),
+                type(period),
             )
+            raise TypeError(msg)
 
-        if isinstance(units, dict):
-            if not all(isinstance(item, str) for item in list(units.keys())) or not all(
-                isinstance(item, str) for item in list(units.values())
-            ):
-                raise TypeError(
-                    "{}: units dictionary key value pair must be strings but got keys: {} and values: {}".format(
-                        self.classname(),
-                        set(type(k) for k in units.keys()),
-                        set(type(v) for v in units.values()),
-                    )
-                )
+        if isinstance(units, dict) and (
+            not all(isinstance(item, str) for item in list(units.keys()))
+            or not all(isinstance(item, str) for item in list(units.values()))
+        ):
+            msg = "{}: units dictionary key value pair must be strings but got keys: {} and values: {}".format(
+                self.classname(),
+                {type(k) for k in units},
+                {type(v) for v in units.values()},
+            )
+            raise TypeError(msg)
 
-        if isinstance(period, dict):
-            if (
-                not all(isinstance(item, str) for item in list(period.keys()))
-                or (
-                    not all(isinstance(item, int) for item in list(period.values()))
-                    and not all(
-                        isinstance(item, float) for item in list(period.values())
-                    )
-                )
-                or any(isinstance(item, bool) for item in list(period.values()))
-            ):
-                raise TypeError(
-                    "{}: period dictionary key value pair must be str:int or str:float but got keys: {} and values: {}".format(
-                        self.classname(),
-                        set(type(k) for k in period.keys()),
-                        set(type(v) for v in period.values()),
-                    )
-                )
+        if isinstance(period, dict) and (
+            not all(isinstance(item, str) for item in list(period.keys()))
+            or (
+                not all(isinstance(item, int) for item in list(period.values()))
+                and not all(isinstance(item, float) for item in list(period.values()))
+            )
+            or any(isinstance(item, bool) for item in list(period.values()))
+        ):
+            msg = "{}: period dictionary key value pair must be str:int or str:float but got keys: {} and values: {}".format(
+                self.classname(),
+                {type(k) for k in period},
+                {type(v) for v in period.values()},
+            )
+            raise TypeError(msg)
 
         valid_method_list = ["sin", "cos"]
 
-        if isinstance(method, str):
-            method_list = [method]
-        else:
-            method_list = method
+        method_list = [method] if isinstance(method, str) else method
 
         for method in method_list:
             if method not in valid_method_list:
-                raise ValueError(
-                    '{}: Invalid method {} supplied, should be "sin", "cos" or a list containing both'.format(
-                        self.classname(), method
-                    )
+                msg = '{}: Invalid method {} supplied, should be "sin", "cos" or a list containing both'.format(
+                    self.classname(),
+                    method,
                 )
+                raise ValueError(msg)
 
         valid_unit_list = [
             "year",
             "month",
             "day",
             "hour",
             "minute",
             "second",
             "microsecond",
         ]
 
         if isinstance(units, dict):
-            if not set(list(units.values())).issubset(valid_unit_list):
-                raise ValueError(
-                    "{}: units dictionary values must be one of 'year', 'month', 'day', 'hour', 'minute', 'second', 'microsecond' but got {}".format(
-                        self.classname(), set(units.values())
-                    )
+            if not set(units.values()).issubset(valid_unit_list):
+                msg = "{}: units dictionary values must be one of 'year', 'month', 'day', 'hour', 'minute', 'second', 'microsecond' but got {}".format(
+                    self.classname(),
+                    set(units.values()),
                 )
+                raise ValueError(msg)
         elif units not in valid_unit_list:
-            raise ValueError(
-                "{}: Invalid units {} supplied, should be in {}".format(
-                    self.classname(), units, valid_unit_list
-                )
+            msg = "{}: Invalid units {} supplied, should be in {}".format(
+                self.classname(),
+                units,
+                valid_unit_list,
             )
+            raise ValueError(msg)
 
         self.method = method_list
         self.units = units
         self.period = period
 
-        if isinstance(units, dict):
-            if not sorted(list(units.keys())) == sorted(list(self.columns)):
-                raise ValueError(
-                    "{}: unit dictionary keys must be the same as columns but got {}".format(
-                        self.classname(), set(units.keys())
-                    )
-                )
+        if isinstance(units, dict) and sorted(units.keys()) != sorted(self.columns):
+            msg = "{}: unit dictionary keys must be the same as columns but got {}".format(
+                self.classname(),
+                set(units.keys()),
+            )
+            raise ValueError(msg)
 
-        if isinstance(period, dict):
-            if not sorted(list(period.keys())) == sorted(list(self.columns)):
-                raise ValueError(
-                    "{}: period dictionary keys must be the same as columns but got {}".format(
-                        self.classname(), set(period.keys())
-                    )
-                )
+        if isinstance(period, dict) and sorted(period.keys()) != sorted(self.columns):
+            msg = "{}: period dictionary keys must be the same as columns but got {}".format(
+                self.classname(),
+                set(period.keys()),
+            )
+            raise ValueError(msg)
 
     def transform(self, X: pd.DataFrame) -> pd.DataFrame:
         """Transform - creates column containing sine or cosine of another datetime column.
 
         Which function is used is stored in the self.method attribute.
 
         Parameters
@@ -1126,22 +1106,20 @@
             Data to transform.
 
         Returns
         -------
         X : pd.DataFrame
             Input X with additional columns added, these are named "<method>_<original_column>"
         """
-
         X = super().transform(X)
 
         for column in self.columns:
             if not pd.api.types.is_datetime64_dtype(X[column]):
-                raise TypeError(
-                    f"{self.classname()} : {column} should be datetime64[ns] type but got {X[column].dtype}"
-                )
+                msg = f"{self.classname()} : {column} should be datetime64[ns] type but got {X[column].dtype}"
+                raise TypeError(msg)
             if not isinstance(self.units, dict):
                 column_in_desired_unit = getattr(X[column].dt, self.units)
                 desired_units = self.units
             elif isinstance(self.units, dict):
                 column_in_desired_unit = getattr(X[column].dt, self.units[column])
                 desired_units = self.units[column]
             if not isinstance(self.period, dict):
@@ -1149,11 +1127,11 @@
             elif isinstance(self.period, dict):
                 desired_period = self.period[column]
 
             for method in self.method:
                 new_column_name = f"{method}_{desired_period}_{desired_units}_{column}"
 
                 X[new_column_name] = getattr(np, method)(
-                    column_in_desired_unit * (2.0 * np.pi / desired_period)
+                    column_in_desired_unit * (2.0 * np.pi / desired_period),
                 )
 
         return X
```

### Comparing `tubular-0.3.7/tubular/imputers.py` & `tubular-0.3.8/tubular/imputers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-"""
-This module contains transformers that deal with imputation of missing values.
-"""
+"""This module contains transformers that deal with imputation of missing values."""
 
-import pandas as pd
-import numpy as np
 import warnings
 
+import numpy as np
+import pandas as pd
 
 from tubular.base import BaseTransformer
 
 
 class BaseImputer(BaseTransformer):
     """Base imputer class containing standard transform method that will use pd.Series.fillna with the
     values in the impute_values_ attribute.
@@ -27,110 +25,103 @@
 
         Returns
         -------
         X : pd.DataFrame
             Transformed input X with nulls imputed with the median value for the specified columns.
 
         """
-
         self.check_is_fitted(["impute_values_"])
 
         X = super().transform(X)
 
         for c in self.columns:
-
             X[c] = X[c].fillna(self.impute_values_[c])
 
         return X
 
 
 class ArbitraryImputer(BaseImputer):
     """Transformer to impute null values with an arbitrary pre-defined value.
+
     Parameters
     ----------
     impute_value : int or float or str
         Value to impute nulls with.
     columns : None or str or list, default = None
         Columns to impute, if the default of None is supplied all columns in X are used
         when the transform method is called.
     **kwargs
         Arbitrary keyword arguments passed onto BaseTransformer.init method.
+
     Attributes
     ----------
     impute_value : int or float or str
         Value to impute nulls with.
     """
 
-    def __init__(self, impute_value, columns, **kwargs):
-
+    def __init__(self, impute_value, columns, **kwargs) -> None:
         if columns is None:
-
-            raise ValueError(
-                f"{self.classname()}: columns must be specified in init for ArbitraryImputer"
-            )
+            msg = f"{self.classname()}: columns must be specified in init for ArbitraryImputer"
+            raise ValueError(msg)
 
         super().__init__(columns=columns, **kwargs)
 
         if (
             not isinstance(impute_value, int)
             and not isinstance(impute_value, float)
             and not isinstance(impute_value, str)
         ):
-
-            raise ValueError(
-                f"{self.classname()}: impute_value should be a single value (int, float or str)"
-            )
+            msg = f"{self.classname()}: impute_value should be a single value (int, float or str)"
+            raise ValueError(msg)
 
         self.impute_values_ = {}
         self.impute_value = impute_value
 
     def transform(self, X):
         """Impute missing values with the supplied impute_value.
         If columns is None all columns in X will be imputed.
+
         Parameters
         ----------
         X : pd.DataFrame
             Data containing columns to impute.
+
         Returns
         -------
         X : pd.DataFrame
             Transformed input X with nulls imputed with the specified impute_value, for the specified columns.
 
         Additions
         ---------
         * Preserving the datatypes of columns
         * Finding the target column dtype and cast imputer values as same dtype
         """
-
         self.check_is_fitted(["impute_value"])
         self.columns_check(X)
 
         for c in self.columns:
-
-            if "category" in X[c].dtype.name:
-
-                if self.impute_value not in X[c].cat.categories:
-
-                    X[c] = X[c].cat.add_categories(
-                        self.impute_value
-                    )  # add new category
+            if (
+                "category" in X[c].dtype.name
+                and self.impute_value not in X[c].cat.categories
+            ):
+                X[c] = X[c].cat.add_categories(
+                    self.impute_value,
+                )  # add new category
 
             dtype = X[c].dtype  # get the dtype of column
 
             X[c] = (
                 X[c].fillna(self.impute_values_).astype(dtype)
             )  # casting imputer value as same dtype
 
             self.impute_values_[
                 c
             ] = self.impute_value  # updating impute_values_ attribute
 
-        X = super().transform(X)  # impute the values
-
-        return X
+        return super().transform(X)  # impute the values
 
 
 class MedianImputer(BaseImputer):
     """Transformer to impute missing values with the median of the supplied columns.
 
     Parameters
     ----------
@@ -148,21 +139,20 @@
     ----------
     impute_values_ : dict
         Created during fit method. Dictionary of float / int (median) values of columns
         in the columns attribute. Keys of impute_values_ give the column names.
 
     """
 
-    def __init__(self, columns=None, weight=None, **kwargs):
-
+    def __init__(self, columns=None, weight=None, **kwargs) -> None:
         super().__init__(columns=columns, **kwargs)
 
-        if not isinstance(weight, str):
-            if weight is not None:
-                raise TypeError("weight should be str or None")
+        if not isinstance(weight, str) and weight is not None:
+            msg = "weight should be str or None"
+            raise TypeError(msg)
 
         self.weight = weight
 
     def fit(self, X, y=None):
         """Calculate median values to impute with from X.
 
         Parameters
@@ -170,48 +160,43 @@
         X : pd.DataFrame
             Data to "learn" the median values from.
 
         y : None or pd.DataFrame or pd.Series, default = None
             Not required.
 
         """
-
         super().fit(X, y)
 
         self.impute_values_ = {}
 
         if self.weight is not None:
-
             super().check_weights_column(X, self.weight)
 
             temp = X.copy()
 
             for c in self.columns:
-
                 # filter out null rows so their weight doesn't influence calc
-                filtered = temp[temp[c].notnull()]
+                filtered = temp[temp[c].notna()]
 
                 # first sort df by column to be imputed (order of weight column shouldn't matter for median)
-                filtered.sort_values(c, inplace=True)
+                filtered = filtered.sort_values(c)
 
                 # next calculate cumulative weight sums
                 cumsum = filtered[self.weight].cumsum()
 
                 # find midpoint
                 cutoff = filtered[self.weight].sum() / 2.0
 
                 # find first value >= this point
                 median = filtered[c][cumsum >= cutoff].iloc[0]
 
                 self.impute_values_[c] = median
 
         else:
-
             for c in self.columns:
-
                 self.impute_values_[c] = X[c].median()
 
         return self
 
 
 class MeanImputer(BaseImputer):
     """Transformer to impute missing values with the mean of the supplied columns.
@@ -232,21 +217,20 @@
     ----------
     impute_values_ : dict
         Created during fit method. Dictionary of float / int (mean) values of columns
         in the columns attribute. Keys of impute_values_ give the column names.
 
     """
 
-    def __init__(self, columns=None, weight=None, **kwargs):
-
+    def __init__(self, columns=None, weight=None, **kwargs) -> None:
         super().__init__(columns=columns, **kwargs)
 
-        if not isinstance(weight, str):
-            if weight is not None:
-                raise TypeError("weight should be str or None")
+        if not isinstance(weight, str) and weight is not None:
+            msg = "weight should be str or None"
+            raise TypeError(msg)
 
         self.weight = weight
 
     def fit(self, X, y=None):
         """Calculate mean values to impute with from X.
 
         Parameters
@@ -254,41 +238,36 @@
         X : pd.DataFrame
             Data to "learn" the mean values from.
 
         y : None or pd.DataFrame or pd.Series, default = None
             Not required.
 
         """
-
         super().fit(X, y)
 
         self.impute_values_ = {}
 
         if self.weight is not None:
-
             super().check_weights_column(X, self.weight)
 
             for c in self.columns:
-
                 # filter out null rows so they don't count towards total weight
-                filtered = X[X[c].notnull()]
+                filtered = X[X[c].notna()]
 
                 # calculate total weight and total of weighted col
                 total_weight = filtered[self.weight].sum()
                 total_weighted_col = filtered[c].mul(filtered[self.weight]).sum()
 
                 # find weighted mean and add to dict
                 weighted_mean = total_weighted_col / total_weight
 
                 self.impute_values_[c] = weighted_mean
 
         else:
-
             for c in self.columns:
-
                 self.impute_values_[c] = X[c].mean()
 
         return self
 
 
 class ModeImputer(BaseImputer):
     """Transformer to impute missing values with the mode of the supplied columns.
@@ -312,23 +291,20 @@
     ----------
     impute_values_ : dict
         Created during fit method. Dictionary of float / int (mode) values of columns
         in the columns attribute. Keys of impute_values_ give the column names.
 
     """
 
-    def __init__(self, columns=None, weight=None, **kwargs):
-
+    def __init__(self, columns=None, weight=None, **kwargs) -> None:
         super().__init__(columns=columns, **kwargs)
 
-        if weight is not None:
-
-            if not isinstance(weight, str):
-
-                raise ValueError("ModeImputer: weight should be a string or None")
+        if weight is not None and not isinstance(weight, str):
+            msg = "ModeImputer: weight should be a string or None"
+            raise ValueError(msg)
 
         self.weight = weight
 
     def fit(self, X, y=None):
         """Calculate mode values to impute with from X.
 
         Parameters
@@ -336,41 +312,34 @@
         X : pd.DataFrame
             Data to "learn" the mode values from.
 
         y : None or pd.DataFrame or pd.Series, default = None
             Not required.
 
         """
-
         super().fit(X, y)
 
         self.impute_values_ = {}
 
         if self.weight is None:
-
             for c in self.columns:
-
                 mode_value = X[c].mode(dropna=True)
 
                 if len(mode_value) == 0:
-
                     self.impute_values_[c] = np.nan
 
                     warnings.warn(f"ModeImputer: The Mode of column {c} is NaN.")
 
                 else:
-
                     self.impute_values_[c] = mode_value[0]
 
         else:
-
             super().check_weights_column(X, self.weight)
 
             for c in self.columns:
-
                 self.impute_values_[c] = X.groupby(c)[self.weight].sum().idxmax()
 
         return self
 
 
 class NearestMeanResponseImputer(BaseImputer):
     """Class to impute missing values with; the value for which the average response is closest
@@ -380,16 +349,15 @@
     ----------
     columns : None or str or list, default = None
         Columns to impute, if the default of None is supplied all columns in X are used
         when the transform method is called.
 
     """
 
-    def __init__(self, columns=None, **kwds):
-
+    def __init__(self, columns=None, **kwds) -> None:
         super().__init__(columns=columns, **kwds)
 
     def fit(self, X, y):
         """Calculate mean values to impute with.
 
         Parameters
         ----------
@@ -398,56 +366,50 @@
 
         y : pd.Series
             Response column used to determine the value to impute with. The average response for
             each level of every column is calculated. The level which has the closest average response
             to the average response of the unknown levels is selected as the imputation value.
 
         """
-
         super().fit(X, y)
 
-        n_nulls = y.isnull().sum()
+        n_nulls = y.isna().sum()
 
         if n_nulls > 0:
-
-            raise ValueError(f"{self.classname()}: y has {n_nulls} null values")
+            msg = f"{self.classname()}: y has {n_nulls} null values"
+            raise ValueError(msg)
 
         self.impute_values_ = {}
 
         X_y = self._combine_X_y(X, y)
         response_column = "_temporary_response"
 
         for c in self.columns:
-
-            c_nulls = X[c].isnull()
+            c_nulls = X[c].isna()
 
             if c_nulls.sum() == 0:
+                msg = f"{self.classname()}: Column {c} has no missing values, cannot use this transformer."
+                raise ValueError(msg)
+
+            mean_response_by_levels = pd.DataFrame(
+                X_y.loc[~c_nulls].groupby(c)[response_column].mean(),
+            ).reset_index()
 
-                raise ValueError(
-                    f"{self.classname()}: Column {c} has no missing values, cannot use this transformer."
-                )
-
-            else:
-
-                mean_response_by_levels = pd.DataFrame(
-                    X_y.loc[~c_nulls].groupby(c)[response_column].mean()
-                ).reset_index()
-
-                mean_response_nulls = X_y.loc[c_nulls, response_column].mean()
-
-                mean_response_by_levels["abs_diff_response"] = np.abs(
-                    mean_response_by_levels[response_column] - mean_response_nulls
-                )
-
-                # take first value having the minimum difference in terms of average response
-                self.impute_values_[c] = mean_response_by_levels.loc[
-                    mean_response_by_levels["abs_diff_response"]
-                    == mean_response_by_levels["abs_diff_response"].min(),
-                    c,
-                ].values[0]
+            mean_response_nulls = X_y.loc[c_nulls, response_column].mean()
+
+            mean_response_by_levels["abs_diff_response"] = np.abs(
+                mean_response_by_levels[response_column] - mean_response_nulls,
+            )
+
+            # take first value having the minimum difference in terms of average response
+            self.impute_values_[c] = mean_response_by_levels.loc[
+                mean_response_by_levels["abs_diff_response"]
+                == mean_response_by_levels["abs_diff_response"].min(),
+                c,
+            ].to_numpy()[0]
 
         return self
 
 
 class NullIndicator(BaseTransformer):
     """Class to create a binary indicator column for null values.
 
@@ -455,28 +417,25 @@
     ----------
     columns : None or str or list, default = None
         Columns to produce indicator columns for, if the default of None is supplied all columns in X are used
         when the transform method is called.
 
     """
 
-    def __init__(self, columns=None, **kwds):
-
+    def __init__(self, columns=None, **kwds) -> None:
         super().__init__(columns=columns, **kwds)
 
     def transform(self, X):
         """Create new columns indicating the position of null values for each variable in self.columns.
 
         Parameters
         ----------
         X : pd.DataFrame
             Data to add indicators to.
 
         """
-
         X = super().transform(X)
 
         for c in self.columns:
-
-            X[f"{c}_nulls"] = X[c].isnull().astype(int)
+            X[f"{c}_nulls"] = X[c].isna().astype(int)
 
         return X
```

### Comparing `tubular-0.3.7/tubular/mapping.py` & `tubular-0.3.8/tubular/mapping.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-"""
-This module contains transformers that apply different types of mappings to columns.
-"""
+"""This module contains transformers that apply different types of mappings to columns."""
 
-import pandas as pd
-from pandas.api.types import is_categorical_dtype
-import numpy as np
-from collections import OrderedDict
 import warnings
+from collections import OrderedDict
 
+import numpy as np
+import pandas as pd
+from pandas.api.types import is_categorical_dtype
 
 from tubular.base import BaseTransformer, ReturnKeyDict
 
 
 class BaseMappingTransformer(BaseTransformer):
     """Base Transformer Extension for mapping transformers.
 
@@ -31,34 +29,29 @@
     mappings : dict
         Dictionary of mappings for each column individually. The dict passed to mappings in
         init is set to the mappings attribute.
 
     """
 
     def __init__(self, mappings, **kwargs):
-
         if isinstance(mappings, dict):
-
             if not len(mappings) > 0:
-
-                raise ValueError(f"{self.classname()}: mappings has no values")
+                msg = f"{self.classname()}: mappings has no values"
+                raise ValueError(msg)
 
             for j in mappings.values():
-
                 if not isinstance(j, dict):
-
-                    raise ValueError(
-                        f"{self.classname()}: values in mappings dictionary should be dictionaries"
-                    )
+                    msg = f"{self.classname()}: values in mappings dictionary should be dictionaries"
+                    raise ValueError(msg)
 
             self.mappings = mappings
 
         else:
-
-            raise ValueError(f"{self.classname()}: mappings must be a dictionary")
+            msg = f"{self.classname()}: mappings must be a dictionary"
+            raise ValueError(msg)
 
         columns = list(mappings.keys())
 
         super().__init__(columns=columns, **kwargs)
 
     def transform(self, X):
         """Base mapping transformer transform method.  Checks that the mappings
@@ -71,20 +64,17 @@
 
         Returns
         -------
         X : pd.DataFrame
             Input X, copied if specified by user.
 
         """
-
         self.check_is_fitted(["mappings"])
 
-        X = super().transform(X)
-
-        return X
+        return super().transform(X)
 
 
 class BaseMappingTransformMixin(BaseTransformer):
     """Mixin class to apply standard pd.Series.map transform method.
 
     Transformer uses the mappings attribute which should be a dict of dicts/mappings
     for each required column.
@@ -102,21 +92,19 @@
 
         Returns
         -------
         X : pd.DataFrame
             Transformed input X with levels mapped accoriding to mappings dict.
 
         """
-
         self.check_is_fitted(["mappings"])
 
         X = super().transform(X)
 
         for c in self.columns:
-
             X[c] = X[c].map(self.mappings[c])
 
         return X
 
 
 class MappingTransformer(BaseMappingTransformer, BaseMappingTransformMixin):
     """Transformer to map values in columns to other values e.g. to merge two levels into one.
@@ -146,26 +134,21 @@
     mappings : dict
         Dictionary of mappings for each column individually. The dict passed to mappings in
         init is set to the mappings attribute.
 
     """
 
     def __init__(self, mappings, **kwargs):
-
         for k, v in mappings.items():
-
             if isinstance(v, dict):
-
                 mappings[k] = ReturnKeyDict(v)
 
             else:
-
-                raise TypeError(
-                    f"{self.classname()}: each item in mappings should be a dict but got type {type(v)} for key {k}"
-                )
+                msg = f"{self.classname()}: each item in mappings should be a dict but got type {type(v)} for key {k}"
+                raise TypeError(msg)
 
         BaseMappingTransformer.__init__(self, mappings=mappings, **kwargs)
 
     def transform(self, X, suppress_dtype_warning=False):
         """Transform the input data X according to the mappings in the mappings attribute dict.
 
         This method calls the BaseMappingTransformMixin.transform. Note, this transform method is
@@ -195,54 +178,48 @@
             Transformed input X with levels mapped accoriding to mappings dict.
 
         """
         mapped_columns = self.mappings.keys()
         original_dtypes = X[mapped_columns].dtypes
 
         for col in mapped_columns:
-
             values_to_be_mapped = set(self.mappings[col].keys())
             values_in_df = set(X[col].unique())
 
             if len(values_to_be_mapped.intersection(values_in_df)) == 0:
-
                 warnings.warn(
-                    f"{self.classname()}: No values from mapping for {col} exist in dataframe."
+                    f"{self.classname()}: No values from mapping for {col} exist in dataframe.",
                 )
 
             if len(values_to_be_mapped.difference(values_in_df)) > 0:
-
                 warnings.warn(
-                    f"{self.classname()}: There are values in the mapping for {col} that are not present in the dataframe"
+                    f"{self.classname()}: There are values in the mapping for {col} that are not present in the dataframe",
                 )
 
         X = BaseMappingTransformMixin.transform(self, X)
 
         mapped_dtypes = X[mapped_columns].dtypes
 
         if not suppress_dtype_warning:
-
             for col in mapped_columns:
-
                 col_mappings = pd.Series(self.mappings[col])
                 mapping_dtype = col_mappings.dtype
 
-                if (mapped_dtypes[col] != mapping_dtype) and (
-                    mapped_dtypes[col] != original_dtypes[col]
-                ):
-
-                    # Confirm the initial and end dtypes are not categories
-                    if not (
+                if (
+                    (mapped_dtypes[col] != mapping_dtype)
+                    and (mapped_dtypes[col] != original_dtypes[col])
+                    and not (
                         is_categorical_dtype(original_dtypes[col])
                         and is_categorical_dtype(mapped_dtypes[col])
-                    ):
-
-                        warnings.warn(
-                            f"{self.classname()}: This mapping changes {col} dtype from {original_dtypes[col]} to {mapped_dtypes[col]}. This is often caused by having multiple dtypes in one column, or by not mapping all values."
-                        )
+                    )
+                ):
+                    # Confirm the initial and end dtypes are not categories
+                    warnings.warn(
+                        f"{self.classname()}: This mapping changes {col} dtype from {original_dtypes[col]} to {mapped_dtypes[col]}. This is often caused by having multiple dtypes in one column, or by not mapping all values.",
+                    )
 
         return X
 
 
 class CrossColumnMappingTransformer(BaseMappingTransformer):
     """Transformer to adjust values in one column based on the values of another column.
 
@@ -261,40 +238,34 @@
         to ensure reproducibility.
 
     **kwargs
         Arbitrary keyword arguments passed onto BaseTransformer.init method.
 
     Attributes
     ----------
-
     adjust_column : str
         Column containing the values to be adjusted.
 
     mappings : dict
         Dictionary of mappings for each column individually to be applied to the adjust_column.
         The dict passed to mappings in init is set to the mappings attribute.
 
 
     """
 
     def __init__(self, adjust_column, mappings, **kwargs):
-
         super().__init__(mappings=mappings, **kwargs)
 
         if not isinstance(adjust_column, str):
+            msg = f"{self.classname()}: adjust_column should be a string"
+            raise TypeError(msg)
 
-            raise TypeError(f"{self.classname()}: adjust_column should be a string")
-
-        if len(mappings) > 1:
-
-            if not isinstance(mappings, OrderedDict):
-
-                raise TypeError(
-                    f"{self.classname()}: mappings should be an ordered dict for 'replace' mappings using multiple columns"
-                )
+        if len(mappings) > 1 and not isinstance(mappings, OrderedDict):
+            msg = f"{self.classname()}: mappings should be an ordered dict for 'replace' mappings using multiple columns"
+            raise TypeError(msg)
 
         self.adjust_column = adjust_column
 
     def transform(self, X):
         """Transforms values in given column using the values provided in the adjustments dictionary.
 
         Parameters
@@ -304,31 +275,28 @@
 
         Returns
         -------
         X : pd.DataFrame
             Transformed data X with adjustments applied to specified columns.
 
         """
-
         self.check_is_fitted(["adjust_column"])
 
         X = super().transform(X)
 
-        if self.adjust_column not in X.columns.values:
-
-            raise ValueError(
-                f"{self.classname()}: variable {self.adjust_column} is not in X"
-            )
+        if self.adjust_column not in X.columns.to_numpy():
+            msg = f"{self.classname()}: variable {self.adjust_column} is not in X"
+            raise ValueError(msg)
 
         for i in self.columns:
-
-            for j in self.mappings[i].keys():
-
+            for j in self.mappings[i]:
                 X[self.adjust_column] = np.where(
-                    (X[i] == j), self.mappings[i][j], X[self.adjust_column]
+                    (X[i] == j),
+                    self.mappings[i][j],
+                    X[self.adjust_column],
                 )
 
         return X
 
 
 class CrossColumnMultiplyTransformer(BaseMappingTransformer):
     """Transformer to apply a multiplicative adjustment to values in one column based on the values of another column.
@@ -348,42 +316,36 @@
         The values within the dicts defining the multipliers must have type int or float.
 
     **kwargs
         Arbitrary keyword arguments passed onto BaseTransformer.init method.
 
     Attributes
     ----------
-
     adjust_column : str
         Column containing the values to be adjusted.
 
     mappings : dict
         Dictionary of multiplicative adjustments for each column individually to be applied to the adjust_column.
         The dict passed to mappings in init is set to the mappings attribute.
 
 
     """
 
     def __init__(self, adjust_column, mappings, **kwargs):
-
         super().__init__(mappings=mappings, **kwargs)
 
         if not isinstance(adjust_column, str):
-
-            raise TypeError(f"{self.classname()}: adjust_column should be a string")
+            msg = f"{self.classname()}: adjust_column should be a string"
+            raise TypeError(msg)
 
         for j in mappings.values():
-
             for k in j.values():
-
                 if type(k) not in [int, float]:
-
-                    raise TypeError(
-                        f"{self.classname()}: mapping values must be numeric"
-                    )
+                    msg = f"{self.classname()}: mapping values must be numeric"
+                    raise TypeError(msg)
 
         self.adjust_column = adjust_column
 
     def transform(self, X):
         """Transforms values in given column using the values provided in the adjustments dictionary.
 
         Parameters
@@ -393,35 +355,28 @@
 
         Returns
         -------
         X : pd.DataFrame
             Transformed data X with adjustments applied to specified columns.
 
         """
-
         self.check_is_fitted(["adjust_column"])
 
         X = super().transform(X)
 
-        if self.adjust_column not in X.columns.values:
-
-            raise ValueError(
-                f"{self.classname()}: variable {self.adjust_column} is not in X"
-            )
+        if self.adjust_column not in X.columns.to_numpy():
+            msg = f"{self.classname()}: variable {self.adjust_column} is not in X"
+            raise ValueError(msg)
 
         if not pd.api.types.is_numeric_dtype(X[self.adjust_column]):
-
-            raise TypeError(
-                f"{self.classname()}: variable {self.adjust_column} must have numeric dtype."
-            )
+            msg = f"{self.classname()}: variable {self.adjust_column} must have numeric dtype."
+            raise TypeError(msg)
 
         for i in self.columns:
-
-            for j in self.mappings[i].keys():
-
+            for j in self.mappings[i]:
                 X[self.adjust_column] = np.where(
                     (X[i] == j),
                     X[self.adjust_column] * self.mappings[i][j],
                     X[self.adjust_column],
                 )
 
         return X
@@ -445,42 +400,36 @@
         The values within the dicts defining the values to be added must have type int or float.
 
     **kwargs
         Arbitrary keyword arguments passed onto BaseTransformer.init method.
 
     Attributes
     ----------
-
     adjust_column : str
         Column containing the values to be adjusted.
 
     mappings : dict
         Dictionary of additive adjustments for each column individually to be applied to the adjust_column.
         The dict passed to mappings in init is set to the mappings attribute.
 
 
     """
 
     def __init__(self, adjust_column, mappings, **kwargs):
-
         super().__init__(mappings=mappings, **kwargs)
 
         if not isinstance(adjust_column, str):
-
-            raise TypeError(f"{self.classname()}: adjust_column should be a string")
+            msg = f"{self.classname()}: adjust_column should be a string"
+            raise TypeError(msg)
 
         for j in mappings.values():
-
             for k in j.values():
-
                 if type(k) not in [int, float]:
-
-                    raise TypeError(
-                        f"{self.classname()}: mapping values must be numeric"
-                    )
+                    msg = f"{self.classname()}: mapping values must be numeric"
+                    raise TypeError(msg)
 
         self.adjust_column = adjust_column
 
     def transform(self, X):
         """Transforms values in given column using the values provided in the adjustments dictionary.
 
         Parameters
@@ -490,37 +439,32 @@
 
         Returns
         -------
         X : pd.DataFrame
             Transformed data X with adjustments applied to specified columns.
 
         """
-
         self.check_is_fitted(["adjust_column"])
 
         X = super().transform(X)
 
-        if self.adjust_column not in X.columns.values:
-
+        if self.adjust_column not in X.columns.to_numpy():
             raise ValueError(
-                f"{self.classname()}: variable " + self.adjust_column + " is not in X"
+                f"{self.classname()}: variable " + self.adjust_column + " is not in X",
             )
 
         if not pd.api.types.is_numeric_dtype(X[self.adjust_column]):
-
             raise TypeError(
                 f"{self.classname()}: variable "
                 + self.adjust_column
-                + " must have numeric dtype."
+                + " must have numeric dtype.",
             )
 
         for i in self.columns:
-
-            for j in self.mappings[i].keys():
-
+            for j in self.mappings[i]:
                 X[self.adjust_column] = np.where(
                     (X[i] == j),
                     X[self.adjust_column] + self.mappings[i][j],
                     X[self.adjust_column],
                 )
 
         return X
```

### Comparing `tubular-0.3.7/tubular/misc.py` & `tubular-0.3.8/tubular/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from tubular.base import BaseTransformer
 import pandas as pd
 
+from tubular.base import BaseTransformer
+
 
 class SetValueTransformer(BaseTransformer):
     """Transformer to set value of column(s) to a given value.
 
     This should be used if columns need to be set to a constant value.
 
     Parameters
@@ -16,16 +17,15 @@
         Value to set.
 
     **kwargs
         Arbitrary keyword arguments passed onto BaseTransformer.init method.
 
     """
 
-    def __init__(self, columns, value, **kwargs):
-
+    def __init__(self, columns, value, **kwargs) -> None:
         self.value = value
 
         super().__init__(columns=columns, **kwargs)
 
     def transform(self, X):
         """Set columns to value.
 
@@ -36,54 +36,48 @@
 
         Returns
         -------
         X : pd.DataFrame
             Transformed input X with columns set to value.
 
         """
-
         X = super().transform(X)
 
         X[self.columns] = self.value
 
         return X
 
 
 class SetColumnDtype(BaseTransformer):
-    """
-    Transformer to set transform columns in a dataframe to a dtype
+    """Transformer to set transform columns in a dataframe to a dtype.
 
     Parameters
     ----------
     columns : str or list
         Columns to set dtype. Must be set or transform will not run.
 
     dtype : type or string
         dtype object to set columns to or a string interpretable as one by pd.api.types.pandas_dtype
         e.g. float or 'float'
     """
 
-    def __init__(self, columns, dtype):
-
+    def __init__(self, columns, dtype) -> None:
         super().__init__(columns, copy=True)
 
         self.__validate_dtype(dtype)
 
         self.dtype = dtype
 
     def transform(self, X):
-
         X = super().transform(X)
 
         X[self.columns] = X[self.columns].astype(self.dtype)
 
         return X
 
     def __validate_dtype(self, dtype: str):
-        """Check string is a valid dtype"""
-
+        """Check string is a valid dtype."""
         try:
             pd.api.types.pandas_dtype(dtype)
         except TypeError:
-            raise TypeError(
-                f"{self.classname()}: data type '{dtype}' not understood as a valid dtype"
-            )
+            msg = f"{self.classname()}: data type '{dtype}' not understood as a valid dtype"
+            raise TypeError(msg)
```

### Comparing `tubular-0.3.7/tubular/nominal.py` & `tubular-0.3.8/tubular/nominal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-"""
-This module contains transformers that apply encodings to nominal columns.
-"""
+"""This module contains transformers that apply encodings to nominal columns."""
 
-import pandas as pd
-import numpy as np
 import warnings
+
+import numpy as np
+import pandas as pd
 from sklearn.preprocessing import OneHotEncoder
 
 from tubular.base import BaseTransformer
 from tubular.mapping import BaseMappingTransformMixin
 
 
 class BaseNominalTransformer(BaseTransformer):
@@ -27,56 +26,47 @@
 
         Parameters
         ----------
         X : pd.DataFrame
             Data to check columns are in.
 
         """
-
         if self.columns is None:
-
             columns = [
                 c for c in X.columns if X[c].dtype.name in ["object", "category"]
             ]
 
             if not len(columns) > 0:
-
-                raise ValueError(
-                    f"{self.classname()}: no object or category columns in X"
-                )
+                msg = f"{self.classname()}: no object or category columns in X"
+                raise ValueError(msg)
 
             self.columns = columns
 
         else:
-
             self.columns_check(X)
 
     def check_mappable_rows(self, X):
         """Method to check that all the rows to apply the transformer to are able to be
         mapped according to the values in the mappings dict.
 
         Raises
         ------
         ValueError
             If any of the rows in a column (c) to be mapped, could not be mapped according to
             the mapping dict in mappings[c].
 
         """
-
         self.check_is_fitted(["mappings"])
 
         for c in self.columns:
-
-            mappable_rows = X[c].isin([k for k in self.mappings[c].keys()]).sum()
+            mappable_rows = X[c].isin(list(self.mappings[c])).sum()
 
             if mappable_rows < X.shape[0]:
-
-                raise ValueError(
-                    f"{self.classname()}: nulls would be introduced into column {c} from levels not present in mapping"
-                )
+                msg = f"{self.classname()}: nulls would be introduced into column {c} from levels not present in mapping"
+                raise ValueError(msg)
 
 
 class NominalToIntegerTransformer(BaseNominalTransformer, BaseMappingTransformMixin):
     """Transformer to convert columns containing nominal values into integer values.
 
     The nominal levels that are mapped to integers are not ordered in any way.
 
@@ -106,20 +96,19 @@
     inverse_mapping_ : dict
         Created in inverse_transform. Inverse mapping of mappings. Maps integer value back to categorical
         levels.
 
     """
 
     def __init__(self, columns=None, start_encoding=0, **kwargs):
-
         BaseNominalTransformer.__init__(self, columns=columns, **kwargs)
 
         if not isinstance(start_encoding, int):
-
-            raise ValueError(f"{self.classname()}: start_encoding should be an integer")
+            msg = f"{self.classname()}: start_encoding should be an integer"
+            raise ValueError(msg)
 
         self.start_encoding = start_encoding
 
     def fit(self, X, y=None):
         """Creates mapping between nominal levels and integer values for categorical variables.
 
         Parameters
@@ -127,21 +116,19 @@
         X : pd.DataFrame
             Data to fit the transformer on, this sets the nominal levels that can be mapped.
 
         y : None or pd.DataFrame or pd.Series, default = None
             Optional argument only required for the transformer to work with sklearn pipelines.
 
         """
-
         BaseNominalTransformer.fit(self, X, y)
 
         self.mappings = {}
 
         for c in self.columns:
-
             col_values = X[c].unique()
 
             self.mappings[c] = {
                 k: i for i, k in enumerate(col_values, self.start_encoding)
             }
 
         return self
@@ -161,20 +148,17 @@
 
         Returns
         -------
         X : pd.DataFrame
             Transformed input X with levels mapped accoriding to mappings dict.
 
         """
-
         self.check_mappable_rows(X)
 
-        X = BaseMappingTransformMixin.transform(self, X)
-
-        return X
+        return BaseMappingTransformMixin.transform(self, X)
 
     def inverse_transform(self, X):
         """Converts integer values back to categorical / nominal values. Does the inverse of the transform method.
 
         Parameters
         ----------
         X : pd.DataFrame
@@ -182,37 +166,34 @@
 
         Returns
         -------
         X : pd.DataFrame
             Transformed input X with integers mapped back to categorical levels.
 
         """
-
         X = BaseNominalTransformer.transform(self, X)
 
         self.check_is_fitted(["mappings"])
 
         self.inverse_mapping_ = {}
 
         for c in self.columns:
-
             # calculate the reverse mapping
             self.inverse_mapping_[c] = {v: k for k, v in self.mappings[c].items()}
 
             mappable_rows = (
                 X[c].isin([k for k, v in self.inverse_mapping_[c].items()]).sum()
             )
 
             X[c] = X[c].replace(self.inverse_mapping_[c])
 
             if (X.shape[0] - mappable_rows) > 0:
-
                 raise ValueError(
                     f"{self.classname()}: nulls introduced from levels not present in mapping for column: "
-                    + c
+                    + c,
                 )
 
         return X
 
 
 class GroupRareLevelsTransformer(BaseNominalTransformer):
     """Transformer to group together rare levels of nominal variables into a new level,
@@ -283,42 +264,37 @@
         columns=None,
         cut_off_percent=0.01,
         weight=None,
         rare_level_name="rare",
         record_rare_levels=True,
         **kwargs,
     ):
-
         super().__init__(columns=columns, **kwargs)
 
         if not isinstance(cut_off_percent, float):
-
-            raise ValueError(f"{self.classname()}: cut_off_percent must be a float")
+            msg = f"{self.classname()}: cut_off_percent must be a float"
+            raise ValueError(msg)
 
         if not ((cut_off_percent > 0) & (cut_off_percent < 1)):
-
-            raise ValueError(f"{self.classname()}: cut_off_percent must be > 0 and < 1")
+            msg = f"{self.classname()}: cut_off_percent must be > 0 and < 1"
+            raise ValueError(msg)
 
         self.cut_off_percent = cut_off_percent
 
-        if weight is not None:
-
-            if not isinstance(weight, str):
-
-                raise ValueError(
-                    f"{self.classname()}: weight should be a single column (str)"
-                )
+        if weight is not None and not isinstance(weight, str):
+            msg = f"{self.classname()}: weight should be a single column (str)"
+            raise ValueError(msg)
 
         self.weight = weight
 
         self.rare_level_name = rare_level_name
 
         if not isinstance(record_rare_levels, bool):
-
-            raise ValueError(f"{self.classname()}: record_rare_levels must be a bool")
+            msg = f"{self.classname()}: record_rare_levels must be a bool"
+            raise ValueError(msg)
 
         self.record_rare_levels = record_rare_levels
 
     def fit(self, X, y=None):
         """Records non-rare levels for categorical variables.
 
         When transform is called, only levels records in mapping_ during fit will remain
@@ -332,95 +308,83 @@
         X : pd.DataFrame
             Data to identify non-rare levels from.
 
         y : None or pd.DataFrame or pd.Series, default = None
             Optional argument only required for the transformer to work with sklearn pipelines.
 
         """
-
         super().fit(X, y)
 
         for c in self.columns:
-
-            if X[c].dtype.name != "category":
-
-                if pd.Series(self.rare_level_name).dtype != X[c].dtypes:
-
-                    raise ValueError(
-                        f"{self.classname()}: rare_level_name must be of the same type of the columns"
-                    )
-
-        if self.weight is not None:
-
-            if self.weight not in X.columns.values:
-
-                raise ValueError(f"{self.classname()}: weight {self.weight} not in X")
+            if (X[c].dtype.name != "category") and (
+                pd.Series(self.rare_level_name).dtype != X[c].dtypes
+            ):
+                msg = f"{self.classname()}: rare_level_name must be of the same type of the columns"
+                raise ValueError(msg)
+
+        if self.weight is not None and self.weight not in X.columns.to_numpy():
+            msg = f"{self.classname()}: weight {self.weight} not in X"
+            raise ValueError(msg)
 
         self.mapping_ = {}
 
         if self.record_rare_levels:
-
             self.rare_levels_record_ = {}
 
         if self.weight is None:
-
             for c in self.columns:
-
                 col_percents = X[c].value_counts(dropna=False) / X.shape[0]
 
                 self.mapping_[c] = list(
-                    col_percents.loc[col_percents >= self.cut_off_percent].index.values
+                    col_percents.loc[col_percents >= self.cut_off_percent].index.values,
                 )
 
                 self.mapping_[c] = sorted(self.mapping_[c], key=str)
 
                 if self.record_rare_levels:
-
                     self.rare_levels_record_[c] = list(
                         col_percents.loc[
                             col_percents < self.cut_off_percent
-                        ].index.values
+                        ].index.values,
                     )
 
                     self.rare_levels_record_[c] = sorted(
-                        self.rare_levels_record_[c], key=str
+                        self.rare_levels_record_[c],
+                        key=str,
                     )
 
         else:
-
             for c in self.columns:
-
                 cols_w_percents = X.groupby(c)[self.weight].sum()
 
                 # nulls are excluded from pandas groupby; https://github.com/pandas-dev/pandas/issues/3729
                 # so add them back in
                 if cols_w_percents.sum() < X[self.weight].sum():
-
-                    cols_w_percents[np.NaN] = X.loc[X[c].isnull(), self.weight].sum()
+                    cols_w_percents[np.NaN] = X.loc[X[c].isna(), self.weight].sum()
 
                 cols_w_percents = cols_w_percents / X[self.weight].sum()
 
                 self.mapping_[c] = list(
                     cols_w_percents.loc[
                         cols_w_percents >= self.cut_off_percent
-                    ].index.values
+                    ].index.values,
                 )
 
                 self.mapping_[c] = sorted(self.mapping_[c], key=str)
 
                 if self.record_rare_levels:
-
                     self.rare_levels_record_[c] = list(
                         cols_w_percents.loc[
                             cols_w_percents < self.cut_off_percent
-                        ].index.values
+                        ].index.values,
                     )
 
                     self.rare_levels_record_[c] = sorted(
-                        self.rare_levels_record_[c], key=str
+                        self.rare_levels_record_[c],
+                        key=str,
                     )
 
         return self
 
     def transform(self, X):
         """Grouped rare levels together into a new 'rare' level.
 
@@ -431,34 +395,32 @@
 
         Returns
         -------
         X : pd.DataFrame
             Transformed input X with rare levels grouped for into a new rare level.
 
         """
-
         X = BaseNominalTransformer.transform(self, X)
 
         self.check_is_fitted(["mapping_"])
 
         for c in self.columns:
-
             # for categorical dtypes have to set new category for the impute values first
             # and convert back to the categorical type, other it will convert to object
             if "category" in X[c].dtype.name:
-
                 if self.rare_level_name not in X[c].cat.categories:
-
                     X[c] = X[c].cat.add_categories(self.rare_level_name)
 
                 dtype_before = X[c].dtype
 
                 X[c] = pd.Series(
                     data=np.where(
-                        X[c].isin(self.mapping_[c]), X[c], self.rare_level_name
+                        X[c].isin(self.mapping_[c]),
+                        X[c],
+                        self.rare_level_name,
                     ),
                     index=X.index,
                 ).astype(dtype_before)
 
             else:
                 # using np.where converts np.NaN to str value if only one row of data frame is passed
                 # instead, using pd.where(), if condition true, keep original value, else replace with self.rare_level_name
@@ -557,41 +519,36 @@
         columns=None,
         weights_column=None,
         prior=0,
         level=None,
         unseen_level_handling=None,
         **kwargs,
     ):
-
-        if weights_column is not None:
-
-            if type(weights_column) is not str:
-
-                raise TypeError(f"{self.classname()}: weights_column should be a str")
+        if weights_column is not None and type(weights_column) is not str:
+            msg = f"{self.classname()}: weights_column should be a str"
+            raise TypeError(msg)
 
         if type(prior) is not int:
-
-            raise TypeError(f"{self.classname()}: prior should be a int")
+            msg = f"{self.classname()}: prior should be a int"
+            raise TypeError(msg)
 
         if not prior >= 0:
-            raise ValueError(f"{self.classname()}: prior should be positive int")
-
-        if level:
+            msg = f"{self.classname()}: prior should be positive int"
+            raise ValueError(msg)
 
-            if not isinstance(level, str) and not isinstance(level, list):
-
-                raise TypeError(
-                    f"{self.classname()}: Level should be a NoneType, list or str but got {type(level)}"
-                )
-        if unseen_level_handling:
-            if unseen_level_handling not in ["Mean", "Median", "Lowest", "Highest"]:
-                if not isinstance(unseen_level_handling, (int, float)):
-                    raise ValueError(
-                        f"{self.classname()}: unseen_level_handling should be the option: Mean, Median, Lowest, Highest or an arbitrary int/float value"
-                    )
+        if level and not isinstance(level, str) and not isinstance(level, list):
+            msg = f"{self.classname()}: Level should be a NoneType, list or str but got {type(level)}"
+            raise TypeError(msg)
+        if (
+            unseen_level_handling
+            and (unseen_level_handling not in ["Mean", "Median", "Lowest", "Highest"])
+            and not (isinstance(unseen_level_handling, (int, float)))
+        ):
+            msg = f"{self.classname()}: unseen_level_handling should be the option: Mean, Median, Lowest, Highest or an arbitrary int/float value"
+            raise ValueError(msg)
 
         self.weights_column = weights_column
         self.prior = prior
         self.level = level
         self.unseen_level_handling = unseen_level_handling
         # TODO: set default prior to None and refactor to only use prior regularisation when it is set?
 
@@ -609,27 +566,23 @@
             Series containing group sizes for levels of column in data
 
         Returns
         -------
         regularised : pd.Series
             Series of regularised encoding values
         """
-
         self.check_is_fitted(["global_mean"])
 
-        regularised = (
+        return (
             target_means.multiply(cat_freq, axis="index")
             + self.global_mean * self.prior
         ).divide(cat_freq + self.prior, axis="index")
 
-        return regularised
-
     def _fit_binary_response(self, X, y, columns):
-        """
-        Function to learn the MRE mappings for a given binary or continuous response.
+        """Function to learn the MRE mappings for a given binary or continuous response.
 
         Parameters
         ----------
         X : pd.DataFrame
             Data to with catgeorical variable columns to transform.
 
         y : pd.Series
@@ -637,71 +590,65 @@
 
         columns : list(str)
             Post transform names of columns to be encoded. In the binary or continous case
             this is just self.columns. In the multi-level case this should be of the form
             {column_in_original_data}_{response_level}, where response_level is the level
             being encoded against in this call of _fit_binary_response.
         """
-        if self.weights_column is not None:
-
-            if self.weights_column not in X.columns.values:
+        if (
+            self.weights_column is not None
+            and self.weights_column not in X.columns.to_numpy()
+        ):
+            msg = f"{self.classname()}: weights column {self.weights_column} not in X"
+            raise ValueError(msg)
 
-                raise ValueError(
-                    f"{self.classname()}: weights column {self.weights_column} not in X"
-                )
-
-        response_null_count = y.isnull().sum()
+        response_null_count = y.isna().sum()
 
         if response_null_count > 0:
-
-            raise ValueError(
-                f"{self.classname()}: y has {response_null_count} null values"
-            )
+            msg = f"{self.classname()}: y has {response_null_count} null values"
+            raise ValueError(msg)
 
         X_y = self._combine_X_y(X, y)
         response_column = "_temporary_response"
 
         if self.weights_column is None:
-
             self.global_mean = X_y[response_column].mean()
 
         else:
-
             X_y["weighted_response"] = X_y[response_column].multiply(
-                X_y[self.weights_column]
+                X_y[self.weights_column],
             )
 
             self.global_mean = (
                 X_y["weighted_response"].sum() / X_y[self.weights_column].sum()
             )
 
         for c in columns:
-
             if self.weights_column is None:
-
                 group_means = X_y.groupby(c)[response_column].mean()
 
                 group_counts = X_y.groupby(c)[response_column].size()
 
                 self.mappings[c] = self._prior_regularisation(
-                    group_means, group_counts
+                    group_means,
+                    group_counts,
                 ).to_dict()
 
             else:
-
                 groupby_sum = X_y.groupby([c])[
                     ["weighted_response", self.weights_column]
                 ].sum()
 
                 group_weight = groupby_sum[self.weights_column]
 
                 group_means = groupby_sum["weighted_response"] / group_weight
 
                 self.mappings[c] = self._prior_regularisation(
-                    group_means, group_weight
+                    group_means,
+                    group_weight,
                 ).to_dict()
 
     def fit(self, X, y):
         """Identify mapping of categorical levels to mean response values.
 
         If the user specified the weights_column arg in when initialising the transformer
         the weighted mean response will be calculated using that column.
@@ -715,36 +662,31 @@
             Data to with catgeorical variable columns to transform and also containing response_column
             column.
 
         y : pd.Series
             Response variable or target.
 
         """
-
         BaseNominalTransformer.fit(self, X, y)
 
         self.mappings = {}
         self.unseen_levels_encoding_dict = {}
         X_temp = X.copy()
 
         if self.level:
-
             if self.level == "all":
-
                 self.response_levels = y.unique()
 
             else:
-
                 if isinstance(self.level, str):
                     self.level = [self.level]
 
-                if any([level not in list(y.unique()) for level in self.level]):
-                    raise ValueError(
-                        "Levels contains a level to encode against that is not present in the response."
-                    )
+                if any(level not in list(y.unique()) for level in self.level):
+                    msg = "Levels contains a level to encode against that is not present in the response."
+                    raise ValueError(msg)
 
                 self.response_levels = self.level
 
             self.transformer_dict = {}
             mapped_columns = []
 
             for level in self.response_levels:
@@ -752,27 +694,28 @@
                     column + "_" + level for column in self.columns
                 ]
 
                 for column in self.columns:
                     X_temp[column + "_" + level] = X[column].copy()
 
                 # keep nans to preserve null check functionality of binary response MRE transformer
-                y_temp = y.apply(lambda x: x == level if not pd.isnull(x) else np.nan)
+                y_temp = y.apply(lambda x: x == level if not pd.isna(x) else np.nan)
 
                 self.transformer_dict[level] = self._fit_binary_response(
-                    X_temp, y_temp, mapping_columns_for_this_level
+                    X_temp,
+                    y_temp,
+                    mapping_columns_for_this_level,
                 )
 
                 mapped_columns += mapping_columns_for_this_level
 
             self.mapped_columns = list(set(mapped_columns) - set(self.columns))
             self.encoded_feature_columns = self.mapped_columns
 
         else:
-
             self._fit_binary_response(X, y, self.columns)
             self.encoded_feature_columns = self.columns
 
         if self.unseen_level_handling == "Mean":
             for c in self.encoded_feature_columns:
                 self.unseen_levels_encoding_dict[c] = (
                     X_temp[c].map(self.mappings[c]).mean()
@@ -844,15 +787,15 @@
         else:
             self.check_mappable_rows(X)
             X = BaseMappingTransformMixin.transform(self, X)
 
         if self.level:
             # Setting self.columns back so that the transformer object is unchanged after transform is called
             self.columns = temp_columns
-            X.drop(columns=self.columns, inplace=True)
+            X = X.drop(columns=self.columns)
 
         return X
 
 
 class OrdinalEncoderTransformer(BaseNominalTransformer, BaseMappingTransformMixin):
     """Transformer to encode categorical variables into ascending rank-ordered integer values variables by mapping
     it's levels to the target-mean response for that level.
@@ -881,20 +824,17 @@
     mappings : dict
         Created in fit. Dict of key (column names) value (mapping of categorical levels to numeric,
         ordinal encoded response values) pairs.
 
     """
 
     def __init__(self, columns=None, weights_column=None, **kwargs):
-
-        if weights_column is not None:
-
-            if type(weights_column) is not str:
-
-                raise TypeError(f"{self.classname()}: weights_column should be a str")
+        if weights_column is not None and type(weights_column) is not str:
+            msg = f"{self.classname()}: weights_column should be a str"
+            raise TypeError(msg)
 
         self.weights_column = weights_column
 
         BaseNominalTransformer.__init__(self, columns=columns, **kwargs)
 
     def fit(self, X, y):
         """Identify mapping of categorical levels to rank-ordered integer values by target-mean in ascending order.
@@ -908,70 +848,63 @@
             Data to with catgeorical variable columns to transform and response_column column
             specified when object was initialised.
 
         y : pd.Series
             Response column or target.
 
         """
-
         BaseNominalTransformer.fit(self, X, y)
 
         self.mappings = {}
 
-        if self.weights_column is not None:
-
-            if self.weights_column not in X.columns.values:
-
-                raise ValueError(
-                    f"{self.classname()}: weights column {self.weights_column} not in X"
-                )
+        if (
+            self.weights_column is not None
+            and self.weights_column not in X.columns.to_numpy()
+        ):
+            msg = f"{self.classname()}: weights column {self.weights_column} not in X"
+            raise ValueError(msg)
 
-        response_null_count = y.isnull().sum()
+        response_null_count = y.isna().sum()
 
         if response_null_count > 0:
-
-            raise ValueError(
-                f"{self.classname()}: y has {response_null_count} null values"
-            )
+            msg = f"{self.classname()}: y has {response_null_count} null values"
+            raise ValueError(msg)
 
         X_y = self._combine_X_y(X, y)
         response_column = "_temporary_response"
 
         for c in self.columns:
-
             if self.weights_column is None:
-
                 # get the indexes of the sorted target mean-encoded dict
                 _idx_target_mean = list(
                     X_y.groupby([c])[response_column]
                     .mean()
                     .sort_values(ascending=True, kind="mergesort")
-                    .index
+                    .index,
                 )
 
                 # create a dictionary whose keys are the levels of the categorical variable
                 # sorted ascending by their target-mean value
                 # and whose values are ascending ordinal integers
                 ordinal_encoded_dict = {
                     k: _idx_target_mean.index(k) + 1 for k in _idx_target_mean
                 }
 
                 self.mappings[c] = ordinal_encoded_dict
 
             else:
-
                 groupby_sum = X_y.groupby([c])[
                     [response_column, self.weights_column]
                 ].sum()
 
                 # get the indexes of the sorted target mean-encoded dict
                 _idx_target_mean = list(
                     (groupby_sum[response_column] / groupby_sum[self.weights_column])
                     .sort_values(ascending=True, kind="mergesort")
-                    .index
+                    .index,
                 )
 
                 # create a dictionary whose keys are the levels of the categorical variable
                 # sorted ascending by their target-mean value
                 # and whose values are ascending ordinal integers
                 ordinal_encoded_dict = {
                     k: _idx_target_mean.index(k) + 1 for k in _idx_target_mean
@@ -996,20 +929,17 @@
 
         Returns
         -------
         X : pd.DataFrame
             Transformed data with levels mapped to ordinal encoded values for categorical variables.
 
         """
-
         self.check_mappable_rows(X)
 
-        X = BaseMappingTransformMixin.transform(self, X)
-
-        return X
+        return BaseMappingTransformMixin.transform(self, X)
 
 
 class OneHotEncodingTransformer(BaseNominalTransformer, OneHotEncoder):
     """Transformer to convert cetegorical variables into dummy columns.
 
     Extends the sklearn OneHotEncoder class to provide easy renaming of dummy columns.
 
@@ -1049,17 +979,19 @@
         columns=None,
         separator="_",
         drop_original=False,
         copy=True,
         verbose=False,
         **kwargs,
     ):
-
         BaseNominalTransformer.__init__(
-            self, columns=columns, copy=copy, verbose=verbose
+            self,
+            columns=columns,
+            copy=copy,
+            verbose=verbose,
         )
 
         # Set attributes for scikit-learn'S OneHotEncoder
         OneHotEncoder.__init__(self, sparse=False, handle_unknown="ignore", **kwargs)
 
         # Set other class attrributes
         self.separator = separator
@@ -1074,76 +1006,67 @@
         X : pd.DataFrame
             Data to identify levels from.
 
         y : None
             Ignored. This parameter exists only for compatibility with sklearn.pipeline.Pipeline.
 
         """
-
         BaseNominalTransformer.fit(self, X=X, y=y)
 
         # Check for nulls
         for c in self.columns:
-
-            if X[c].isnull().sum() > 0:
-
+            if X[c].isna().sum() > 0:
                 raise ValueError(
                     f"{self.classname()}: column %s has nulls - replace before proceeding"
-                    % c
+                    % c,
                 )
 
         # Check each field has less than 100 categories/levels
         for c in self.columns:
-
             levels = X[c].unique().tolist()
 
             if len(levels) > 100:
-
                 raise ValueError(
                     f"{self.classname()}: column %s has over 100 unique values - consider another type of encoding"
-                    % c
+                    % c,
                 )
 
         OneHotEncoder.fit(self, X=X[self.columns], y=y)
 
         return self
 
     def _get_feature_names(self, input_features, **kwargs):
-        """
-        Function to access the get_feature_names attribute of the scikit learn attribute. Will return the output columns of the OHE transformer.
+        """Function to access the get_feature_names attribute of the scikit learn attribute. Will return the output columns of the OHE transformer.
 
         In scikit learn 1.0 "get_feature_names" was deprecated and then replaced with "get_feature_names_out" in version 1.2. The logic in this
         function will call the correct attribute, or raise an error if it can't be found.
 
         Parameters
         ----------
         input_features : list(str)
             Input columns being transformed by the OHE transformer.
 
         kwargs : dict
             Keyword arguments to be passed on to the scikit learn attriute.
         """
-
         if hasattr(self, "get_feature_names"):
-
             input_columns = self.get_feature_names(
-                input_features=input_features, **kwargs
+                input_features=input_features,
+                **kwargs,
             )
 
         elif hasattr(self, "get_feature_names_out"):
-
             input_columns = self.get_feature_names_out(
-                input_features=input_features, **kwargs
+                input_features=input_features,
+                **kwargs,
             )
 
         else:
-
-            raise AttributeError(
-                "Cannot access scikit learn OneHotEncoder get_feature_names method, may be a version issue"
-            )
+            msg = "Cannot access scikit learn OneHotEncoder get_feature_names method, may be a version issue"
+            raise AttributeError(msg)
 
         return input_columns
 
     def transform(self, X):
         """Create new dummy columns from categorical fields.
 
         Parameters
@@ -1155,75 +1078,67 @@
         -------
         X_transformed : pd.DataFrame
             Transformed input X with dummy columns derived from categorical columns added. If drop_original
             = True then the original categorical columns that the dummies are created from will not be in
             the output X.
 
         """
-
         self.check_is_fitted(["separator"])
         self.check_is_fitted(["drop_original"])
 
         self.columns_check(X)
 
         # Check for nulls
         for c in self.columns:
-
-            if X[c].isnull().sum() > 0:
-
+            if X[c].isna().sum() > 0:
                 raise ValueError(
                     f"{self.classname()}: column %s has nulls - replace before proceeding"
-                    % c
+                    % c,
                 )
 
         X = BaseNominalTransformer.transform(self, X)
 
         # Apply OHE transform
         X_transformed = OneHotEncoder.transform(self, X[self.columns])
 
         input_columns = self._get_feature_names(input_features=self.columns)
 
         X_transformed = pd.DataFrame(
-            X_transformed, columns=input_columns, index=X.index
+            X_transformed,
+            columns=input_columns,
+            index=X.index,
         )
 
         # Rename dummy fields if separator is specified
         if self.separator != "_":
-
             old_names = [
                 c + "_" + str(lvl)
                 for i, c in enumerate(self.columns)
                 for lvl in self.categories_[i]
             ]
             new_names = [
                 c + self.separator + str(lvl)
                 for i, c in enumerate(self.columns)
                 for lvl in self.categories_[i]
             ]
 
-            X_transformed.rename(
-                columns={i: j for i, j in zip(old_names, new_names)}, inplace=True
+            X_transformed = X_transformed.rename(
+                columns=dict(zip(old_names, new_names)),
             )
 
         # Print warning for unseen levels
         if self.verbose:
-
             for i, c in enumerate(self.columns):
-
                 unseen_levels = set(X[c].unique().tolist()) - set(self.categories_[i])
 
                 if len(unseen_levels) > 0:
-
                     warnings.warn(
                         f"{self.classname()}: column %s has unseen categories: %s"
-                        % (c, unseen_levels)
+                        % (c, unseen_levels),
                     )
 
         # Drop original columns
         if self.drop_original:
-
-            X.drop(self.columns, axis=1, inplace=True)
+            X = X.drop(self.columns, axis=1)
 
         # Concatenate original and new dummy fields
-        X_transformed = pd.concat((X, X_transformed), axis=1)
-
-        return X_transformed
+        return pd.concat((X, X_transformed), axis=1)
```

### Comparing `tubular-0.3.7/tubular/numeric.py` & `tubular-0.3.8/tubular/numeric.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-"""
-This module contains transformers that apply numeric functions.
-"""
+"""This module contains transformers that apply numeric functions."""
 
 import numpy as np
 import pandas as pd
+from sklearn.decomposition import PCA
 from sklearn.preprocessing import (
-    MinMaxScaler,
     MaxAbsScaler,
-    StandardScaler,
+    MinMaxScaler,
     PolynomialFeatures,
+    StandardScaler,
 )
-from sklearn.decomposition import PCA
 
 from tubular.base import BaseTransformer, DataFrameMethodTransformer
 
 
 class LogTransformer(BaseTransformer):
     """Transformer to apply log transformation.
 
@@ -54,26 +52,31 @@
 
     suffix : str
         The suffix to add onto the end of column names for new columns.
 
     """
 
     def __init__(
-        self, columns, base=None, add_1=False, drop=True, suffix="log", **kwargs
-    ):
-
+        self,
+        columns,
+        base=None,
+        add_1=False,
+        drop=True,
+        suffix="log",
+        **kwargs,
+    ) -> None:
         super().__init__(columns=columns, **kwargs)
 
         if base is not None:
             if not isinstance(base, (int, float)):
-                raise ValueError(f"{self.classname()}: base should be numeric or None")
+                msg = f"{self.classname()}: base should be numeric or None"
+                raise ValueError(msg)
             if not base > 0:
-                raise ValueError(
-                    f"{self.classname()}: base should be strictly positive"
-                )
+                msg = f"{self.classname()}: base should be strictly positive"
+                raise ValueError(msg)
 
         self.base = base
         self.add_1 = add_1
         self.drop = drop
         self.suffix = suffix
 
     def transform(self, X):
@@ -90,68 +93,55 @@
         Returns
         -------
         X : pd.DataFrame
             The dataframe with the specified columns logged, optionally dropping the original
             columns if self.drop is True.
 
         """
-
         X = super().transform(X)
 
         numeric_column_types = X[self.columns].apply(
-            pd.api.types.is_numeric_dtype, axis=0
+            pd.api.types.is_numeric_dtype,
+            axis=0,
         )
 
         if not numeric_column_types.all():
-
             non_numeric_columns = list(
-                numeric_column_types.loc[~numeric_column_types].index
+                numeric_column_types.loc[~numeric_column_types].index,
             )
 
-            raise TypeError(
-                f"{self.classname()}: The following columns are not numeric in X; {non_numeric_columns}"
-            )
+            msg = f"{self.classname()}: The following columns are not numeric in X; {non_numeric_columns}"
+            raise TypeError(msg)
 
         new_column_names = [f"{column}_{self.suffix}" for column in self.columns]
 
         if self.add_1:
-
             if (X[self.columns] <= -1).sum().sum() > 0:
-
-                raise ValueError(
-                    f"{self.classname()}: values less than or equal to 0 in columns (after adding 1), make greater than 0 before using transform"
-                )
+                msg = f"{self.classname()}: values less than or equal to 0 in columns (after adding 1), make greater than 0 before using transform"
+                raise ValueError(msg)
 
             if self.base is None:
-
                 X[new_column_names] = np.log(X[self.columns] + 1)
 
             else:
-
                 X[new_column_names] = np.log(X[self.columns] + 1) / np.log(self.base)
 
         else:
-
             if (X[self.columns] <= 0).sum().sum() > 0:
-
-                raise ValueError(
-                    f"{self.classname()}: values less than or equal to 0 in columns, make greater than 0 before using transform"
-                )
+                msg = f"{self.classname()}: values less than or equal to 0 in columns, make greater than 0 before using transform"
+                raise ValueError(msg)
 
             if self.base is None:
-
                 X[new_column_names] = np.log(X[self.columns])
 
             else:
-
                 X[new_column_names] = np.log(X[self.columns]) / np.log(self.base)
 
         if self.drop:
-
-            X.drop(self.columns, axis=1, inplace=True)
+            X = X.drop(self.columns, axis=1)
 
         return X
 
 
 class CutTransformer(BaseTransformer):
     """Class to bin a column into discrete intervals.
 
@@ -170,41 +160,31 @@
         A dictionary of keyword arguments to be passed to the pd.cut method when it is called in transform.
 
     **kwargs
         Arbitrary keyword arguments passed onto BaseTransformer.init().
 
     """
 
-    def __init__(self, column, new_column_name, cut_kwargs={}, **kwargs):
-
-        if not type(column) is str:
-
-            raise TypeError(
-                f"{self.classname()}: column arg (name of column) should be a single str giving the column to discretise"
-            )
-
-        if not type(new_column_name) is str:
-
-            raise TypeError(f"{self.classname()}: new_column_name must be a str")
-
-        if not type(cut_kwargs) is dict:
-
-            raise TypeError(
-                f"{self.classname()}: cut_kwargs should be a dict but got type {type(cut_kwargs)}"
-            )
-
-        else:
-
-            for i, k in enumerate(cut_kwargs.keys()):
-
-                if not type(k) is str:
-
-                    raise TypeError(
-                        f"{self.classname()}: unexpected type ({type(k)}) for cut_kwargs key in position {i}, must be str"
-                    )
+    def __init__(self, column, new_column_name, cut_kwargs={}, **kwargs) -> None:
+        if type(column) is not str:
+            msg = f"{self.classname()}: column arg (name of column) should be a single str giving the column to discretise"
+            raise TypeError(msg)
+
+        if type(new_column_name) is not str:
+            msg = f"{self.classname()}: new_column_name must be a str"
+            raise TypeError(msg)
+
+        if type(cut_kwargs) is not dict:
+            msg = f"{self.classname()}: cut_kwargs should be a dict but got type {type(cut_kwargs)}"
+            raise TypeError(msg)
+
+        for i, k in enumerate(cut_kwargs.keys()):
+            if type(k) is not str:
+                msg = f"{self.classname()}: unexpected type ({type(k)}) for cut_kwargs key in position {i}, must be str"
+                raise TypeError(msg)
 
         self.cut_kwargs = cut_kwargs
         self.new_column_name = new_column_name
 
         # This attribute is not for use in any method, use 'columns' instead.
         # Here only as a fix to allow string representation of transformer.
         self.column = column
@@ -216,32 +196,27 @@
 
         Parameters
         ----------
         X : pd.DataFrame
             Data with column to transform.
 
         """
-
         X = super().transform(X)
 
         if not pd.api.types.is_numeric_dtype(X[self.columns[0]]):
-
-            raise TypeError(
-                f"{self.classname()}: {self.columns[0]} should be a numeric dtype but got {X[self.columns[0]].dtype}"
-            )
+            msg = f"{self.classname()}: {self.columns[0]} should be a numeric dtype but got {X[self.columns[0]].dtype}"
+            raise TypeError(msg)
 
         X[self.new_column_name] = pd.cut(X[self.columns[0]], **self.cut_kwargs)
 
         return X
 
 
 class TwoColumnOperatorTransformer(DataFrameMethodTransformer):
-
-    """
-    This transformer applies a pandas.DataFrame method to two columns (add, sub, mul, div, mod, pow).
+    """This transformer applies a pandas.DataFrame method to two columns (add, sub, mul, div, mod, pow).
 
     Transformer assigns the output of the method to a new column. The method will be applied
     in the form (column 1)operator(column 2), so order matters (if the method does not commute). It is possible to
     supply other key word arguments to the transform method, which will be passed to the pandas.DataFrame method being called.
 
     Parameters
     ----------
@@ -286,34 +261,27 @@
     def __init__(
         self,
         pd_method_name,
         columns,
         new_column_name,
         pd_method_kwargs={"axis": 0},
         **kwargs,
-    ):
-        """
-        Performs input checks not done in either DataFrameMethodTransformer.__init__ or BaseTransformer.__init__
-        """
-
+    ) -> None:
+        """Performs input checks not done in either DataFrameMethodTransformer.__init__ or BaseTransformer.__init__."""
         if "axis" not in pd_method_kwargs.keys():
-            raise ValueError(
-                f'{self.classname()}: pd_method_kwargs must contain an entry "axis" set to 0 or 1'
-            )
+            msg = f'{self.classname()}: pd_method_kwargs must contain an entry "axis" set to 0 or 1'
+            raise ValueError(msg)
 
         if pd_method_kwargs["axis"] not in [0, 1]:
-            raise ValueError(
-                f"{self.classname()}: pd_method_kwargs 'axis' must be 0 or 1"
-            )
+            msg = f"{self.classname()}: pd_method_kwargs 'axis' must be 0 or 1"
+            raise ValueError(msg)
 
-        if not type(columns) is list:
-            if len(columns) != 2:
-                raise ValueError(
-                    f"{self.classname()}: columns must be a list containing two column names but got {columns}"
-                )
+        if type(columns) is not list and len(columns) != 2:
+            msg = f"{self.classname()}: columns must be a list containing two column names but got {columns}"
+            raise ValueError(msg)
 
         self.column1_name = columns[0]
         self.column2_name = columns[1]
 
         # call DataFrameMethodTransformer.__init__
         # This class will inherit all the below attributes from DataFrameMethodTransformer
         super().__init__(
@@ -321,35 +289,36 @@
             pd_method_name=pd_method_name,
             columns=columns,
             pd_method_kwargs=pd_method_kwargs,
             **kwargs,
         )
 
     def transform(self, X):
-        """
-        Transform input data by applying the chosen method to the two specified columns
+        """Transform input data by applying the chosen method to the two specified columns.
 
         Args:
+        ----
             X (pd.DataFrame): Data to transform.
 
         Returns:
+        -------
             pd.DataFrame: Input X with an additional column.
         """
         # call BaseTransformer.transform
         X = super(DataFrameMethodTransformer, self).transform(X)
 
         is_numeric = X[self.columns].apply(pd.api.types.is_numeric_dtype, axis=0)
 
         if not is_numeric.all():
-            raise TypeError(
-                f"{self.classname()}: input columns in X must contain only numeric values"
-            )
+            msg = f"{self.classname()}: input columns in X must contain only numeric values"
+            raise TypeError(msg)
 
         X[self.new_column_name] = getattr(X[[self.column1_name]], self.pd_method_name)(
-            X[self.column2_name], **self.pd_method_kwargs
+            X[self.column2_name],
+            **self.pd_method_kwargs,
         )
 
         return X
 
 
 class ScalingTransformer(BaseTransformer):
     """Transformer to perform scaling of numeric columns.
@@ -370,50 +339,37 @@
         A dictionary of keyword arguments to be passed to the scaler object when it is initialised.
 
     **kwargs
         Arbitrary keyword arguments passed onto BaseTransformer.init().
 
     """
 
-    def __init__(self, columns, scaler_type, scaler_kwargs={}, **kwargs):
-
-        if not type(scaler_kwargs) is dict:
-
-            raise TypeError(
-                f"{self.classname()}: scaler_kwargs should be a dict but got type {type(scaler_kwargs)}"
-            )
-
-        else:
-
-            for i, k in enumerate(scaler_kwargs.keys()):
-
-                if not type(k) is str:
-
-                    raise TypeError(
-                        f"{self.classname()}: unexpected type ({type(k)}) for scaler_kwargs key in position {i}, must be str"
-                    )
+    def __init__(self, columns, scaler_type, scaler_kwargs={}, **kwargs) -> None:
+        if type(scaler_kwargs) is not dict:
+            msg = f"{self.classname()}: scaler_kwargs should be a dict but got type {type(scaler_kwargs)}"
+            raise TypeError(msg)
+
+        for i, k in enumerate(scaler_kwargs.keys()):
+            if type(k) is not str:
+                msg = f"{self.classname()}: unexpected type ({type(k)}) for scaler_kwargs key in position {i}, must be str"
+                raise TypeError(msg)
 
         allowed_scaler_values = ["min_max", "max_abs", "standard"]
 
         if scaler_type not in allowed_scaler_values:
-
-            raise ValueError(
-                f"{self.classname()}: scaler_type should be one of; {allowed_scaler_values}"
-            )
+            msg = f"{self.classname()}: scaler_type should be one of; {allowed_scaler_values}"
+            raise ValueError(msg)
 
         if scaler_type == "min_max":
-
             self.scaler = MinMaxScaler(**scaler_kwargs)
 
         elif scaler_type == "max_abs":
-
             self.scaler = MaxAbsScaler(**scaler_kwargs)
 
         elif scaler_type == "standard":
-
             self.scaler = StandardScaler(**scaler_kwargs)
 
         # This attribute is not for use in any method
         # Here only as a fix to allow string representation of transformer.
         self.scaler_kwargs = scaler_kwargs
         self.scaler_type = scaler_type
 
@@ -424,28 +380,26 @@
 
         Parameters
         ----------
         X : pd.DataFrame
             Data containing columns to check.
 
         """
-
         numeric_column_types = X[self.columns].apply(
-            pd.api.types.is_numeric_dtype, axis=0
+            pd.api.types.is_numeric_dtype,
+            axis=0,
         )
 
         if not numeric_column_types.all():
-
             non_numeric_columns = list(
-                numeric_column_types.loc[~numeric_column_types].index
+                numeric_column_types.loc[~numeric_column_types].index,
             )
 
-            raise TypeError(
-                f"{self.classname()}: The following columns are not numeric in X; {non_numeric_columns}"
-            )
+            msg = f"{self.classname()}: The following columns are not numeric in X; {non_numeric_columns}"
+            raise TypeError(msg)
 
         return X
 
     def fit(self, X, y=None):
         """Fit scaler to input data.
 
         Parameters
@@ -453,15 +407,14 @@
         X : pd.DataFrame
             Dataframe with columns to learn scaling values from.
 
         y : None
             Required for pipeline.
 
         """
-
         super().fit(X, y)
 
         X = self.check_numeric_columns(X)
 
         self.scaler.fit(X[self.columns])
 
         return self
@@ -476,15 +429,14 @@
 
         Returns
         -------
         X : pd.DataFrame
             Input X with columns scaled.
 
         """
-
         X = super().transform(X)
 
         X = self.check_numeric_columns(X)
 
         X[self.columns] = self.scaler.transform(X[self.columns])
 
         return X
@@ -495,34 +447,34 @@
     Transformer generates a new column  for all combinations from the selected columns up to the maximum degree
     provided. (For sklearn version higher than 1.0.0>, only interaction of a degree higher or equal to the minimum
     degree would be computed).
     Each interaction column consists of the product of the specific combination of columns.
     Ex: with 3 columns provided ["a","b","c"], if max degree is 3, the total possible combinations are :
     - of degree 1 : ["a","b","c"]
     - of degree 2 : ["a b","b c","a c"]
-    - of degree 3 : ["a b c"]
+    - of degree 3 : ["a b c"].
 
-        Parameters
-        ----------
+    Parameters
+    ----------
         columns : None or list or str
             Columns to apply the transformer to. If a str is passed this is put into a list. Value passed
             in columns is saved in the columns attribute on the object. Note this has no default value so
             the user has to specify the columns when initialising the transformer. This is avoid likely
             when the user forget to set columns, in this case all columns would be picked up when super
             transform runs.
         min_degree : int
             minimum degree of interaction features to be considered. For example if min_degree=3, only interaction
             columns from at least 3 columns would be generated. NB- only applies if sklearn version is 1.0.0>=
         max_degree : int
             maximum degree of interaction features to be considered. For example if max_degree=3, only interaction
             columns from up to 3 columns would be generated.
 
 
-         Attributes
-        ----------
+    Attributes
+    ----------
         min_degree : int
             minimum degree of interaction features to be considered
         max_degree : int
             maximum degree of interaction features to be considered
         nb_features_to_interact : int
             number of selected columns from which interactions should be computed. (=len(columns))
         nb_combinations : int
@@ -531,57 +483,45 @@
             names of each new interaction feature. The name of an interaction feature is the combinations of previous
             column names joined with a whitespace. Interaction feature of ["col1","col2","col3] would be "col1 col2 col3".
         nb_feature_out : int
             number of total columns of transformed dataset, including new interaction features
 
     """
 
-    def __init__(self, columns, min_degree=2, max_degree=2, **kwargs):
-
+    def __init__(self, columns, min_degree=2, max_degree=2, **kwargs) -> None:
         super().__init__(columns=columns, **kwargs)
 
         if len(columns) < 2:
-            raise ValueError(
-                f"{self.classname()}: number of columns must be equal or greater than 2, got {str(len(columns))} column."
-            )
+            msg = f"{self.classname()}: number of columns must be equal or greater than 2, got {str(len(columns))} column."
+            raise ValueError(msg)
 
         if type(min_degree) is int:
             if min_degree < 2:
-                raise ValueError(
-                    f"{self.classname()}: min_degree must be equal or greater than 2, got {str(min_degree)}"
-                )
-            else:
-                self.min_degree = min_degree
+                msg = f"{self.classname()}: min_degree must be equal or greater than 2, got {str(min_degree)}"
+                raise ValueError(msg)
+            self.min_degree = min_degree
         else:
-            raise TypeError(
-                f"{self.classname()}: unexpected type ({type(min_degree)}) for min_degree, must be int"
-            )
+            msg = f"{self.classname()}: unexpected type ({type(min_degree)}) for min_degree, must be int"
+            raise TypeError(msg)
         if type(max_degree) is int:
             if min_degree > max_degree:
-                raise ValueError(
-                    f"{self.classname()}: max_degree must be equal or greater than min_degree"
-                )
-            else:
-                self.max_degree = max_degree
+                msg = f"{self.classname()}: max_degree must be equal or greater than min_degree"
+                raise ValueError(msg)
+            self.max_degree = max_degree
             if max_degree > len(columns):
-                raise ValueError(
-                    f"{self.classname()}: max_degree must be equal or lower than number of columns"
-                )
-            else:
-                self.max_degree = max_degree
+                msg = f"{self.classname()}: max_degree must be equal or lower than number of columns"
+                raise ValueError(msg)
+            self.max_degree = max_degree
             if max_degree > len(columns):
-                raise ValueError(
-                    "max_degree must be equal or lower than number of columns"
-                )
-            else:
-                self.max_degree = max_degree
+                msg = f"{self.classname()}: max_degree must be equal or lower than number of columns"
+                raise ValueError(msg)
+            self.max_degree = max_degree
         else:
-            raise TypeError(
-                f"{self.classname()}: unexpected type ({type(max_degree)}) for max_degree, must be int"
-            )
+            msg = f"{self.classname()}: unexpected type ({type(max_degree)}) for max_degree, must be int"
+            raise TypeError(msg)
 
         self.nb_features_to_interact = len(self.columns)
         self.nb_combinations = -1
         self.interaction_colname = []
         self.nb_feature_out = -1
 
     def transform(self, X):
@@ -647,16 +587,16 @@
 class PCATransformer(BaseTransformer):
     """Transformer that generates variables using Principal component analysis (PCA).
     Linear dimensionality reduction using Singular Value Decomposition of the
     data to project it to a lower dimensional space.
 
     It is based on sklearn class sklearn.decomposition.PCA
 
-        Parameters
-        ----------
+    Parameters
+    ----------
         columns : None or list or str
             Columns to apply the transformer to. If a str is passed this is put into a list. Value passed
             in columns is saved in the columns attribute on the object. Note this has no default value so
             the user has to specify the columns when initialising the transformer. When the user forget to set columns,
             all columns would be picked up when super transform runs.
         n_components : int, float or 'mle', default=None
             Number of components to keep.
@@ -696,15 +636,14 @@
             for reproducible results across multiple function calls.
             .. sklearn versionadded:: 0.18.0
         pca_column_prefix : str, prefix added to each the n components features generated. Default is "pca_"
             example: if n_components = 3, new columns would be 'pca_0','pca_1','pca_2'.
 
     Attributes
     ----------
-
     pca : PCA class from sklearn.decomposition
     n_components_ : int
         The estimated number of components. When n_components is set
         to 'mle' or a number between 0 and 1 (with svd_solver == 'full') this
         number is estimated from input data. Otherwise it equals the parameter
         n_components, or the lesser value of n_features and n_samples
         if n_components is None.
@@ -718,78 +657,63 @@
         self,
         columns,
         n_components=2,
         svd_solver="auto",
         random_state=None,
         pca_column_prefix="pca_",
         **kwargs,
-    ):
-
+    ) -> None:
         super().__init__(columns=columns, **kwargs)
 
         if type(n_components) is int:
             if n_components < 1:
-                raise ValueError(
-                    f"{self.classname()}:n_components must be strictly positive got {str(n_components)}"
-                )
-            else:
-                self.n_components = n_components
+                msg = f"{self.classname()}:n_components must be strictly positive got {str(n_components)}"
+                raise ValueError(msg)
+            self.n_components = n_components
         elif type(n_components) is float:
             if 0 < n_components < 1:
                 self.n_components = n_components
             else:
-                raise ValueError(
-                    f"{self.classname()}:n_components must be strictly positive and must be of type int when greater than or equal to 1. Got {str(n_components)}"
-                )
+                msg = f"{self.classname()}:n_components must be strictly positive and must be of type int when greater than or equal to 1. Got {str(n_components)}"
+                raise ValueError(msg)
 
         else:
             if n_components == "mle":
                 self.n_components = n_components
             else:
-                raise TypeError(
-                    f"{self.classname()}:unexpected type {type(n_components)} for n_components, must be int, float (0-1) or equal to 'mle'."
-                )
+                msg = f"{self.classname()}:unexpected type {type(n_components)} for n_components, must be int, float (0-1) or equal to 'mle'."
+                raise TypeError(msg)
 
         if type(svd_solver) is str:
             if svd_solver not in ["auto", "full", "arpack", "randomized"]:
-                raise ValueError(
-                    f"{self.classname()}:svd_solver {svd_solver} is unknown. Please select among 'auto', 'full', 'arpack', 'randomized'."
-                )
-            else:
-                self.svd_solver = svd_solver
+                msg = f"{self.classname()}:svd_solver {svd_solver} is unknown. Please select among 'auto', 'full', 'arpack', 'randomized'."
+                raise ValueError(msg)
+            self.svd_solver = svd_solver
         else:
-            raise TypeError(
-                f"{self.classname()}:unexpected type {type(svd_solver)} for svd_solver, must be str"
-            )
+            msg = f"{self.classname()}:unexpected type {type(svd_solver)} for svd_solver, must be str"
+            raise TypeError(msg)
 
-        if type(random_state) is int:
+        if type(random_state) is int or random_state is None:
             self.random_state = random_state
         else:
-            if random_state is None:
-                self.random_state = random_state
-            else:
-                raise TypeError(
-                    f"{self.classname()}:unexpected type {type(random_state)} for random_state, must be int or None."
-                )
+            msg = f"{self.classname()}:unexpected type {type(random_state)} for random_state, must be int or None."
+            raise TypeError(msg)
 
         if (svd_solver == "arpack") and (n_components == "mle"):
-            raise ValueError(
-                f"{self.classname()}: n_components='mle' cannot be a string with svd_solver='arpack'"
-            )
+            msg = f"{self.classname()}: n_components='mle' cannot be a string with svd_solver='arpack'"
+            raise ValueError(msg)
         if (svd_solver in ["randomized", "arpack"]) and (type(n_components) is float):
-            raise TypeError(
-                f"{self.classname()}: n_components {n_components} cannot be a float with svd_solver='{svd_solver}'"
-            )
+            msg = f"{self.classname()}: n_components {n_components} cannot be a float with svd_solver='{svd_solver}'"
+            raise TypeError(msg)
 
         if type(pca_column_prefix) is str:
             self.pca_column_prefix = pca_column_prefix
         else:
-            raise TypeError(
-                f"{self.classname()}:unexpected type {type(pca_column_prefix)} for pca_column_prefix, must be str"
-            )
+            msg = f"{self.classname()}:unexpected type {type(pca_column_prefix)} for pca_column_prefix, must be str"
+            raise TypeError(msg)
 
         self.pca = PCA(
             n_components=self.n_components,
             svd_solver=self.svd_solver,
             random_state=self.random_state,
         )
 
@@ -802,28 +726,26 @@
 
         Parameters
         ----------
         X : pd.DataFrame
             Data containing columns to check.
 
         """
-
         numeric_column_types = X[self.columns].apply(
-            pd.api.types.is_numeric_dtype, axis=0
+            pd.api.types.is_numeric_dtype,
+            axis=0,
         )
 
         if not numeric_column_types.all():
-
             non_numeric_columns = list(
-                numeric_column_types.loc[~numeric_column_types].index
+                numeric_column_types.loc[~numeric_column_types].index,
             )
 
-            raise TypeError(
-                f"{self.classname()}: The following columns are not numeric in X; {non_numeric_columns}"
-            )
+            msg = f"{self.classname()}: The following columns are not numeric in X; {non_numeric_columns}"
+            raise TypeError(msg)
 
         return X
 
     def fit(self, X, y=None):
         """Fit PCA to input data.
 
         Parameters
@@ -831,41 +753,41 @@
         X : pd.DataFrame
             Dataframe with columns to learn scaling values from.
 
         y : None
             Required for pipeline.
 
         """
-
         super().fit(X, y)
 
         X = self.check_numeric_columns(X)
 
         if self.n_components != "mle":
             if 0 < self.n_components <= min(X[self.columns].shape):
                 pass
             else:
-                raise ValueError(
-                    f"""{self.classname()}: n_components {self.n_components} must be between 1 and min(n_samples {X[self.columns].shape[0]}, n_features {X[self.columns].shape[1]}) is {min(X[self.columns].shape)} with svd_solver '{self.svd_solver}'"""
-                )
+                msg = f"{self.classname()}: n_components {self.n_components} must be between 1 and min(n_samples {X[self.columns].shape[0]}, n_features {X[self.columns].shape[1]}) is {min(X[self.columns].shape)} with svd_solver '{self.svd_solver}'"
+                raise ValueError(msg)
 
         self.pca.fit(X[self.columns])
         self.n_components_ = self.pca.n_components_
         self.feature_names_out = [
             self.pca_column_prefix + str(i) for i in range(self.n_components_)
         ]
 
         return self
 
     def transform(self, X):
         """Generate from input pandas DataFrame (X) PCA features and add this column or columns in X.
+
         Parameters
         ----------
         X : pd.DataFrame
             Data to transform.
+
         Returns
         -------
         X : pd.DataFrame
             Input X with additional column or columns (self.interaction_colname) added. These contain the output of
             running the  product pandas DataFrame method on identified combinations.
         """
         X = super().transform(X)
```

### Comparing `tubular-0.3.7/tubular/strings.py` & `tubular-0.3.8/tubular/strings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-This module contains transformers that apply string functions.
-"""
+"""This module contains transformers that apply string functions."""
 
 import pandas as pd
 
 from tubular.base import BaseTransformer
 
 
 class SeriesStrMethodTransformer(BaseTransformer):
@@ -48,69 +46,55 @@
 
     pd_method_name : str
         The name of the pd.Series.str method to call.
 
     """
 
     def __init__(
-        self, new_column_name, pd_method_name, columns, pd_method_kwargs={}, **kwargs
-    ):
-
-        if type(columns) is list:
-
-            if len(columns) > 1:
-
-                raise ValueError(
-                    f"{self.classname()}: columns arg should contain only 1 column name but got {len(columns)}"
-                )
+        self,
+        new_column_name,
+        pd_method_name,
+        columns,
+        pd_method_kwargs={},
+        **kwargs,
+    ) -> None:
+        if type(columns) is list and len(columns) > 1:
+            msg = f"{self.classname()}: columns arg should contain only 1 column name but got {len(columns)}"
+            raise ValueError(msg)
 
         super().__init__(columns=columns, **kwargs)
 
         if type(new_column_name) is not str:
-
-            raise TypeError(
-                f"{self.classname()}: unexpected type ({type(new_column_name)}) for new_column_name, must be str"
-            )
+            msg = f"{self.classname()}: unexpected type ({type(new_column_name)}) for new_column_name, must be str"
+            raise TypeError(msg)
 
         if type(pd_method_name) is not str:
-
-            raise TypeError(
-                f"{self.classname()}: unexpected type ({type(pd_method_name)}) for pd_method_name, expecting str"
-            )
+            msg = f"{self.classname()}: unexpected type ({type(pd_method_name)}) for pd_method_name, expecting str"
+            raise TypeError(msg)
 
         if type(pd_method_kwargs) is not dict:
+            msg = f"{self.classname()}: pd_method_kwargs should be a dict but got type {type(pd_method_kwargs)}"
+            raise TypeError(msg)
 
-            raise TypeError(
-                f"{self.classname()}: pd_method_kwargs should be a dict but got type {type(pd_method_kwargs)}"
-            )
-
-        else:
-
-            for i, k in enumerate(pd_method_kwargs.keys()):
-
-                if not type(k) is str:
-
-                    raise TypeError(
-                        f"{self.classname()}: unexpected type ({type(k)}) for pd_method_kwargs key in position {i}, must be str"
-                    )
+        for i, k in enumerate(pd_method_kwargs.keys()):
+            if type(k) is not str:
+                msg = f"{self.classname()}: unexpected type ({type(k)}) for pd_method_kwargs key in position {i}, must be str"
+                raise TypeError(msg)
 
         self.new_column_name = new_column_name
         self.pd_method_name = pd_method_name
         self.pd_method_kwargs = pd_method_kwargs
 
         try:
-
             ser = pd.Series(["a"])
             getattr(ser.str, pd_method_name)
 
         except Exception as err:
-
-            raise AttributeError(
-                f"""{self.classname()}: error accessing "str.{pd_method_name}" method on pd.Series object - pd_method_name should be a pd.Series.str method"""
-            ) from err
+            msg = f'{self.classname()}: error accessing "str.{pd_method_name}" method on pd.Series object - pd_method_name should be a pd.Series.str method'
+            raise AttributeError(msg) from err
 
     def transform(self, X):
         """Transform specific column on input pandas.DataFrame (X) using the given pandas.Series.str method and
         assign the output back to column in X.
 
         Any keyword arguments set in the pd_method_kwargs attribute are passed onto the pd.Series.str method
         when calling it.
@@ -123,68 +107,65 @@
         Returns
         -------
         X : pd.DataFrame
             Input X with additional column (self.new_column_name) added. These contain the output of
             running the pd.Series.str method.
 
         """
-
         X = super().transform(X)
 
         X[self.new_column_name] = getattr(X[self.columns[0]].str, self.pd_method_name)(
-            **self.pd_method_kwargs
+            **self.pd_method_kwargs,
         )
 
         return X
 
 
 class StringConcatenator(BaseTransformer):
-    """
-    Transformer to combine data from specified columns, of mixed datatypes, into a new column containing one string.
+    """Transformer to combine data from specified columns, of mixed datatypes, into a new column containing one string.
 
     Parameters
     ----------
     columns : str or list of str
         Columns to concatenate.
     new_column : str, default = "new_column"
         New column name
     separator : str, default = " "
         Separator for the new string value
     """
 
-    def __init__(self, columns, new_column="new_column", separator=" "):
-
+    def __init__(self, columns, new_column="new_column", separator=" ") -> None:
         super().__init__(columns=columns, copy=True)
 
         if not isinstance(new_column, str):
-            raise TypeError(f"{self.classname()}: new_column should be a str")
+            msg = f"{self.classname()}: new_column should be a str"
+            raise TypeError(msg)
 
         self.new_column = new_column
 
         if not isinstance(separator, str):
-            raise TypeError(f"{self.classname()}: The separator should be a str")
+            msg = f"{self.classname()}: The separator should be a str"
+            raise TypeError(msg)
 
         self.separator = separator
 
     def transform(self, X):
-        """
-        Combine data from specified columns, of mixed datatypes, into a new column containing one string.
+        """Combine data from specified columns, of mixed datatypes, into a new column containing one string.
 
-         Parameters
+        Parameters
         ----------
         X : df
             Data to concatenate values on.
 
         Returns
         -------
         X : df
             Returns a dataframe with concatenated values.
 
         """
-
         X = super().transform(X)
 
         X[self.new_column] = (
             X[self.columns].astype(str).apply(lambda x: self.separator.join(x), axis=1)
         )
 
         return X
```

### Comparing `tubular-0.3.7/tubular.egg-info/PKG-INFO` & `tubular-0.3.8/tubular.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tubular
-Version: 0.3.7
+Version: 0.3.8
 Summary: Package to perform pre processing steps for machine learning models
 Author: LV GI Data Science Team
 Author-email: #DataSciencePackages@lv.co.uk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -109,8 +109,8 @@
 pytest
 ```
 
 ## Contribute
 
 `tubular` is under active development, we're super excited if you're interested in contributing! 
 
-See the [CONTRIBUTING](https://github.com/lvgig/tubular/blob/main/CONTRIBUTING.md) file for the full details of our working practices.
+See the [CONTRIBUTING](https://github.com/lvgig/tubular/blob/main/CONTRIBUTING.rst) file for the full details of our working practices.
```

