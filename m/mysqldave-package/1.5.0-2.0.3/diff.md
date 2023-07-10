# Comparing `tmp/mysqldave_package-1.5.0.tar.gz` & `tmp/mysqldave_package-2.0.3.tar.gz`

## Comparing `mysqldave_package-1.5.0.tar` & `mysqldave_package-2.0.3.tar`

### file list

```diff
@@ -1,28 +1,35 @@
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/QuickStart.md
--rwxr-xr-x   0        0        0      538 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/export_to_csv.bat
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/methods.md
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/src/mysqldave_package/.schemawiz_config2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/src/mysqldave_package/__init__.py
--rw-r--r--   0        0        0    14301 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/src/mysqldave_package/mysqldave.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/src/mysqldave_package/restored_sample.ddl
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/src/mysqldave_package/sample.csv
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/src/mysqldave_package/testcase1.csv
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/.schemawiz_config2
--rwxr-xr-x   0        0        0      316 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/backup.bat
--rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/restore.bat
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/sample7.csv
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/sample8.csv
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/tester.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/thistbl.csv
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/z.new_sample7.ddl
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/z.new_sample8.ddl
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/z.new_thistbl.ddl
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/z.restored_1sample7.ddl
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/z.restored_sample7.ddl
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/z.restored_sample8.ddl
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/z.restored_thistbl.ddl
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/LICENSE
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/README.md
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/Admin Query SQL.md
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/Admin Statitics SQL.md
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/Cancel Queries.md
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/DB Analysis Queries.md
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/MySQL_basics.sql
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/QuickStart.md
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/Restore.md
+-rwxr-xr-x   0        0        0      538 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/export_to_csv.bat
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/methods.md
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/src/mysqldave_package/.schemawiz_config2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/src/mysqldave_package/__init__.py
+-rw-r--r--   0        0        0    14754 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/src/mysqldave_package/mysqldave.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/src/mysqldave_package/restored_sample.ddl
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/src/mysqldave_package/sample.csv
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/src/mysqldave_package/testcase1.csv
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/tests/.schemawiz_config2
+-rwxr-xr-x   0        0        0      316 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/tests/backup.bat
+-rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/tests/restore.bat
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/tests/sample7.csv
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/tests/sample8.csv
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/tests/test_query_lock.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/tests/tester.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/tests/thistbl.csv
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/tests/z.new_sample7.ddl
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/tests/z.new_sample8.ddl
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/tests/z.new_thistbl.ddl
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/tests/z.restored_1sample7.ddl
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/tests/z.restored_sample7.ddl
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/tests/z.restored_sample8.ddl
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/tests/z.restored_thistbl.ddl
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/LICENSE
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/README.md
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 mysqldave_package-2.0.3/PKG-INFO
```

### Comparing `mysqldave_package-1.5.0/QuickStart.md` & `mysqldave_package-2.0.3/QuickStart.md`

 * *Files identical despite different names*

### Comparing `mysqldave_package-1.5.0/export_to_csv.bat` & `mysqldave_package-2.0.3/export_to_csv.bat`

 * *Files identical despite different names*

### Comparing `mysqldave_package-1.5.0/methods.md` & `mysqldave_package-2.0.3/methods.md`

 * *Files identical despite different names*

### Comparing `mysqldave_package-1.5.0/src/mysqldave_package/mysqldave.py` & `mysqldave_package-2.0.3/src/mysqldave_package/mysqldave.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,36 @@
 """
 import os
 import sys
 import mysql.connector 
 from datetime import *
 import time
 from garbledave_package.garbledave import garbledave 
+import logging
+
+logging.basicConfig(level=logging.INFO)
 
 def main():
-	mydb = mysql_db()
+	mydb = mysql_db('this connection')
+	mydb.connect()
+	mydb = mysql_db('another connection')
 	mydb.connect()
 	print(mydb.dbstr())
 
 	#csvfilename = 'testcase1.csv'
 	#tblname = 'testcase1'
 	#mydb.load_csv_to_table(csvfilename,tblname,True,',')
 
 	mydb.close()
 
 
 class dbconnection_details: 
-	def __init__(self): 
+	def __init__(self,DSN):
+		self.DSN = DSN
+
 		self.DatabaseType='MySQL' 
 		self.updated='Feb 28/2023' 
 
 		self.settings_loaded_from_file = False
 
 		self.DB_USERNAME='' 
 		self.DB_USERPWD=''
@@ -35,62 +42,74 @@
 		self.DB_PORT='' 
 		self.DB_NAME='' 
 		self.loadSettingsFromFile()
 
 	def loadSettingsFromFile(self):
 		try:
 			f = open('.schemawiz_config2','r')
-			connectionstrlines = f.read()
-			connectionstr = garbledave().ungarbleit(connectionstrlines.splitlines()[0])
+			connectionfiledata = f.read()
+			connectionstrlines = connectionfiledata.split('\n')
 			f.close()
-			connarr = connectionstr.split(' - ')
-
-			self.DB_USERNAME	= connarr[0]
-			self.DB_USERPWD		= connarr[1]
-			self.DB_HOST			= connarr[2] 
-			self.DB_PORT			= connarr[3]
-			self.DB_NAME			= connarr[4]
+			found_dsn = False
+			for connectionline in connectionstrlines:
+				logging.info(connectionline)
+				connectionstr = garbledave().ungarbleit(connectionline)
+				connarr = connectionstr.split(' - ')
+				if connarr[0] == self.DSN:
+					logging.info('found DSN: ' + self.DSN)
+
+					self.DB_USERNAME	= connarr[1]
+					self.DB_USERPWD		= connarr[2]
+					self.DB_HOST			= connarr[3] 
+					self.DB_PORT			= connarr[4]
+					self.DB_NAME			= connarr[5]
+					found_dsn = True
+					break;
 
 			self.settings_loaded_from_file = True
 
 		except:
+			found_dsn = False
+
+		if not found_dsn:
 			#saved connection details not found. using defaults
 			self.DB_USERNAME='no db user' 
 			self.DB_HOST='localhost' 
 			self.DB_PORT='3306' 
 			self.DB_NAME='no-db-name-given' 
 			self.DB_USERPWD='no-password-supplied'
 
 	def dbconnectionstr(self):
-		return 'usr=' + self.DB_USERNAME + '; svr=' + self.DB_HOST + '; port=' + self.DB_PORT + '; Database=' + self.DB_NAME + '; pwd=' + self.DB_USERPWD
+		return 'dsn=' + self.DSN + '; usr=' + self.DB_USERNAME + '; svr=' + self.DB_HOST + '; port=' + self.DB_PORT + '; DB Name=' + self.DB_NAME 
 
 	def saveConnectionDefaults(self,DB_USERNAME='postgres',DB_USERPWD='no-password-supplied',DB_HOST='localhost',DB_PORT='1532',DB_NAME='postgres'):
 
-		f = open('.schemawiz_config2','w')
-		f.write(garbledave().garbleit(DB_USERNAME + ' - ' + DB_USERPWD + ' - ' + DB_HOST + ' - ' + DB_PORT + ' - ' + DB_NAME ))
+		f = open('.schemawiz_config2','a')
+		f.write(garbledave().garbleit(self.DSN + ' - ' + DB_USERNAME + ' - ' + DB_USERPWD + ' - ' + DB_HOST + ' - ' + DB_PORT + ' - ' + DB_NAME )+ '\n')
 		f.close()
 
 		self.loadSettingsFromFile()
 
 class tfield:
 	def __init__(self):
 		self.table_name = ''
 		self.column_name = ''
 		self.data_type = ''
 		self.Need_Quotes = ''
 		self.ordinal_position = -1
 		self.comment = '' # dateformat in csv [%Y/%m/%d]
 
 class mysql_db:
-	def __init__(self,DB_USERPWD='no-password-supplied',DB_SCHEMA='no-schema-supplied'):
+	def __init__(self,DSN='default',DB_USERPWD='no-password-supplied',DB_SCHEMA='no-schema-supplied'):
+		self.DSN = DSN.replace('_','')
 		self.delimiter = ''
 		self.delimiter_replace = '^~^'
 		self.enable_logging = False
 		self.max_loglines = 500
-		self.db_conn_dets = dbconnection_details()
+		self.db_conn_dets = dbconnection_details(self.DSN)
 		self.dbconn = None
 		self.cur = None
 
 		if DB_USERPWD != 'no-password-supplied':
 			self.db_conn_dets.DB_USERPWD = DB_USERPWD			#if you pass in a password it overwrites the stored pwd
 
 		if DB_SCHEMA != 'no-schema-supplied':
@@ -144,15 +163,15 @@
 			fld.comment = row[4]
 
 			tablefields.append(fld)
 
 		return tablefields
 
 	def dbstr(self):
-		return 'usr=' + self.db_conn_dets.DB_USERNAME + '; svr=' + self.db_conn_dets.DB_HOST + '; port=' + self.db_conn_dets.DB_PORT + '; Database=' + self.db_conn_dets.DB_NAME
+		return self.db_conn_dets.dbconnectionstr()
 
 	def dbversion(self):
 		return self.queryone('SELECT VERSION()')
 
 	def clean_column_name(self,col_name):
 
 		col = col_name.replace(' ','_')
@@ -289,15 +308,15 @@
 		self.export_query_to_csv('SELECT * FROM ' + tblname,csvfile,szdelimiter)
 
 
 	def handledblquotes(self,rowwithquotes):
 		newstr = ''
 		quotecount = 0
 		cvtmode = False
-		for i in range (0,len(rowwithquotes)-1):
+		for i in range (0,len(rowwithquotes)):
 			if rowwithquotes[i] == '"':
 				quotecount += 1
 			
 			if (quotecount % 2) == 1:
 				cvtmode = True 
 			else:
 				cvtmode = False
@@ -415,14 +434,15 @@
 
 
 	def close(self):
 		if self.dbconn.is_connected():
 			self.dbconn.close()
 
 	def ask_for_database_details(self):
+		print('Asking about DSN: ' +  self.DSN)
 		self.db_conn_dets.DB_HOST = input('DB_HOST (localhost): ') or 'localhost'
 		self.db_conn_dets.DB_PORT = input('DB_PORT (3306): ') or '3306'
 		self.db_conn_dets.DB_NAME = input('DB_NAME (atlas): ') or 'atlas'
 		self.db_conn_dets.DB_USERNAME = input('DB_USERNAME (dave): ') or 'dave'
 		self.db_conn_dets.DB_USERPWD = input('DB_USERPWD: ') or 'dave'
 
 	def connect(self):
```

### Comparing `mysqldave_package-1.5.0/src/mysqldave_package/restored_sample.ddl` & `mysqldave_package-2.0.3/src/mysqldave_package/restored_sample.ddl`

 * *Files identical despite different names*

### Comparing `mysqldave_package-1.5.0/LICENSE` & `mysqldave_package-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqldave_package-1.5.0/pyproject.toml` & `mysqldave_package-2.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling","mysql.connector","garbledave_package"]
 
 build-backend = "hatchling.build"
 
 [project]
 name = "mysqldave_package"
-version = "1.5.0"
+version = "2.0.3"
 dependencies = [
   'mysql-connector-python >= 8.0.32',
   'garbledave_package >= 1.0.0'
 ]
 authors = [
   { name="Dave Skura", email="dskura@gmail.com" },
 ]
```

### Comparing `mysqldave_package-1.5.0/PKG-INFO` & `mysqldave_package-2.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqldave_package
-Version: 1.5.0
+Version: 2.0.3
 Summary: A wrapper for simplified Postgres usage using mysql.connector.
 Project-URL: Homepage, https://github.com/daveskura/mysqldave
 Project-URL: Author Linkedin, https://www.linkedin.com/in/2166883
 Author-email: Dave Skura <dskura@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

