# Comparing `tmp/yplib-2.3.5.tar.gz` & `tmp/yplib-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.3.5.tar", last modified: Mon Jul 10 01:03:33 2023, max compression
+gzip compressed data, was "dist\yplib-2.3.6.tar", last modified: Mon Jul 10 01:59:53 2023, max compression
```

## Comparing `yplib-2.3.5.tar` & `yplib-2.3.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 01:03:33.982107 yplib-2.3.5/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.3.5/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-10 01:03:33.981652 yplib-2.3.5/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.3.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-10 01:03:33.982107 yplib-2.3.5/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-10 01:02:40.000000 yplib-2.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 01:03:33.978014 yplib-2.3.5/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.3.5/yplib/__init__.py
--rw-rw-rw-   0        0        0    10012 2023-07-07 00:30:37.000000 yplib-2.3.5/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.3.5/yplib/chart_html.py
--rw-rw-rw-   0        0        0      892 2023-07-07 00:36:13.000000 yplib-2.3.5/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.3.5/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.3.5/yplib/http_util.py
--rw-rw-rw-   0        0        0    32089 2023-07-10 01:02:03.000000 yplib-2.3.5/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.3.5/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.3.5/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.3.5/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.3.5/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-10 01:03:33.980571 yplib-2.3.5/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-10 01:03:33.000000 yplib-2.3.5/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-10 01:03:33.000000 yplib-2.3.5/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 01:03:33.000000 yplib-2.3.5/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-10 01:03:33.000000 yplib-2.3.5/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 01:59:53.531352 yplib-2.3.6/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.3.6/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-10 01:59:53.530609 yplib-2.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.3.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-10 01:59:53.531426 yplib-2.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-10 01:59:40.000000 yplib-2.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 01:59:53.525761 yplib-2.3.6/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.3.6/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-07 00:30:37.000000 yplib-2.3.6/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.3.6/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     1285 2023-07-10 01:59:01.000000 yplib-2.3.6/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.3.6/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.3.6/yplib/http_util.py
+-rw-rw-rw-   0        0        0    32089 2023-07-10 01:02:03.000000 yplib-2.3.6/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.3.6/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.3.6/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.3.6/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.3.6/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-10 01:59:53.529818 yplib-2.3.6/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-10 01:59:53.000000 yplib-2.3.6/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-10 01:59:53.000000 yplib-2.3.6/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 01:59:53.000000 yplib-2.3.6/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-10 01:59:53.000000 yplib-2.3.6/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.3.5/LICENSE` & `yplib-2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.3.5/setup.py` & `yplib-2.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.3.5",
+  version="2.3.6",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.3.5/yplib/__init__.py` & `yplib-2.3.6/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.5/yplib/chart.py` & `yplib-2.3.6/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.5/yplib/chart_html.py` & `yplib-2.3.6/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.5/yplib/db.py` & `yplib-2.3.6/yplib/db.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,19 +8,30 @@
     #                        port=3307,
     #                        host='192.168.40.230')
     return pymysql.connect(db=db, user=user, passwd=passwd, charset=charset, port=port, host=host)
 
 
 # 执行 sql 语句
 def exec_sql(db_conn, sql='', commit=True):
+    if db_conn is None or sql is None or sql == '':
+        to_log_file("db_conn is None or sql is None or sql == '', so return")
+        return
     db_cursor = db_conn.cursor()
     if isinstance(sql, list) or isinstance(sql, set):
         for s in sql:
             to_log_file(s)
             db_cursor.execute(s)
     else:
         to_log_file(sql)
         db_cursor.execute(str(sql))
     if commit:
         db_conn.commit()
 
-# print('end')
+
+# 执行 sql 语句, 不提交
+def exec_sql_un_commit(db_conn, sql=''):
+    exec_sql(db_conn=db_conn, sql=sql, commit=False)
+
+
+# 执行 sql 语句, 并且提交
+def exec_sql_commit(db_conn, sql=''):
+    exec_sql(db_conn=db_conn, sql=sql, commit=True)
```

### Comparing `yplib-2.3.5/yplib/file.py` & `yplib-2.3.6/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.5/yplib/http_util.py` & `yplib-2.3.6/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.5/yplib/index.py` & `yplib-2.3.6/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.5/yplib/mail.py` & `yplib-2.3.6/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.5/yplib/mail_html.py` & `yplib-2.3.6/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.5/yplib/markdown.py` & `yplib-2.3.6/yplib/markdown.py`

 * *Files identical despite different names*

