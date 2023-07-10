# Comparing `tmp/airflow-data-validation-4.0.5.tar.gz` & `tmp/airflow-data-validation-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-data-validation-4.0.5.tar", max compression
+gzip compressed data, was "airflow-data-validation-4.0.6.tar", max compression
```

## Comparing `airflow-data-validation-4.0.5.tar` & `airflow-data-validation-4.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-06 08:59:19.718494 airflow-data-validation-4.0.5/README.md
--rw-r--r--   0        0        0        0 2023-06-08 08:24:12.682050 airflow-data-validation-4.0.5/airflow_data_validation/__init__.py
--rw-r--r--   0        0        0    10421 2023-07-09 12:00:47.761778 airflow-data-validation-4.0.5/airflow_data_validation/data_validation.py
--rw-r--r--   0        0        0      279 2023-07-09 12:05:10.216892 airflow-data-validation-4.0.5/airflow_data_validation/setup.py
--rw-r--r--   0        0        0      603 2023-07-09 12:11:58.824024 airflow-data-validation-4.0.5/pyproject.toml
--rw-r--r--   0        0        0      710 2023-07-09 12:12:02.125887 airflow-data-validation-4.0.5/setup.py
--rw-r--r--   0        0        0      694 2023-07-09 12:12:02.126101 airflow-data-validation-4.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-06 08:59:19.718494 airflow-data-validation-4.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 08:24:12.682050 airflow-data-validation-4.0.6/airflow_data_validation/__init__.py
+-rw-r--r--   0        0        0    10424 2023-07-10 06:10:41.840031 airflow-data-validation-4.0.6/airflow_data_validation/data_validation.py
+-rw-r--r--   0        0        0      279 2023-07-09 12:05:10.216892 airflow-data-validation-4.0.6/airflow_data_validation/setup.py
+-rw-r--r--   0        0        0      603 2023-07-10 06:13:34.983327 airflow-data-validation-4.0.6/pyproject.toml
+-rw-r--r--   0        0        0      710 2023-07-10 06:13:37.981975 airflow-data-validation-4.0.6/setup.py
+-rw-r--r--   0        0        0      694 2023-07-10 06:13:37.982190 airflow-data-validation-4.0.6/PKG-INFO
```

### Comparing `airflow-data-validation-4.0.5/airflow_data_validation/data_validation.py` & `airflow-data-validation-4.0.6/airflow_data_validation/data_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             SELECT MAX(_CHANGE_TIMESTAMP) dt
               FROM appends(table `{destination_table}`, '2023-06-29', null)
              WHERE _CHANGE_TYPE = 'INSERT'
         '''
         if is_partitioned:
             sql = f'''SELECT MAX({partition_field}) dt
                         FROM `{destination_table}` 
-                        WHERE {partition_field} >= DATE_SUB(current_date, INTERVAL 2 DAY)))'''
+                        WHERE {partition_field} >= DATE_SUB(current_date, INTERVAL 2 DAY)'''
 
         final_sql = f'''
         SELECT EXISTS (SELECT *
                FROM   ({sql}) c
                WHERE  DATE(dt) != CURRENT_DATE()) 
                 '''
         return final_sql
@@ -179,15 +179,15 @@
             elif isinstance(value, float):
                 float_value = float(value)
                 integer_value = int(float_value)
                 return integer_value
             else:
                 raise Exception("Error: Unable to convert the value to an integer.")
 
-    def test_data(self, destination_table, test_name, column_ids_list,
+    def test_data(self, destination_table, test_name, column_ids_list=None,
                   is_partitioned=False, min_value=None, max_value=None,
                   set_of_values=None, partition_field='partition_date', exit_on_failure=False):
         ## duplication QA ##
         if destination_table:
             self.table_name = destination_table.split('.')[2]
 
         if test_name == 'expect_columns_distinct_values':
```

### Comparing `airflow-data-validation-4.0.5/pyproject.toml` & `airflow-data-validation-4.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airflow-data-validation"
-version = "4.0.5"
+version = "4.0.6"
 description = ""
 authors = ["sapir.krespil <sapir.krespil@guesty.com>"]
 readme = "README.md"
 homepage = "https://github.com/guestyorg/airflow_data_validation"
 repository = "https://github.com/guestyorg/airflow_data_validation"
 packages = [{include = "airflow_data_validation"}]
```

### Comparing `airflow-data-validation-4.0.5/setup.py` & `airflow-data-validation-4.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['google-cloud-bigquery>=2.4.0,<3.0.0', 'requests>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'airflow-data-validation',
-    'version': '4.0.5',
+    'version': '4.0.6',
     'description': '',
     'long_description': '',
     'author': 'sapir.krespil',
     'author_email': 'sapir.krespil@guesty.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/guestyorg/airflow_data_validation',
```

### Comparing `airflow-data-validation-4.0.5/PKG-INFO` & `airflow-data-validation-4.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-data-validation
-Version: 4.0.5
+Version: 4.0.6
 Summary: 
 Home-page: https://github.com/guestyorg/airflow_data_validation
 Author: sapir.krespil
 Author-email: sapir.krespil@guesty.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

