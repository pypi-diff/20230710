# Comparing `tmp/shaku-database-1.1.2.tar.gz` & `tmp/shaku-database-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaku-database-1.1.2.tar", last modified: Fri Jul  7 09:42:02 2023, max compression
+gzip compressed data, was "shaku-database-1.1.3.tar", last modified: Mon Jul 10 06:31:13 2023, max compression
```

## Comparing `shaku-database-1.1.2.tar` & `shaku-database-1.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:42:02.358436 shaku-database-1.1.2/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.1.2/LICENSE
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-07 09:42:02.358236 shaku-database-1.1.2/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.1.2/README.md
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:42:02.355414 shaku-database-1.1.2/database/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.2/database/__init__.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:42:02.355983 shaku-database-1.1.2/database/bigquery/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.2/database/bigquery/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1452 2023-07-07 09:40:34.000000 shaku-database-1.1.2/database/bigquery/bq_sql_parser.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-20 03:32:33.000000 shaku-database-1.1.2/database/bigquery/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:42:02.356388 shaku-database-1.1.2/database/cloud_sql/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.2/database/cloud_sql/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1139 2023-06-16 06:51:48.000000 shaku-database-1.1.2/database/cloud_sql/crud.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:42:02.356620 shaku-database-1.1.2/gdrive_gcs_toolkit/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.2/gdrive_gcs_toolkit/__init__.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:42:02.356880 shaku-database-1.1.2/gdrive_gcs_toolkit/cloud_storage/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.2/gdrive_gcs_toolkit/cloud_storage/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-07-07 09:40:26.000000 shaku-database-1.1.2/gdrive_gcs_toolkit/cloud_storage/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:42:02.357277 shaku-database-1.1.2/gdrive_gcs_toolkit/google_shared_drive/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.2/gdrive_gcs_toolkit/google_shared_drive/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)    11602 2023-07-07 09:40:26.000000 shaku-database-1.1.2/gdrive_gcs_toolkit/google_shared_drive/util.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-07-07 09:42:02.358480 shaku-database-1.1.2/setup.cfg
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1169 2023-07-07 09:40:50.000000 shaku-database-1.1.2/setup.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:42:02.358044 shaku-database-1.1.2/shaku_database.egg-info/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-07 09:42:02.000000 shaku-database-1.1.2/shaku_database.egg-info/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)      600 2023-07-07 09:42:02.000000 shaku-database-1.1.2/shaku_database.egg-info/SOURCES.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-07-07 09:42:02.000000 shaku-database-1.1.2/shaku_database.egg-info/dependency_links.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1044 2023-07-07 09:42:02.000000 shaku-database-1.1.2/shaku_database.egg-info/requires.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)       28 2023-07-07 09:42:02.000000 shaku-database-1.1.2/shaku_database.egg-info/top_level.txt
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-10 06:31:13.218353 shaku-database-1.1.3/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.1.3/LICENSE
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-10 06:31:13.218112 shaku-database-1.1.3/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.1.3/README.md
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-10 06:31:13.215652 shaku-database-1.1.3/database/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.3/database/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-10 06:31:13.216021 shaku-database-1.1.3/database/bigquery/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.3/database/bigquery/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1452 2023-07-07 09:40:34.000000 shaku-database-1.1.3/database/bigquery/bq_sql_parser.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-20 03:32:33.000000 shaku-database-1.1.3/database/bigquery/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-10 06:31:13.216296 shaku-database-1.1.3/database/cloud_sql/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.3/database/cloud_sql/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1139 2023-06-16 06:51:48.000000 shaku-database-1.1.3/database/cloud_sql/crud.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-10 06:31:13.216429 shaku-database-1.1.3/gdrive_gcs_toolkit/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.3/gdrive_gcs_toolkit/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-10 06:31:13.216738 shaku-database-1.1.3/gdrive_gcs_toolkit/cloud_storage/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.3/gdrive_gcs_toolkit/cloud_storage/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-07-07 09:40:26.000000 shaku-database-1.1.3/gdrive_gcs_toolkit/cloud_storage/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-10 06:31:13.217135 shaku-database-1.1.3/gdrive_gcs_toolkit/google_shared_drive/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.3/gdrive_gcs_toolkit/google_shared_drive/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)    11601 2023-07-10 06:30:13.000000 shaku-database-1.1.3/gdrive_gcs_toolkit/google_shared_drive/util.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-07-10 06:31:13.218396 shaku-database-1.1.3/setup.cfg
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1169 2023-07-10 06:30:17.000000 shaku-database-1.1.3/setup.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-10 06:31:13.217898 shaku-database-1.1.3/shaku_database.egg-info/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-10 06:31:13.000000 shaku-database-1.1.3/shaku_database.egg-info/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)      600 2023-07-10 06:31:13.000000 shaku-database-1.1.3/shaku_database.egg-info/SOURCES.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-07-10 06:31:13.000000 shaku-database-1.1.3/shaku_database.egg-info/dependency_links.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1044 2023-07-10 06:31:13.000000 shaku-database-1.1.3/shaku_database.egg-info/requires.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       28 2023-07-10 06:31:13.000000 shaku-database-1.1.3/shaku_database.egg-info/top_level.txt
```

### Comparing `shaku-database-1.1.2/LICENSE` & `shaku-database-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.2/PKG-INFO` & `shaku-database-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.1.2
+Version: 1.1.3
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shaku-database-1.1.2/README.md` & `shaku-database-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.2/database/bigquery/bq_sql_parser.py` & `shaku-database-1.1.3/database/bigquery/bq_sql_parser.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.2/database/bigquery/util.py` & `shaku-database-1.1.3/database/bigquery/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.2/database/cloud_sql/crud.py` & `shaku-database-1.1.3/database/cloud_sql/crud.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.2/gdrive_gcs_toolkit/cloud_storage/util.py` & `shaku-database-1.1.3/gdrive_gcs_toolkit/cloud_storage/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.2/gdrive_gcs_toolkit/google_shared_drive/util.py` & `shaku-database-1.1.3/gdrive_gcs_toolkit/google_shared_drive/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
 
         file_extension = Path(file_name).suffix
 
         try:
 
             if file_extension == ".csv":
                 # .csv is textual data so use StringIO
-                data_buffer = io.StringIO()
+                data_buffer = io.BytesIO()
                 df.to_csv(data_buffer, index=False)
                 mimetype = 'text/csv'
             elif file_extension in [".xlsx", ".xls"]:
                 # .xlsx and .xls are binary data so use BytesIO
                 data_buffer = io.BytesIO()
                 df.to_excel(data_buffer, index=False, engine='openpyxl')
                 mimetype = 'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet'
```

### Comparing `shaku-database-1.1.2/setup.py` & `shaku-database-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 HERE = pathlib.Path(__file__).parent.resolve()
 requirements = (HERE / "requirements.txt").read_text(encoding="utf8")
 EX_INSTALL_REQUIRES = {s.strip().split('==')[0]: s.strip().split('==')[1] if len(s.strip().split('==')) > 1 else ""
                        for s in requirements.split("\n")}
 INSTALL_REQUIRES = [s.strip() for s in requirements.split("\n")]
 setup(
     name="shaku-database",
-    version="1.1.2",
+    version="1.1.3",
     author="hawktorng",
     author_email="hawktorng@shaku.com.tw",
     description="Shaku Database util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/hawktorng1/test_shaku",
     packages=find_packages(),
```

### Comparing `shaku-database-1.1.2/shaku_database.egg-info/PKG-INFO` & `shaku-database-1.1.3/shaku_database.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.1.2
+Version: 1.1.3
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shaku-database-1.1.2/shaku_database.egg-info/SOURCES.txt` & `shaku-database-1.1.3/shaku_database.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.2/shaku_database.egg-info/requires.txt` & `shaku-database-1.1.3/shaku_database.egg-info/requires.txt`

 * *Files identical despite different names*

