# Comparing `tmp/datachain-1.2.2.tar.gz` & `tmp/datachain-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datachain-1.2.2.tar", max compression
+gzip compressed data, was "datachain-1.2.3.tar", max compression
```

## Comparing `datachain-1.2.2.tar` & `datachain-1.2.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    35060 2023-03-26 22:49:34.715348 datachain-1.2.2/LICENSE
--rw-r--r--   0        0        0        0 2023-03-26 22:49:34.715403 datachain-1.2.2/README.md
--rw-r--r--   0        0        0      187 2023-03-27 10:55:56.699305 datachain-1.2.2/datachain/__init__.py
--rw-r--r--   0        0        0      120 2023-06-01 01:19:09.359858 datachain-1.2.2/datachain/config/__init__.py
--rw-r--r--   0        0        0     2749 2023-07-05 12:28:32.475128 datachain-1.2.2/datachain/config/logging.py
--rw-r--r--   0        0        0      752 2023-07-05 12:28:32.475276 datachain-1.2.2/datachain/config/params.py
--rw-r--r--   0        0        0       32 2023-03-26 22:49:34.715707 datachain-1.2.2/datachain/core/__init__.py
--rw-r--r--   0        0        0    19005 2023-07-05 12:32:35.621608 datachain-1.2.2/datachain/core/common.py
--rw-r--r--   0        0        0     3044 2023-03-27 10:29:58.237300 datachain-1.2.2/datachain/core/lazy.py
--rw-r--r--   0        0        0     2243 2023-03-31 01:27:20.943629 datachain-1.2.2/datachain/core/sync.py
--rw-r--r--   0        0        0      479 2023-07-05 12:28:32.475949 datachain-1.2.2/datachain/sources/__init__.py
--rw-r--r--   0        0        0     3919 2023-07-05 12:28:32.476031 datachain-1.2.2/datachain/sources/_utils.py
--rw-r--r--   0        0        0       32 2023-07-05 12:28:32.476123 datachain-1.2.2/datachain/sources/bytes/__init__.py
--rw-r--r--   0        0        0     1338 2023-07-05 12:28:32.476184 datachain-1.2.2/datachain/sources/bytes/_pandas.py
--rw-r--r--   0        0        0      816 2023-07-05 12:28:32.476234 datachain-1.2.2/datachain/sources/file.py
--rw-r--r--   0        0        0       32 2023-07-05 12:28:32.476296 datachain-1.2.2/datachain/sources/files/__init__.py
--rw-r--r--   0        0        0     1038 2023-07-05 12:28:32.476354 datachain-1.2.2/datachain/sources/files/_file.py
--rw-r--r--   0        0        0     1135 2023-07-05 12:28:32.476414 datachain-1.2.2/datachain/sources/files/_ftp.py
--rw-r--r--   0        0        0      859 2023-07-05 12:28:32.476467 datachain-1.2.2/datachain/sources/files/_http.py
--rw-r--r--   0        0        0      624 2023-07-05 12:28:32.476517 datachain-1.2.2/datachain/sources/files/_jsonfile.py
--rw-r--r--   0        0        0      442 2023-07-05 12:28:32.476571 datachain-1.2.2/datachain/sources/files/_local.py
--rw-r--r--   0        0        0     2825 2023-07-05 12:28:32.476628 datachain-1.2.2/datachain/sources/files/_pandas.py
--rw-r--r--   0        0        0     1281 2023-07-05 12:28:32.476685 datachain-1.2.2/datachain/sources/files/_sftp.py
--rw-r--r--   0        0        0     1232 2023-07-05 12:28:32.476753 datachain-1.2.2/datachain/sources/ftp.py
--rw-r--r--   0        0        0     1847 2023-07-05 12:28:32.476807 datachain-1.2.2/datachain/sources/http.py
--rw-r--r--   0        0        0       32 2023-07-05 12:28:32.476886 datachain-1.2.2/datachain/sources/query/__init__.py
--rw-r--r--   0        0        0     3038 2023-07-05 12:28:32.476941 datachain-1.2.2/datachain/sources/query/_pandas.py
--rw-r--r--   0        0        0     1348 2023-07-05 12:28:32.476989 datachain-1.2.2/datachain/sources/sftp.py
--rw-r--r--   0        0        0     2139 2023-07-05 12:28:32.477051 datachain-1.2.2/datachain/sources/sharepoint.py
--rw-r--r--   0        0        0     2473 2023-07-05 12:28:32.477107 datachain-1.2.2/datachain/sources/sql.py
--rw-r--r--   0        0        0      353 2023-07-05 12:28:32.477181 datachain-1.2.2/datachain/sources/utils/__init__.py
--rw-r--r--   0        0        0     2241 2023-07-05 12:28:32.477233 datachain-1.2.2/datachain/sources/utils/_column.py
--rw-r--r--   0        0        0     4577 2023-07-05 12:28:32.477292 datachain-1.2.2/datachain/sources/utils/_dataframe.py
--rw-r--r--   0        0        0      410 2023-07-05 12:28:32.477347 datachain-1.2.2/datachain/sources/utils/_func.py
--rw-r--r--   0        0        0      567 2023-07-05 12:28:32.477401 datachain-1.2.2/datachain/sources/utils/utils.py
--rw-r--r--   0        0        0      617 2023-03-28 17:59:32.602567 datachain-1.2.2/datachain/utils/func.py
--rw-r--r--   0        0        0     2019 2023-07-05 12:42:19.073251 datachain-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     2005 1970-01-01 00:00:00.000000 datachain-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35060 2023-03-26 22:49:34.715348 datachain-1.2.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-03-26 22:49:34.715403 datachain-1.2.3/README.md
+-rw-r--r--   0        0        0      187 2023-03-27 10:55:56.699305 datachain-1.2.3/datachain/__init__.py
+-rw-r--r--   0        0        0      120 2023-06-01 01:19:09.359858 datachain-1.2.3/datachain/config/__init__.py
+-rw-r--r--   0        0        0     2749 2023-07-05 12:28:32.475128 datachain-1.2.3/datachain/config/logging.py
+-rw-r--r--   0        0        0      752 2023-07-05 12:28:32.475276 datachain-1.2.3/datachain/config/params.py
+-rw-r--r--   0        0        0       32 2023-03-26 22:49:34.715707 datachain-1.2.3/datachain/core/__init__.py
+-rw-r--r--   0        0        0    19005 2023-07-05 12:32:35.621608 datachain-1.2.3/datachain/core/common.py
+-rw-r--r--   0        0        0     3044 2023-03-27 10:29:58.237300 datachain-1.2.3/datachain/core/lazy.py
+-rw-r--r--   0        0        0     2243 2023-03-31 01:27:20.943629 datachain-1.2.3/datachain/core/sync.py
+-rw-r--r--   0        0        0      479 2023-07-05 12:28:32.475949 datachain-1.2.3/datachain/sources/__init__.py
+-rw-r--r--   0        0        0     3919 2023-07-05 12:28:32.476031 datachain-1.2.3/datachain/sources/_utils.py
+-rw-r--r--   0        0        0       32 2023-07-05 12:28:32.476123 datachain-1.2.3/datachain/sources/bytes/__init__.py
+-rw-r--r--   0        0        0     1338 2023-07-05 12:28:32.476184 datachain-1.2.3/datachain/sources/bytes/_pandas.py
+-rw-r--r--   0        0        0      816 2023-07-05 12:28:32.476234 datachain-1.2.3/datachain/sources/file.py
+-rw-r--r--   0        0        0       32 2023-07-05 12:28:32.476296 datachain-1.2.3/datachain/sources/files/__init__.py
+-rw-r--r--   0        0        0     1038 2023-07-05 12:28:32.476354 datachain-1.2.3/datachain/sources/files/_file.py
+-rw-r--r--   0        0        0     1135 2023-07-05 12:28:32.476414 datachain-1.2.3/datachain/sources/files/_ftp.py
+-rw-r--r--   0        0        0      859 2023-07-05 12:28:32.476467 datachain-1.2.3/datachain/sources/files/_http.py
+-rw-r--r--   0        0        0      624 2023-07-05 12:28:32.476517 datachain-1.2.3/datachain/sources/files/_jsonfile.py
+-rw-r--r--   0        0        0      442 2023-07-05 12:28:32.476571 datachain-1.2.3/datachain/sources/files/_local.py
+-rw-r--r--   0        0        0     2825 2023-07-05 12:28:32.476628 datachain-1.2.3/datachain/sources/files/_pandas.py
+-rw-r--r--   0        0        0     1281 2023-07-05 12:28:32.476685 datachain-1.2.3/datachain/sources/files/_sftp.py
+-rw-r--r--   0        0        0     1232 2023-07-05 12:28:32.476753 datachain-1.2.3/datachain/sources/ftp.py
+-rw-r--r--   0        0        0     1847 2023-07-05 12:28:32.476807 datachain-1.2.3/datachain/sources/http.py
+-rw-r--r--   0        0        0       32 2023-07-05 12:28:32.476886 datachain-1.2.3/datachain/sources/query/__init__.py
+-rw-r--r--   0        0        0     3050 2023-07-10 09:51:33.411623 datachain-1.2.3/datachain/sources/query/_pandas.py
+-rw-r--r--   0        0        0     1348 2023-07-05 12:28:32.476989 datachain-1.2.3/datachain/sources/sftp.py
+-rw-r--r--   0        0        0     2139 2023-07-05 12:28:32.477051 datachain-1.2.3/datachain/sources/sharepoint.py
+-rw-r--r--   0        0        0     2473 2023-07-05 12:28:32.477107 datachain-1.2.3/datachain/sources/sql.py
+-rw-r--r--   0        0        0      353 2023-07-05 12:28:32.477181 datachain-1.2.3/datachain/sources/utils/__init__.py
+-rw-r--r--   0        0        0     2241 2023-07-05 12:28:32.477233 datachain-1.2.3/datachain/sources/utils/_column.py
+-rw-r--r--   0        0        0     4577 2023-07-05 12:28:32.477292 datachain-1.2.3/datachain/sources/utils/_dataframe.py
+-rw-r--r--   0        0        0      410 2023-07-05 12:28:32.477347 datachain-1.2.3/datachain/sources/utils/_func.py
+-rw-r--r--   0        0        0      567 2023-07-05 12:28:32.477401 datachain-1.2.3/datachain/sources/utils/utils.py
+-rw-r--r--   0        0        0      617 2023-03-28 17:59:32.602567 datachain-1.2.3/datachain/utils/func.py
+-rw-r--r--   0        0        0     2019 2023-07-10 09:52:02.809513 datachain-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2005 1970-01-01 00:00:00.000000 datachain-1.2.3/PKG-INFO
```

### Comparing `datachain-1.2.2/LICENSE` & `datachain-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/config/logging.py` & `datachain-1.2.3/datachain/config/logging.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/config/params.py` & `datachain-1.2.3/datachain/config/params.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/core/common.py` & `datachain-1.2.3/datachain/core/common.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/core/lazy.py` & `datachain-1.2.3/datachain/core/lazy.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/core/sync.py` & `datachain-1.2.3/datachain/core/sync.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/sources/_utils.py` & `datachain-1.2.3/datachain/sources/_utils.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/sources/bytes/_pandas.py` & `datachain-1.2.3/datachain/sources/bytes/_pandas.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/sources/file.py` & `datachain-1.2.3/datachain/sources/file.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/sources/files/_file.py` & `datachain-1.2.3/datachain/sources/files/_file.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/sources/files/_ftp.py` & `datachain-1.2.3/datachain/sources/files/_ftp.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/sources/files/_http.py` & `datachain-1.2.3/datachain/sources/files/_http.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/sources/files/_jsonfile.py` & `datachain-1.2.3/datachain/sources/files/_jsonfile.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/sources/files/_pandas.py` & `datachain-1.2.3/datachain/sources/files/_pandas.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/sources/files/_sftp.py` & `datachain-1.2.3/datachain/sources/files/_sftp.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/sources/ftp.py` & `datachain-1.2.3/datachain/sources/ftp.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/sources/http.py` & `datachain-1.2.3/datachain/sources/http.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/sources/query/_pandas.py` & `datachain-1.2.3/datachain/sources/query/_pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,14 @@
         database (str): Database to access in the sql server.
         table_name (str, optional): Table name to query. Defaults to "".
         **kwds (Any): Keyword arguments to pass to the writing method.
     """
     uri = f"{dialect}://{username}:{quote(password)}@{address}/{database}"
     engine = sqlalchemy.create_engine(uri)
     conn = engine.connect()
-    if data:
+    if data is not None:
         data.to_sql(
             table_name,
             con=conn,
             **kwds,
         )
     conn.close()
```

### Comparing `datachain-1.2.2/datachain/sources/sftp.py` & `datachain-1.2.3/datachain/sources/sftp.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/sources/sharepoint.py` & `datachain-1.2.3/datachain/sources/sharepoint.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/sources/sql.py` & `datachain-1.2.3/datachain/sources/sql.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/sources/utils/_column.py` & `datachain-1.2.3/datachain/sources/utils/_column.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/sources/utils/_dataframe.py` & `datachain-1.2.3/datachain/sources/utils/_dataframe.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/sources/utils/utils.py` & `datachain-1.2.3/datachain/sources/utils/utils.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/datachain/utils/func.py` & `datachain-1.2.3/datachain/utils/func.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.2/pyproject.toml` & `datachain-1.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datachain"
-version = "1.2.2"
+version = "1.2.3"
 description = "Tools to build data pipelines."
 authors = ["Rayane AMROUCHE <rayaneamrouche@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 packages = [{ include = "datachain" }, { include = "datachain/**/*.py" }]
```

### Comparing `datachain-1.2.2/PKG-INFO` & `datachain-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datachain
-Version: 1.2.2
+Version: 1.2.3
 Summary: Tools to build data pipelines.
 License: GPL-3.0-or-later
 Author: Rayane AMROUCHE
 Author-email: rayaneamrouche@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

