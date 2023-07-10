# Comparing `tmp/datamazing-0.0.6.tar.gz` & `tmp/datamazing-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamazing-0.0.6.tar", max compression
+gzip compressed data, was "datamazing-0.0.7.tar", max compression
```

## Comparing `datamazing-0.0.6.tar` & `datamazing-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       21 2023-06-23 10:50:45.566720 datamazing-0.0.6/datamazing/__init__.py
--rw-r--r--   0        0        0      295 2023-06-23 10:50:45.566720 datamazing-0.0.6/datamazing/pandas/__init__.py
--rw-r--r--   0        0        0      267 2023-06-23 10:50:45.566720 datamazing-0.0.6/datamazing/pandas/datacollection/__init__.py
--rw-r--r--   0        0        0      113 2023-06-23 10:50:45.566720 datamazing-0.0.6/datamazing/pandas/testing/__init__.py
--rw-r--r--   0        0        0      826 2023-06-23 10:50:45.566720 datamazing-0.0.6/datamazing/pandas/testing/assertions.py
--rw-r--r--   0        0        0     3752 2023-06-23 10:50:45.566720 datamazing-0.0.6/datamazing/pandas/testing/data.py
--rw-r--r--   0        0        0        0 2023-06-23 10:50:45.566720 datamazing-0.0.6/datamazing/pandas/transformations/__init__.py
--rw-r--r--   0        0        0      649 2023-06-23 10:50:45.566720 datamazing-0.0.6/datamazing/pandas/transformations/basic.py
--rw-r--r--   0        0        0     1998 2023-06-23 10:50:45.566720 datamazing-0.0.6/datamazing/pandas/transformations/grouping.py
--rw-r--r--   0        0        0      868 2023-06-23 10:50:45.566720 datamazing-0.0.6/datamazing/pandas/transformations/resampling.py
--rw-r--r--   0        0        0      660 2023-06-23 10:50:45.566720 datamazing-0.0.6/datamazing/pandas/types.py
--rw-r--r--   0        0        0      690 2023-06-23 10:50:45.566720 datamazing-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 datamazing-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       21 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/__init__.py
+-rw-r--r--   0        0        0      295 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/pandas/__init__.py
+-rw-r--r--   0        0        0      267 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/pandas/datacollection/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/pandas/testing/__init__.py
+-rw-r--r--   0        0        0      826 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/pandas/testing/assertions.py
+-rw-r--r--   0        0        0     3752 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/pandas/testing/data.py
+-rw-r--r--   0        0        0        0 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/pandas/transformations/__init__.py
+-rw-r--r--   0        0        0      649 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/pandas/transformations/basic.py
+-rw-r--r--   0        0        0     2763 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/pandas/transformations/grouping.py
+-rw-r--r--   0        0        0      868 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/pandas/transformations/resampling.py
+-rw-r--r--   0        0        0      660 2023-07-10 09:30:34.668805 datamazing-0.0.7/datamazing/pandas/types.py
+-rw-r--r--   0        0        0      690 2023-07-10 09:30:34.672805 datamazing-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 datamazing-0.0.7/PKG-INFO
```

### Comparing `datamazing-0.0.6/datamazing/pandas/testing/assertions.py` & `datamazing-0.0.7/datamazing/pandas/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.6/datamazing/pandas/testing/data.py` & `datamazing-0.0.7/datamazing/pandas/testing/data.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.6/datamazing/pandas/transformations/basic.py` & `datamazing-0.0.7/datamazing/pandas/transformations/basic.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.6/datamazing/pandas/transformations/resampling.py` & `datamazing-0.0.7/datamazing/pandas/transformations/resampling.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.6/datamazing/pandas/types.py` & `datamazing-0.0.7/datamazing/pandas/types.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.6/pyproject.toml` & `datamazing-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datamazing"
-version = "0.0.6"
+version = "0.0.7"
 description = "Package for working with pandas Dataset, but wit specialized functions used for Energinet"
 authors = ["Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "datamazing" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `datamazing-0.0.6/PKG-INFO` & `datamazing-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamazing
-Version: 0.0.6
+Version: 0.0.7
 Summary: Package for working with pandas Dataset, but wit specialized functions used for Energinet
 Author: Mikkel Ladekarl Folmersen Nygaard
 Author-email: mny@energinet.dk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

