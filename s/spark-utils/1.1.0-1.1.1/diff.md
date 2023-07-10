# Comparing `tmp/spark_utils-1.1.0.tar.gz` & `tmp/spark_utils-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_utils-1.1.0.tar", max compression
+gzip compressed data, was "spark_utils-1.1.1.tar", max compression
```

## Comparing `spark_utils-1.1.0.tar` & `spark_utils-1.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1075 2023-05-30 16:08:05.598116 spark_utils-1.1.0/LICENSE
--rw-r--r--   0        0        0     6766 2023-05-30 16:08:05.598116 spark_utils-1.1.0/README.md
--rw-r--r--   0        0        0      791 2023-05-30 16:08:21.997662 spark_utils-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1135 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/__init__.py
--rw-r--r--   0        0        0       22 2023-05-30 16:08:21.997662 spark_utils-1.1.0/spark_utils/_version.py
--rw-r--r--   0        0        0     1134 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/common/__init__.py
--rw-r--r--   0        0        0     4257 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/common/functions.py
--rw-r--r--   0        0        0     5977 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/common/spark_job_args.py
--rw-r--r--   0        0        0     9716 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/common/spark_session_provider.py
--rw-r--r--   0        0        0     3381 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/common/spark_sql_utils.py
--rw-r--r--   0        0        0     1449 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/common/spark_udf.py
--rw-r--r--   0        0        0     1135 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/dataframes/__init__.py
--rw-r--r--   0        0        0    10376 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/dataframes/functions.py
--rw-r--r--   0        0        0     2325 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/dataframes/models.py
--rw-r--r--   0        0        0     1135 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/dataframes/sets/__init__.py
--rw-r--r--   0        0        0     1631 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/dataframes/sets/functions.py
--rw-r--r--   0        0        0     1135 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/delta_lake/__init__.py
--rw-r--r--   0        0        0     1691 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/delta_lake/delta_log.py
--rw-r--r--   0        0        0     5982 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/delta_lake/functions.py
--rw-r--r--   0        0        0     1135 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/models/__init__.py
--rw-r--r--   0        0        0     1641 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/models/hive_metastore_config.py
--rw-r--r--   0        0        0     1318 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/models/hive_table.py
--rw-r--r--   0        0        0     1868 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/models/job_socket.py
--rw-r--r--   0        0        0     1129 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/models/k8s_config.py
--rw-r--r--   0        0        0     7658 1970-01-01 00:00:00.000000 spark_utils-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-10 08:41:14.574930 spark_utils-1.1.1/LICENSE
+-rw-r--r--   0        0        0     6766 2023-07-10 08:41:14.574930 spark_utils-1.1.1/README.md
+-rw-r--r--   0        0        0      791 2023-07-10 08:41:35.873870 spark_utils-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1135 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-10 08:41:35.873870 spark_utils-1.1.1/spark_utils/_version.py
+-rw-r--r--   0        0        0     1134 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/common/__init__.py
+-rw-r--r--   0        0        0     4257 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/common/functions.py
+-rw-r--r--   0        0        0     5977 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/common/spark_job_args.py
+-rw-r--r--   0        0        0    11437 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/common/spark_session_provider.py
+-rw-r--r--   0        0        0     3381 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/common/spark_sql_utils.py
+-rw-r--r--   0        0        0     1449 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/common/spark_udf.py
+-rw-r--r--   0        0        0     1135 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0    10376 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/dataframes/functions.py
+-rw-r--r--   0        0        0     2325 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/dataframes/models.py
+-rw-r--r--   0        0        0     1135 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/dataframes/sets/__init__.py
+-rw-r--r--   0        0        0     1631 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/dataframes/sets/functions.py
+-rw-r--r--   0        0        0     1135 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/delta_lake/__init__.py
+-rw-r--r--   0        0        0     1691 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/delta_lake/delta_log.py
+-rw-r--r--   0        0        0     5982 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/delta_lake/functions.py
+-rw-r--r--   0        0        0     1135 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/models/__init__.py
+-rw-r--r--   0        0        0     1641 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/models/hive_metastore_config.py
+-rw-r--r--   0        0        0     1318 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/models/hive_table.py
+-rw-r--r--   0        0        0     1868 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/models/job_socket.py
+-rw-r--r--   0        0        0     1129 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/models/k8s_config.py
+-rw-r--r--   0        0        0     7658 1970-01-01 00:00:00.000000 spark_utils-1.1.1/PKG-INFO
```

### Comparing `spark_utils-1.1.0/LICENSE` & `spark_utils-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.0/README.md` & `spark_utils-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.0/pyproject.toml` & `spark_utils-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "spark-utils"
-version = "1.1.0"
+version = "1.1.1"
 description = "Utility classes for comfy Spark job authoriing."
 authors = ["ECCO Sneaks & Data <esdsupport@ecco.com>"]
 maintainers = ['GZU <gzu@ecco.com>', 'JRB <ext-jrb@ecco.com>']
 license = 'MIT'
 readme = "README.md"
 repository = 'https://github.com/SneaksAndData/spark-utils'
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
-hadoop-fs-wrapper = "~0.6.0"
+hadoop-fs-wrapper = "~0.6.1"
 cryptography = "~36.0"
 delta-spark = "~2.4.0"
 
 kubernetes = { version = "24.2.0", optional = true }
 
 [tool.poetry.extras]
 k8s = [
```

### Comparing `spark_utils-1.1.0/spark_utils/__init__.py` & `spark_utils-1.1.1/spark_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.0/spark_utils/common/__init__.py` & `spark_utils-1.1.1/spark_utils/common/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.0/spark_utils/common/functions.py` & `spark_utils-1.1.1/spark_utils/common/functions.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.0/spark_utils/common/spark_job_args.py` & `spark_utils-1.1.1/spark_utils/common/spark_job_args.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.0/spark_utils/common/spark_session_provider.py` & `spark_utils-1.1.1/spark_utils/common/spark_session_provider.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """
   Provides convenient building of a Spark Session
 """
+import base64
 import json
 import os
 import tempfile
 import uuid
 from typing import Optional, List, Dict
 
 try:
@@ -130,14 +131,47 @@
     @property
     def session_builder(self) -> pyspark.sql.session.SparkSession.Builder:
         """
         Return a current session builder object.
         """
         return self._spark_session_builder
 
+    def with_astra_db(
+        self, db_name: str, bundle_bytes: str, client_id: str, client_secret: str
+    ) -> "SparkSessionProvider":
+        """
+        If you do not have the jar available, remember to create the session provider with this package added:
+          SparkSessionProvider(additional_packages=["com.datastax.spark:spark-cassandra-connector_2.12:3.4.0"])
+
+        :param db_name: Astra database name to use as Spark Catalog reference
+        :param bundle_bytes: Base64 encoded secure bundle zip content. Generate with `cat bundle.zip | base64`
+        :param client_id: Connection token client id
+        :param client_secret: Connection token client secret
+        """
+        bundle_file_name = f"{db_name}_bundle"
+        bundle_path = os.path.join(tempfile.gettempdir(), ".astra")
+        os.makedirs(bundle_path, exist_ok=True)
+
+        with open(os.path.join(bundle_path, bundle_file_name), "wb") as bundle_file:
+            bundle_file.write(base64.b64decode(bundle_bytes))
+
+        self._spark_session_builder = (
+            self._spark_session_builder.config(
+                "spark.sql.extensions", "com.datastax.spark.connector.CassandraSparkExtensions"
+            )
+            .config(f"spark.sql.catalog.{db_name}", "com.datastax.spark.connector.datasource.CassandraCatalog")
+            .config("spark.files", os.path.join(bundle_path, bundle_file_name))
+            .config("spark.cassandra.connection.config.cloud.path", bundle_file_name)
+            .config("spark.cassandra.auth.username", client_id)
+            .config("spark.cassandra.auth.password", client_secret)
+            .config("spark.dse.continuousPagingEnabled", "false")
+        )
+
+        return self
+
     def configure_for_k8s(
         self, master_url: str, spark_config: SparkKubernetesConfig, master_port: int = 443
     ) -> "SparkSessionProvider":
         """
         Configures spark session for using Kubernetes as a resource manager.
 
         :param master_url: Kubernetes API URL, i.e. https://my-server-api.mydomain.com.
```

### Comparing `spark_utils-1.1.0/spark_utils/common/spark_sql_utils.py` & `spark_utils-1.1.1/spark_utils/common/spark_sql_utils.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.0/spark_utils/common/spark_udf.py` & `spark_utils-1.1.1/spark_utils/common/spark_udf.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.0/spark_utils/dataframes/__init__.py` & `spark_utils-1.1.1/spark_utils/dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.0/spark_utils/dataframes/functions.py` & `spark_utils-1.1.1/spark_utils/dataframes/functions.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.0/spark_utils/dataframes/models.py` & `spark_utils-1.1.1/spark_utils/dataframes/models.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.0/spark_utils/dataframes/sets/__init__.py` & `spark_utils-1.1.1/spark_utils/dataframes/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.0/spark_utils/dataframes/sets/functions.py` & `spark_utils-1.1.1/spark_utils/dataframes/sets/functions.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.0/spark_utils/delta_lake/__init__.py` & `spark_utils-1.1.1/spark_utils/delta_lake/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.0/spark_utils/delta_lake/delta_log.py` & `spark_utils-1.1.1/spark_utils/delta_lake/delta_log.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.0/spark_utils/delta_lake/functions.py` & `spark_utils-1.1.1/spark_utils/delta_lake/functions.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.0/spark_utils/models/__init__.py` & `spark_utils-1.1.1/spark_utils/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.0/spark_utils/models/hive_metastore_config.py` & `spark_utils-1.1.1/spark_utils/models/hive_metastore_config.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.0/spark_utils/models/hive_table.py` & `spark_utils-1.1.1/spark_utils/models/hive_table.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.0/spark_utils/models/job_socket.py` & `spark_utils-1.1.1/spark_utils/models/job_socket.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.0/spark_utils/models/k8s_config.py` & `spark_utils-1.1.1/spark_utils/models/k8s_config.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.0/PKG-INFO` & `spark_utils-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-utils
-Version: 1.1.0
+Version: 1.1.1
 Summary: Utility classes for comfy Spark job authoriing.
 Home-page: https://github.com/SneaksAndData/spark-utils
 License: MIT
 Author: ECCO Sneaks & Data
 Author-email: esdsupport@ecco.com
 Maintainer: GZU
 Maintainer-email: gzu@ecco.com
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: k8s
 Requires-Dist: cryptography (>=36.0,<36.1)
 Requires-Dist: delta-spark (>=2.4.0,<2.5.0)
-Requires-Dist: hadoop-fs-wrapper (>=0.6.0,<0.7.0)
+Requires-Dist: hadoop-fs-wrapper (>=0.6.1,<0.7.0)
 Requires-Dist: kubernetes (==24.2.0) ; extra == "k8s"
 Project-URL: Repository, https://github.com/SneaksAndData/spark-utils
 Description-Content-Type: text/markdown
 
 # Introduction
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

