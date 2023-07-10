# Comparing `tmp/dela-0.1.0.tar.gz` & `tmp/dela-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dela-0.1.0.tar", max compression
+gzip compressed data, was "dela-0.1.1.tar", max compression
```

## Comparing `dela-0.1.0.tar` & `dela-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1338 2023-07-10 15:23:29.663091 dela-0.1.0/README.md
--rw-r--r--   0        0        0      267 2023-07-10 15:04:23.423813 dela-0.1.0/dela/FileReader.py
--rw-r--r--   0        0        0     2958 2023-07-10 15:04:23.540481 dela-0.1.0/dela/ListCommand.py
--rw-r--r--   0        0        0     1248 2023-07-10 15:04:23.473813 dela-0.1.0/dela/Todo.py
--rw-r--r--   0        0        0      521 2023-07-10 15:04:23.427146 dela-0.1.0/dela/TodoPresentation.py
--rw-r--r--   0        0        0        0 2023-07-10 12:20:05.111914 dela-0.1.0/dela/__init__.py
--rw-r--r--   0        0        0     1776 2023-07-10 15:21:39.464846 dela-0.1.0/dela/__main__.py
--rw-r--r--   0        0        0      123 2023-07-10 15:04:23.420479 dela-0.1.0/dela/logger.py
--rw-r--r--   0        0        0      367 2023-07-10 12:38:02.072606 dela-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1916 1970-01-01 00:00:00.000000 dela-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1345 2023-07-10 15:34:23.747731 dela-0.1.1/README.md
+-rw-r--r--   0        0        0      267 2023-07-10 15:34:23.747731 dela-0.1.1/dela/FileReader.py
+-rw-r--r--   0        0        0     2958 2023-07-10 15:34:23.747731 dela-0.1.1/dela/ListCommand.py
+-rw-r--r--   0        0        0     1248 2023-07-10 15:34:23.747731 dela-0.1.1/dela/Todo.py
+-rw-r--r--   0        0        0      521 2023-07-10 15:34:23.747731 dela-0.1.1/dela/TodoPresentation.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:34:23.747731 dela-0.1.1/dela/__init__.py
+-rw-r--r--   0        0        0     1776 2023-07-10 15:34:23.747731 dela-0.1.1/dela/__main__.py
+-rw-r--r--   0        0        0      123 2023-07-10 15:34:23.747731 dela-0.1.1/dela/logger.py
+-rw-r--r--   0        0        0      367 2023-07-10 15:34:23.747731 dela-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1923 1970-01-01 00:00:00.000000 dela-0.1.1/PKG-INFO
```

### Comparing `dela-0.1.0/README.md` & `dela-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ## Dela
 
 ![dela](./imgs/dela.png)
 
 ### Installation
 
 ```
-pip install dela
+pip install --user dela
 ```
 
 ### Help
 
 ```
 CLI to list todos in markdown files, like Obsidian Vaults.
```

### Comparing `dela-0.1.0/dela/ListCommand.py` & `dela-0.1.1/dela/ListCommand.py`

 * *Files identical despite different names*

### Comparing `dela-0.1.0/dela/Todo.py` & `dela-0.1.1/dela/Todo.py`

 * *Files identical despite different names*

### Comparing `dela-0.1.0/dela/TodoPresentation.py` & `dela-0.1.1/dela/TodoPresentation.py`

 * *Files identical despite different names*

### Comparing `dela-0.1.0/dela/__main__.py` & `dela-0.1.1/dela/__main__.py`

 * *Files identical despite different names*

### Comparing `dela-0.1.0/PKG-INFO` & `dela-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dela
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: 'Anton Shuvalov'
 Author-email: anton@shuvalov.info
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 ## Dela
 
 ![dela](./imgs/dela.png)
 
 ### Installation
 
 ```
-pip install dela
+pip install --user dela
 ```
 
 ### Help
 
 ```
 CLI to list todos in markdown files, like Obsidian Vaults.
```

