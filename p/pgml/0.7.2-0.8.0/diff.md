# Comparing `tmp/pgml-0.7.2-cp39-none-win_amd64.whl.zip` & `tmp/pgml-0.8.0-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2642745 bytes, number of entries: 5
--rw-r--r--  4.6 unx    17320 b- defN 23-Jun-30 21:12 pgml-0.7.2.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 23-Jun-30 21:12 pgml-0.7.2.dist-info/WHEEL
--rw-r--r--  4.6 unx      107 b- defN 23-Jun-30 21:12 pgml/__init__.py
--rwxr-xr-x  4.6 unx  7121920 b- defN 23-Jun-30 21:12 pgml/pgml.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      358 b- defN 23-Jun-30 21:12 pgml-0.7.2.dist-info/RECORD
-5 files, 7139799 bytes uncompressed, 2642091 bytes compressed:  63.0%
+Zip file size: 2746706 bytes, number of entries: 5
+-rw-r--r--  4.6 unx    17320 b- defN 23-Jul-10 19:47 pgml-0.8.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Jul-10 19:47 pgml-0.8.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx      107 b- defN 23-Jul-10 19:47 pgml/__init__.py
+-rwxr-xr-x  4.6 unx  7506944 b- defN 23-Jul-10 19:47 pgml/pgml.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      358 b- defN 23-Jul-10 19:47 pgml-0.8.0.dist-info/RECORD
+5 files, 7524823 bytes uncompressed, 2746052 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: pgml-0.7.2.dist-info/METADATA
+Filename: pgml-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: pgml-0.7.2.dist-info/WHEEL
+Filename: pgml-0.8.0.dist-info/WHEEL
 Comment: 
 
 Filename: pgml/__init__.py
 Comment: 
 
 Filename: pgml/pgml.cp39-win_amd64.pyd
 Comment: 
 
-Filename: pgml-0.7.2.dist-info/RECORD
+Filename: pgml-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pgml-0.7.2.dist-info/METADATA` & `pgml-0.8.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgml
-Version: 0.7.2
+Version: 0.8.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Python SDK is designed to facilitate the development of scalable vector search applications on PostgreSQL databases.
 Keywords: postgres,machine learning,vector databases,embeddings
 Author-email: PostgresML <team@postgresml.org>
 Requires-Python: >=3.7
```

