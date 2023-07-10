# Comparing `tmp/yastas-data-0.2.0.tar.gz` & `tmp/yastas-data-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yastas-data-0.2.0.tar", last modified: Mon Jul 10 20:04:20 2023, max compression
+gzip compressed data, was "yastas-data-0.3.0.tar", last modified: Mon Jul 10 21:09:03 2023, max compression
```

## Comparing `yastas-data-0.2.0.tar` & `yastas-data-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 20:04:20.784901 yastas-data-0.2.0/
--rw-rw-rw-   0        0        0      583 2023-07-10 20:04:20.773774 yastas-data-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-07-10 20:00:47.000000 yastas-data-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 20:04:20.552157 yastas-data-0.2.0/data_code/
--rw-rw-rw-   0        0        0        0 2023-06-22 23:24:11.000000 yastas-data-0.2.0/data_code/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 20:04:20.565014 yastas-data-0.2.0/data_code/beam/
--rw-rw-rw-   0        0        0        0 2023-07-10 19:17:14.000000 yastas-data-0.2.0/data_code/beam/__init__.py
--rw-rw-rw-   0        0        0     1682 2023-07-10 19:42:59.000000 yastas-data-0.2.0/data_code/beam/database.py
-drwxrwxrwx   0        0        0        0 2023-07-10 20:04:20.643351 yastas-data-0.2.0/data_code/gcp/
--rw-rw-rw-   0        0        0        0 2023-06-22 23:34:31.000000 yastas-data-0.2.0/data_code/gcp/__init__.py
--rw-rw-rw-   0        0        0     1684 2023-07-07 18:59:37.000000 yastas-data-0.2.0/data_code/gcp/bq.py
--rw-rw-rw-   0        0        0      416 2023-06-26 22:44:12.000000 yastas-data-0.2.0/data_code/gcp/secrets.py
--rw-rw-rw-   0        0        0        0 2023-06-23 22:17:23.000000 yastas-data-0.2.0/data_code/gcp/service_account.py
--rw-rw-rw-   0        0        0     3541 2023-07-10 19:19:15.000000 yastas-data-0.2.0/data_code/gcp/sql.py
--rw-rw-rw-   0        0        0       43 2023-06-21 19:52:01.000000 yastas-data-0.2.0/data_code/gcp/storage.py
-drwxrwxrwx   0        0        0        0 2023-07-10 20:04:20.685056 yastas-data-0.2.0/data_code/parquets/
--rw-rw-rw-   0        0        0        0 2023-06-22 23:30:05.000000 yastas-data-0.2.0/data_code/parquets/__init__.py
--rw-rw-rw-   0        0        0      490 2023-06-27 22:57:11.000000 yastas-data-0.2.0/data_code/parquets/get_schema.py
--rw-rw-rw-   0        0        0      998 2023-06-13 02:01:53.000000 yastas-data-0.2.0/data_code/parquets/parquet2csv.py
--rw-rw-rw-   0        0        0       42 2023-07-10 20:04:20.785038 yastas-data-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      700 2023-07-10 20:00:28.000000 yastas-data-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 20:04:20.742680 yastas-data-0.2.0/yastas_data.egg-info/
--rw-rw-rw-   0        0        0      583 2023-07-10 20:04:20.000000 yastas-data-0.2.0/yastas_data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-07-10 20:04:20.000000 yastas-data-0.2.0/yastas_data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 20:04:20.000000 yastas-data-0.2.0/yastas_data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-10 20:04:20.000000 yastas-data-0.2.0/yastas_data.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 21:09:03.640427 yastas-data-0.3.0/
+-rw-rw-rw-   0        0        0      583 2023-07-10 21:09:03.631727 yastas-data-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-07-10 20:00:47.000000 yastas-data-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 21:09:03.466417 yastas-data-0.3.0/data_code/
+-rw-rw-rw-   0        0        0        0 2023-06-22 23:24:11.000000 yastas-data-0.3.0/data_code/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 21:09:03.478759 yastas-data-0.3.0/data_code/beam/
+-rw-rw-rw-   0        0        0        0 2023-07-10 19:17:14.000000 yastas-data-0.3.0/data_code/beam/__init__.py
+-rw-rw-rw-   0        0        0     1079 2023-07-10 21:03:38.000000 yastas-data-0.3.0/data_code/beam/database.py
+drwxrwxrwx   0        0        0        0 2023-07-10 21:09:03.548075 yastas-data-0.3.0/data_code/gcp/
+-rw-rw-rw-   0        0        0        0 2023-06-22 23:34:31.000000 yastas-data-0.3.0/data_code/gcp/__init__.py
+-rw-rw-rw-   0        0        0     1684 2023-07-07 18:59:37.000000 yastas-data-0.3.0/data_code/gcp/bq.py
+-rw-rw-rw-   0        0        0      416 2023-06-26 22:44:12.000000 yastas-data-0.3.0/data_code/gcp/secrets.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 22:17:23.000000 yastas-data-0.3.0/data_code/gcp/service_account.py
+-rw-rw-rw-   0        0        0     3555 2023-07-10 20:36:32.000000 yastas-data-0.3.0/data_code/gcp/sql.py
+-rw-rw-rw-   0        0        0       43 2023-06-21 19:52:01.000000 yastas-data-0.3.0/data_code/gcp/storage.py
+drwxrwxrwx   0        0        0        0 2023-07-10 21:09:03.581602 yastas-data-0.3.0/data_code/parquets/
+-rw-rw-rw-   0        0        0        0 2023-06-22 23:30:05.000000 yastas-data-0.3.0/data_code/parquets/__init__.py
+-rw-rw-rw-   0        0        0      490 2023-06-27 22:57:11.000000 yastas-data-0.3.0/data_code/parquets/get_schema.py
+-rw-rw-rw-   0        0        0      998 2023-06-13 02:01:53.000000 yastas-data-0.3.0/data_code/parquets/parquet2csv.py
+-rw-rw-rw-   0        0        0       42 2023-07-10 21:09:03.642066 yastas-data-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      700 2023-07-10 21:05:58.000000 yastas-data-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 21:09:03.623598 yastas-data-0.3.0/yastas_data.egg-info/
+-rw-rw-rw-   0        0        0      583 2023-07-10 21:09:03.000000 yastas-data-0.3.0/yastas_data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-07-10 21:09:03.000000 yastas-data-0.3.0/yastas_data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 21:09:03.000000 yastas-data-0.3.0/yastas_data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-10 21:09:03.000000 yastas-data-0.3.0/yastas_data.egg-info/top_level.txt
```

### Comparing `yastas-data-0.2.0/PKG-INFO` & `yastas-data-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: yastas-data
-Version: 0.2.0
+Version: 0.3.0
 Summary: Paquete distribuible en repositorio de funciones locales
 Home-page: https://bitbucket.org/gentera-insumos/data-code
 Author: Data - Aaron
 Author-email: e-ajuareza@minsait.com
 License: MIT
 Description: # InstalaciÃ³n
```

### Comparing `yastas-data-0.2.0/data_code/gcp/bq.py` & `yastas-data-0.3.0/data_code/gcp/bq.py`

 * *Files identical despite different names*

### Comparing `yastas-data-0.2.0/data_code/gcp/sql.py` & `yastas-data-0.3.0/data_code/gcp/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from secrets import get_secret
+from data_code.gcp.secrets import get_secret
 import psycopg2
 import logging
 import os
 
 class Proxy():
     """Funcionalidades relacionadas al proxy para lograr comunicación con bases de datos.
     """
```

### Comparing `yastas-data-0.2.0/data_code/parquets/parquet2csv.py` & `yastas-data-0.3.0/data_code/parquets/parquet2csv.py`

 * *Files identical despite different names*

### Comparing `yastas-data-0.2.0/setup.py` & `yastas-data-0.3.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open('requirements.txt') as file:
         return file.read().splitlines()
     
 readme = open("./README.md", "r")
 
 setup(
     name='yastas-data',
-    version='0.2.0',
+    version='0.3.0',
     author='Data - Aaron',
     author_email="e-ajuareza@minsait.com",
     description='Paquete distribuible en repositorio de funciones locales',
     long_description=readme.read(),
     packages=find_packages(),
     url="https://bitbucket.org/gentera-insumos/data-code",
     keywords=['data', 'big_data', 'data_analytics', 'data_engineer', 'data_science'],
```

### Comparing `yastas-data-0.2.0/yastas_data.egg-info/PKG-INFO` & `yastas-data-0.3.0/yastas_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: yastas-data
-Version: 0.2.0
+Version: 0.3.0
 Summary: Paquete distribuible en repositorio de funciones locales
 Home-page: https://bitbucket.org/gentera-insumos/data-code
 Author: Data - Aaron
 Author-email: e-ajuareza@minsait.com
 License: MIT
 Description: # InstalaciÃ³n
```

