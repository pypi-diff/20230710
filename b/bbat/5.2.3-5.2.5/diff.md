# Comparing `tmp/bbat-5.2.3.tar.gz` & `tmp/bbat-5.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbat-5.2.3.tar", last modified: Mon Jul 10 06:24:36 2023, max compression
+gzip compressed data, was "bbat-5.2.5.tar", last modified: Mon Jul 10 08:41:55 2023, max compression
```

## Comparing `bbat-5.2.3.tar` & `bbat-5.2.5.tar`

### file list

```diff
@@ -1,48 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 06:24:36.042263 bbat-5.2.3/
--rw-rw-rw-   0        0        0      289 2023-07-10 06:24:36.042263 bbat-5.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-07-10 01:19:32.000000 bbat-5.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 06:24:36.004265 bbat-5.2.3/bbat/
--rw-rw-rw-   0        0        0        0 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/__init__.py
--rw-rw-rw-   0        0        0     1525 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/config.py
--rw-rw-rw-   0        0        0     1228 2023-07-10 03:21:13.000000 bbat-5.2.3/bbat/date.py
-drwxrwxrwx   0        0        0        0 2023-07-10 06:24:36.019266 bbat-5.2.3/bbat/db/
--rw-rw-rw-   0        0        0        0 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/db/__init__.py
--rw-rw-rw-   0        0        0     5371 2023-07-10 05:33:54.000000 bbat-5.2.3/bbat/db/a_mysql.py
--rw-rw-rw-   0        0        0     2632 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/db/a_sqlite.py
--rw-rw-rw-   0        0        0     2339 2023-07-10 05:34:01.000000 bbat-5.2.3/bbat/db/mysql.py
--rw-rw-rw-   0        0        0     1006 2023-07-10 02:28:31.000000 bbat-5.2.3/bbat/file.py
--rw-rw-rw-   0        0        0      287 2023-07-10 03:36:58.000000 bbat-5.2.3/bbat/hash.py
--rw-rw-rw-   0        0        0       30 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/hi.py
--rw-rw-rw-   0        0        0     1978 2023-07-10 03:27:55.000000 bbat-5.2.3/bbat/image.py
--rw-rw-rw-   0        0        0        0 2023-07-10 06:10:55.000000 bbat-5.2.3/bbat/log.py
--rw-rw-rw-   0        0        0      924 2023-07-10 06:16:29.000000 bbat-5.2.3/bbat/machine.py
--rw-rw-rw-   0        0        0     1670 2023-07-10 04:38:59.000000 bbat-5.2.3/bbat/notice.py
--rw-rw-rw-   0        0        0     2413 2023-07-10 06:14:27.000000 bbat-5.2.3/bbat/np.py
--rw-rw-rw-   0        0        0     4266 2023-07-10 06:03:39.000000 bbat-5.2.3/bbat/text.py
-drwxrwxrwx   0        0        0        0 2023-07-10 06:24:36.026266 bbat-5.2.3/bbat/web/
--rw-rw-rw-   0        0        0     1774 2023-07-10 06:09:52.000000 bbat-5.2.3/bbat/web/__init__.py
--rw-rw-rw-   0        0        0      504 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/web/cors.py
--rw-rw-rw-   0        0        0     4444 2023-07-10 03:01:15.000000 bbat-5.2.3/bbat/web/db_server.py
--rw-rw-rw-   0        0        0      177 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/web/flask.py
--rw-rw-rw-   0        0        0     1279 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/web/sanic.py
-drwxrwxrwx   0        0        0        0 2023-07-10 06:24:36.034265 bbat-5.2.3/bbat/web/url_to_sql/
--rw-rw-rw-   0        0        0        0 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/web/url_to_sql/__init__.py
--rw-rw-rw-   0        0        0     1489 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/web/url_to_sql/field.py
--rw-rw-rw-   0        0        0     7556 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/web/url_to_sql/query.py
--rw-rw-rw-   0        0        0     2258 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/web/url_to_sql/relation.py
--rw-rw-rw-   0        0        0      723 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/web/url_to_sql/test.py
--rw-rw-rw-   0        0        0      964 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/web/url_to_sql/util.py
--rw-rw-rw-   0        0        0     1474 2023-07-10 01:19:32.000000 bbat-5.2.3/bbat/web/url_to_sql/where.py
-drwxrwxrwx   0        0        0        0 2023-07-10 06:24:36.015266 bbat-5.2.3/bbat.egg-info/
--rw-rw-rw-   0        0        0      289 2023-07-10 06:24:35.000000 bbat-5.2.3/bbat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      790 2023-07-10 06:24:35.000000 bbat-5.2.3/bbat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 06:24:35.000000 bbat-5.2.3/bbat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-10 06:24:35.000000 bbat-5.2.3/bbat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 06:24:36.043265 bbat-5.2.3/setup.cfg
--rw-rw-rw-   0        0        0      487 2023-07-10 06:18:54.000000 bbat-5.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 06:24:36.040265 bbat-5.2.3/test/
--rw-rw-rw-   0        0        0      191 2023-07-10 01:19:32.000000 bbat-5.2.3/test/test_config.py
--rw-rw-rw-   0        0        0      178 2023-07-10 01:19:32.000000 bbat-5.2.3/test/test_db_mysql.py
--rw-rw-rw-   0        0        0     2559 2023-07-10 06:04:28.000000 bbat-5.2.3/test/test_http_flask.py
--rw-rw-rw-   0        0        0      814 2023-07-10 06:04:34.000000 bbat-5.2.3/test/test_http_sanic.py
--rw-rw-rw-   0        0        0       68 2023-07-10 06:04:44.000000 bbat-5.2.3/test/test_http_server_db.py
+drwxrwxrwx   0        0        0        0 2023-07-10 08:41:55.275664 bbat-5.2.5/
+-rw-rw-rw-   0        0        0      289 2023-07-10 08:41:55.273663 bbat-5.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-07-10 01:19:32.000000 bbat-5.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 08:41:55.225149 bbat-5.2.5/bbat/
+-rw-rw-rw-   0        0        0        0 2023-07-10 08:21:51.000000 bbat-5.2.5/bbat/__init__.py
+-rw-rw-rw-   0        0        0     1654 2023-07-10 07:31:31.000000 bbat-5.2.5/bbat/config.py
+-rw-rw-rw-   0        0        0     1228 2023-07-10 03:21:13.000000 bbat-5.2.5/bbat/date.py
+drwxrwxrwx   0        0        0        0 2023-07-10 08:41:55.247152 bbat-5.2.5/bbat/db/
+-rw-rw-rw-   0        0        0        0 2023-07-10 01:19:32.000000 bbat-5.2.5/bbat/db/__init__.py
+-rw-rw-rw-   0        0        0     5371 2023-07-10 05:33:54.000000 bbat-5.2.5/bbat/db/aio_mysql.py
+-rw-rw-rw-   0        0        0     2632 2023-07-10 01:19:32.000000 bbat-5.2.5/bbat/db/aio_sqlite.py
+-rw-rw-rw-   0        0        0     2339 2023-07-10 05:34:01.000000 bbat-5.2.5/bbat/db/mysql.py
+-rw-rw-rw-   0        0        0      287 2023-07-10 03:36:58.000000 bbat-5.2.5/bbat/hash.py
+-rw-rw-rw-   0        0        0       30 2023-07-10 01:19:32.000000 bbat-5.2.5/bbat/hi.py
+-rw-rw-rw-   0        0        0     1978 2023-07-10 03:27:55.000000 bbat-5.2.5/bbat/image.py
+-rw-rw-rw-   0        0        0      920 2023-07-10 08:19:47.000000 bbat-5.2.5/bbat/log.py
+-rw-rw-rw-   0        0        0      822 2023-07-10 08:19:52.000000 bbat-5.2.5/bbat/machine.py
+-rw-rw-rw-   0        0        0     1670 2023-07-10 04:38:59.000000 bbat-5.2.5/bbat/notice.py
+-rw-rw-rw-   0        0        0     2413 2023-07-10 06:14:27.000000 bbat-5.2.5/bbat/np.py
+-rw-rw-rw-   0        0        0      981 2023-07-10 08:07:34.000000 bbat-5.2.5/bbat/path.py
+-rw-rw-rw-   0        0        0     4198 2023-07-10 06:52:29.000000 bbat-5.2.5/bbat/text.py
+drwxrwxrwx   0        0        0        0 2023-07-10 08:41:55.255152 bbat-5.2.5/bbat/web/
+-rw-rw-rw-   0        0        0     1756 2023-07-10 07:07:01.000000 bbat-5.2.5/bbat/web/__init__.py
+-rw-rw-rw-   0        0        0      504 2023-07-10 01:19:32.000000 bbat-5.2.5/bbat/web/cors.py
+-rw-rw-rw-   0        0        0     4503 2023-07-10 07:58:06.000000 bbat-5.2.5/bbat/web/db_server.py
+-rw-rw-rw-   0        0        0      177 2023-07-10 01:19:32.000000 bbat-5.2.5/bbat/web/flask_app.py
+-rw-rw-rw-   0        0        0     1571 2023-07-10 08:38:58.000000 bbat-5.2.5/bbat/web/sanic_app.py
+drwxrwxrwx   0        0        0        0 2023-07-10 08:41:55.268664 bbat-5.2.5/bbat/web/url_to_sql/
+-rw-rw-rw-   0        0        0        0 2023-07-10 01:19:32.000000 bbat-5.2.5/bbat/web/url_to_sql/__init__.py
+-rw-rw-rw-   0        0        0     1488 2023-07-10 07:04:39.000000 bbat-5.2.5/bbat/web/url_to_sql/field.py
+-rw-rw-rw-   0        0        0     7552 2023-07-10 07:04:45.000000 bbat-5.2.5/bbat/web/url_to_sql/query.py
+-rw-rw-rw-   0        0        0     2256 2023-07-10 07:04:49.000000 bbat-5.2.5/bbat/web/url_to_sql/relation.py
+-rw-rw-rw-   0        0        0      722 2023-07-10 07:04:52.000000 bbat-5.2.5/bbat/web/url_to_sql/test.py
+-rw-rw-rw-   0        0        0      964 2023-07-10 01:19:32.000000 bbat-5.2.5/bbat/web/url_to_sql/util.py
+-rw-rw-rw-   0        0        0     1473 2023-07-10 07:04:56.000000 bbat-5.2.5/bbat/web/url_to_sql/where.py
+drwxrwxrwx   0        0        0        0 2023-07-10 08:41:55.240148 bbat-5.2.5/bbat.egg-info/
+-rw-rw-rw-   0        0        0      289 2023-07-10 08:41:54.000000 bbat-5.2.5/bbat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      726 2023-07-10 08:41:55.000000 bbat-5.2.5/bbat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 08:41:54.000000 bbat-5.2.5/bbat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-10 08:41:54.000000 bbat-5.2.5/bbat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 08:41:55.275664 bbat-5.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      487 2023-07-10 08:41:43.000000 bbat-5.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 08:41:55.272662 bbat-5.2.5/test/
+-rw-rw-rw-   0        0        0      209 2023-07-10 06:44:06.000000 bbat-5.2.5/test/test_config.py
+-rw-rw-rw-   0        0        0      194 2023-07-10 06:44:18.000000 bbat-5.2.5/test/test_db_mysql.py
```

### Comparing `bbat-5.2.3/bbat/config.py` & `bbat-5.2.5/bbat/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import os 
-import yaml
 
 def get_env(key, default=""): 
     val = os.getenv(key)
     return val if val else default
 
 class Config:
-    def __init__(self, yamlpath=None):
-        self.yamlpath = yamlpath
+    def __init__(self):
         self.config = {}
-        if yamlpath :
-            with open(yamlpath, 'r') as conf_file:
-                self.config = yaml.safe_load(conf_file)
+    
+    def load_yaml(self, file):
+        import yaml
+        with open(file, 'r') as conf_file:
+            self.config = yaml.safe_load(conf_file)
+
+    def load_json(self, file):
+        import json
+        with open(file, 'r') as conf_file:
+            self.config = json.load(conf_file)
 
     def set(self, key, value):
         '''set config'''
         keys = key.split(".")
         config_value = self.config
         for k in keys:
             config_value = config_value[k]
@@ -29,14 +34,15 @@
     def get(self, key):
         '''
         Args：
             key - 配置key，支持级联：app.name
         Return:
             config['app']['name'] else None
         '''
+        print(key)
         keys = key.split(".")
         config_value = self.config
         for k in keys:
             config_value = config_value.get(k)
         return config_value
 
     def get_env(self, key):
```

### Comparing `bbat-5.2.3/bbat/date.py` & `bbat-5.2.5/bbat/date.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.3/bbat/db/a_mysql.py` & `bbat-5.2.5/bbat/db/aio_mysql.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.3/bbat/db/a_sqlite.py` & `bbat-5.2.5/bbat/db/aio_sqlite.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.3/bbat/db/mysql.py` & `bbat-5.2.5/bbat/db/mysql.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.3/bbat/file.py` & `bbat-5.2.5/bbat/path.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 def get_file_size(file_path):
     return os.path.getsize(file_path)
 
 def is_file_exists(file_path):
     return os.path.exists(file_path)
 
-def create_dir(directory_path):
-    os.makedirs(directory_path, exist_ok=True)
+def mkdir(path):
+    os.makedirs(path, exist_ok=True)
 
 def read_file(file_path):
     try:
         with open(file_path, 'r') as file:
             content = file.read()
             return content
     except FileNotFoundError:
```

### Comparing `bbat-5.2.3/bbat/image.py` & `bbat-5.2.5/bbat/image.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.3/bbat/notice.py` & `bbat-5.2.5/bbat/notice.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.3/bbat/np.py` & `bbat-5.2.5/bbat/np.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.3/bbat/text.py` & `bbat-5.2.5/bbat/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,11 +145,7 @@
         translation = data['translation']
         if not translation:
             return ''
         if len(translation) > 0:
             return "".join(data['translation'])
         return translation
     
-
-if __name__ == '__main__':
-
-    print(Translator()("你是谁"))
```

### Comparing `bbat-5.2.3/bbat/web/__init__.py` & `bbat-5.2.5/bbat/web/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         for chunk in response.iter_content(chunk_size=8192):
             if chunk:
                 file.write(chunk)
     return output
 
 
 
-def xpath(url, path: Union(str, list)="//text()", encoding='utf-8', **kwargs):
+def xpath(url, path="//text()", encoding='utf-8', **kwargs):
     '''
     Args:
         url - string URL to
         path - xpath ql
         encoding - default utf-8
     '''
     from lxml.etree import HTML
```

### Comparing `bbat-5.2.3/bbat/web/db_server.py` & `bbat-5.2.5/bbat/web/db_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from bbat.http.sanic import app, success, error
-from bbat.http.url_to_sql.query import Query
+from bbat.web.sanic_app import app, success, error
+from bbat.web.url_to_sql.query import Query
 
 
 
 # get方法查询函数
 @app.route("/api/<table>", methods=["GET"])
 async def query(request, table):
-    
+    db = request.app.db
     result = {}
     query_string = request.query_string
     query = Query(table, query_string)
 
     sql = query.to_sql()
     # 1.主表查询
     data = await db.query(sql)
@@ -77,15 +77,15 @@
     res = await db.create_table(table)
     return success(res.lastrowid)
 
 # 查所有表
 @app.route("/table", methods=["GET"])
 async def get_tables(request):
     db = request.app.db
-    database = config.get("database.db")
+    database = db.db_args['db']
     tables = await db.tables(database=database)
     return success(tables)
 
 # 查表结构
 @app.route("/table/field", methods=["GET"])
 async def table_struct(request):
     db = request.app.db
@@ -120,19 +120,23 @@
         return ValueError('Invalid data')
     res = await db.drop_field(table=table, field=field)
     return success(res)
 
 
 if __name__ == "__main__":
     from bbat.config import Config
-    from bbat.db.a_mysql import Mysql
+    from bbat.db.aio_mysql import Mysql
     import argparse
+
     parser = argparse.ArgumentParser()
     parser.add_argument('-c', '--config', required=True, help="server_db config 参考: test/config.yaml")
     parser.add_argument('-k', '--key', default="mysql", help="config中数据库的配置key")
     parser.add_argument('-d', '--debug', action='store_true')
     args = parser.parse_args()
 
-    config = Config(args.config)
+    config = Config()
+    config.load_yaml(args.config)
+
     dbconf = config.get(args.key)
     db = Mysql(**dbconf)
+    app.db = db
     app.run(debug=args.debug)
```

### Comparing `bbat-5.2.3/bbat/web/sanic.py` & `bbat-5.2.5/bbat/web/sanic_app.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 from sanic import Sanic, response
 from sanic.exceptions import RequestTimeout, NotFound
 from sanic.log import logger, access_logger, error_logger
+from bbat.path import mkdir
+from bbat.web import cors
 
 
 app = Sanic('sanic_app')
+
+
 # Route: ping
 @app.route("/ping")
 def ping(request):
     return response.text('pong')
 
 # Public static dir
+mkdir('./static')
 app.static('/static', './static/')
 
+# middleware
+@app.middleware("request")
+async def before_request(request):
+    if request.method == "OPTIONS":
+        headers = cors.get_headers()
+        return response.json({"code": 0}, headers=headers)
 
 # Exception defined
 @app.exception(RequestTimeout)
 def timeout(request, exception):
     return response.json({"msg": "Request Timeout", "code": 408}, 408)
 
 @app.exception(NotFound)
```

### Comparing `bbat-5.2.3/bbat/web/url_to_sql/field.py` & `bbat-5.2.5/bbat/web/url_to_sql/field.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 import datetime
 import json
-from bbat.http.url_to_sql.util import cutout
+from bbat.web.url_to_sql.util import cutout
 
 class Field:
     ''' 查询字段 
         field=id,name,created_at:ca
     '''
     def __init__(self, query):
         self.query = query
```

### Comparing `bbat-5.2.3/bbat/web/url_to_sql/query.py` & `bbat-5.2.5/bbat/web/url_to_sql/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ''' query_string 解析 '''
 
 import re
 from urllib.parse import unquote
-from bbat.http.url_to_sql.util import symbol_split
-from bbat.http.url_to_sql.where import Where
-from bbat.http.url_to_sql.field import Field
-from bbat.http.url_to_sql.relation import Relation
+from bbat.web.url_to_sql.util import symbol_split
+from bbat.web.url_to_sql.where import Where
+from bbat.web.url_to_sql.field import Field
+from bbat.web.url_to_sql.relation import Relation
 
 class Query:
     def __init__(self, table, query_string):
         if not table:
             raise Exception("params error: table")
         self.table_name  = table
         self.table_query = unquote(query_string)
```

### Comparing `bbat-5.2.3/bbat/web/url_to_sql/relation.py` & `bbat-5.2.5/bbat/web/url_to_sql/relation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from itertools import groupby
-from bbat.http.url_to_sql.util import cutout
-from bbat.http.url_to_sql.field import Field
+from bbat.web.url_to_sql.util import cutout
+from bbat.web.url_to_sql.field import Field
 import re
 
 
 class Relation:
     ''' 连表信息 
         jobs[project_id=id, name,created_at]
     '''
```

### Comparing `bbat-5.2.3/bbat/web/url_to_sql/test.py` & `bbat-5.2.5/bbat/web/url_to_sql/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from pprint import pprint
-from bbat.http.url_to_sql.query import Query
+from bbat.web.url_to_sql.query import Query
 
 query_list = [
     ['user', "field=id,name,car[id,brand]"],
     ['car', "field=id,name,user{id,name}"],
     ['user', "field=id,name,car[id,name],driving_license[id,name]"],
     ['car', "field=id,name,user{id,name}"],
     ['car', "field=id:iii,name,user{id,name}"],
```

### Comparing `bbat-5.2.3/bbat/web/url_to_sql/util.py` & `bbat-5.2.5/bbat/web/url_to_sql/util.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.3/bbat/web/url_to_sql/where.py` & `bbat-5.2.5/bbat/web/url_to_sql/where.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding: utf-8
-from bbat.http.url_to_sql.util import cutout
+from bbat.web.url_to_sql.util import cutout
 
 class Where:
     ''' 条件解析 '''
     def __init__(self, key, value):
         self.key = key
         self.value = value
         self.opt_map = {
```

### Comparing `bbat-5.2.3/bbat.egg-info/SOURCES.txt` & `bbat-5.2.5/bbat.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 README.md
 setup.py
 bbat/__init__.py
 bbat/config.py
 bbat/date.py
-bbat/file.py
 bbat/hash.py
 bbat/hi.py
 bbat/image.py
 bbat/log.py
 bbat/machine.py
 bbat/notice.py
 bbat/np.py
+bbat/path.py
 bbat/text.py
 bbat.egg-info/PKG-INFO
 bbat.egg-info/SOURCES.txt
 bbat.egg-info/dependency_links.txt
 bbat.egg-info/top_level.txt
 bbat/db/__init__.py
-bbat/db/a_mysql.py
-bbat/db/a_sqlite.py
+bbat/db/aio_mysql.py
+bbat/db/aio_sqlite.py
 bbat/db/mysql.py
 bbat/web/__init__.py
 bbat/web/cors.py
 bbat/web/db_server.py
-bbat/web/flask.py
-bbat/web/sanic.py
+bbat/web/flask_app.py
+bbat/web/sanic_app.py
 bbat/web/url_to_sql/__init__.py
 bbat/web/url_to_sql/field.py
 bbat/web/url_to_sql/query.py
 bbat/web/url_to_sql/relation.py
 bbat/web/url_to_sql/test.py
 bbat/web/url_to_sql/util.py
 bbat/web/url_to_sql/where.py
 test/test_config.py
-test/test_db_mysql.py
-test/test_http_flask.py
-test/test_http_sanic.py
-test/test_http_server_db.py
+test/test_db_mysql.py
```

