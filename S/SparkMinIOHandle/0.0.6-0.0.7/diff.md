# Comparing `tmp/SparkMinIOHandle-0.0.6.tar.gz` & `tmp/SparkMinIOHandle-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SparkMinIOHandle-0.0.6.tar", last modified: Mon Jul 10 13:01:44 2023, max compression
+gzip compressed data, was "SparkMinIOHandle-0.0.7.tar", last modified: Mon Jul 10 13:31:00 2023, max compression
```

## Comparing `SparkMinIOHandle-0.0.6.tar` & `SparkMinIOHandle-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 13:01:44.028451 SparkMinIOHandle-0.0.6/
--rw-rw-rw-   0        0        0      664 2023-07-10 13:01:44.027450 SparkMinIOHandle-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-07-10 11:54:22.000000 SparkMinIOHandle-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 13:01:44.023450 SparkMinIOHandle-0.0.6/SparkMinIOHandle.egg-info/
--rw-rw-rw-   0        0        0      664 2023-07-10 13:01:43.000000 SparkMinIOHandle-0.0.6/SparkMinIOHandle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-07-10 13:01:43.000000 SparkMinIOHandle-0.0.6/SparkMinIOHandle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 13:01:43.000000 SparkMinIOHandle-0.0.6/SparkMinIOHandle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-07-10 13:01:43.000000 SparkMinIOHandle-0.0.6/SparkMinIOHandle.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-10 13:01:43.000000 SparkMinIOHandle-0.0.6/SparkMinIOHandle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 13:01:44.028451 SparkMinIOHandle-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1148 2023-07-10 13:01:03.000000 SparkMinIOHandle-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 13:01:44.025449 SparkMinIOHandle-0.0.6/sparkminiohandler/
--rw-rw-rw-   0        0        0        0 2023-06-21 15:23:14.000000 SparkMinIOHandle-0.0.6/sparkminiohandler/__init__.py
--rw-rw-rw-   0        0        0     3067 2023-07-10 12:57:45.000000 SparkMinIOHandle-0.0.6/sparkminiohandler/sparkminiohandler.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:31:00.550144 SparkMinIOHandle-0.0.7/
+-rw-rw-rw-   0        0        0      664 2023-07-10 13:31:00.549144 SparkMinIOHandle-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2072 2023-07-10 13:14:02.000000 SparkMinIOHandle-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 13:31:00.538144 SparkMinIOHandle-0.0.7/SparkMinIOHandle.egg-info/
+-rw-rw-rw-   0        0        0      664 2023-07-10 13:31:00.000000 SparkMinIOHandle-0.0.7/SparkMinIOHandle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-07-10 13:31:00.000000 SparkMinIOHandle-0.0.7/SparkMinIOHandle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 13:31:00.000000 SparkMinIOHandle-0.0.7/SparkMinIOHandle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-10 13:31:00.000000 SparkMinIOHandle-0.0.7/SparkMinIOHandle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-10 13:31:00.000000 SparkMinIOHandle-0.0.7/SparkMinIOHandle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 13:31:00.550144 SparkMinIOHandle-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1148 2023-07-10 13:30:36.000000 SparkMinIOHandle-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:31:00.547143 SparkMinIOHandle-0.0.7/sparkminiohandler/
+-rw-rw-rw-   0        0        0        0 2023-06-21 15:23:14.000000 SparkMinIOHandle-0.0.7/sparkminiohandler/__init__.py
+-rw-rw-rw-   0        0        0     2961 2023-07-10 13:30:56.000000 SparkMinIOHandle-0.0.7/sparkminiohandler/sparkminiohandler.py
```

### Comparing `SparkMinIOHandle-0.0.6/PKG-INFO` & `SparkMinIOHandle-0.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: SparkMinIOHandle
-Version: 0.0.6
+Version: 0.0.7
 Summary: Spark MinIO Handler Package
 Home-page: UNKNOWN
 Author: Yuri Dimitri
 Author-email: yuridrcosta@gmail.com
 License: UNKNOWN
 Description: Pacote para gerenciar views e dataframes spark consumindo de tabelas JSON armazenadas no Object Storage MinIO
 Keywords: python,minio,pyspark
```

### Comparing `SparkMinIOHandle-0.0.6/SparkMinIOHandle.egg-info/PKG-INFO` & `SparkMinIOHandle-0.0.7/SparkMinIOHandle.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: SparkMinIOHandle
-Version: 0.0.6
+Version: 0.0.7
 Summary: Spark MinIO Handler Package
 Home-page: UNKNOWN
 Author: Yuri Dimitri
 Author-email: yuridrcosta@gmail.com
 License: UNKNOWN
 Description: Pacote para gerenciar views e dataframes spark consumindo de tabelas JSON armazenadas no Object Storage MinIO
 Keywords: python,minio,pyspark
```

### Comparing `SparkMinIOHandle-0.0.6/setup.py` & `SparkMinIOHandle-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6' 
+VERSION = '0.0.7' 
 DESCRIPTION = 'Spark MinIO Handler Package'
 LONG_DESCRIPTION = 'Pacote para gerenciar views e dataframes spark consumindo de tabelas JSON armazenadas no Object Storage MinIO'
 
 # Setting up
 setup(
        # 'name' deve corresponder ao nome da pasta 'verysimplemodule'
         name="SparkMinIOHandle",
```

### Comparing `SparkMinIOHandle-0.0.6/sparkminiohandler/sparkminiohandler.py` & `SparkMinIOHandle-0.0.7/sparkminiohandler/sparkminiohandler.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,26 @@
 import pandas as pd
 
 class SparkMinIOHandler:
     """
     Classe para manipulação de dados do PySpark com o MinIO.
     """
 
-    def _init_(self, client_minio, bucket_name, spark_session, spark_context):
+    def _init_(self, client_minio, bucket_name, spark_session):
         """
         Inicializa o SparkMinIOHandler.
 
         Args:
             client_minio: Cliente MinIO.
             bucket_name: Nome do bucket do MinIO.
             spark_session: Sessão do Spark.
-            spark_context: Contexto do Spark.
         """
         self.client_minio = client_minio
         self.bucket_name = bucket_name
         self.spark_session = spark_session
-        self.spark_context = spark_context
 
 
     def get_recent_table(self, tablename: str):
         """Obtém o nome do arquivo JSON (de uma tabela) mais recente em um bucket do MinIO.
         """
 
         # Padrão de nome dos arquivos
```

