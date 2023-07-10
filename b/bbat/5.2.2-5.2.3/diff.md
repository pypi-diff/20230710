# Comparing `tmp/bbat-5.2.2.tar.gz` & `tmp/bbat-5.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbat-5.2.2.tar", last modified: Sun Jul  9 16:22:55 2023, max compression
+gzip compressed data, was "bbat-5.2.3.tar", last modified: Mon Jul 10 06:24:36 2023, max compression
```

## Comparing `bbat-5.2.2.tar` & `bbat-5.2.3.tar`

### file list

```diff
@@ -1,41 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 16:22:55.103239 bbat-5.2.2/
--rw-rw-rw-   0        0        0      289 2023-07-09 16:22:55.102242 bbat-5.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-07-09 07:13:47.000000 bbat-5.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 16:22:55.054648 bbat-5.2.2/bbat/
--rw-rw-rw-   0        0        0        0 2023-07-09 13:29:16.000000 bbat-5.2.2/bbat/__init__.py
--rw-rw-rw-   0        0        0     1525 2023-07-09 15:58:34.000000 bbat-5.2.2/bbat/config.py
--rw-rw-rw-   0        0        0      587 2023-07-09 13:24:38.000000 bbat-5.2.2/bbat/date.py
-drwxrwxrwx   0        0        0        0 2023-07-09 16:22:55.077221 bbat-5.2.2/bbat/db/
--rw-rw-rw-   0        0        0        0 2023-07-09 13:50:01.000000 bbat-5.2.2/bbat/db/__init__.py
--rw-rw-rw-   0        0        0     5357 2023-07-09 16:15:32.000000 bbat-5.2.2/bbat/db/a_mysql.py
--rw-rw-rw-   0        0        0     2632 2023-07-05 12:04:50.000000 bbat-5.2.2/bbat/db/a_sqlite.py
--rw-rw-rw-   0        0        0     2321 2023-07-09 14:43:07.000000 bbat-5.2.2/bbat/db/mysql.py
--rw-rw-rw-   0        0        0       30 2023-07-09 12:57:03.000000 bbat-5.2.2/bbat/hi.py
-drwxrwxrwx   0        0        0        0 2023-07-09 16:22:55.084335 bbat-5.2.2/bbat/http/
--rw-rw-rw-   0        0        0        0 2023-07-09 13:29:16.000000 bbat-5.2.2/bbat/http/__init__.py
--rw-rw-rw-   0        0        0      504 2023-07-05 12:04:50.000000 bbat-5.2.2/bbat/http/cors.py
--rw-rw-rw-   0        0        0     4442 2023-07-09 16:17:08.000000 bbat-5.2.2/bbat/http/db_server.py
--rw-rw-rw-   0        0        0      177 2023-07-09 15:23:45.000000 bbat-5.2.2/bbat/http/flask.py
--rw-rw-rw-   0        0        0     1279 2023-07-09 15:06:59.000000 bbat-5.2.2/bbat/http/sanic.py
-drwxrwxrwx   0        0        0        0 2023-07-09 16:22:55.094159 bbat-5.2.2/bbat/http/url_to_sql/
--rw-rw-rw-   0        0        0        0 2023-07-09 14:55:40.000000 bbat-5.2.2/bbat/http/url_to_sql/__init__.py
--rw-rw-rw-   0        0        0     1489 2023-07-09 15:37:00.000000 bbat-5.2.2/bbat/http/url_to_sql/field.py
--rw-rw-rw-   0        0        0     7556 2023-07-09 15:36:55.000000 bbat-5.2.2/bbat/http/url_to_sql/query.py
--rw-rw-rw-   0        0        0     2258 2023-07-09 15:37:13.000000 bbat-5.2.2/bbat/http/url_to_sql/relation.py
--rw-rw-rw-   0        0        0      723 2023-07-09 15:37:17.000000 bbat-5.2.2/bbat/http/url_to_sql/test.py
--rw-rw-rw-   0        0        0      964 2023-07-05 12:04:50.000000 bbat-5.2.2/bbat/http/url_to_sql/util.py
--rw-rw-rw-   0        0        0     1474 2023-07-09 15:37:22.000000 bbat-5.2.2/bbat/http/url_to_sql/where.py
--rw-rw-rw-   0        0        0      142 2023-07-09 14:27:43.000000 bbat-5.2.2/bbat/uuid.py
-drwxrwxrwx   0        0        0        0 2023-07-09 16:22:55.072037 bbat-5.2.2/bbat.egg-info/
--rw-rw-rw-   0        0        0      289 2023-07-09 16:22:54.000000 bbat-5.2.2/bbat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      708 2023-07-09 16:22:54.000000 bbat-5.2.2/bbat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 16:22:54.000000 bbat-5.2.2/bbat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-09 16:22:54.000000 bbat-5.2.2/bbat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 16:22:55.104239 bbat-5.2.2/setup.cfg
--rw-rw-rw-   0        0        0      487 2023-07-09 16:22:23.000000 bbat-5.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 16:22:55.101207 bbat-5.2.2/test/
--rw-rw-rw-   0        0        0      191 2023-07-09 14:21:27.000000 bbat-5.2.2/test/test_config.py
--rw-rw-rw-   0        0        0      178 2023-07-09 14:38:03.000000 bbat-5.2.2/test/test_db_mysql.py
--rw-rw-rw-   0        0        0     2560 2023-07-09 15:27:40.000000 bbat-5.2.2/test/test_http_flask.py
--rw-rw-rw-   0        0        0      815 2023-07-09 16:18:43.000000 bbat-5.2.2/test/test_http_sanic.py
--rw-rw-rw-   0        0        0       69 2023-07-09 15:37:38.000000 bbat-5.2.2/test/test_http_server_db.py
+drwxrwxrwx   0        0        0        0 2023-07-10 06:24:36.042263 bbat-5.2.3/
+-rw-rw-rw-   0        0        0      289 2023-07-10 06:24:36.042263 bbat-5.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-07-10 01:19:32.000000 bbat-5.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 06:24:36.004265 bbat-5.2.3/bbat/
+-rw-rw-rw-   0        0        0        0 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/__init__.py
+-rw-rw-rw-   0        0        0     1525 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/config.py
+-rw-rw-rw-   0        0        0     1228 2023-07-10 03:21:13.000000 bbat-5.2.3/bbat/date.py
+drwxrwxrwx   0        0        0        0 2023-07-10 06:24:36.019266 bbat-5.2.3/bbat/db/
+-rw-rw-rw-   0        0        0        0 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/db/__init__.py
+-rw-rw-rw-   0        0        0     5371 2023-07-10 05:33:54.000000 bbat-5.2.3/bbat/db/a_mysql.py
+-rw-rw-rw-   0        0        0     2632 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/db/a_sqlite.py
+-rw-rw-rw-   0        0        0     2339 2023-07-10 05:34:01.000000 bbat-5.2.3/bbat/db/mysql.py
+-rw-rw-rw-   0        0        0     1006 2023-07-10 02:28:31.000000 bbat-5.2.3/bbat/file.py
+-rw-rw-rw-   0        0        0      287 2023-07-10 03:36:58.000000 bbat-5.2.3/bbat/hash.py
+-rw-rw-rw-   0        0        0       30 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/hi.py
+-rw-rw-rw-   0        0        0     1978 2023-07-10 03:27:55.000000 bbat-5.2.3/bbat/image.py
+-rw-rw-rw-   0        0        0        0 2023-07-10 06:10:55.000000 bbat-5.2.3/bbat/log.py
+-rw-rw-rw-   0        0        0      924 2023-07-10 06:16:29.000000 bbat-5.2.3/bbat/machine.py
+-rw-rw-rw-   0        0        0     1670 2023-07-10 04:38:59.000000 bbat-5.2.3/bbat/notice.py
+-rw-rw-rw-   0        0        0     2413 2023-07-10 06:14:27.000000 bbat-5.2.3/bbat/np.py
+-rw-rw-rw-   0        0        0     4266 2023-07-10 06:03:39.000000 bbat-5.2.3/bbat/text.py
+drwxrwxrwx   0        0        0        0 2023-07-10 06:24:36.026266 bbat-5.2.3/bbat/web/
+-rw-rw-rw-   0        0        0     1774 2023-07-10 06:09:52.000000 bbat-5.2.3/bbat/web/__init__.py
+-rw-rw-rw-   0        0        0      504 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/web/cors.py
+-rw-rw-rw-   0        0        0     4444 2023-07-10 03:01:15.000000 bbat-5.2.3/bbat/web/db_server.py
+-rw-rw-rw-   0        0        0      177 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/web/flask.py
+-rw-rw-rw-   0        0        0     1279 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/web/sanic.py
+drwxrwxrwx   0        0        0        0 2023-07-10 06:24:36.034265 bbat-5.2.3/bbat/web/url_to_sql/
+-rw-rw-rw-   0        0        0        0 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/web/url_to_sql/__init__.py
+-rw-rw-rw-   0        0        0     1489 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/web/url_to_sql/field.py
+-rw-rw-rw-   0        0        0     7556 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/web/url_to_sql/query.py
+-rw-rw-rw-   0        0        0     2258 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/web/url_to_sql/relation.py
+-rw-rw-rw-   0        0        0      723 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/web/url_to_sql/test.py
+-rw-rw-rw-   0        0        0      964 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/web/url_to_sql/util.py
+-rw-rw-rw-   0        0        0     1474 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/web/url_to_sql/where.py
+drwxrwxrwx   0        0        0        0 2023-07-10 06:24:36.015266 bbat-5.2.3/bbat.egg-info/
+-rw-rw-rw-   0        0        0      289 2023-07-10 06:24:35.000000 bbat-5.2.3/bbat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      790 2023-07-10 06:24:35.000000 bbat-5.2.3/bbat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 06:24:35.000000 bbat-5.2.3/bbat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-10 06:24:35.000000 bbat-5.2.3/bbat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 06:24:36.043265 bbat-5.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      487 2023-07-10 06:18:54.000000 bbat-5.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 06:24:36.040265 bbat-5.2.3/test/
+-rw-rw-rw-   0        0        0      191 2023-07-10 01:19:32.000000 bbat-5.2.3/test/test_config.py
+-rw-rw-rw-   0        0        0      178 2023-07-10 01:19:32.000000 bbat-5.2.3/test/test_db_mysql.py
+-rw-rw-rw-   0        0        0     2559 2023-07-10 06:04:28.000000 bbat-5.2.3/test/test_http_flask.py
+-rw-rw-rw-   0        0        0      814 2023-07-10 06:04:34.000000 bbat-5.2.3/test/test_http_sanic.py
+-rw-rw-rw-   0        0        0       68 2023-07-10 06:04:44.000000 bbat-5.2.3/test/test_http_server_db.py
```

### Comparing `bbat-5.2.2/bbat/config.py` & `bbat-5.2.3/bbat/config.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.2/bbat/db/a_mysql.py` & `bbat-5.2.3/bbat/db/a_mysql.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 import aiomysql
 import pymysql
 
 
 class Mysql:
     """A lightweight wrapper around aiomysql.Pool for easy to use
     """
-    def __init__(self, host, port, db, user, password,
+    def __init__(self, host, port, database, user, password,
                  loop=None, sanic=None,
                  minsize=3, maxsize=5,
                  return_dict=True,
                  pool_recycle=7*3600,
                  autocommit=True,
                  charset = "utf8mb4", **kwargs):
         '''
         kwargs: all parameters that aiomysql.connect() accept.
         '''
         self.db_args = {
             'host': host,
             'port': port,
-            'db': db,
+            'db': database,
             'user': user,
             'password': password,
             'minsize': minsize,
             'maxsize': maxsize,
             'charset': charset,
             'loop': loop,
             'autocommit': autocommit,
@@ -61,15 +61,15 @@
                     ret = await cur.fetchall()
                 except pymysql.err.InternalError:
                     await conn.ping()
                     await cur.execute(query)
                     ret = await cur.fetchall()
                 return ret
 
-    async def get(self, query, *parameters, **kwparameters):
+    async def fetch(self, query, *parameters, **kwparameters):
         """Returns the (singular) row returned by the given query.
         """
         if not self.pool:
             await self.init_pool()
         async with self.pool.acquire() as conn:
             async with conn.cursor() as cur:
                 try:
```

### Comparing `bbat-5.2.2/bbat/db/a_sqlite.py` & `bbat-5.2.3/bbat/db/a_sqlite.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.2/bbat/db/mysql.py` & `bbat-5.2.3/bbat/db/mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pymysql
 
 
 class Mysql:
-    def __init__(self, host=None, port=None, db=None, user=None, password=None, connect_timeout=20, read_timeout=20, write_timeout=20):
+    def __init__(self, host=None, port=None, database=None, user=None, password=None, connect_timeout=20, read_timeout=20, write_timeout=20):
         self.conn = pymysql.connect(
             host=host,
             port=int(port),
-            db=db,
+            database=database,
             user=user,
             passwd=str(password),
             connect_timeout=connect_timeout,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             cursorclass=pymysql.cursors.DictCursor,
         )
```

### Comparing `bbat-5.2.2/bbat/http/db_server.py` & `bbat-5.2.3/bbat/web/db_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     sql = query.to_sql()
     # 1.主表查询
     data = await db.query(sql)
     # 根据field定义，做数据处理
     data = query.data_convert(query.fields, data)
     # 2.统计查询
-    info = await db.get(query.to_count_sql())
+    info = await db.fetch(query.to_count_sql())
     result['meta'] = {"total": info['cnt']}
     # 3.子表查询
     for relation in query.relation:
         # master表外键所有id
         idhub = set([str(i[relation.master_key]) for i in data])
         if len(idhub) == 0:
             continue
```

### Comparing `bbat-5.2.2/bbat/http/sanic.py` & `bbat-5.2.3/bbat/web/sanic.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.2/bbat/http/url_to_sql/field.py` & `bbat-5.2.3/bbat/web/url_to_sql/field.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.2/bbat/http/url_to_sql/query.py` & `bbat-5.2.3/bbat/web/url_to_sql/query.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.2/bbat/http/url_to_sql/relation.py` & `bbat-5.2.3/bbat/web/url_to_sql/relation.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.2/bbat/http/url_to_sql/test.py` & `bbat-5.2.3/bbat/web/url_to_sql/test.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.2/bbat/http/url_to_sql/util.py` & `bbat-5.2.3/bbat/web/url_to_sql/util.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.2/bbat/http/url_to_sql/where.py` & `bbat-5.2.3/bbat/web/url_to_sql/where.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.2/test/test_http_flask.py` & `bbat-5.2.3/test/test_http_flask.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from bbat.http.flask import app
+from bbat.web.flask import app
 from bbat.db.mysql import Mysql
 from bbat.config import Config
 from flask import request, jsonify, render_template, redirect
 import hashlib
 
 
 @app.route('/hi')
```

### Comparing `bbat-5.2.2/test/test_http_sanic.py` & `bbat-5.2.3/test/test_http_sanic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from bbat.http.sanic import app, success, error
+from bbat.web.sanic import app, success, error
 from bbat.date import time_to_str
 import os
 
 @app.route('/hi')
 def hi(request):
     return success({}, "Hi")
```

