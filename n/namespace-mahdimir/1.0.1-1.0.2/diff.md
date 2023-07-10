# Comparing `tmp/namespace_mahdimir-1.0.1.tar.gz` & `tmp/namespace_mahdimir-1.0.2.tar.gz`

## Comparing `namespace_mahdimir-1.0.1.tar` & `namespace_mahdimir-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 namespace_mahdimir-1.0.1/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namespace_mahdimir-1.0.1/src/namespace_mahdimir/__init__.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 namespace_mahdimir-1.0.1/src/namespace_mahdimir/tse.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 namespace_mahdimir-1.0.1/src/namespace_mahdimir/tse_github_data_url.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 namespace_mahdimir-1.0.1/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 namespace_mahdimir-1.0.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namespace_mahdimir-1.0.1/README.md
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 namespace_mahdimir-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 namespace_mahdimir-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 namespace_mahdimir-1.0.2/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namespace_mahdimir-1.0.2/src/namespace_mahdimir/__init__.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 namespace_mahdimir-1.0.2/src/namespace_mahdimir/tse.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 namespace_mahdimir-1.0.2/src/namespace_mahdimir/tse_github_data_url.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 namespace_mahdimir-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 namespace_mahdimir-1.0.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namespace_mahdimir-1.0.2/README.md
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 namespace_mahdimir-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 namespace_mahdimir-1.0.2/PKG-INFO
```

### Comparing `namespace_mahdimir-1.0.1/src/namespace_mahdimir/tse.py` & `namespace_mahdimir-1.0.2/src/namespace_mahdimir/tse.py`

 * *Files identical despite different names*

### Comparing `namespace_mahdimir-1.0.1/src/namespace_mahdimir/tse_github_data_url.py` & `namespace_mahdimir-1.0.2/src/namespace_mahdimir/tse_github_data_url.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
     """
 
 my_github_username = "imahdimir"
 m = my_github_username + "/"
 
 class GitHubDataUrl :
-    ind_ins = "u-d-Ind-Ins"
+    ind_ins = "d-Ind-Ins"
     id_2_tic = 'd-TSETMC_ID-2-Ticker'
     adj_ret = 'd-Adjusted-Returns'
     rf = 'd-Iran-RiskFree-Rate-Monthly'
     mkt_indx = 'd-TSE-Overall-Index-TEDPIX'
     codal_ltrs = 'd-all-Codal-letters'
     codal_tics_2_ftics = 'd-CodalTicker-2-FirmTicker'
```

### Comparing `namespace_mahdimir-1.0.1/.gitignore` & `namespace_mahdimir-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `namespace_mahdimir-1.0.1/LICENSE` & `namespace_mahdimir-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `namespace_mahdimir-1.0.1/pyproject.toml` & `namespace_mahdimir-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "namespace_mahdimir"
-version = "1.0.1"
+version = "1.0.2"
 authors = [{ name = "Mahdi Mir", email = "imahdimir@gmail.com" }]
 description = "Some Namespaces for Python"
 readme = "README.md"
 license = { file = "LICENSE" }
 dependencies = [
 
 ]
```

### Comparing `namespace_mahdimir-1.0.1/PKG-INFO` & `namespace_mahdimir-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: namespace_mahdimir
-Version: 1.0.1
+Version: 1.0.2
 Summary: Some Namespaces for Python
 Project-URL: Homepage, https://github.com/imahdimir/namespace_mahdimir
 Project-URL: Bug Tracker, https://github.com/imahdimir/namespace_mahdimir/issues
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
```

