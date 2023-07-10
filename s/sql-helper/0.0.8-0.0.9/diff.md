# Comparing `tmp/sql_helper-0.0.8-py3-none-any.whl.zip` & `tmp/sql_helper-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5634 bytes, number of entries: 7
--rw-rw-r--  2.0 unx    13914 b- defN 20-Oct-04 13:59 sql_helper/__init__.py
--rw-rw-r--  2.0 unx       40 b- defN 20-Aug-08 21:00 sql_helper/settings.ini
--rw-rw-r--  2.0 unx      608 b- defN 20-Oct-12 04:08 sql_helper-0.0.8.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     2151 b- defN 20-Oct-12 04:08 sql_helper-0.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 20-Oct-12 04:08 sql_helper-0.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 20-Oct-12 04:08 sql_helper-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      562 b- defN 20-Oct-12 04:08 sql_helper-0.0.8.dist-info/RECORD
-7 files, 17378 bytes uncompressed, 4634 bytes compressed:  73.3%
+Zip file size: 5763 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx    14296 b- defN 22-Feb-21 00:10 sql_helper/__init__.py
+-rw-rw-r--  2.0 unx       40 b- defN 21-Nov-14 19:56 sql_helper/settings.ini
+-rw-rw-r--  2.0 unx      608 b- defN 22-Feb-21 00:14 sql_helper-0.0.9.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     2211 b- defN 22-Feb-21 00:14 sql_helper-0.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Feb-21 00:14 sql_helper-0.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 22-Feb-21 00:14 sql_helper-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      562 b- defN 22-Feb-21 00:14 sql_helper-0.0.9.dist-info/RECORD
+7 files, 17820 bytes uncompressed, 4763 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: sql_helper/__init__.py
 Comment: 
 
 Filename: sql_helper/settings.ini
 Comment: 
 
-Filename: sql_helper-0.0.8.dist-info/LICENSE.txt
+Filename: sql_helper-0.0.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: sql_helper-0.0.8.dist-info/METADATA
+Filename: sql_helper-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: sql_helper-0.0.8.dist-info/WHEEL
+Filename: sql_helper-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: sql_helper-0.0.8.dist-info/top_level.txt
+Filename: sql_helper-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: sql_helper-0.0.8.dist-info/RECORD
+Filename: sql_helper-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sql_helper/__init__.py

```diff
@@ -15,19 +15,27 @@
 class SQL(object):
     def __init__(self, url, connect_timeout=connect_timeout, **connect_args):
         """An instance that can execute SQL statements on a SQL db (mysql/postgresql)
 
         - url: connection url to a SQL db
             - postgresql://someuser:somepassword@somehost[:someport]/somedatabase
             - mysql://someuser:somepassword@somehost[:someport]/somedatabase
+            - sqlite:///somedb.db
+            - redshift+psycopg2://someuser:somepassword@somehost/somedatabase
+                - You must install the `sqlalchemy-redshift` package wherever you
+                  installed `sql-helper` to connect to a redshift instance
 
         Other kwargs passed in will be passed to sqlalchemy.create_engine as
         connect_args
         """
-        connect_args['connect_timeout'] = connect_timeout
+        if url.startswith('sqlite://'):
+            connect_args['timeout'] = connect_timeout
+        else:
+            connect_args['connect_timeout'] = connect_timeout
+
         url = self._fix_mysql_url(url)
         self._engine = create_engine(url, connect_args=connect_args)
         self._inspector = inspect(self._engine)
         if (
             self._engine.url.drivername.startswith('postgresql') or
             self._engine.url.drivername == 'redshift+psycopg2'
         ):
```

## Comparing `sql_helper-0.0.8.dist-info/LICENSE.txt` & `sql_helper-0.0.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `sql_helper-0.0.8.dist-info/METADATA` & `sql_helper-0.0.9.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: sql-helper
-Version: 0.0.8
+Version: 0.0.9
 Summary: Helper funcs and tools for working with SQL in mysql or postgresql
 Home-page: https://github.com/kenjyco/sql-helper
+Download-URL: https://github.com/kenjyco/sql-helper/tarball/v0.0.9
 Author: Ken
 Author-email: kenjyco@gmail.com
 License: MIT
-Download-URL: https://github.com/kenjyco/sql-helper/tarball/v0.0.8
 Keywords: sql,mysql,postgresql,helper
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
+License-File: LICENSE.txt
 Requires-Dist: PyMySQL (==0.9.3)
 Requires-Dist: SQLAlchemy (==1.3.2)
 Requires-Dist: bg-helper
 Requires-Dist: psycopg2-binary (==2.8.1)
 Requires-Dist: settings-helper
 
 About
 -----
 
-This is meant to be a simple way to explore a postgresql/mysql database
-and get data out (super light wrapper to SQLAlchemy).
+This is meant to be a simple way to explore a postgresql/mysql/sqlite
+database and get data out (super light wrapper to SQLAlchemy).
 
 Connect with DB url in the following formats:
 
 -  ``postgresql://someuser:somepassword@somehost[:someport]/somedatabase``
 -  ``mysql://someuser:somepassword@somehost[:someport]/somedatabase``
+-  ``sqlite:///somedb.db``
 
 ..
 
    Note: This package uses ``pymysql`` driver for connecting to mysql.
    Urls that start with ``mysql://`` will automatically be changed to
    use ``mysql+pymysql://``.
```

