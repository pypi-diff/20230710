# Comparing `tmp/dynamodb-csv-1.5.0.tar.gz` & `tmp/dynamodb-csv-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamodb-csv-1.5.0.tar", last modified: Mon Feb 20 14:36:35 2023, max compression
+gzip compressed data, was "dynamodb-csv-1.5.1.tar", last modified: Mon Jul 10 14:55:09 2023, max compression
```

## Comparing `dynamodb-csv-1.5.0.tar` & `dynamodb-csv-1.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 14:36:35.394641 dynamodb-csv-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-02-20 14:36:22.000000 dynamodb-csv-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-02-20 14:36:35.394641 dynamodb-csv-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-02-20 14:36:22.000000 dynamodb-csv-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 14:36:35.390641 dynamodb-csv-1.5.0/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 14:36:22.000000 dynamodb-csv-1.5.0/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 14:36:35.390641 dynamodb-csv-1.5.0/app/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-20 14:36:22.000000 dynamodb-csv-1.5.0/app/dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-02-20 14:36:22.000000 dynamodb-csv-1.5.0/app/dynamodb/csv_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-02-20 14:36:22.000000 dynamodb-csv-1.5.0/app/dynamodb/csv_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-02-20 14:36:22.000000 dynamodb-csv-1.5.0/app/dynamodb/move.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-02-20 14:36:22.000000 dynamodb-csv-1.5.0/app/dynamodb/truncate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-02-20 14:36:22.000000 dynamodb-csv-1.5.0/app/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 14:36:35.390641 dynamodb-csv-1.5.0/dynamodb_csv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-02-20 14:36:35.000000 dynamodb-csv-1.5.0/dynamodb_csv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-02-20 14:36:35.000000 dynamodb-csv-1.5.0/dynamodb_csv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 14:36:35.000000 dynamodb-csv-1.5.0/dynamodb_csv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-20 14:36:35.000000 dynamodb-csv-1.5.0/dynamodb_csv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 14:36:35.000000 dynamodb-csv-1.5.0/dynamodb_csv.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-20 14:36:35.000000 dynamodb-csv-1.5.0/dynamodb_csv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-20 14:36:35.000000 dynamodb-csv-1.5.0/dynamodb_csv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-02-20 14:36:35.394641 dynamodb-csv-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 14:36:22.000000 dynamodb-csv-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:09.639480 dynamodb-csv-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-10 14:54:57.000000 dynamodb-csv-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-07-10 14:55:09.643480 dynamodb-csv-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-07-10 14:54:57.000000 dynamodb-csv-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:09.639480 dynamodb-csv-1.5.1/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:54:57.000000 dynamodb-csv-1.5.1/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:09.639480 dynamodb-csv-1.5.1/app/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-10 14:54:57.000000 dynamodb-csv-1.5.1/app/dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-10 14:54:57.000000 dynamodb-csv-1.5.1/app/dynamodb/csv_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-10 14:54:57.000000 dynamodb-csv-1.5.1/app/dynamodb/csv_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-10 14:54:57.000000 dynamodb-csv-1.5.1/app/dynamodb/move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-10 14:54:57.000000 dynamodb-csv-1.5.1/app/dynamodb/truncate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-10 14:54:57.000000 dynamodb-csv-1.5.1/app/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:55:09.639480 dynamodb-csv-1.5.1/dynamodb_csv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-07-10 14:55:09.000000 dynamodb-csv-1.5.1/dynamodb_csv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-10 14:55:09.000000 dynamodb-csv-1.5.1/dynamodb_csv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:55:09.000000 dynamodb-csv-1.5.1/dynamodb_csv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-10 14:55:09.000000 dynamodb-csv-1.5.1/dynamodb_csv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:55:09.000000 dynamodb-csv-1.5.1/dynamodb_csv.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 14:55:09.000000 dynamodb-csv-1.5.1/dynamodb_csv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 14:55:09.000000 dynamodb-csv-1.5.1/dynamodb_csv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-10 14:55:09.643480 dynamodb-csv-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 14:54:57.000000 dynamodb-csv-1.5.1/setup.py
```

### Comparing `dynamodb-csv-1.5.0/LICENSE` & `dynamodb-csv-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamodb-csv-1.5.0/PKG-INFO` & `dynamodb-csv-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: dynamodb-csv
-Version: 1.5.0
+Version: 1.5.1
 Summary: A utility that allows CSV import / export to DynamoDB on the command line
 Home-page: https://github.com/danishi/dynamodb-csv
 Author: danishi
 Author-email: dns2developer@gmail.com
 License: MIT
 Keywords: AWS,DynamoDB,CSV
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DynamoDB CSV utility
 
 [![ci](https://github.com/danishi/DynamoDB-CSV/actions/workflows/ci.yaml/badge.svg?branch=master)](https://github.com/danishi/DynamoDBImportCSV/actions/workflows/ci.yaml)
 [![codecov](https://codecov.io/gh/danishi/dynamodb-csv/branch/master/graph/badge.svg?token=KRA27MJN42)](https://codecov.io/gh/danishi/dynamodb-csv)
+[![Maintainability](https://api.codeclimate.com/v1/badges/c1d2a51bbd72d6198e0c/maintainability)](https://codeclimate.com/github/danishi/dynamodb-csv/maintainability)
 ![MIT](https://img.shields.io/github/license/danishi/DynamoDB-CSV)
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/dynamodb-csv.svg?color=%2334D058)
 [![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)
 [![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
 [![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)
 [![PyPI](https://badge.fury.io/py/dynamodb-csv.svg)](https://badge.fury.io/py/dynamodb-csv)
 [![Downloads](https://pepy.tech/badge/dynamodb-csv)](https://pepy.tech/project/dynamodb-csv)
 [![Downloads week](https://pepy.tech/badge/dynamodb-csv/week)](https://pepy.tech/project/dynamodb-csv)
 [![Downloads month](https://pepy.tech/badge/dynamodb-csv/month)](https://pepy.tech/project/dynamodb-csv)
 [![Docker Pulls](https://img.shields.io/docker/pulls/danishi/dynamodb-csv)](https://hub.docker.com/r/danishi/dynamodb-csv)
+[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
 
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/danishi)
 
 ![DynamoDBCSV](https://user-images.githubusercontent.com/56535085/159007555-e72d1c26-eb44-46ca-bc38-c752164995bf.png)
 
 A utility that allows CSV import / export to DynamoDB on the command line
 
@@ -46,14 +47,16 @@
 ## Introduction
 
 I made this command because I didn't have any tools to satisfy my modest desire to make it easy to import CSV files into DynamoDB.
 Written in a simple Python script, it's easy to parse and modify.
 
 It works for me.
 
+![terminalizer](https://user-images.githubusercontent.com/13270461/237145047-ec815dad-1ff6-4678-baa4-fd182ee35269.gif)
+
 ## Getting started 🚀
 
 ### Install
 
 ```shell
 $ python -m venv venv
 $ . venv/bin/activate
@@ -375,15 +378,16 @@
 100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 300/300 [00:07<00:00, 40.95it/s]
 my_table truncated
 ```
 
 ### Table move
 
 Move all items from table to table.
-A table with the same schema must be prepared in advance.
+A table with the same schema must be prepared in advance.  
+Table items is not deleted and behaves like a copy.
 
 ```shell
 $ dynamodb-csv --move -t my_table_from my_table_to
 my_table_from scan 300 items
 please wait my_table_to moving
 100%|███████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 300/300 [00:15<00:00, 20.00it/s]
 my_table_to moved 300 items
```

### Comparing `dynamodb-csv-1.5.0/README.md` & `dynamodb-csv-1.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # DynamoDB CSV utility
 
 [![ci](https://github.com/danishi/DynamoDB-CSV/actions/workflows/ci.yaml/badge.svg?branch=master)](https://github.com/danishi/DynamoDBImportCSV/actions/workflows/ci.yaml)
 [![codecov](https://codecov.io/gh/danishi/dynamodb-csv/branch/master/graph/badge.svg?token=KRA27MJN42)](https://codecov.io/gh/danishi/dynamodb-csv)
+[![Maintainability](https://api.codeclimate.com/v1/badges/c1d2a51bbd72d6198e0c/maintainability)](https://codeclimate.com/github/danishi/dynamodb-csv/maintainability)
 ![MIT](https://img.shields.io/github/license/danishi/DynamoDB-CSV)
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/dynamodb-csv.svg?color=%2334D058)
 [![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)
 [![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
 [![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)
 [![PyPI](https://badge.fury.io/py/dynamodb-csv.svg)](https://badge.fury.io/py/dynamodb-csv)
 [![Downloads](https://pepy.tech/badge/dynamodb-csv)](https://pepy.tech/project/dynamodb-csv)
 [![Downloads week](https://pepy.tech/badge/dynamodb-csv/week)](https://pepy.tech/project/dynamodb-csv)
 [![Downloads month](https://pepy.tech/badge/dynamodb-csv/month)](https://pepy.tech/project/dynamodb-csv)
 [![Docker Pulls](https://img.shields.io/docker/pulls/danishi/dynamodb-csv)](https://hub.docker.com/r/danishi/dynamodb-csv)
+[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
 
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/danishi)
 
 ![DynamoDBCSV](https://user-images.githubusercontent.com/56535085/159007555-e72d1c26-eb44-46ca-bc38-c752164995bf.png)
 
 A utility that allows CSV import / export to DynamoDB on the command line
 
@@ -24,14 +26,16 @@
 ## Introduction
 
 I made this command because I didn't have any tools to satisfy my modest desire to make it easy to import CSV files into DynamoDB.
 Written in a simple Python script, it's easy to parse and modify.
 
 It works for me.
 
+![terminalizer](https://user-images.githubusercontent.com/13270461/237145047-ec815dad-1ff6-4678-baa4-fd182ee35269.gif)
+
 ## Getting started 🚀
 
 ### Install
 
 ```shell
 $ python -m venv venv
 $ . venv/bin/activate
@@ -353,15 +357,16 @@
 100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 300/300 [00:07<00:00, 40.95it/s]
 my_table truncated
 ```
 
 ### Table move
 
 Move all items from table to table.
-A table with the same schema must be prepared in advance.
+A table with the same schema must be prepared in advance.  
+Table items is not deleted and behaves like a copy.
 
 ```shell
 $ dynamodb-csv --move -t my_table_from my_table_to
 my_table_from scan 300 items
 please wait my_table_to moving
 100%|███████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 300/300 [00:15<00:00, 20.00it/s]
 my_table_to moved 300 items
```

### Comparing `dynamodb-csv-1.5.0/app/dynamodb/csv_export.py` & `dynamodb-csv-1.5.1/app/dynamodb/csv_export.py`

 * *Files identical despite different names*

### Comparing `dynamodb-csv-1.5.0/app/dynamodb/csv_import.py` & `dynamodb-csv-1.5.1/app/dynamodb/csv_import.py`

 * *Files identical despite different names*

### Comparing `dynamodb-csv-1.5.0/app/dynamodb/move.py` & `dynamodb-csv-1.5.1/app/dynamodb/move.py`

 * *Files identical despite different names*

### Comparing `dynamodb-csv-1.5.0/app/dynamodb/truncate.py` & `dynamodb-csv-1.5.1/app/dynamodb/truncate.py`

 * *Files identical despite different names*

### Comparing `dynamodb-csv-1.5.0/app/main.py` & `dynamodb-csv-1.5.1/app/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import configparser
 import argparse
 import sys
 from typing import Any, Tuple, List
 
 from app.dynamodb import csv_import, csv_export, truncate, move
 
-__version__ = "1.5.0"
+__version__ = "1.5.1"
 config_file = "config.ini"
 
 
 def main() -> None:
     """Main routine
     """
     (message, code) = execute()
@@ -20,15 +20,15 @@
     sys.exit(code)
 
 
 def execute() -> Tuple:
     """Command execute
 
     Raises:
-        ValueError: invalied config
+        ValueError: invalid config
 
     Returns:
         Tuple: result message and exit code
     """
 
     result = "No operations."
 
@@ -136,18 +136,20 @@
         config.read_dict({"AWS": {"ENDPOINT_URL": ""}})
         config.read(config_file)
 
         endpoint_url = None
         if config.get("AWS", "ENDPOINT_URL"):
             endpoint_url = config.get("AWS", "ENDPOINT_URL")
         dynamodb = boto3.resource("dynamodb",
-            region_name=config.get("AWS", "REGION"),
-            aws_access_key_id=config.get("AWS", "AWS_ACCESS_KEY_ID"),
-            aws_secret_access_key=config.get("AWS", "AWS_SECRET_ACCESS_KEY"),
-            endpoint_url=endpoint_url)
+                                  region_name=config.get("AWS", "REGION"),
+                                  aws_access_key_id=config.get(
+                                      "AWS", "AWS_ACCESS_KEY_ID"),
+                                  aws_secret_access_key=config.get(
+                                      "AWS", "AWS_SECRET_ACCESS_KEY"),
+                                  endpoint_url=endpoint_url)
 
     tables = []
     for table in args.table:
         tables.append(dynamodb.Table(table))
 
     return tables
```

### Comparing `dynamodb-csv-1.5.0/dynamodb_csv.egg-info/PKG-INFO` & `dynamodb-csv-1.5.1/dynamodb_csv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: dynamodb-csv
-Version: 1.5.0
+Version: 1.5.1
 Summary: A utility that allows CSV import / export to DynamoDB on the command line
 Home-page: https://github.com/danishi/dynamodb-csv
 Author: danishi
 Author-email: dns2developer@gmail.com
 License: MIT
 Keywords: AWS,DynamoDB,CSV
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DynamoDB CSV utility
 
 [![ci](https://github.com/danishi/DynamoDB-CSV/actions/workflows/ci.yaml/badge.svg?branch=master)](https://github.com/danishi/DynamoDBImportCSV/actions/workflows/ci.yaml)
 [![codecov](https://codecov.io/gh/danishi/dynamodb-csv/branch/master/graph/badge.svg?token=KRA27MJN42)](https://codecov.io/gh/danishi/dynamodb-csv)
+[![Maintainability](https://api.codeclimate.com/v1/badges/c1d2a51bbd72d6198e0c/maintainability)](https://codeclimate.com/github/danishi/dynamodb-csv/maintainability)
 ![MIT](https://img.shields.io/github/license/danishi/DynamoDB-CSV)
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/dynamodb-csv.svg?color=%2334D058)
 [![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)
 [![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
 [![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)
 [![PyPI](https://badge.fury.io/py/dynamodb-csv.svg)](https://badge.fury.io/py/dynamodb-csv)
 [![Downloads](https://pepy.tech/badge/dynamodb-csv)](https://pepy.tech/project/dynamodb-csv)
 [![Downloads week](https://pepy.tech/badge/dynamodb-csv/week)](https://pepy.tech/project/dynamodb-csv)
 [![Downloads month](https://pepy.tech/badge/dynamodb-csv/month)](https://pepy.tech/project/dynamodb-csv)
 [![Docker Pulls](https://img.shields.io/docker/pulls/danishi/dynamodb-csv)](https://hub.docker.com/r/danishi/dynamodb-csv)
+[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
 
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/danishi)
 
 ![DynamoDBCSV](https://user-images.githubusercontent.com/56535085/159007555-e72d1c26-eb44-46ca-bc38-c752164995bf.png)
 
 A utility that allows CSV import / export to DynamoDB on the command line
 
@@ -46,14 +47,16 @@
 ## Introduction
 
 I made this command because I didn't have any tools to satisfy my modest desire to make it easy to import CSV files into DynamoDB.
 Written in a simple Python script, it's easy to parse and modify.
 
 It works for me.
 
+![terminalizer](https://user-images.githubusercontent.com/13270461/237145047-ec815dad-1ff6-4678-baa4-fd182ee35269.gif)
+
 ## Getting started 🚀
 
 ### Install
 
 ```shell
 $ python -m venv venv
 $ . venv/bin/activate
@@ -375,15 +378,16 @@
 100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 300/300 [00:07<00:00, 40.95it/s]
 my_table truncated
 ```
 
 ### Table move
 
 Move all items from table to table.
-A table with the same schema must be prepared in advance.
+A table with the same schema must be prepared in advance.  
+Table items is not deleted and behaves like a copy.
 
 ```shell
 $ dynamodb-csv --move -t my_table_from my_table_to
 my_table_from scan 300 items
 please wait my_table_to moving
 100%|███████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 300/300 [00:15<00:00, 20.00it/s]
 my_table_to moved 300 items
```

### Comparing `dynamodb-csv-1.5.0/setup.cfg` & `dynamodb-csv-1.5.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 [metadata]
 name = dynamodb-csv
-version = 1.5.0
+version = 1.5.1
 description = A utility that allows CSV import / export to DynamoDB on the command line
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/danishi/dynamodb-csv
 keywords = AWS, DynamoDB, CSV
 license = MIT
 author = danishi
 author_email = dns2developer@gmail.com
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Utilities
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.8
 zip_safe = False
 include_package_data = False
 packages = 
 	app
 	app.dynamodb
 install_requires = 
 	boto3
```

