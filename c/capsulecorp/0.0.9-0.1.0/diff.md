# Comparing `tmp/capsulecorp-0.0.9.tar.gz` & `tmp/capsulecorp-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capsulecorp-0.0.9.tar", last modified: Mon Feb 20 19:07:30 2023, max compression
+gzip compressed data, was "capsulecorp-0.1.0.tar", last modified: Mon Jul 10 15:02:18 2023, max compression
```

## Comparing `capsulecorp-0.0.9.tar` & `capsulecorp-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-02-20 19:07:30.561112 capsulecorp-0.0.9/
--rw-r--r--   0 daless383   (502) staff       (20)    11357 2023-02-13 20:25:15.000000 capsulecorp-0.0.9/LICENSE
--rw-r--r--   0 daless383   (502) staff       (20)      416 2023-02-20 19:07:30.560795 capsulecorp-0.0.9/PKG-INFO
--rw-r--r--   0 daless383   (502) staff       (20)       99 2023-02-13 20:25:15.000000 capsulecorp-0.0.9/README.md
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-02-20 19:07:30.558177 capsulecorp-0.0.9/capsulecorp/
--rw-r--r--   0 daless383   (502) staff       (20)       63 2023-02-14 15:14:02.000000 capsulecorp-0.0.9/capsulecorp/__init__.py
--rw-r--r--   0 daless383   (502) staff       (20)    11476 2023-02-20 19:02:38.000000 capsulecorp-0.0.9/capsulecorp/utils.py
--rw-r--r--   0 daless383   (502) staff       (20)      269 2023-02-20 18:55:49.000000 capsulecorp-0.0.9/capsulecorp/version.py
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-02-20 19:07:30.560406 capsulecorp-0.0.9/capsulecorp.egg-info/
--rw-r--r--   0 daless383   (502) staff       (20)      416 2023-02-20 19:07:30.000000 capsulecorp-0.0.9/capsulecorp.egg-info/PKG-INFO
--rw-r--r--   0 daless383   (502) staff       (20)      283 2023-02-20 19:07:30.000000 capsulecorp-0.0.9/capsulecorp.egg-info/SOURCES.txt
--rw-r--r--   0 daless383   (502) staff       (20)        1 2023-02-20 19:07:30.000000 capsulecorp-0.0.9/capsulecorp.egg-info/dependency_links.txt
--rw-r--r--   0 daless383   (502) staff       (20)       55 2023-02-20 19:07:30.000000 capsulecorp-0.0.9/capsulecorp.egg-info/requires.txt
--rw-r--r--   0 daless383   (502) staff       (20)       12 2023-02-20 19:07:30.000000 capsulecorp-0.0.9/capsulecorp.egg-info/top_level.txt
--rw-r--r--   0 daless383   (502) staff       (20)       86 2023-02-14 15:04:49.000000 capsulecorp-0.0.9/pyproject.toml
--rw-r--r--   0 daless383   (502) staff       (20)       38 2023-02-20 19:07:30.561224 capsulecorp-0.0.9/setup.cfg
--rw-r--r--   0 daless383   (502) staff       (20)     6493 2023-02-20 18:55:51.000000 capsulecorp-0.0.9/setup.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-10 15:02:18.458333 capsulecorp-0.1.0/
+-rw-r--r--   0 daless383   (502) staff       (20)    11357 2023-02-13 20:25:15.000000 capsulecorp-0.1.0/LICENSE
+-rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-10 15:02:18.457821 capsulecorp-0.1.0/PKG-INFO
+-rw-r--r--   0 daless383   (502) staff       (20)       99 2023-02-13 20:25:15.000000 capsulecorp-0.1.0/README.md
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-10 15:02:18.450141 capsulecorp-0.1.0/capsulecorp/
+-rw-r--r--   0 daless383   (502) staff       (20)       63 2023-02-14 15:14:02.000000 capsulecorp-0.1.0/capsulecorp/__init__.py
+-rw-r--r--   0 daless383   (502) staff       (20)     7967 2023-05-04 16:53:29.000000 capsulecorp-0.1.0/capsulecorp/query_driver.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-10 15:02:18.456932 capsulecorp-0.1.0/capsulecorp/utilities/
+-rw-r--r--   0 daless383   (502) staff       (20)        0 2023-07-10 14:36:34.000000 capsulecorp-0.1.0/capsulecorp/utilities/__init__.py
+-rw-r--r--   0 daless383   (502) staff       (20)     5686 2023-07-10 14:56:05.000000 capsulecorp-0.1.0/capsulecorp/utilities/databricks_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)     2320 2023-05-18 14:36:49.000000 capsulecorp-0.1.0/capsulecorp/utilities/slack_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)    14740 2023-07-06 17:37:40.000000 capsulecorp-0.1.0/capsulecorp/utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)      269 2023-07-10 14:39:24.000000 capsulecorp-0.1.0/capsulecorp/version.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-10 15:02:18.454634 capsulecorp-0.1.0/capsulecorp.egg-info/
+-rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-10 15:02:17.000000 capsulecorp-0.1.0/capsulecorp.egg-info/PKG-INFO
+-rw-r--r--   0 daless383   (502) staff       (20)      424 2023-07-10 15:02:18.000000 capsulecorp-0.1.0/capsulecorp.egg-info/SOURCES.txt
+-rw-r--r--   0 daless383   (502) staff       (20)        1 2023-07-10 15:02:17.000000 capsulecorp-0.1.0/capsulecorp.egg-info/dependency_links.txt
+-rw-r--r--   0 daless383   (502) staff       (20)       91 2023-07-10 15:02:18.000000 capsulecorp-0.1.0/capsulecorp.egg-info/requires.txt
+-rw-r--r--   0 daless383   (502) staff       (20)       12 2023-07-10 15:02:18.000000 capsulecorp-0.1.0/capsulecorp.egg-info/top_level.txt
+-rw-r--r--   0 daless383   (502) staff       (20)       86 2023-02-14 15:04:49.000000 capsulecorp-0.1.0/pyproject.toml
+-rw-r--r--   0 daless383   (502) staff       (20)       38 2023-07-10 15:02:18.458521 capsulecorp-0.1.0/setup.cfg
+-rw-r--r--   0 daless383   (502) staff       (20)     6584 2023-07-10 14:39:22.000000 capsulecorp-0.1.0/setup.py
```

### Comparing `capsulecorp-0.0.9/LICENSE` & `capsulecorp-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.0.9/capsulecorp/utils.py` & `capsulecorp-0.1.0/capsulecorp/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,26 @@
-""" Capsule Corp Utilities Module """
+"""
+Capsule Corp Utilities Module
+
+TODO: Break this up into a subpackage and separate the methods logically into
+different modules.
+"""
 import io
 import os
 import datetime
 import itertools
 from concurrent.futures import ThreadPoolExecutor
 import zipfile
 from urllib.parse import urlparse
 import logging
 import yaml
 import boto3
 import numpy as np
 import pandas as pd
+from scipy.stats import shapiro, normaltest
 
 # Setup logging
 logging.basicConfig(
     level=logging.INFO,
     format="%(levelname)s:%(message)s")
 logging.getLogger("py4j").setLevel(logging.ERROR)
 
@@ -69,19 +75,19 @@
 
         Returns:
             list of unique key value dict permutations
     """
     # Set default
     dict_permutations = [{}]
     # Check whether input is valid nonempty dictionary
-    if (type(raw_dict) == dict) and (len(raw_dict) > 0):
+    if isinstance(raw_dict, dict) and (len(raw_dict) > 0):
         # Make sure all values are lists
         dict_of_lists = {}
         for key, value in raw_dict.items():
-            if type(value) != list:
+            if not isinstance(value, list):
                 dict_of_lists[key] = [value]
             else:
                 dict_of_lists[key] = value
         # Create all unique permutations
         keys, values = zip(*dict_of_lists.items())
         dict_permutations = [
             dict(zip(keys, v)) for v in itertools.product(*values)]
@@ -238,28 +244,29 @@
         Args:
             bucket_name (str): name of s3 bucket
             s3_path (str): path to s3 file
 
         Returns:
             boolean for whether the path exists
     """
-    s3 = boto3.client(
+    s3_client = boto3.client(
         's3', aws_access_key_id=S3_ACCESS_KEY,
         aws_secret_access_key=S3_SECRET_KEY)
     # --- Setup key ---
     # Remove bucket from path to get prefix if applicable
     if bucket_name in s3_path:
         s3_prefix = s3_path.split(bucket_name)[1][1:]
     else:
         s3_prefix = s3_path
     # Get prefix to the left of the glob character
     if "*" in s3_prefix:
         s3_prefix = s3_prefix.split("*")[0]
     # Get list response
-    resp = s3.list_objects(Bucket=bucket_name, Prefix=s3_prefix, MaxKeys=1)
+    resp = s3_client.list_objects(
+        Bucket=bucket_name, Prefix=s3_prefix, MaxKeys=1)
 
     return "Contents" in resp
 
 
 def get_responses(
         bucket, prefix, s3_access_key=S3_ACCESS_KEY,
         s3_secret_key=S3_SECRET_KEY):
@@ -324,20 +331,20 @@
             old_key (str): old s3 prefix
             new_key (str): new s3 prefix
 
         Returns:
             success boolean and exception message
     """
     success = True
-    s3 = boto3.resource(
+    s3_client = boto3.resource(
         's3', aws_access_key_id=S3_ACCESS_KEY,
         aws_secret_access_key=S3_SECRET_KEY)
     # Try to copy file
     try:
-        s3.Object(bucket, new_key).copy_from(
+        s3_client.Object(bucket, new_key).copy_from(
             CopySource=f"{bucket}/" + old_key)
     # If the copy fails for any reason set success to False
     except Exception as e:
         success = False
 
     return success
 
@@ -381,7 +388,119 @@
         copies_failed = len(failed_tasks)
         if copies_failed > 0:
             logging.error(
                 f"WARNING: {copies_failed} copies failed.")
             success = False
 
     return success
+
+
+def pooled_stddev(stddevs, n):
+    """
+        This method will calculate the pooled standard deviation across a
+        group of samples given each samples standard deviation and size.
+
+        Source: https://www.statisticshowto.com/pooled-standard-deviation/
+
+        Args:
+            stddevs (numpy.ndarray): standard deviations of samples
+            n (numpy.ndarray): samples sizes
+
+        Returns:
+            pooled stddev
+    """
+    return np.sqrt(np.sum([
+        (n[i] - 1) * np.power(stddevs[i], 2)
+        for i in range(len(n))]) / (np.sum(n) - len(n)))
+
+
+def get_null_columns(df):
+    """
+        This function will get null columns.
+
+        Args:
+            df (pandas.core.frame.DataFrame): pandas DataFrame
+
+        Returns:
+            list of non null columns
+    """
+    return [
+        column_header
+        for column_header, is_null in df.isnull().all().iteritems()
+        if is_null]
+
+
+def get_non_null_columns(df):
+    """
+        This function will get non null columns.
+
+        Args:
+            df (pandas.core.frame.DataFrame): pandas DataFrame
+
+        Returns:
+            list of non null columns
+    """
+    return [
+        column_header
+        for column_header, is_null in df.isnull().all().iteritems()
+        if not is_null]
+
+
+def test_normal(values, alpha=0.05):
+    """
+        This method will test whether distributions are guassian.
+
+        Args:
+            values (np.array):
+
+        Return:
+            boolean result
+    """
+    shapiro_stat, shapiro_p = shapiro(values)
+    normal_stat, normal_p = normaltest(values)
+    is_normal = np.all([p < alpha for p in (shapiro_p, normal_p)])
+
+    return is_normal
+
+
+def collapse_dataframe_columns(df):
+    """
+        This method will collapse DataFrame column values into a list.
+
+        Args:
+            df (pandas.DataFrame): pandas DataFrame
+
+        Returns:
+            list of unique column values
+    """
+    return list(set(itertools.chain.from_iterable([
+        df[~df[col].isnull()][col].values.tolist() for col in df.columns])))
+
+
+def filter_dataframe(
+        df, cols, filter_out=False, use_substring=False,
+        use_startswith=False):
+    """
+        This method will filter a DataFrame by a list of columns.
+
+        Args:
+            df (pandas.DataFrame): pandas DataFrame
+            cols (list): list of desired columns
+            filter_out (bool): switch to filter columns out of DataFrame
+            use_substring (bool): switch to use substring logic
+            use_startswith (bool): switch to use startswith logic
+
+        Returns:
+            filtered DataFrame
+    """
+    # Create condition lambda function
+    if use_substring:
+        f = lambda c: any(str(substring) in c for substring in cols)
+    elif use_startswith:
+        f = lambda c: any(c.startswith(substring) for substring in cols)
+    else:
+        f = lambda c: c in cols
+    # Return DataFrame with filtered columns
+    if filter_out:
+        return df.loc[:, [c for c in df.columns if not f(c)]]
+    else:
+        return df.loc[:, [c for c in df.columns if f(c)]]
```

### Comparing `capsulecorp-0.0.9/setup.py` & `capsulecorp-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,19 @@
         'Development Status :: 3 - Alpha',
         'Programming Language :: Python :: 3.9',
     ],
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
     python_requires='>=3.9',
     # Dependencies
     install_requires=[
-        'PyYAML>=5.3',
-        'numpy>=1.20.3',
-        'pandas>=1.3.4',
-        'boto3==1.24.75'
+        'PyYAML',
+        'numpy',
+        'pandas',
+        'boto3',
+        'psycopg2-binary==2.9.3',
+        'PyMySQL',
+        'slack-sdk',
+        'tabulate',
+        'databricks-cli'
     ],
     include_package_data=True
 )
```

