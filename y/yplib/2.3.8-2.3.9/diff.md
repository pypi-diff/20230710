# Comparing `tmp/yplib-2.3.8.tar.gz` & `tmp/yplib-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.3.8.tar", last modified: Mon Jul 10 07:21:29 2023, max compression
+gzip compressed data, was "dist\yplib-2.3.9.tar", last modified: Mon Jul 10 07:30:59 2023, max compression
```

## Comparing `yplib-2.3.8.tar` & `yplib-2.3.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 07:21:29.358428 yplib-2.3.8/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.3.8/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-10 07:21:29.356896 yplib-2.3.8/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.3.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-10 07:21:29.358428 yplib-2.3.8/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-10 07:21:02.000000 yplib-2.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 07:21:29.353644 yplib-2.3.8/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.3.8/yplib/__init__.py
--rw-rw-rw-   0        0        0    10012 2023-07-07 00:30:37.000000 yplib-2.3.8/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.3.8/yplib/chart_html.py
--rw-rw-rw-   0        0        0     1628 2023-07-10 07:20:32.000000 yplib-2.3.8/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.3.8/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.3.8/yplib/http_util.py
--rw-rw-rw-   0        0        0    32177 2023-07-10 03:17:28.000000 yplib-2.3.8/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.3.8/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.3.8/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.3.8/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.3.8/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-10 07:21:29.356211 yplib-2.3.8/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-10 07:21:29.000000 yplib-2.3.8/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-10 07:21:29.000000 yplib-2.3.8/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 07:21:29.000000 yplib-2.3.8/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-10 07:21:29.000000 yplib-2.3.8/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 07:30:59.415307 yplib-2.3.9/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.3.9/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-10 07:30:59.414929 yplib-2.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.3.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-10 07:30:59.415526 yplib-2.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-10 07:30:40.000000 yplib-2.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:30:59.411960 yplib-2.3.9/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.3.9/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-07 00:30:37.000000 yplib-2.3.9/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.3.9/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.3.9/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.3.9/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.3.9/yplib/http_util.py
+-rw-rw-rw-   0        0        0    32177 2023-07-10 03:17:28.000000 yplib-2.3.9/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.3.9/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.3.9/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.3.9/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.3.9/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:30:59.414389 yplib-2.3.9/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-10 07:30:59.000000 yplib-2.3.9/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-10 07:30:59.000000 yplib-2.3.9/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 07:30:59.000000 yplib-2.3.9/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-10 07:30:59.000000 yplib-2.3.9/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.3.8/LICENSE` & `yplib-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.3.8/setup.py` & `yplib-2.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.3.8",
+  version="2.3.9",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.3.8/yplib/__init__.py` & `yplib-2.3.9/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.8/yplib/chart.py` & `yplib-2.3.9/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.8/yplib/chart_html.py` & `yplib-2.3.9/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.8/yplib/db.py` & `yplib-2.3.9/yplib/db.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def get_connect(db='MoneyKing', user='moneyking_uer', passwd='3^qp3Xqt4bG7', charset='utf8mb4', port=3306, host='192.168.40.230'):
     # return pymysql.connect(db='MoneyKing', user='moneyking_uer', passwd='3^qp3Xqt4bG7', charset="utf8mb4",
     #                        port=3307,
     #                        host='192.168.40.230')
     return pymysql.connect(db=db, user=user, passwd=passwd, charset=charset, port=port, host=host)
 
 
-# 执行 sql 语句
+# 执行 sql 语句, 并且提交, 默认值提交的了
 def exec_sql(db_conn, sql='', commit=True):
     if db_conn is None or sql is None or sql == '':
         to_log_file("db_conn is None or sql is None or sql == '', so return")
         return
     db_cursor = db_conn.cursor()
     if isinstance(sql, list) or isinstance(sql, set):
         for s in sql:
@@ -28,19 +28,14 @@
 
 
 # 执行 sql 语句, 不提交
 def exec_sql_un_commit(db_conn, sql=''):
     exec_sql(db_conn=db_conn, sql=sql, commit=False)
 
 
-# 执行 sql 语句, 并且提交
-def exec_sql_commit(db_conn, sql=''):
-    exec_sql(db_conn=db_conn, sql=sql, commit=True)
-
-
 # 执行 sql 获得 数据
 def get_data_from_sql(db_conn, sql=''):
     if db_conn is None or sql is None or sql == '':
         to_log_file("db_conn is None or sql is None or sql == '', so return")
         return
     db_cursor = db_conn.cursor()
     to_log_file(sql)
```

### Comparing `yplib-2.3.8/yplib/file.py` & `yplib-2.3.9/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.8/yplib/http_util.py` & `yplib-2.3.9/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.8/yplib/index.py` & `yplib-2.3.9/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.8/yplib/mail.py` & `yplib-2.3.9/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.8/yplib/mail_html.py` & `yplib-2.3.9/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.8/yplib/markdown.py` & `yplib-2.3.9/yplib/markdown.py`

 * *Files identical despite different names*

