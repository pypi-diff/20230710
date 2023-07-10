# Comparing `tmp/bruneus-0.1.11.tar.gz` & `tmp/bruneus-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bruneus-0.1.11.tar", last modified: Thu Jul  6 01:54:38 2023, max compression
+gzip compressed data, was "bruneus-0.1.12.tar", last modified: Mon Jul 10 04:46:47 2023, max compression
```

## Comparing `bruneus-0.1.11.tar` & `bruneus-0.1.12.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 kreuz45    (501) staff       (20)        0 2023-07-06 01:54:38.170019 bruneus-0.1.11/
--rw-r--r--   0 kreuz45    (501) staff       (20)     1062 2023-07-06 01:40:31.000000 bruneus-0.1.11/LICENSE
--rw-r--r--   0 kreuz45    (501) staff       (20)     1606 2023-07-06 01:54:38.169889 bruneus-0.1.11/PKG-INFO
--rw-r--r--   0 kreuz45    (501) staff       (20)     1102 2023-07-06 01:52:29.000000 bruneus-0.1.11/README.md
--rw-r--r--   0 kreuz45    (501) staff       (20)       38 2023-07-06 01:54:38.170053 bruneus-0.1.11/setup.cfg
--rw-r--r--   0 kreuz45    (501) staff       (20)     1293 2023-07-06 01:41:43.000000 bruneus-0.1.11/setup.py
-drwxr-xr-x   0 kreuz45    (501) staff       (20)        0 2023-07-06 01:54:38.166778 bruneus-0.1.11/src/
-drwxr-xr-x   0 kreuz45    (501) staff       (20)        0 2023-07-06 01:54:38.168771 bruneus-0.1.11/src/bruneus/
--rw-r--r--   0 kreuz45    (501) staff       (20)      219 2023-07-06 01:40:31.000000 bruneus-0.1.11/src/bruneus/__init__.py
--rw-r--r--   0 kreuz45    (501) staff       (20)      277 2023-07-06 01:44:02.000000 bruneus-0.1.11/src/bruneus/bruneus.py
--rw-r--r--   0 kreuz45    (501) staff       (20)     1280 2023-07-06 01:44:21.000000 bruneus-0.1.11/src/bruneus/create_table.py
--rw-r--r--   0 kreuz45    (501) staff       (20)     1755 2023-07-06 01:40:31.000000 bruneus-0.1.11/src/bruneus/export_table.py
--rw-r--r--   0 kreuz45    (501) staff       (20)      285 2023-07-06 01:40:31.000000 bruneus-0.1.11/src/bruneus/naming.py
--rw-r--r--   0 kreuz45    (501) staff       (20)     2815 2023-07-06 01:40:31.000000 bruneus-0.1.11/src/bruneus/select.py
-drwxr-xr-x   0 kreuz45    (501) staff       (20)        0 2023-07-06 01:54:38.169685 bruneus-0.1.11/src/bruneus.egg-info/
--rw-r--r--   0 kreuz45    (501) staff       (20)     1606 2023-07-06 01:54:38.000000 bruneus-0.1.11/src/bruneus.egg-info/PKG-INFO
--rw-r--r--   0 kreuz45    (501) staff       (20)      347 2023-07-06 01:54:38.000000 bruneus-0.1.11/src/bruneus.egg-info/SOURCES.txt
--rw-r--r--   0 kreuz45    (501) staff       (20)        1 2023-07-06 01:54:38.000000 bruneus-0.1.11/src/bruneus.egg-info/dependency_links.txt
--rw-r--r--   0 kreuz45    (501) staff       (20)       74 2023-07-06 01:54:38.000000 bruneus-0.1.11/src/bruneus.egg-info/requires.txt
--rw-r--r--   0 kreuz45    (501) staff       (20)        8 2023-07-06 01:54:38.000000 bruneus-0.1.11/src/bruneus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:46:47.787945 bruneus-0.1.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-10 04:46:38.000000 bruneus-0.1.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-10 04:46:47.787945 bruneus-0.1.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-10 04:46:38.000000 bruneus-0.1.12/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 04:46:47.787945 bruneus-0.1.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-10 04:46:38.000000 bruneus-0.1.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:46:47.783945 bruneus-0.1.12/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:46:47.783945 bruneus-0.1.12/src/bruneus/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-10 04:46:38.000000 bruneus-0.1.12/src/bruneus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-10 04:46:38.000000 bruneus-0.1.12/src/bruneus/bruneus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-10 04:46:38.000000 bruneus-0.1.12/src/bruneus/create_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-10 04:46:38.000000 bruneus-0.1.12/src/bruneus/export_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-10 04:46:38.000000 bruneus-0.1.12/src/bruneus/naming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-10 04:46:38.000000 bruneus-0.1.12/src/bruneus/select.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:46:47.783945 bruneus-0.1.12/src/bruneus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-10 04:46:47.000000 bruneus-0.1.12/src/bruneus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-10 04:46:47.000000 bruneus-0.1.12/src/bruneus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 04:46:47.000000 bruneus-0.1.12/src/bruneus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-10 04:46:47.000000 bruneus-0.1.12/src/bruneus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 04:46:47.000000 bruneus-0.1.12/src/bruneus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:46:47.787945 bruneus-0.1.12/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-10 04:46:38.000000 bruneus-0.1.12/tests/test_naming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-10 04:46:38.000000 bruneus-0.1.12/tests/test_select.py
```

### Comparing `bruneus-0.1.11/LICENSE` & `bruneus-0.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `bruneus-0.1.11/PKG-INFO` & `bruneus-0.1.12/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: bruneus
-Version: 0.1.11
+Version: 0.1.12
 Summary: bruneus: BigQuery helper utils.
 Home-page: https://github.com/yokoe/bruneus
+Download-URL: https://github.com/yokoe/bruneus
 Author: yokoe
 Author-email: kreuz45@kreuz45.com
 Maintainer: yokoe
 Maintainer-email: kreuz45@kreuz45.com
 License: MIT
-Download-URL: https://github.com/yokoe/bruneus
 Keywords: bigquery
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bruneus
 [![Maintainability](https://api.codeclimate.com/v1/badges/c9d020ea15b032c4cefb/maintainability)](https://codeclimate.com/github/yokoe/bruneus/maintainability)
@@ -52,9 +51,7 @@
 ```
 
 ## Development
 ### Run tests
 ```
 docker compose run bruneus
 ```
-
-
```

### Comparing `bruneus-0.1.11/README.md` & `bruneus-0.1.12/README.md`

 * *Files identical despite different names*

### Comparing `bruneus-0.1.11/setup.py` & `bruneus-0.1.12/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 DESCRIPTION = "bruneus: BigQuery helper utils."
 NAME = "bruneus"
 AUTHOR = "yokoe"
 AUTHOR_EMAIL = "kreuz45@kreuz45.com"
 URL = "https://github.com/yokoe/bruneus"
 LICENSE = "MIT"
 DOWNLOAD_URL = URL
-VERSION = "0.1.11"
+VERSION = "0.1.12"
 PYTHON_REQUIRES = ">=3.9"
 INSTALL_REQUIRES = [
     "google-cloud-bigquery>=3.4.0",
     "Jinja2>=3.0.0",
     "pandas>=1.4.0",
     "db-dtypes>=1.0.5",
 ]
```

### Comparing `bruneus-0.1.11/src/bruneus/create_table.py` & `bruneus-0.1.12/src/bruneus/create_table.py`

 * *Files identical despite different names*

### Comparing `bruneus-0.1.11/src/bruneus/export_table.py` & `bruneus-0.1.12/src/bruneus/export_table.py`

 * *Files identical despite different names*

### Comparing `bruneus-0.1.11/src/bruneus/select.py` & `bruneus-0.1.12/src/bruneus/select.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,17 @@
             overwrite=overwrite,
             client=self.client,
         )
 
     def to_dataframe(self):
         return self.job().to_dataframe()
 
+    def to_df(self):
+        return self.to_dataframe()
+
 
 def select(
     query: str,
     query_parameters=None,
     client: google.cloud.bigquery.Client = None,
 ):
     return SelectTask(client=client, query=query).params(
```

### Comparing `bruneus-0.1.11/src/bruneus.egg-info/PKG-INFO` & `bruneus-0.1.12/src/bruneus.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: bruneus
-Version: 0.1.11
+Version: 0.1.12
 Summary: bruneus: BigQuery helper utils.
 Home-page: https://github.com/yokoe/bruneus
+Download-URL: https://github.com/yokoe/bruneus
 Author: yokoe
 Author-email: kreuz45@kreuz45.com
 Maintainer: yokoe
 Maintainer-email: kreuz45@kreuz45.com
 License: MIT
-Download-URL: https://github.com/yokoe/bruneus
 Keywords: bigquery
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bruneus
 [![Maintainability](https://api.codeclimate.com/v1/badges/c9d020ea15b032c4cefb/maintainability)](https://codeclimate.com/github/yokoe/bruneus/maintainability)
@@ -52,9 +51,7 @@
 ```
 
 ## Development
 ### Run tests
 ```
 docker compose run bruneus
 ```
-
-
```

