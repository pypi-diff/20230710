# Comparing `tmp/lib310_lite-0.1.0.dev6.tar.gz` & `tmp/lib310_lite-0.1.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib310_lite-0.1.0.dev6.tar", max compression
+gzip compressed data, was "lib310_lite-0.1.0.dev7.tar", max compression
```

## Comparing `lib310_lite-0.1.0.dev6.tar` & `lib310_lite-0.1.0.dev7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      253 2023-07-06 11:48:04.613198 lib310_lite-0.1.0.dev6/lib310_lite/__init__.py
--rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.1.0.dev6/lib310_lite/bigquery/_functions.py
--rw-r--r--   0        0        0     7479 2023-05-12 13:53:49.135436 lib310_lite-0.1.0.dev6/lib310_lite/bigquery/client.py
--rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.1.0.dev6/lib310_lite/bigquery/constants.py
--rw-r--r--   0        0        0    13104 2023-07-07 12:57:20.468868 lib310_lite-0.1.0.dev6/lib310_lite/laser/laser.py
--rw-r--r--   0        0        0      778 2023-07-07 12:57:24.832886 lib310_lite-0.1.0.dev6/pyproject.toml
--rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev6/setup.py
--rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev6/PKG-INFO
+-rw-r--r--   0        0        0      253 2023-07-06 11:48:04.613198 lib310_lite-0.1.0.dev7/lib310_lite/__init__.py
+-rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.1.0.dev7/lib310_lite/bigquery/_functions.py
+-rw-r--r--   0        0        0     7479 2023-05-12 13:53:49.135436 lib310_lite-0.1.0.dev7/lib310_lite/bigquery/client.py
+-rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.1.0.dev7/lib310_lite/bigquery/constants.py
+-rw-r--r--   0        0        0    13317 2023-07-10 15:07:23.808910 lib310_lite-0.1.0.dev7/lib310_lite/laser/laser.py
+-rw-r--r--   0        0        0      778 2023-07-10 15:05:37.985366 lib310_lite-0.1.0.dev7/pyproject.toml
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev7/setup.py
+-rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev7/PKG-INFO
```

### Comparing `lib310_lite-0.1.0.dev6/lib310_lite/bigquery/client.py` & `lib310_lite-0.1.0.dev7/lib310_lite/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.1.0.dev6/lib310_lite/bigquery/constants.py` & `lib310_lite-0.1.0.dev7/lib310_lite/bigquery/constants.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.1.0.dev6/lib310_lite/laser/laser.py` & `lib310_lite-0.1.0.dev7/lib310_lite/laser/laser.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,25 @@
 
 
 class Laser:
 
     instances = 0
     instances_limit = 5
 
-    def __init__(self, db_config: dict, cache_size: int = 30, num_threads: int = 10):
+    def __init__(self, db_config: dict, cache_size: int = 30, num_threads: int = 10, columns: str = '*'):
         if Laser.instances >= Laser.instances_limit:
             raise Exception('Too many instances of Laser')
         if db_config is None:
             raise Exception('db_config must be provided')
         Laser.instances += 1
 
         # Constants
         self.MAIN_TABLE_NAME = 'fs'
         self.CACHED_TABLE_NAME = 'cached'
+        self.COLUMNS = columns
 
         # This is the configuration for the database
         self.db_config = db_config
 
         # This is the configuration for the cache
         self.cache_size = cache_size
         # This is the configuration for the number of threads for buffering
@@ -171,36 +172,41 @@
             cursor = cnx.cursor()
             # check if the query is already in the database
             cursor.execute("SELECT * FROM cached WHERE hash = %s", (h,))
             result = cursor.fetchone()
             if result is None:
                 raise Exception("Pool does not exist")
             # return SELECT * from pool_{hash}
-            cursor.execute("SELECT * FROM pool_{}".format(h))
+
+            pool_q = "SELECT * FROM pool_{}".format(h)
+            if num_parts > 1:
+                cursor.execute("SELECT count(*) FROM pool_{}".format(h))
+                count = cursor.fetchone()[0]
+                part_size = count // num_parts
+                pool_q += " LIMIT {} OFFSET {}".format(part_size, part * part_size)
+
+            # s = time.perf_counter()
+            cursor.execute(pool_q)
             pool = cursor.fetchall()
+            # e = time.perf_counter()
+            # print("Fetched pool in {} seconds".format(e - s))
             self.pool = pool
         except Exception as e:
             print(e)
         finally:
             if cursor is not None:
                 cursor.close()
             if cnx is not None:
                 cnx.close()
             if self.pool is None:
                 return None
             if collate_fn is not None:
                 self.pool = collate_fn(self.pool)
             else:
                 self.pool = [t[0] for t in self.pool]
-
-            pool_len = len(self.pool)
-            if num_parts > 1:
-                # If distributed, split the pool into num_parts parts and return the part with index part
-                self.pool = [self.pool[j:j + pool_len // num_parts] for j in range(0, pool_len, pool_len // num_parts)][part]
-
             return self.pool
 
     def start_buffering(self, sample_number: int, short_nap: int = 2, starting_batch_number: int = 0) -> None:
         """
         Start buffering technique
         :param sample_number: the number of row_id's in each chunk
         :param short_nap: the time to sleep at begging of starting the buffering to let buffer fill
@@ -283,15 +289,15 @@
         """
         cnx = None
         cursor = None
         result = None
         try:
             cnx = MySQLdb.connect(**self.db_config)
             cursor = cnx.cursor(cursorclass=MySQLdb.cursors.DictCursor)
-            query = "SELECT * FROM {} WHERE row_id IN ({})".format(self.MAIN_TABLE_NAME, ','.join(map(str, index_list)))
+            query = "SELECT {} FROM {} WHERE row_id IN ({})".format(self.COLUMNS, self.MAIN_TABLE_NAME, ','.join(map(str, index_list)))
             cursor.execute(query)
             result = cursor.fetchall()
         except Exception as e:
             result = None
             print(e)
         finally:
             if cursor is not None:
```

### Comparing `lib310_lite-0.1.0.dev6/pyproject.toml` & `lib310_lite-0.1.0.dev7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib310_lite"
-version = "0.1.0.dev6"
+version = "0.1.0.dev7"
 description = "lib310 Lite Python Package"
 authors = ["310 <info@310.ai>"]
 maintainers = ["Saman Fekri <saman@310.ai>"]
 keywords = ["biology", "AI", "genomics", "bioinforma", "machine learning", "GAN"]
 packages = [
     { include = "lib310_lite" }
 ]
```

### Comparing `lib310_lite-0.1.0.dev6/setup.py` & `lib310_lite-0.1.0.dev7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'google-cloud-bigquery>=3.2.0',
  'google-cloud>=0.34.0',
  'mysqlclient>=2.0.0',
  'numpy<1.23.0']
 
 setup_kwargs = {
     'name': 'lib310-lite',
-    'version': '0.1.0.dev6',
+    'version': '0.1.0.dev7',
     'description': 'lib310 Lite Python Package',
     'long_description': 'None',
     'author': '310',
     'author_email': 'info@310.ai',
     'maintainer': 'Saman Fekri',
     'maintainer_email': 'saman@310.ai',
     'url': 'None',
```

### Comparing `lib310_lite-0.1.0.dev6/PKG-INFO` & `lib310_lite-0.1.0.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib310-lite
-Version: 0.1.0.dev6
+Version: 0.1.0.dev7
 Summary: lib310 Lite Python Package
 Keywords: biology,AI,genomics,bioinforma,machine learning,GAN
 Author: 310
 Author-email: info@310.ai
 Maintainer: Saman Fekri
 Maintainer-email: saman@310.ai
 Requires-Python: >=3.8
```

