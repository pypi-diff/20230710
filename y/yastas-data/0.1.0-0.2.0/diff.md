# Comparing `tmp/yastas-data-0.1.0.tar.gz` & `tmp/yastas-data-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yastas-data-0.1.0.tar", last modified: Thu Jul  6 20:29:29 2023, max compression
+gzip compressed data, was "yastas-data-0.2.0.tar", last modified: Mon Jul 10 20:04:20 2023, max compression
```

## Comparing `yastas-data-0.1.0.tar` & `yastas-data-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 20:29:29.185768 yastas-data-0.1.0/
--rw-rw-rw-   0        0        0      455 2023-07-06 20:29:29.175506 yastas-data-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       85 2023-07-03 20:57:32.000000 yastas-data-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 20:29:29.022435 yastas-data-0.1.0/data_code/
--rw-rw-rw-   0        0        0        0 2023-06-22 23:24:11.000000 yastas-data-0.1.0/data_code/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 20:29:29.088093 yastas-data-0.1.0/data_code/gcp/
--rw-rw-rw-   0        0        0        0 2023-06-22 23:34:31.000000 yastas-data-0.1.0/data_code/gcp/__init__.py
--rw-rw-rw-   0        0        0     1959 2023-06-21 20:23:02.000000 yastas-data-0.1.0/data_code/gcp/bq.py
--rw-rw-rw-   0        0        0      416 2023-06-26 22:44:12.000000 yastas-data-0.1.0/data_code/gcp/secrets.py
--rw-rw-rw-   0        0        0        0 2023-06-23 22:17:23.000000 yastas-data-0.1.0/data_code/gcp/service_account.py
--rw-rw-rw-   0        0        0     4167 2023-06-26 23:08:55.000000 yastas-data-0.1.0/data_code/gcp/sql.py
--rw-rw-rw-   0        0        0       43 2023-06-21 19:52:01.000000 yastas-data-0.1.0/data_code/gcp/storage.py
-drwxrwxrwx   0        0        0        0 2023-07-06 20:29:29.117201 yastas-data-0.1.0/data_code/parquets/
--rw-rw-rw-   0        0        0        0 2023-06-22 23:30:05.000000 yastas-data-0.1.0/data_code/parquets/__init__.py
--rw-rw-rw-   0        0        0      490 2023-06-27 22:57:11.000000 yastas-data-0.1.0/data_code/parquets/get_schema.py
--rw-rw-rw-   0        0        0      998 2023-06-13 02:01:53.000000 yastas-data-0.1.0/data_code/parquets/parquet2csv.py
--rw-rw-rw-   0        0        0       42 2023-07-06 20:29:29.186268 yastas-data-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      700 2023-07-06 20:29:21.000000 yastas-data-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 20:29:29.165025 yastas-data-0.1.0/yastas_data.egg-info/
--rw-rw-rw-   0        0        0      455 2023-07-06 20:29:28.000000 yastas-data-0.1.0/yastas_data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2023-07-06 20:29:28.000000 yastas-data-0.1.0/yastas_data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 20:29:28.000000 yastas-data-0.1.0/yastas_data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-06 20:29:28.000000 yastas-data-0.1.0/yastas_data.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 20:04:20.784901 yastas-data-0.2.0/
+-rw-rw-rw-   0        0        0      583 2023-07-10 20:04:20.773774 yastas-data-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-07-10 20:00:47.000000 yastas-data-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 20:04:20.552157 yastas-data-0.2.0/data_code/
+-rw-rw-rw-   0        0        0        0 2023-06-22 23:24:11.000000 yastas-data-0.2.0/data_code/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 20:04:20.565014 yastas-data-0.2.0/data_code/beam/
+-rw-rw-rw-   0        0        0        0 2023-07-10 19:17:14.000000 yastas-data-0.2.0/data_code/beam/__init__.py
+-rw-rw-rw-   0        0        0     1682 2023-07-10 19:42:59.000000 yastas-data-0.2.0/data_code/beam/database.py
+drwxrwxrwx   0        0        0        0 2023-07-10 20:04:20.643351 yastas-data-0.2.0/data_code/gcp/
+-rw-rw-rw-   0        0        0        0 2023-06-22 23:34:31.000000 yastas-data-0.2.0/data_code/gcp/__init__.py
+-rw-rw-rw-   0        0        0     1684 2023-07-07 18:59:37.000000 yastas-data-0.2.0/data_code/gcp/bq.py
+-rw-rw-rw-   0        0        0      416 2023-06-26 22:44:12.000000 yastas-data-0.2.0/data_code/gcp/secrets.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 22:17:23.000000 yastas-data-0.2.0/data_code/gcp/service_account.py
+-rw-rw-rw-   0        0        0     3541 2023-07-10 19:19:15.000000 yastas-data-0.2.0/data_code/gcp/sql.py
+-rw-rw-rw-   0        0        0       43 2023-06-21 19:52:01.000000 yastas-data-0.2.0/data_code/gcp/storage.py
+drwxrwxrwx   0        0        0        0 2023-07-10 20:04:20.685056 yastas-data-0.2.0/data_code/parquets/
+-rw-rw-rw-   0        0        0        0 2023-06-22 23:30:05.000000 yastas-data-0.2.0/data_code/parquets/__init__.py
+-rw-rw-rw-   0        0        0      490 2023-06-27 22:57:11.000000 yastas-data-0.2.0/data_code/parquets/get_schema.py
+-rw-rw-rw-   0        0        0      998 2023-06-13 02:01:53.000000 yastas-data-0.2.0/data_code/parquets/parquet2csv.py
+-rw-rw-rw-   0        0        0       42 2023-07-10 20:04:20.785038 yastas-data-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      700 2023-07-10 20:00:28.000000 yastas-data-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 20:04:20.742680 yastas-data-0.2.0/yastas_data.egg-info/
+-rw-rw-rw-   0        0        0      583 2023-07-10 20:04:20.000000 yastas-data-0.2.0/yastas_data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-07-10 20:04:20.000000 yastas-data-0.2.0/yastas_data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 20:04:20.000000 yastas-data-0.2.0/yastas_data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-10 20:04:20.000000 yastas-data-0.2.0/yastas_data.egg-info/top_level.txt
```

### Comparing `yastas-data-0.1.0/data_code/gcp/bq.py` & `yastas-data-0.2.0/data_code/gcp/bq.py`

 * *Files 17% similar despite different names*

```diff
@@ -34,14 +34,8 @@
         table_id (str): _description_
 
     Returns:
         dict: _description_
     """
     metadata_table_bq = subprocess.run(["bq","show","--format=prettyjson", table_id], capture_output=True, shell=True).stdout
     metadata_table_bq = ast.literal_eval(metadata_table_bq.decode('UTF-8'))
-    return metadata_table_bq
-
-# table = 'yas-dev-sii-pid:sii_yas_de_raw.wrk_streaming_movimientos'
-# parquet = 'gs://yas-dev-sii-raw/AB/raw_streaming_movimientos/2023-06-06/raw_streaming_movimientos-00000-of-00001.parquet'
-
-# metadata = create_or_evaluate_bq_table(table,parquet)
-# print(metadata)
+    return metadata_table_bq
```

### Comparing `yastas-data-0.1.0/data_code/gcp/sql.py` & `yastas-data-0.2.0/data_code/gcp/sql.py`

 * *Files 15% similar despite different names*

```diff
@@ -92,36 +92,21 @@
         # Crear un cursor para ejecutar consultas
         cursor = connection.cursor()
 
         # Ejecutar una consulta de ejemplo
         cursor.execute(query)
 
         # Obtener los resultados de la consulta
-        filas = cursor.fetchall()
+        query_result = cursor.fetchall()
 
         # Procesar los resultados
-        for fila in filas:
-            print(fila)
+        # for fila in filas:
+        #     print(fila)
 
         # Cerrar el cursor y la conexión
         cursor.close()
+        return query_result
 
     def close_connection(self, connection:psycopg2):
         # Cerrar el cursor y la conexión
         connection.close()
 
-host='127.0.0.1'
-port=5432
-database='yas-inversiones'
-query = "SELECT * FROM estatus_movimiento"
-string_conn = "cloud_sql_proxy -instances=yas-dev-infraestructura:us-east1:yas-inversiones=tcp:5432"
-project_id = "yas-dev-infraestructura"
-secret_name = "yas-cierre-user-sql-name-infraestructura-2891887f"
-secret_password = "yas-cierre-user-sql-password-infraestructura-2891887f"
-
-postgres = Database(host,port,database,secret_name,secret_password, project_id)
-postgres.raise_proxy(string_conn)
-conn = postgres.get_connection()
-postgres.get_tables(conn)
-postgres.execute_query(conn, query=query)
-postgres.close_connection(conn)
-postgres.shut_down_proxy()
```

### Comparing `yastas-data-0.1.0/data_code/parquets/parquet2csv.py` & `yastas-data-0.2.0/data_code/parquets/parquet2csv.py`

 * *Files identical despite different names*

### Comparing `yastas-data-0.1.0/setup.py` & `yastas-data-0.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open('requirements.txt') as file:
         return file.read().splitlines()
     
 readme = open("./README.md", "r")
 
 setup(
     name='yastas-data',
-    version='0.1.0',
+    version='0.2.0',
     author='Data - Aaron',
     author_email="e-ajuareza@minsait.com",
     description='Paquete distribuible en repositorio de funciones locales',
     long_description=readme.read(),
     packages=find_packages(),
     url="https://bitbucket.org/gentera-insumos/data-code",
     keywords=['data', 'big_data', 'data_analytics', 'data_engineer', 'data_science'],
```

