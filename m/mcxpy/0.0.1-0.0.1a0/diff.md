# Comparing `tmp/mcxpy-0.0.1.tar.gz` & `tmp/mcxpy-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcxpy-0.0.1.tar", last modified: Mon Jul 10 18:04:34 2023, max compression
+gzip compressed data, was "mcxpy-0.0.1a0.tar", last modified: Mon Jul 10 18:34:39 2023, max compression
```

## Comparing `mcxpy-0.0.1.tar` & `mcxpy-0.0.1a0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 18:04:34.773804 mcxpy-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-07-10 16:20:44.000000 mcxpy-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2853 2023-07-10 18:04:34.749781 mcxpy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1210 2023-07-10 16:45:37.000000 mcxpy-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 18:04:34.668716 mcxpy-0.0.1/mcxpy/
--rw-rw-rw-   0        0        0      405 2023-07-09 17:22:38.000000 mcxpy-0.0.1/mcxpy/__init__.py
--rw-rw-rw-   0        0        0      393 2023-07-09 17:22:53.000000 mcxpy-0.0.1/mcxpy/__init__.pyi
--rw-rw-rw-   0        0        0    13363 2023-07-09 17:33:24.000000 mcxpy-0.0.1/mcxpy/mcx.py
--rw-rw-rw-   0        0        0     1240 2023-07-09 17:23:32.000000 mcxpy-0.0.1/mcxpy/mcx.pyi
--rw-rw-rw-   0        0        0        0 2023-07-09 17:16:19.000000 mcxpy-0.0.1/mcxpy/py.typed
-drwxrwxrwx   0        0        0        0 2023-07-10 18:04:34.746780 mcxpy-0.0.1/mcxpy.egg-info/
--rw-rw-rw-   0        0        0     2853 2023-07-10 18:04:33.000000 mcxpy-0.0.1/mcxpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-07-10 18:04:34.000000 mcxpy-0.0.1/mcxpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 18:04:34.000000 mcxpy-0.0.1/mcxpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-10 18:04:34.000000 mcxpy-0.0.1/mcxpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-10 18:04:34.000000 mcxpy-0.0.1/mcxpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      609 2023-07-10 18:03:58.000000 mcxpy-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-10 18:04:34.774788 mcxpy-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-10 18:34:39.064533 mcxpy-0.0.1a0/
+-rw-rw-rw-   0        0        0     1091 2023-07-10 16:20:44.000000 mcxpy-0.0.1a0/LICENSE
+-rw-rw-rw-   0        0        0     2875 2023-07-10 18:34:39.041530 mcxpy-0.0.1a0/PKG-INFO
+-rw-rw-rw-   0        0        0     1230 2023-07-10 18:29:11.000000 mcxpy-0.0.1a0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 18:34:38.991517 mcxpy-0.0.1a0/mcxpy/
+-rw-rw-rw-   0        0        0      405 2023-07-09 17:22:38.000000 mcxpy-0.0.1a0/mcxpy/__init__.py
+-rw-rw-rw-   0        0        0      393 2023-07-09 17:22:53.000000 mcxpy-0.0.1a0/mcxpy/__init__.pyi
+-rw-rw-rw-   0        0        0    13363 2023-07-09 17:33:24.000000 mcxpy-0.0.1a0/mcxpy/mcx.py
+-rw-rw-rw-   0        0        0     1240 2023-07-09 17:23:32.000000 mcxpy-0.0.1a0/mcxpy/mcx.pyi
+-rw-rw-rw-   0        0        0        0 2023-07-09 17:16:19.000000 mcxpy-0.0.1a0/mcxpy/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-10 18:34:39.023524 mcxpy-0.0.1a0/mcxpy.egg-info/
+-rw-rw-rw-   0        0        0     2875 2023-07-10 18:34:38.000000 mcxpy-0.0.1a0/mcxpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-07-10 18:34:38.000000 mcxpy-0.0.1a0/mcxpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 18:34:38.000000 mcxpy-0.0.1a0/mcxpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-10 18:34:38.000000 mcxpy-0.0.1a0/mcxpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-10 18:34:38.000000 mcxpy-0.0.1a0/mcxpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      611 2023-07-10 18:34:03.000000 mcxpy-0.0.1a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-10 18:34:39.064533 mcxpy-0.0.1a0/setup.cfg
```

### Comparing `mcxpy-0.0.1/LICENSE` & `mcxpy-0.0.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcxpy-0.0.1/PKG-INFO` & `mcxpy-0.0.1a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcxpy
-Version: 0.0.1
+Version: 0.0.1a0
 Summary: For fetching mcx data
 Author: Tapan Hazarika
 License: MIT License
         
         Copyright (c)  2023 Tapan Hazarika
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,17 +35,27 @@
 
 Functions:
 
 Below Functions will return data in pandas dataframe.. Any of the functions accepts date/expiry as %d-%m-%Y / 
 datetime.datetime / datetime.date
 
 mcx_bhavcopy(bhavdate) -> Returns bhacopy for the given bhavdate.
+
 mcx_marketwatch() -> Returns marketwatch.
+
 mcx_circulars(from_date, to_date) -> By default returns circulars within 4 days.
+
 mcx_topgainers() -> Returns top gainers.
+
 mcx_toploosers() -> Returns top loosers.
+
 mcx_mostactiveoptions() -> Returns most active options.
+
 mcx_mostactivecontracts() -> Returns most active contracts.
+
 mcx_optionchain(commodity, expiry) -> Returns option chain of the given commodity of the given expiry.
+
 mcx_pcr(expirywise) -> Returns commoditywise pcr if expirywise is False. If not, returns pcr expiry wise.
+
 mcx_expiry(commodity, expirytype) -> By default returns current expiry date of Crudeoil.
+
 mcx_heatmap() -> Returns heatmap dataframe.
```

### Comparing `mcxpy-0.0.1/README.md` & `mcxpy-0.0.1a0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,27 @@
 
 Functions:
 
 Below Functions will return data in pandas dataframe.. Any of the functions accepts date/expiry as %d-%m-%Y / 
 datetime.datetime / datetime.date
 
 mcx_bhavcopy(bhavdate) -> Returns bhacopy for the given bhavdate.
+
 mcx_marketwatch() -> Returns marketwatch.
+
 mcx_circulars(from_date, to_date) -> By default returns circulars within 4 days.
+
 mcx_topgainers() -> Returns top gainers.
+
 mcx_toploosers() -> Returns top loosers.
+
 mcx_mostactiveoptions() -> Returns most active options.
+
 mcx_mostactivecontracts() -> Returns most active contracts.
+
 mcx_optionchain(commodity, expiry) -> Returns option chain of the given commodity of the given expiry.
+
 mcx_pcr(expirywise) -> Returns commoditywise pcr if expirywise is False. If not, returns pcr expiry wise.
+
 mcx_expiry(commodity, expirytype) -> By default returns current expiry date of Crudeoil.
+
 mcx_heatmap() -> Returns heatmap dataframe.
```

### Comparing `mcxpy-0.0.1/mcxpy/mcx.py` & `mcxpy-0.0.1a0/mcxpy/mcx.py`

 * *Files identical despite different names*

### Comparing `mcxpy-0.0.1/mcxpy/mcx.pyi` & `mcxpy-0.0.1a0/mcxpy/mcx.pyi`

 * *Files identical despite different names*

### Comparing `mcxpy-0.0.1/mcxpy.egg-info/PKG-INFO` & `mcxpy-0.0.1a0/mcxpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcxpy
-Version: 0.0.1
+Version: 0.0.1a0
 Summary: For fetching mcx data
 Author: Tapan Hazarika
 License: MIT License
         
         Copyright (c)  2023 Tapan Hazarika
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,17 +35,27 @@
 
 Functions:
 
 Below Functions will return data in pandas dataframe.. Any of the functions accepts date/expiry as %d-%m-%Y / 
 datetime.datetime / datetime.date
 
 mcx_bhavcopy(bhavdate) -> Returns bhacopy for the given bhavdate.
+
 mcx_marketwatch() -> Returns marketwatch.
+
 mcx_circulars(from_date, to_date) -> By default returns circulars within 4 days.
+
 mcx_topgainers() -> Returns top gainers.
+
 mcx_toploosers() -> Returns top loosers.
+
 mcx_mostactiveoptions() -> Returns most active options.
+
 mcx_mostactivecontracts() -> Returns most active contracts.
+
 mcx_optionchain(commodity, expiry) -> Returns option chain of the given commodity of the given expiry.
+
 mcx_pcr(expirywise) -> Returns commoditywise pcr if expirywise is False. If not, returns pcr expiry wise.
+
 mcx_expiry(commodity, expirytype) -> By default returns current expiry date of Crudeoil.
+
 mcx_heatmap() -> Returns heatmap dataframe.
```

### Comparing `mcxpy-0.0.1/pyproject.toml` & `mcxpy-0.0.1a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mcxpy"
-version = "0.0.1"
+version = "0.0.1.a"
 description = "For fetching mcx data"
 authors = [{ name = "Tapan Hazarika" }]
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = ["pandas>=2.0.0","requests"]
 classifiers = [
     "Programming Language :: Python :: 3",
```

