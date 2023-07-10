# Comparing `tmp/SparkMinIOHandle-0.0.5.tar.gz` & `tmp/SparkMinIOHandle-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SparkMinIOHandle-0.0.5.tar", last modified: Fri Jun 23 16:46:28 2023, max compression
+gzip compressed data, was "SparkMinIOHandle-0.0.6.tar", last modified: Mon Jul 10 13:01:44 2023, max compression
```

## Comparing `SparkMinIOHandle-0.0.5.tar` & `SparkMinIOHandle-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 16:46:28.175163 SparkMinIOHandle-0.0.5/
--rw-rw-rw-   0        0        0      653 2023-06-23 16:46:28.173165 SparkMinIOHandle-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      133 2023-06-22 12:50:58.000000 SparkMinIOHandle-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 16:46:28.157169 SparkMinIOHandle-0.0.5/SparkMinIOHandle.egg-info/
--rw-rw-rw-   0        0        0      653 2023-06-23 16:46:27.000000 SparkMinIOHandle-0.0.5/SparkMinIOHandle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-06-23 16:46:27.000000 SparkMinIOHandle-0.0.5/SparkMinIOHandle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 16:46:27.000000 SparkMinIOHandle-0.0.5/SparkMinIOHandle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-23 16:46:27.000000 SparkMinIOHandle-0.0.5/SparkMinIOHandle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 16:46:28.175163 SparkMinIOHandle-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1120 2023-06-23 16:46:20.000000 SparkMinIOHandle-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 16:46:28.171166 SparkMinIOHandle-0.0.5/sparkminiohandler/
--rw-rw-rw-   0        0        0        0 2023-06-22 12:50:58.000000 SparkMinIOHandle-0.0.5/sparkminiohandler/__init__.py
--rw-rw-rw-   0        0        0     2032 2023-06-23 16:46:05.000000 SparkMinIOHandle-0.0.5/sparkminiohandler/sparkminiohandler.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:01:44.028451 SparkMinIOHandle-0.0.6/
+-rw-rw-rw-   0        0        0      664 2023-07-10 13:01:44.027450 SparkMinIOHandle-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-07-10 11:54:22.000000 SparkMinIOHandle-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 13:01:44.023450 SparkMinIOHandle-0.0.6/SparkMinIOHandle.egg-info/
+-rw-rw-rw-   0        0        0      664 2023-07-10 13:01:43.000000 SparkMinIOHandle-0.0.6/SparkMinIOHandle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-07-10 13:01:43.000000 SparkMinIOHandle-0.0.6/SparkMinIOHandle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 13:01:43.000000 SparkMinIOHandle-0.0.6/SparkMinIOHandle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-10 13:01:43.000000 SparkMinIOHandle-0.0.6/SparkMinIOHandle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-10 13:01:43.000000 SparkMinIOHandle-0.0.6/SparkMinIOHandle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 13:01:44.028451 SparkMinIOHandle-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1148 2023-07-10 13:01:03.000000 SparkMinIOHandle-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:01:44.025449 SparkMinIOHandle-0.0.6/sparkminiohandler/
+-rw-rw-rw-   0        0        0        0 2023-06-21 15:23:14.000000 SparkMinIOHandle-0.0.6/sparkminiohandler/__init__.py
+-rw-rw-rw-   0        0        0     3067 2023-07-10 12:57:45.000000 SparkMinIOHandle-0.0.6/sparkminiohandler/sparkminiohandler.py
```

### Comparing `SparkMinIOHandle-0.0.5/PKG-INFO` & `SparkMinIOHandle-0.0.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: SparkMinIOHandle
-Version: 0.0.5
+Version: 0.0.6
 Summary: Spark MinIO Handler Package
 Home-page: UNKNOWN
 Author: Yuri Dimitri
 Author-email: yuridrcosta@gmail.com
 License: UNKNOWN
-Keywords: python,minio,spark
+Description: Pacote para gerenciar views e dataframes spark consumindo de tabelas JSON armazenadas no Object Storage MinIO
+Keywords: python,minio,pyspark
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-
-Pacote para gerenciar views e dataframes spark consumindo de tabelas JSON armazenadas no Object Storage MinIO
-
```

### Comparing `SparkMinIOHandle-0.0.5/SparkMinIOHandle.egg-info/PKG-INFO` & `SparkMinIOHandle-0.0.6/SparkMinIOHandle.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: SparkMinIOHandle
-Version: 0.0.5
+Version: 0.0.6
 Summary: Spark MinIO Handler Package
 Home-page: UNKNOWN
 Author: Yuri Dimitri
 Author-email: yuridrcosta@gmail.com
 License: UNKNOWN
-Keywords: python,minio,spark
+Description: Pacote para gerenciar views e dataframes spark consumindo de tabelas JSON armazenadas no Object Storage MinIO
+Keywords: python,minio,pyspark
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-
-Pacote para gerenciar views e dataframes spark consumindo de tabelas JSON armazenadas no Object Storage MinIO
-
```

### Comparing `SparkMinIOHandle-0.0.5/setup.py` & `SparkMinIOHandle-0.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5' 
+VERSION = '0.0.6' 
 DESCRIPTION = 'Spark MinIO Handler Package'
 LONG_DESCRIPTION = 'Pacote para gerenciar views e dataframes spark consumindo de tabelas JSON armazenadas no Object Storage MinIO'
 
 # Setting up
 setup(
        # 'name' deve corresponder ao nome da pasta 'verysimplemodule'
         name="SparkMinIOHandle", 
         version=VERSION,
         author="Yuri Dimitri",
         author_email="yuridrcosta@gmail.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=[], # adicione outros pacotes que 
+        install_requires=['minio','pyspark','pandas'], # adicione outros pacotes que 
         # precisem ser instalados com o seu pacote. Ex: 'caer'
         
-        keywords=['python', 'minio', 'spark'],
+        keywords=['python', 'minio', 'pyspark'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
             "Programming Language :: Python :: 2",
             "Programming Language :: Python :: 3",
             "Operating System :: MacOS :: MacOS X",
             "Operating System :: Microsoft :: Windows",
```

### Comparing `SparkMinIOHandle-0.0.5/sparkminiohandler/sparkminiohandler.py` & `SparkMinIOHandle-0.0.6/sparkminiohandler/sparkminiohandler.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,35 @@
 from datetime import datetime
+import pandas as pd
 
 class SparkMinIOHandler:
+    """
+    Classe para manipulação de dados do PySpark com o MinIO.
+    """
 
-    def __init__(self, client_minio, bucket_name, spark_session, spark_context):
+    def _init_(self, client_minio, bucket_name, spark_session, spark_context):
+        """
+        Inicializa o SparkMinIOHandler.
+
+        Args:
+            client_minio: Cliente MinIO.
+            bucket_name: Nome do bucket do MinIO.
+            spark_session: Sessão do Spark.
+            spark_context: Contexto do Spark.
+        """
         self.client_minio = client_minio
         self.bucket_name = bucket_name
         self.spark_session = spark_session
-        self.spark_context = spark_context 
+        self.spark_context = spark_context
 
 
     def get_recent_table(self, tablename: str):
+        """Obtém o nome do arquivo JSON (de uma tabela) mais recente em um bucket do MinIO.
+        """
+
         # Padrão de nome dos arquivos
         
         # Obter lista de arquivos correspondentes ao padrão
         arquivos =  [object.object_name for object in self.client_minio.list_objects(self.bucket_name) if f'{tablename}_' in object.object_name]
         
         # Função para extrair a data do nome do arquivo
         def extrair_data(nome_arquivo):
@@ -25,24 +41,50 @@
         # Ordenar a lista de arquivos pela data mais recente
         arquivos_ordenados = sorted(arquivos, key=lambda x: extrair_data(x), reverse=True)
         
         # Obter o arquivo mais recente
         arquivo_recente = arquivos_ordenados[0]
         print(f"Arquivo mais recente: {arquivo_recente}")
         return arquivo_recente
-    
+
     def load_json_spark_dataframe(self,  filename: str):
+        """
+        Carrega um arquivo JSON como um DataFrame do Spark.
+
+        Args:
+            filename: Nome do arquivo JSON.
+
+        Returns:
+            DataFrame do Spark.
+        """
         response = self.client_minio.get_object(self.bucket_name, filename)
-        with open("temptable.json",'wb') as f:
-            f.write(response.data)
-        df = self.spark_session.read.option("multiline", "true").json('temptable.json')
+        df = pd.read_json(response)
+        df = self.spark_session.createDataFrame(df)
         return df
     
-    def create_view_from_json_minio(self, tablename) :
+    def create_view_from_json_minio(self, tablename):
+        """
+        Cria uma view do Spark a partir de um arquivo JSON do MinIO.
+
+        Args:
+            tablename: Nome da tabela/view.
+
+        Returns:
+            True se a view foi criada com sucesso.
+        """
         filename = self.get_recent_table(tablename)
         df = self.load_json_spark_dataframe(filename)
         df.createOrReplaceTempView(tablename)
         return True
     
     def create_multiple_table_views(self, tablenames: list):
+        """
+        Cria várias views do Spark a partir de uma lista de tabelas.
+
+        Args:
+            tablenames: Lista de nomes das tabelas/views.
+
+        Returns:
+            None.
+        """
         for table in tablenames:
             self.create_view_from_json_minio(table)
```

