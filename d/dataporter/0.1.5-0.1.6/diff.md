# Comparing `tmp/dataporter-0.1.5.tar.gz` & `tmp/dataporter-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataporter-0.1.5.tar", max compression
+gzip compressed data, was "dataporter-0.1.6.tar", max compression
```

## Comparing `dataporter-0.1.5.tar` & `dataporter-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      354 2023-06-14 10:59:50.072481 dataporter-0.1.5/README.md
--rw-r--r--   0        0        0      225 2023-07-07 12:27:43.595700 dataporter-0.1.5/dataporter/__init__.py
--rw-r--r--   0        0        0     4752 2023-07-07 13:14:56.566444 dataporter-0.1.5/dataporter/csv2csv.py
--rw-r--r--   0        0        0     7001 2023-07-07 12:14:47.084091 dataporter-0.1.5/dataporter/csv2sql.py
--rw-r--r--   0        0        0     3598 2023-07-07 11:52:32.112896 dataporter-0.1.5/dataporter/sql2csv.py
--rw-r--r--   0        0        0     1828 2023-06-14 11:17:06.906524 dataporter-0.1.5/dataporter/sql_schema2txt.py
--rw-r--r--   0        0        0      373 2023-07-07 12:03:48.359884 dataporter-0.1.5/dataporter/utils.py
--rw-r--r--   0        0        0      577 2023-07-07 12:28:59.493693 dataporter-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 dataporter-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      354 2023-06-14 10:59:50.072481 dataporter-0.1.6/README.md
+-rw-r--r--   0        0        0      228 2023-07-10 07:28:06.020794 dataporter-0.1.6/dataporter/__init__.py
+-rw-r--r--   0        0        0     6890 2023-07-10 08:04:38.673802 dataporter-0.1.6/dataporter/csv2file.py
+-rw-r--r--   0        0        0     7001 2023-07-07 12:14:47.084091 dataporter-0.1.6/dataporter/csv2sql.py
+-rw-r--r--   0        0        0     3598 2023-07-07 11:52:32.112896 dataporter-0.1.6/dataporter/sql2csv.py
+-rw-r--r--   0        0        0     1828 2023-06-14 11:17:06.906524 dataporter-0.1.6/dataporter/sql_schema2txt.py
+-rw-r--r--   0        0        0      373 2023-07-07 14:17:22.768820 dataporter-0.1.6/dataporter/utils.py
+-rw-r--r--   0        0        0      584 2023-07-10 08:06:01.076214 dataporter-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 dataporter-0.1.6/PKG-INFO
```

### Comparing `dataporter-0.1.5/dataporter/csv2sql.py` & `dataporter-0.1.6/dataporter/csv2sql.py`

 * *Files identical despite different names*

### Comparing `dataporter-0.1.5/dataporter/sql2csv.py` & `dataporter-0.1.6/dataporter/sql2csv.py`

 * *Files identical despite different names*

### Comparing `dataporter-0.1.5/dataporter/sql_schema2txt.py` & `dataporter-0.1.6/dataporter/sql_schema2txt.py`

 * *Files identical despite different names*

### Comparing `dataporter-0.1.5/pyproject.toml` & `dataporter-0.1.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "dataporter"
-version = "0.1.5"
-description = "convert csv to csv/sql or convert sql to csv"
+version = "0.1.6"
+description = "convert csv to csv/json/sql or convert sql to csv"
 authors = ["AuthorPlaceholder"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 fire = "^0.5.0"
 loguru = "^0.7.0"
@@ -13,14 +13,14 @@
 sqlalchemy = "^2.0.13"
 pymysql = "^1.0.3"
 cryptography = "^40.0.2"
 
 [tool.poetry.scripts]
 sql2csv = "dataporter:sql2csv"
 csv2sql = "dataporter:csv2sql"
-csv2csv = "dataporter:csv2csv"
+csv2file = "dataporter:csv2file"
 sql_schema2txt = "dataporter:sql_schema2txt"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dataporter-0.1.5/PKG-INFO` & `dataporter-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dataporter
-Version: 0.1.5
-Summary: convert csv to csv/sql or convert sql to csv
+Version: 0.1.6
+Summary: convert csv to csv/json/sql or convert sql to csv
 Author: AuthorPlaceholder
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cryptography (>=40.0.2,<41.0.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
```

