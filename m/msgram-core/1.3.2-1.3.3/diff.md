# Comparing `tmp/msgram_core-1.3.2.tar.gz` & `tmp/msgram_core-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgram_core-1.3.2.tar", last modified: Mon Jul  3 01:03:15 2023, max compression
+gzip compressed data, was "msgram_core-1.3.3.tar", last modified: Mon Jul 10 04:16:28 2023, max compression
```

## Comparing `msgram_core-1.3.2.tar` & `msgram_core-1.3.3.tar`

### file list

```diff
@@ -1,38 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:03:15.515213 msgram_core-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34464 2023-07-03 01:02:54.000000 msgram_core-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44641 2023-07-03 01:03:15.515213 msgram_core-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-03 01:02:54.000000 msgram_core-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-03 01:02:54.000000 msgram_core-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 01:03:15.515213 msgram_core-1.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:03:15.511213 msgram_core-1.3.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:03:15.511213 msgram_core-1.3.2/src/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/core/aggregated_normalized_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/core/measures_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/core/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/core/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:03:15.511213 msgram_core-1.3.2/src/msgram_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44641 2023-07-03 01:03:15.000000 msgram_core-1.3.2/src/msgram_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-03 01:03:15.000000 msgram_core-1.3.2/src/msgram_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:03:15.000000 msgram_core-1.3.2/src/msgram_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-03 01:03:15.000000 msgram_core-1.3.2/src/msgram_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-03 01:03:15.000000 msgram_core-1.3.2/src/msgram_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:03:15.515213 msgram_core-1.3.2/src/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/parsers/sonarqube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:03:15.515213 msgram_core-1.3.2/src/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/resources/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:03:15.515213 msgram_core-1.3.2/src/staticfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/staticfiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/staticfiles/default_pre_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    34977 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/staticfiles/sonarqube_available_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/staticfiles/sonarqube_supported_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:03:15.515213 msgram_core-1.3.2/src/util/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/util/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/util/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:03:15.515213 msgram_core-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-03 01:02:54.000000 msgram_core-1.3.2/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:16:28.079086 msgram_core-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34464 2023-07-10 04:16:08.000000 msgram_core-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44641 2023-07-10 04:16:28.079086 msgram_core-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-10 04:16:08.000000 msgram_core-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-10 04:16:08.000000 msgram_core-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 04:16:28.079086 msgram_core-1.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:16:28.075086 msgram_core-1.3.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 04:16:08.000000 msgram_core-1.3.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:16:28.079086 msgram_core-1.3.3/src/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 04:16:08.000000 msgram_core-1.3.3/src/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-07-10 04:16:08.000000 msgram_core-1.3.3/src/core/aggregated_normalized_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-07-10 04:16:08.000000 msgram_core-1.3.3/src/core/measures_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-10 04:16:08.000000 msgram_core-1.3.3/src/core/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-10 04:16:08.000000 msgram_core-1.3.3/src/core/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:16:28.079086 msgram_core-1.3.3/src/msgram_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44641 2023-07-10 04:16:28.000000 msgram_core-1.3.3/src/msgram_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-10 04:16:28.000000 msgram_core-1.3.3/src/msgram_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 04:16:28.000000 msgram_core-1.3.3/src/msgram_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 04:16:28.000000 msgram_core-1.3.3/src/msgram_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 04:16:28.000000 msgram_core-1.3.3/src/msgram_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:16:28.079086 msgram_core-1.3.3/src/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-10 04:16:08.000000 msgram_core-1.3.3/src/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-07-10 04:16:08.000000 msgram_core-1.3.3/src/resources/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:16:28.079086 msgram_core-1.3.3/src/staticfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 04:16:08.000000 msgram_core-1.3.3/src/staticfiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-10 04:16:08.000000 msgram_core-1.3.3/src/staticfiles/default_pre_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-10 04:16:08.000000 msgram_core-1.3.3/src/staticfiles/supported_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:16:28.079086 msgram_core-1.3.3/src/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-10 04:16:08.000000 msgram_core-1.3.3/src/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-10 04:16:08.000000 msgram_core-1.3.3/src/util/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-10 04:16:08.000000 msgram_core-1.3.3/src/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-10 04:16:08.000000 msgram_core-1.3.3/src/util/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:16:28.079086 msgram_core-1.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-10 04:16:08.000000 msgram_core-1.3.3/tests/test_helpers.py
```

### Comparing `msgram_core-1.3.2/LICENSE` & `msgram_core-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `msgram_core-1.3.2/PKG-INFO` & `msgram_core-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram_core
-Version: 1.3.2
+Version: 1.3.3
 Summary: The MeasureSoftGram-Core is a Software system for continuous quality of product observation and multidimensional use in continuous design engineering software and is where you have the innovative mathematical models for software analysis.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram_core-1.3.2/README.md` & `msgram_core-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `msgram_core-1.3.2/pyproject.toml` & `msgram_core-1.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msgram_core"
-version = "1.3.2"
+version = "1.3.3"
 description = "The MeasureSoftGram-Core is a Software system for continuous quality of product observation and multidimensional use in continuous design engineering software and is where you have the innovative mathematical models for software analysis."
 readme = "README.md"
 authors = [
     { name = "MeasureSoftGram", email = "measuresoftgram@gmail.com" }
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

### Comparing `msgram_core-1.3.2/src/core/aggregated_normalized_measures.py` & `msgram_core-1.3.3/src/core/aggregated_normalized_measures.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.3.2/src/core/measures_functions.py` & `msgram_core-1.3.3/src/core/measures_functions.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.3.2/src/core/schemas.py` & `msgram_core-1.3.3/src/core/schemas.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.3.2/src/core/transformations.py` & `msgram_core-1.3.3/src/core/transformations.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.3.2/src/msgram_core.egg-info/PKG-INFO` & `msgram_core-1.3.3/src/msgram_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram-core
-Version: 1.3.2
+Version: 1.3.3
 Summary: The MeasureSoftGram-Core is a Software system for continuous quality of product observation and multidimensional use in continuous design engineering software and is where you have the innovative mathematical models for software analysis.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram_core-1.3.2/src/msgram_core.egg-info/SOURCES.txt` & `msgram_core-1.3.3/src/msgram_core.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -8,20 +8,17 @@
 src/core/schemas.py
 src/core/transformations.py
 src/msgram_core.egg-info/PKG-INFO
 src/msgram_core.egg-info/SOURCES.txt
 src/msgram_core.egg-info/dependency_links.txt
 src/msgram_core.egg-info/requires.txt
 src/msgram_core.egg-info/top_level.txt
-src/parsers/__init__.py
-src/parsers/sonarqube.py
 src/resources/__init__.py
 src/resources/analysis.py
 src/staticfiles/__init__.py
 src/staticfiles/default_pre_config.py
-src/staticfiles/sonarqube_available_metrics.py
-src/staticfiles/sonarqube_supported_metrics.py
+src/staticfiles/supported_metrics.py
 src/util/__init__.py
 src/util/check.py
 src/util/constants.py
 src/util/exceptions.py
 tests/test_helpers.py
```

### Comparing `msgram_core-1.3.2/src/resources/analysis.py` & `msgram_core-1.3.3/src/resources/analysis.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.3.2/src/staticfiles/default_pre_config.py` & `msgram_core-1.3.3/src/staticfiles/default_pre_config.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.3.2/src/staticfiles/sonarqube_supported_metrics.py` & `msgram_core-1.3.3/src/staticfiles/supported_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-SONARQUBE_SUPPORTED_MEASURES = [
+SUPPORTED_MEASURES = [
     {
         "passed_tests": {
             "metrics": [
                 "tests",
                 "test_failures",
                 "test_errors",
             ],
```

### Comparing `msgram_core-1.3.2/src/util/check.py` & `msgram_core-1.3.3/src/util/check.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.3.2/src/util/constants.py` & `msgram_core-1.3.3/src/util/constants.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.3.2/src/util/exceptions.py` & `msgram_core-1.3.3/src/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.3.2/tests/test_helpers.py` & `msgram_core-1.3.3/tests/test_helpers.py`

 * *Files identical despite different names*

