# Comparing `tmp/labelspark-0.7.28.tar.gz` & `tmp/labelspark-0.7.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelspark-0.7.28.tar", last modified: Tue Mar 14 16:15:56 2023, max compression
+gzip compressed data, was "labelspark-0.7.29.tar", last modified: Mon Jul 10 14:04:04 2023, max compression
```

## Comparing `labelspark-0.7.28.tar` & `labelspark-0.7.29.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:15:56.506128 labelspark-0.7.28/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-14 16:15:44.000000 labelspark-0.7.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-03-14 16:15:56.506128 labelspark-0.7.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-03-14 16:15:44.000000 labelspark-0.7.28/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:15:56.506128 labelspark-0.7.28/labelspark/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-14 16:15:44.000000 labelspark-0.7.28/labelspark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-03-14 16:15:44.000000 labelspark-0.7.28/labelspark/add_json_answers_to_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-14 16:15:44.000000 labelspark-0.7.28/labelspark/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-03-14 16:15:44.000000 labelspark-0.7.28/labelspark/bronze_to_silver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12630 2023-03-14 16:15:44.000000 labelspark-0.7.28/labelspark/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-03-14 16:15:44.000000 labelspark-0.7.28/labelspark/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-14 16:15:44.000000 labelspark-0.7.28/labelspark/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-14 16:15:44.000000 labelspark-0.7.28/labelspark/create_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-03-14 16:15:44.000000 labelspark-0.7.28/labelspark/create_labelbox_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-14 16:15:44.000000 labelspark-0.7.28/labelspark/dataframe_schema_enrichment.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-14 16:15:44.000000 labelspark-0.7.28/labelspark/dictionary_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-03-14 16:15:44.000000 labelspark-0.7.28/labelspark/flatten_bronze_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-14 16:15:44.000000 labelspark-0.7.28/labelspark/get_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-14 16:15:44.000000 labelspark-0.7.28/labelspark/get_videoframe_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-14 16:15:44.000000 labelspark-0.7.28/labelspark/is_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-14 16:15:44.000000 labelspark-0.7.28/labelspark/jsonToDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-03-14 16:15:44.000000 labelspark-0.7.28/labelspark/spark_schema_to_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-03-14 16:15:44.000000 labelspark-0.7.28/labelspark/update_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-03-14 16:15:44.000000 labelspark-0.7.28/labelspark/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:15:56.506128 labelspark-0.7.28/labelspark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-03-14 16:15:56.000000 labelspark-0.7.28/labelspark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-14 16:15:56.000000 labelspark-0.7.28/labelspark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 16:15:56.000000 labelspark-0.7.28/labelspark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-14 16:15:56.000000 labelspark-0.7.28/labelspark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-14 16:15:56.000000 labelspark-0.7.28/labelspark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 16:15:56.510128 labelspark-0.7.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-14 16:15:44.000000 labelspark-0.7.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:04:04.693280 labelspark-0.7.29/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 14:03:54.000000 labelspark-0.7.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-10 14:04:04.693280 labelspark-0.7.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-10 14:03:54.000000 labelspark-0.7.29/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:04:04.693280 labelspark-0.7.29/labelspark/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/add_json_answers_to_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/bronze_to_silver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34256 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/create_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/create_labelbox_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/dataframe_schema_enrichment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/dictionary_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/flatten_bronze_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/get_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/get_videoframe_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/is_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/jsonToDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/spark_schema_to_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/update_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16543 2023-07-10 14:03:54.000000 labelspark-0.7.29/labelspark/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:04:04.693280 labelspark-0.7.29/labelspark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-10 14:04:04.000000 labelspark-0.7.29/labelspark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-10 14:04:04.000000 labelspark-0.7.29/labelspark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:04:04.000000 labelspark-0.7.29/labelspark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 14:04:04.000000 labelspark-0.7.29/labelspark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 14:04:04.000000 labelspark-0.7.29/labelspark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 14:04:04.693280 labelspark-0.7.29/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-10 14:03:54.000000 labelspark-0.7.29/setup.py
```

### Comparing `labelspark-0.7.28/LICENSE` & `labelspark-0.7.29/LICENSE`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.28/PKG-INFO` & `labelspark-0.7.29/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelspark
-Version: 0.7.28
+Version: 0.7.29
 Summary: Labelbox Connector for Databricks
 Home-page: https://github.com/Labelbox/LabelSpark.git
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
@@ -63,16 +63,14 @@
 | Putting it all Together        | [![Github](https://img.shields.io/badge/GitHub-100000?logo=github&logoColor=white)](notebooks/full-demo.ipynb)  | 
 ------
 
 ### Exporting Data
 
 |            Notebook            |  Github  |
 | ------------------------------ | -------- |
-| Exporting Data to a Spark Table*            | [![Github](https://img.shields.io/badge/GitHub-100000?logo=github&logoColor=white)](notebooks/export.ipynb)  |
+| Exporting Data to a Spark Table            | [![Github](https://img.shields.io/badge/GitHub-100000?logo=github&logoColor=white)](notebooks/export.ipynb)  |
 ------
 
-* = Coming Soon
-
 While using LabelSpark, you will likely also use the Labelbox SDK (e.g. for programmatic ontology creation). These resources will help familiarize you with the Labelbox Python SDK: 
 * [Visit our docs](https://docs.labelbox.com/reference/install-python-sdk) to learn how the SDK works
 * Checkout our [notebook examples](https://github.com/Labelbox/labelspark/tree/master/notebooks) to follow along with interactive tutorials
 * View the Labelbox [API reference](https://labelbox-python.readthedocs.io/en/latest/).
```

### Comparing `labelspark-0.7.28/README.md` & `labelspark-0.7.29/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,14 @@
 | Putting it all Together        | [![Github](https://img.shields.io/badge/GitHub-100000?logo=github&logoColor=white)](notebooks/full-demo.ipynb)  | 
 ------
 
 ### Exporting Data
 
 |            Notebook            |  Github  |
 | ------------------------------ | -------- |
-| Exporting Data to a Spark Table*            | [![Github](https://img.shields.io/badge/GitHub-100000?logo=github&logoColor=white)](notebooks/export.ipynb)  |
+| Exporting Data to a Spark Table            | [![Github](https://img.shields.io/badge/GitHub-100000?logo=github&logoColor=white)](notebooks/export.ipynb)  |
 ------
 
-* = Coming Soon
-
 While using LabelSpark, you will likely also use the Labelbox SDK (e.g. for programmatic ontology creation). These resources will help familiarize you with the Labelbox Python SDK: 
 * [Visit our docs](https://docs.labelbox.com/reference/install-python-sdk) to learn how the SDK works
 * Checkout our [notebook examples](https://github.com/Labelbox/labelspark/tree/master/notebooks) to follow along with interactive tutorials
 * View the Labelbox [API reference](https://labelbox-python.readthedocs.io/en/latest/).
```

### Comparing `labelspark-0.7.28/labelspark/__init__.py` & `labelspark-0.7.29/labelspark/__init__.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.28/labelspark/add_json_answers_to_dictionary.py` & `labelspark-0.7.29/labelspark/add_json_answers_to_dictionary.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.28/labelspark/api_key.py` & `labelspark-0.7.29/labelspark/api_key.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.28/labelspark/bronze_to_silver.py` & `labelspark-0.7.29/labelspark/bronze_to_silver.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.28/labelspark/connector.py` & `labelspark-0.7.29/labelspark/connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 - add_col(table, col, default)                            : Creates a column where all values equal the default value
 - get_table_length(table)                                 : Gets the length of a DataFrame
 - rename_col(table, col, to)                              : Renames a given column
 
 """
 
 import pyspark
-from labelbase.connector import validate_column_name_change
 
 def check_pyspark():
     try:
         import pyspark.pandas as pd
     except:
         raise RuntimeError(f'labelspark.Client() requires pyspark to be installed - please update your Databricks runtime to support pyspark')
```

### Comparing `labelspark-0.7.28/labelspark/create_dataset.py` & `labelspark-0.7.29/labelspark/create_dataset.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.28/labelspark/create_labelbox_dataset.py` & `labelspark-0.7.29/labelspark/create_labelbox_dataset.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.28/labelspark/dataframe_schema_enrichment.py` & `labelspark-0.7.29/labelspark/dataframe_schema_enrichment.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.28/labelspark/flatten_bronze_table.py` & `labelspark-0.7.29/labelspark/flatten_bronze_table.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.28/labelspark/get_annotations.py` & `labelspark-0.7.29/labelspark/get_annotations.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.28/labelspark/get_videoframe_annotations.py` & `labelspark-0.7.29/labelspark/get_videoframe_annotations.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.28/labelspark/spark_schema_to_string.py` & `labelspark-0.7.29/labelspark/spark_schema_to_string.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.28/labelspark/update_metadata.py` & `labelspark-0.7.29/labelspark/update_metadata.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.28/labelspark/uploader.py` & `labelspark-0.7.29/labelspark/uploader.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,19 +25,19 @@
             "annotations" : []
         }
     }
 }
 
 This uniforms input formats so that they can leverage labelbase - Labelbox base code for best practices
 """
-
 import pyspark
 from pyspark.sql.functions import lit, udf
 from pyspark.sql.types import StructType, StructField, StringType, MapType, ArrayType
 from labelbox import Client as labelboxClient
+from labelbox.schema.ontology import Ontology as labelboxOntology
 from labelspark.connector import get_table_length, get_unique_values
 from labelbase.metadata import get_metadata_schema_to_name_key, process_metadata_value
 from labelbase.ontology import get_ontology_schema_to_name_path
 from labelbase.annotate import create_ndjsons
 import json
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
@@ -75,36 +75,36 @@
     # Check that global key column is entirely unique values
     table_length = get_table_length(table=table, extra_client=extra_client)
     if verbose:
         print(f'Creating upload list - {table_length} rows in Pandas DataFrame')
     unique_global_key_count = len(get_unique_values(table=table, col=global_key_col, extra_client=extra_client))
     if table_length != unique_global_key_count:
         print(f"Warning: Your global key column is not unique - upload will resume, only uploading 1 data row per unique global key")      
-    # Initiate your upload dict, where they keys are all your dataset IDs
-    if dataset_id:
-        upload_dict = {dataset_id : {}}
-    else:
-        upload_dict = {id : {} for id in get_unique_values(table=table, col=dataset_id_col)}
+
     # Create your column of upload dict values using UDFs
     uploads_table = create_uploads_column(
         client=client, table=table, row_data_col=row_data_col, global_key_col=global_key_col, external_id_col=external_id_col, 
         dataset_id_col=dataset_id_col, dataset_id=dataset_id, project_id_col=project_id_col, project_id=project_id, metadata_index=metadata_index, 
         attachment_index=attachment_index, annotation_index=annotation_index, 
         upload_method=upload_method, mask_method=mask_method, divider=divider, verbose=verbose 
     )
     # Query your uploads column and create your upload dict
-    res = uploads_table.select("uploads").rdd.map(lambda x: x.uploads.asDict()).collect()
+
+    upload_dict = {}
+    res = uploads_table.select("uploads").rdd.map(lambda x: {'data_row': {'row_data': x['uploads']['data_row']['row_data'], 'global_key': x['uploads']['data_row']['global_key'], 'external_id': x['uploads']['data_row']['external_id'], 'metadata_fields': x['uploads']['data_row']['metadata_fields'], 'attachments': x['uploads']['data_row']['attachments']}, 'dataset_id': x['uploads']['dataset_id'], 'project_id': x['uploads']['project_id'], 'annotations': x['uploads']['annotations']}).collect()
+
     with ThreadPoolExecutor() as exc:
         futures = [exc.submit(process_upload, x) for x in res]
         for future in as_completed(futures):
             y = future.result()
-            upload_dict[y["dataset_id"]][y["data_row"]["global_key"]] = {
+            upload_dict[y["data_row"]["global_key"]] = {
                 "data_row" : y["data_row"],
                 "project_id" : y["project_id"],
-                "annotations" : y["annotations"]
+                "annotations" : y["annotations"],
+                "dataset_id" : y["dataset_id"]
             }        
     return upload_dict
 
 def create_uploads_column(client:labelboxClient, table:pyspark.sql.dataframe.DataFrame,
                           row_data_col:str, global_key_col:str, external_id_col:str, 
                           dataset_id_col:str, dataset_id:str, project_id_col:str, project_id:str,
                           metadata_index:dict, attachment_index:dict, annotation_index:dict,
@@ -130,15 +130,18 @@
         project_ids = get_unique_values(table=table, col=project_id_col, extra_client=extra_client)
     else:
         project_ids = []
     project_id_to_ontology_index = {}        
     if (project_ids!=[]) and (annotation_index!={}) and (upload_method in ["mal", "import"]): # If we're uploading annotations
         for projectId in project_ids:
             ontology = client.get_project(projectId).ontology()
-            project_id_to_ontology_index[projectId] = get_ontology_schema_to_name_path(ontology=ontology,divider=divider,invert=True,detailed=True)    
+            project_type = client.get_project(projectId).media_type
+            project_id_to_ontology_index[projectId] = get_ontology_schema_to_name_path(ontology=ontology,divider=divider,invert=True,detailed=True)
+            project_id_to_ontology_index[projectId]['project_type'] = str(project_type)
+
     project_id_to_ontology_index_bytes = json.dumps(project_id_to_ontology_index)          
     # Create your upload column's syntax
     upload_schema = StructType([
         StructField(
             "data_row", StructType([
                 StructField("row_data", StringType()), StructField("global_key", StringType()), StructField("external_id", StringType()),
                 StructField("metadata_fields", ArrayType(MapType(StringType(), StringType(), True))),
@@ -149,29 +152,33 @@
         StructField("annotations", ArrayType(MapType(StringType(), StringType(), True)))
     ])
     x = get_metadata_schema_to_name_key(client=client, divider=divider, invert=True) # Get metadata dict where {key=name : value=schema_id}
     metadata_name_key_to_schema_bytes = json.dumps(x) # Convert reference dict to bytes    
     # Run a UDF to create row values
     data_rows_udf = udf(create_data_row, upload_schema)    
     project_input = lit(project_id_col) if not project_id_col else project_id_col
-    dataset_input = lit(dataset_id_col) if not dataset_id_col else dataset_id_col   
+    dataset_input = lit(dataset_id_col) if not dataset_id_col else dataset_id_col
+
     table = table.withColumn(
       'uploads', data_rows_udf(
           row_data_col, global_key_col, external_id_col, lit(metadata_name_key_to_schema_bytes),
           lit(project_id_col), project_input, lit(project_id), lit(dataset_id_col), dataset_input, lit(dataset_id)
       )
     )
+    print(table.collect()[0])
     # Run a UDF to add attachments, if applicable  
     if attachment_index:
+        print(attachment_index)
         attachments_udf = udf(create_attachments, upload_schema)  # Create a UDF
         for attachment_column_name in attachment_index: # Run this UDF for each attachment column in the attachment index
             attachment_type = attachment_index[attachment_column_name]
             table = table.withColumn('uploads', attachments_udf('uploads', lit(attachment_type), attachment_column_name))        
     # Run a UDF to add metadata, if applicable
     if metadata_index:
+        print(metadata_index)
         metadata_udf = udf(create_metadata, upload_schema) # Create a UDF
         for metadata_field_name in metadata_index: # Run this UDF for each metadata field name in the metadata index
             metadata_type = metadata_index[metadata_field_name]
             metadata_column_name = f"metadata{divider}{metadata_type}{divider}{metadata_field_name}"
             table = table.withColumn(
                 'uploads', metadata_udf(
                     'uploads', lit(metadata_field_name), metadata_column_name, lit(metadata_type), lit(metadata_name_key_to_schema_bytes), lit(divider)
@@ -181,15 +188,15 @@
     if (annotation_index!={}) and (project_id_to_ontology_index!={}) and (upload_method in ["mal", "import"]):
         annotation_udf = udf(create_annotations, upload_schema) # Create a UDF
         for annotation_column_name in annotation_index: # Run this UDF for each attachment column name in the attachment index
             top_level_feature_name = annotation_index[annotation_column_name]
             annotation_type = annotation_column_name.split(divider)[1]
             table = table.withColumn(
               'uploads', annotation_udf(
-                  'uploads', lit(top_level_feature_name), annotation_column_name, lit(mask_method), lit(project_id_to_ontology_index_bytes), lit(divider)
+                  'uploads', lit(top_level_feature_name), annotation_column_name, lit(mask_method), lit(annotation_type), lit(project_id_to_ontology_index_bytes), lit(divider)
               )
             )        
     return table
 
 def create_data_row(row_data_col, global_key_col, external_id_col, metadata_name_key_to_schema_bytes,
                     project_id_col_name, project_id_col_value, project_id_str,
                     dataset_id_col_name, dataset_id_col_value, dataset_id_str):
@@ -228,53 +235,49 @@
 def create_attachments(uploads_col, attachment_type, attachment_col_value):
     """ Function to-be-wrapped in a UDF that adds attachments to your upload dict
     """  
     if attachment_col_value:
         uploads_col["data_row"]["attachments"].append({"type" : attachment_type, "value" : attachment_col_value})
     return uploads_col  
 
-def create_annotations(uploads_col, top_level_feature_name, annotations, mask_method, project_id_to_ontology_index_bytes, divider):
+def create_annotations(uploads_col, top_level_feature_name, annotations, mask_method, annotation_type, project_id_to_ontology_index_bytes, divider):
     """ Function to-be-wrapped in a UDF that adds attachments to your upload dict
     """  
     project_id_to_ontology_index = json.loads(project_id_to_ontology_index_bytes)
     ontology_index = project_id_to_ontology_index[uploads_col["project_id"]]
-    uploads_col["annotations"].extend(
-        create_ndjsons(
-            top_level_name=top_level_feature_name,
-            annotation_inputs=annotations,
-            ontology_index=ontology_index,
-            mask_method=mask_method,
-            divider=divider    
+    print(annotations)
+    if annotations is not None:
+        annotation_list = []
+        ndjsons = create_ndjsons(
+                    top_level_name=top_level_feature_name,
+                    annotation_inputs=annotations,
+                    ontology_index=ontology_index,
+                    mask_method=mask_method,
+                    divider=divider    
+                )
+        for ndjson in ndjsons:
+            annotation_list.append({annotation_type:json.dumps(ndjson)})
+        print(annotation_list)
+        uploads_col["annotations"].extend(
+            annotation_list
         )
-    )
     return uploads_col
 
+
 def process_upload(x):
     """ Function to-be-multithreaded that processes rows into the upload_dict format
     """
     annotations = [string_to_ndjson(x) for x in x["annotations"]]
     return {
-        "data_row" : x["data_row"].asDict(),
+        "data_row" : x["data_row"],
         "project_id" : x["project_id"],
         "annotations" : annotations,
         "dataset_id" : x["dataset_id"]
     }
 
 def string_to_ndjson(annotation):
     """ Function that takes stringtype representation of an annotation and converts it into the Labelbox ndjson format
     """
     for key, value in annotation.items():
-        x = ""
-        if key == "bbox":
-            x = value.replace('width=', '"width":').replace('top=', '"top":').replace('left=', '"left":').replace('height=', '"height":') 
-        elif key == "mask":
-            x = value.replace('png=', '"png":"')[:-1] + '"}'
-        elif key in ["point", "line", "polygon"]:
-            x = value.replace('x=', '"x":').replace('y=', '"y":')
-        elif (key == "answers") or ((key=="answer") and ("}" in value)) or (key=="classifications"):
-            x = value.replace('answer=', '"answer": "').replace(', classifications=', '", "classifications":').replace('name=', '"name":"').replace(', "name":', '", "name":',).replace('}', '"}').replace(']"', ']').replace('"{', '{').replace('}"', '}')
-        else:
-            pass
-        if x:
-            annotation[key] = json.loads(x)
+        annotation[key] = json.loads(value)
     return annotation
```

### Comparing `labelspark-0.7.28/labelspark.egg-info/PKG-INFO` & `labelspark-0.7.29/labelspark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelspark
-Version: 0.7.28
+Version: 0.7.29
 Summary: Labelbox Connector for Databricks
 Home-page: https://github.com/Labelbox/LabelSpark.git
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
@@ -63,16 +63,14 @@
 | Putting it all Together        | [![Github](https://img.shields.io/badge/GitHub-100000?logo=github&logoColor=white)](notebooks/full-demo.ipynb)  | 
 ------
 
 ### Exporting Data
 
 |            Notebook            |  Github  |
 | ------------------------------ | -------- |
-| Exporting Data to a Spark Table*            | [![Github](https://img.shields.io/badge/GitHub-100000?logo=github&logoColor=white)](notebooks/export.ipynb)  |
+| Exporting Data to a Spark Table            | [![Github](https://img.shields.io/badge/GitHub-100000?logo=github&logoColor=white)](notebooks/export.ipynb)  |
 ------
 
-* = Coming Soon
-
 While using LabelSpark, you will likely also use the Labelbox SDK (e.g. for programmatic ontology creation). These resources will help familiarize you with the Labelbox Python SDK: 
 * [Visit our docs](https://docs.labelbox.com/reference/install-python-sdk) to learn how the SDK works
 * Checkout our [notebook examples](https://github.com/Labelbox/labelspark/tree/master/notebooks) to follow along with interactive tutorials
 * View the Labelbox [API reference](https://labelbox-python.readthedocs.io/en/latest/).
```

### Comparing `labelspark-0.7.28/labelspark.egg-info/SOURCES.txt` & `labelspark-0.7.29/labelspark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.28/setup.py` & `labelspark-0.7.29/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='labelspark',
-    version='0.7.28',
+    version='0.7.29',
     author='Labelbox',
     author_email="raphael@labelbox.com",      
     packages=find_packages(),
     url='https://github.com/Labelbox/LabelSpark.git',
     description='Labelbox Connector for Databricks',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

