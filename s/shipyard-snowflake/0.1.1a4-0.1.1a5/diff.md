# Comparing `tmp/shipyard_snowflake-0.1.1a4.tar.gz` & `tmp/shipyard_snowflake-0.1.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_snowflake-0.1.1a4.tar", max compression
+gzip compressed data, was "shipyard_snowflake-0.1.1a5.tar", max compression
```

## Comparing `shipyard_snowflake-0.1.1a4.tar` & `shipyard_snowflake-0.1.1a5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-05-03 22:01:51.349436 shipyard_snowflake-0.1.1a4/README.md
--rw-r--r--   0        0        0      684 2023-07-06 14:56:44.163150 shipyard_snowflake-0.1.1a4/pyproject.toml
--rw-r--r--   0        0        0      172 2023-07-05 22:46:06.931185 shipyard_snowflake-0.1.1a4/shipyard_snowflake/__init__.py
--rw-r--r--   0        0        0      605 2023-07-06 03:14:48.097910 shipyard_snowflake-0.1.1a4/shipyard_snowflake/cli/authtest.py
--rw-r--r--   0        0        0     2299 2023-07-06 14:38:13.916031 shipyard_snowflake-0.1.1a4/shipyard_snowflake/cli/execute_sql.py
--rw-r--r--   0        0        0     3822 2023-07-06 14:37:31.909918 shipyard_snowflake-0.1.1a4/shipyard_snowflake/cli/fetch.py
--rw-r--r--   0        0        0     5843 2023-07-06 14:42:34.285035 shipyard_snowflake-0.1.1a4/shipyard_snowflake/cli/upload.py
--rw-r--r--   0        0        0     5744 2023-07-06 13:23:29.267906 shipyard_snowflake-0.1.1a4/shipyard_snowflake/snowflake.py
--rw-r--r--   0        0        0     1828 2023-07-05 22:46:06.932851 shipyard_snowflake-0.1.1a4/shipyard_snowflake/test/tests.py
--rw-r--r--   0        0        0     5580 2023-07-06 14:22:11.764268 shipyard_snowflake-0.1.1a4/shipyard_snowflake/utils.py
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 shipyard_snowflake-0.1.1a4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-03 22:01:51.349436 shipyard_snowflake-0.1.1a5/README.md
+-rw-r--r--   0        0        0      684 2023-07-10 21:17:17.942299 shipyard_snowflake-0.1.1a5/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-07-10 21:17:17.943024 shipyard_snowflake-0.1.1a5/shipyard_snowflake/__init__.py
+-rw-r--r--   0        0        0      808 2023-07-10 21:17:17.943716 shipyard_snowflake-0.1.1a5/shipyard_snowflake/cli/authtest.py
+-rw-r--r--   0        0        0     2195 2023-07-10 21:17:17.944125 shipyard_snowflake-0.1.1a5/shipyard_snowflake/cli/execute_sql.py
+-rw-r--r--   0        0        0     3533 2023-07-10 21:17:17.944462 shipyard_snowflake-0.1.1a5/shipyard_snowflake/cli/fetch.py
+-rw-r--r--   0        0        0     6420 2023-07-10 21:17:17.944714 shipyard_snowflake-0.1.1a5/shipyard_snowflake/cli/upload.py
+-rw-r--r--   0        0        0     5556 2023-07-10 21:17:17.945116 shipyard_snowflake-0.1.1a5/shipyard_snowflake/snowflake.py
+-rw-r--r--   0        0        0     1828 2023-07-10 21:17:17.945669 shipyard_snowflake-0.1.1a5/shipyard_snowflake/test/tests.py
+-rw-r--r--   0        0        0     5580 2023-07-10 21:17:17.946185 shipyard_snowflake-0.1.1a5/shipyard_snowflake/utils.py
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 shipyard_snowflake-0.1.1a5/PKG-INFO
```

### Comparing `shipyard_snowflake-0.1.1a4/pyproject.toml` & `shipyard_snowflake-0.1.1a5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-snowflake"
-version = "0.1.1a4"
+version = "0.1.1a5"
 description = "A local client for conecting and working with Snowflake"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "shipyard_snowflake"}]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_snowflake-0.1.1a4/shipyard_snowflake/cli/authtest.py` & `shipyard_snowflake-0.1.1a5/shipyard_snowflake/cli/authtest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import os
 from shipyard_blueprints import SnowflakeClient
+from shipyard_templates import ExitCodeException
 
 
 def get_args():
     args = {}
     args["user"] = os.getenv("SNOWFLAKE_USERNAME")
     args["password"] = os.getenv("SNOWFLAKE_PASSWORD")
     args["account"] = os.getenv("SNOWFLAKE_ACCOUNT")
@@ -14,16 +15,18 @@
 def main():
     args = get_args()
     user = args["user"]
     pwd = args["password"]
     account = args["account"]
 
     snowflake = SnowflakeClient(username=user, pwd=pwd, account=account)
-    conn = snowflake.connect()
-    if conn == 1:
-        return 1
-    else:
+    try:
+        conn = snowflake.connect()
+        snowflake.logger.info("Successfully connected to Snowflake")
         return 0
+    except ExitCodeException as e:
+        snowflake.logger.error("Could not connect to Snowflake")
+        return 1
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_snowflake-0.1.1a4/shipyard_snowflake/cli/execute_sql.py` & `shipyard_snowflake-0.1.1a5/shipyard_snowflake/cli/execute_sql.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,16 +19,15 @@
     )
     parser.add_argument("--account", dest="account", required=True)
     parser.add_argument("--warehouse", dest="warehouse", required=False)
     parser.add_argument("--database", dest="database", required=True)
     parser.add_argument("--schema", dest="schema", required=False, default="")
     parser.add_argument("--query", dest="query", required=True)
     parser.add_argument("--user-role", dest="user_role", required=False, default="")
-    args = parser.parse_args()
-    return args
+    return parser.parse_args()
 
 
 def main():
     args = get_args()
     client_args = {
         "username": args.username,
         "pwd": None if args.password == "" else args.password,
@@ -44,19 +43,17 @@
     )
     client = SnowflakeClient(**client_args)
     if client.rsa_key and not private_key_passphrase:
         client.logger.error(
             "Private key passphrase is required when using a private key"
         )
         sys.exit(client.EXIT_CODE_INVALID_CREDENTIALS)
-    conn = client.connect()
-    if conn == 1:
-        sys.exit(client.EXIT_CODE_INVALID_CREDENTIALS)
     try:
+        conn = client.connect()
         client.execute_query(conn=conn, query=args.query)
     except ExitCodeException as e:
         client.logger.error(e)
-        sys.exit(client.EXIT_CODE_INVALID_QUERY)
+        sys.exit(e.exit_code)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_snowflake-0.1.1a4/shipyard_snowflake/cli/fetch.py` & `shipyard_snowflake-0.1.1a5/shipyard_snowflake/cli/fetch.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,16 +32,15 @@
         default="",
         required=False,
     )
     parser.add_argument(
         "--file-header", dest="file_header", default="True", required=False
     )
     parser.add_argument("--user-role", dest="user_role", required=False, default="")
-    args = parser.parse_args()
-    return args
+    return parser.parse_args()
 
 
 def main():
     args = get_args()
     client_args = {
         "username": args.username,
         "pwd": None if args.password == "" else args.password,
@@ -70,31 +69,26 @@
     if client.rsa_key and not private_key_passphrase:
         client.logger.error(
             "Error: A private key passphrase must be provided if using a private key"
         )
         sys.exit(client.EXIT_CODE_INVALID_ARGUMENTS)
     try:
         conn = client.connect()
-        if conn == 1:
-            sys.exit(client.EXIT_CODE_INVALID_CREDENTIALS)
     except ExitCodeException as e:
-        if client_args["password"] != "":
-            client.logger.error(
-                f"Ensure the password is correct for user {client_args['username']}"
-            )
-        if client_args["rsa_key"] != "":
-            client.logger.error(
-                f"Ensure the private key is correct for user {client_args['username']}"
-            )
+        client.logger.error(e.message)
         sys.exit(client.EXIT_CODE_INVALID_CREDENTIALS)
+
     df = client.fetch(conn, args.query)
+    if df.empty:
+        client.logger.error("No results returned from query")
+        sys.exit(client.EXIT_CODE_NO_RESULTS)
     try:
         df.to_csv(destination_full_path, index=False, header=file_header)
-        client.logger.info(f"Successfuly wrote file to {destination_full_path}")
-    except ExitCodeException as e:
+        client.logger.info(f"Successfully wrote file to {destination_full_path}")
+    except Exception as e:
         client.logger.error(f"Error writing file to {destination_full_path}")
         client.logger.error(e)
         sys.exit(client.EXIT_CODE_NO_RESULTS)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_snowflake-0.1.1a4/shipyard_snowflake/cli/upload.py` & `shipyard_snowflake-0.1.1a5/shipyard_snowflake/cli/upload.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,17 +53,15 @@
     parser.add_argument(
         "--snowflake-data-types",
         dest="snowflake_data_types",
         required=False,
         default="",
     )
     parser.add_argument("--user-role", dest="user_role", required=False, default="")
-    args = parser.parse_args()
-
-    return args
+    return parser.parse_args()
 
 
 def upload_multiple(
     client: SnowflakeClient,
     conn: snowflake.connector.connection.SnowflakeConnection,
     files: list,
     table_name: str,
@@ -116,40 +114,51 @@
     )
 
     if client.rsa_key and not private_key_passphrase:
         client.logger.error(
             "Error: A private key passphrase must be provided if using a private key"
         )
         sys.exit(client.EXIT_CODE_INVALID_ARGUMENTS)
-    if (not client.username and not client.pwd) and (
-        not client.username and not client.rsa_key
-    ):
+    if not client.pwd and not client.rsa_key:
         client.logger.error(
             "Error: Either a username and password must be provided, or a username and private key file"
         )
         sys.exit(client.EXIT_CODE_INVALID_CREDENTIALS)
 
-    conn = client.connect()  # establish connection to snowflake
+    try:
+        conn = client.connect()  # establish connection to snowflake
     # for authtests, connection returns 1 if unsuccessful
-    if conn == 1:
+    except ExitCodeException as e:
+        client.logger.error(e.message)
         sys.exit(client.EXIT_CODE_INVALID_CREDENTIALS)
+
     if args.snowflake_data_types != "":
         snowflake_data_types = ast.literal_eval(args.snowflake_data_types)
     else:
         snowflake_data_types = None
 
     if args.source_file_name_match_type == "regex_match":
         # match files based on pattern
         file_names = shipyard.find_all_local_file_names(args.source_folder_name)
         matching_file_names = shipyard.find_all_file_matches(
             file_names, re.compile(args.source_file_name)
         )
         client.logger.info(
             f"{len(matching_file_names)} files found. Preparing to upload..."
         )
+        for i, file_match in enumerate(matching_file_names, start=1):
+            client.logger.info(f"Uploading file {i} of {len(matching_file_names)}")
+            insert_method = args.insert_method
+            if insert_method == "replace" and i > 1:
+                insert_method = "append"
+            df = ss.read_file(file_match, snowflake_data_types)
+            success, nchunks, nrows, output = client.upload(
+                conn, df, table_name=args.table_name, if_exists=insert_method
+            )
+            client.logger.info(f"Uploaded {nrows} rows to {args.table_name}")
     else:
         fp = shipyard.combine_folder_and_file_name(
             args.source_folder_name, args.source_file_name
         )
         df = ss.read_file(fp, snowflake_data_types)
         success, nchunks, nrows, output = client.upload(
             conn, df, table_name=args.table_name, if_exists=args.insert_method
```

### Comparing `shipyard_snowflake-0.1.1a4/shipyard_snowflake/snowflake.py` & `shipyard_snowflake-0.1.1a5/shipyard_snowflake/snowflake.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import snowflake.connector
 import pandas as pd
 from dask import dataframe as dd
 from typing import Dict, List, Optional, Tuple, Union
-from shipyard_templates import Database, ExitCodeError, ExitCodeException
+from shipyard_templates import Database, ExitCodeException
 from snowflake.connector import pandas_tools as pt
 from .utils import (
     _decode_rsa,
     _file_fits_in_memory,
     _get_file_size,
     _get_memory,
     map_snowflake_to_pandas,
@@ -62,56 +62,54 @@
                     account=self.account,
                     private_key=private_key,
                     warehouse=self.warehouse,
                     database=self.database,
                     schema=self.schema,
                     role=self.role,
                 )
-                self.logger.info(f"Successfully connected to Snowflake")
+                self.logger.info("Successfully connected to Snowflake")
                 return con
             except Exception as e:
-                self.logger.error(
-                    f"Could not authenticate to Snowflake for user {self.username} with credentials in {self.rsa_key}"
+                raise ExitCodeException(
+                    message=f"Could not authenticate to Snowflake for user {self.username} with credentials in {self.rsa_key}",
+                    exit_code=self.EXIT_CODE_INVALID_CREDENTIALS,
                 )
-                self.logger.exception(e)
-                return 1
         else:
             try:
                 con = snowflake.connector.connect(
                     user=self.username,
                     password=self.pwd,
                     account=self.account,
                     warehouse=self.warehouse,
                     database=self.database,
                     schema=self.schema,
                     role=self.role,
                 )
-                self.logger.info(f"Successfully connected to snowflake")
+                self.logger.info("Successfully connected to snowflake")
                 return con
             except Exception as e:
-                self.logger.error(
-                    f"Could not authenticate to account {self.account} for user {self.username}"
+                raise ExitCodeException(
+                    f"Could not authenticate to Snowflake due to {e}",
+                    self.EXIT_CODE_INVALID_CREDENTIALS,
                 )
-                self.logger.exception(e)
-                return 1  # failed connection
 
     def upload(
         self,
         conn: snowflake.connector.SnowflakeConnection,
         df: pd.DataFrame,
         table_name: str,
         if_exists: str = "replace",
     ):
         """Uploads a pandas dataframe to a snowflake table
 
         Args:
             conn (snowflake.connector.SnowflakeConnection): The snowflake connection object
             df (pd.DataFrame): The dataframe to be uploaded
             table_name (str): The name of the Snowflake Table to, if it doesn't exist, it will be created
-            insert_method (str): The method to use when inserting the data into the table. Options are replace or append Defaults to 'replace'
+            if_exists (str): The method to use when inserting the data into the table. Options are replace or append Defaults to 'replace'
 
         Returns:
             _type_: A tuple of the success of the upload, the number of chunks, the number of rows, and the output
         """
         if if_exists not in ["replace", "append"]:
             raise ExitCodeException(
                 f"Invalid insert method: {if_exists} is not a valid insert method. Choose between 'replace' or 'append'",
@@ -120,23 +118,21 @@
 
         if if_exists == "replace":
             self.logger.info("Uploading data to Snowflake via replace")
             self.execute_query(conn, f"DROP TABLE IF EXISTS {table_name}")
             success, nchunks, nrows, output = pt.write_pandas(
                 conn=conn, df=df, table_name=table_name, auto_create_table=True
             )
-            self.logger.info("Successfully uploaded data to Snowflake")
-            return success, nchunks, nrows, output
         else:
             self.logger.info("Uploading data to Snowflake via append")
             success, nchunks, nrows, output = pt.write_pandas(
                 conn=conn, df=df, table_name=table_name
             )
-            self.logger.info("Successfully uploaded data to Snowflake")
-            return success, nchunks, nrows, output
+        self.logger.info("Successfully uploaded data to Snowflake")
+        return success, nchunks, nrows, output
 
     def execute_query(
         self, conn: snowflake.connector.SnowflakeConnection, query: str
     ) -> snowflake.connector.cursor.SnowflakeCursor:
         try:
             cursor = conn.cursor()
             cursor.execute(query)
```

### Comparing `shipyard_snowflake-0.1.1a4/shipyard_snowflake/test/tests.py` & `shipyard_snowflake-0.1.1a5/shipyard_snowflake/test/tests.py`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.1.1a4/shipyard_snowflake/utils.py` & `shipyard_snowflake-0.1.1a5/shipyard_snowflake/utils.py`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.1.1a4/PKG-INFO` & `shipyard_snowflake-0.1.1a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-snowflake
-Version: 0.1.1a4
+Version: 0.1.1a5
 Summary: A local client for conecting and working with Snowflake
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

