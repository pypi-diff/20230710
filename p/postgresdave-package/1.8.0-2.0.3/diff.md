# Comparing `tmp/postgresdave_package-1.8.0.tar.gz` & `tmp/postgresdave_package-2.0.3.tar.gz`

## Comparing `postgresdave_package-1.8.0.tar` & `postgresdave_package-2.0.3.tar`

### file list

```diff
@@ -1,10 +1,34 @@
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 postgresdave_package-1.8.0/QuickStart.md
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 postgresdave_package-1.8.0/methods.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 postgresdave_package-1.8.0/src/postgresdave_package/__init__.py
--rw-r--r--   0        0        0    16115 2020-02-02 00:00:00.000000 postgresdave_package-1.8.0/src/postgresdave_package/postgresdave.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 postgresdave_package-1.8.0/src/postgresdave_package/testcase1.csv
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 postgresdave_package-1.8.0/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 postgresdave_package-1.8.0/LICENSE
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 postgresdave_package-1.8.0/README.md
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 postgresdave_package-1.8.0/pyproject.toml
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 postgresdave_package-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/01) create the database.sql
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/02) create the schemas.sql
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/03) create roles.sql
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/04) grant usage.sql
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/05) create the users.sql
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/06) Admin Queries.md
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/07) CancelQueries.md
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/08) CREATE TABLE AS.sql
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/09) pk_fk_example.sql
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/10) SELECT LAG LEAD RANK.sql
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/11) tables.ddl
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/12) Levenshtein.ddl
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/13) Database Profiling.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/14) Iterative, Dynamic SQL.md
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/Backup.md
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/Basics.md
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/QuickStart.md
+-rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/backup.bat
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/methods.md
+-rwxr-xr-x   0        0        0      720 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/restore.bat
+-rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/src/postgresdave_package/.querylog
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/src/postgresdave_package/__init__.py
+-rw-r--r--   0        0        0    16758 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/src/postgresdave_package/postgresdave.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/src/postgresdave_package/testcase1.csv
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/test/.schemawiz_config1
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/test/.schemawiz_config3
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/test/Test_Connect.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/test/Test_SQLite.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/test/local_sqlite_db
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/LICENSE
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/README.md
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 postgresdave_package-2.0.3/PKG-INFO
```

### Comparing `postgresdave_package-1.8.0/QuickStart.md` & `postgresdave_package-2.0.3/QuickStart.md`

 * *Files identical despite different names*

### Comparing `postgresdave_package-1.8.0/methods.md` & `postgresdave_package-2.0.3/methods.md`

 * *Files identical despite different names*

### Comparing `postgresdave_package-1.8.0/src/postgresdave_package/postgresdave.py` & `postgresdave_package-2.0.3/src/postgresdave_package/postgresdave.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,39 @@
 import os
 import sys
 import psycopg2 
 from datetime import *
 import time
 from garbledave_package.garbledave import garbledave 
 
+def main():
+	mydb = postgres_db('thisone')
+	mydb.connect()
+	mydb = postgres_db('that one')
+	mydb.connect()
+	print(mydb.dbstr())	
+
+	#print(mydb.does_table_exist('projectbuckets'))
+	#mydb.enable_logging = True
+	#mydb.logquery(mydb.db_conn_dets.dbconnectionstr())
+
+	#print('Connected to ' + mydb.dbversion())
+	#qry = """
+	#SELECT DISTINCT table_catalog as database_name, table_schema as schema 
+	#FROM INFORMATION_SCHEMA.TABLES
+	#"""
+	#print(mydb.export_query_to_str(qry,'\t'))
+
+	#mydb.load_csv_to_table('projectbuckets.tsv','projectbuckets',True,'\t')
+
+	mydb.close()	
+
 class dbconnection_details: 
-	def __init__(self): 
+	def __init__(self,DSN): 
+		self.DSN = DSN
 		self.DatabaseType='Postgres' 
 		self.updated='Mar 8/2023' 
 		self.settings_loaded_from_file = False
 
 		self.DB_USERNAME='' 
 		self.DB_USERPWD=''
 		self.DB_HOST='' 
@@ -22,63 +45,75 @@
 		self.DB_SCHEMA=''
 		self.loadSettingsFromFile()
 
 	def loadSettingsFromFile(self):
 		try:
 			f = open('.schemawiz_config1','r')
 			connectionstrlines = f.read()
-			connectionstr = garbledave().ungarbleit(connectionstrlines.splitlines()[0])
 			f.close()
-			connarr = connectionstr.split(' - ')
-
-			self.DB_USERNAME	= connarr[0]
-			self.DB_USERPWD		= connarr[1]
-			self.DB_HOST			= connarr[2] 
-			self.DB_PORT			= connarr[3]
-			self.DB_NAME			= connarr[4]
-			self.DB_SCHEMA		= connarr[5]
-			if self.DB_SCHEMA.strip() == '':
-				self.DB_SCHEMA = 'public'
+			connectionlines = connectionstrlines.split('\n')
+			for connectionline in connectionlines:
+				connectionstr = garbledave().ungarbleit(connectionline)
+				connarr = connectionstr.split(' - ')
+				if connarr[0] == self.DSN:
+						
+					self.DB_USERNAME	= connarr[1]
+					self.DB_USERPWD		= connarr[2]
+					self.DB_HOST			= connarr[3] 
+					self.DB_PORT			= connarr[4]
+					self.DB_NAME			= connarr[5]
+					self.DB_SCHEMA		= connarr[6]
+					if self.DB_SCHEMA.strip() == '':
+						self.DB_SCHEMA = 'public'
 			
-			self.settings_loaded_from_file = True
+					self.settings_loaded_from_file = True
+					break
+
 		except:
+			self.settings_loaded_from_file = False
+		
+		if not self.settings_loaded_from_file:
 			#saved connection details not found. using defaults
 			self.DB_USERNAME='postgres' 
 			self.DB_HOST='localhost' 
 			self.DB_PORT='1532' 
 			self.DB_NAME='postgres' 
 			self.DB_SCHEMA='public'		
 			self.DB_USERPWD='no-password-supplied'
 
+		return self.settings_loaded_from_file
+
 	def dbconnectionstr(self):
-		return 'usr=' + self.DB_USERNAME + '; svr=' + self.DB_HOST + '; port=' + self.DB_PORT + '; Database=' + self.DB_NAME + '; Schema=' + self.DB_SCHEMA + '; pwd=' + self.DB_USERPWD
+		return 'usr=' + self.DB_USERNAME + '; svr=' + self.DB_HOST + '; port=' + self.DB_PORT + '; Database=' + self.DB_NAME + '; Schema=' + self.DB_SCHEMA 
 
 	def saveConnectionDefaults(self,DB_USERNAME='postgres',DB_USERPWD='no-password-supplied',DB_HOST='localhost',DB_PORT='1532',DB_NAME='postgres',DB_SCHEMA='public'):
-		f = open('.schemawiz_config1','w')
-		f.write(garbledave().garbleit(DB_USERNAME + ' - ' + DB_USERPWD + ' - ' + DB_HOST + ' - ' + DB_PORT + ' - ' + DB_NAME + ' - ' + DB_SCHEMA))
+		f = open('.schemawiz_config1','a')
+		f.write(garbledave().garbleit(self.DSN + ' - ' + DB_USERNAME + ' - ' + DB_USERPWD + ' - ' + DB_HOST + ' - ' + DB_PORT + ' - ' + DB_NAME + ' - ' + DB_SCHEMA) + '\n')
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
 
 class postgres_db:
-	def __init__(self,DB_USERPWD='no-password-supplied',DB_SCHEMA='no-schema-supplied'):
+	def __init__(self,DSN='default',DB_USERPWD='no-password-supplied',DB_SCHEMA='no-schema-supplied'):
+		self.DSN = DSN
+
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
@@ -297,15 +332,15 @@
 
 		self.export_query_to_csv('SELECT * FROM ' + qualified_table,csvfile,szdelimiter)
 
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
@@ -358,14 +393,18 @@
 				if line.strip()!='':
 					if skiprow1 == 0:
 						skiprow1 = 1
 					else:
 						batchcount += 1
 						unquotedline = self.handledblquotes(line.rstrip("\n"))
 						row = unquotedline.split(szdelimiter)
+						missingfldcount = len(hdrs) - len(row)
+						for x in range(0,missingfldcount):
+							row.append('NULL')
+
 						newline = "("
 						for var in withextrafields:
 							newline += "'" + withextrafields[var]  + "',"
 
 						for j in range(0,len(row)):
 							if row[j].lower() == 'none' or row[j].lower() == 'null':
 								newline += "NULL,"
@@ -396,14 +435,16 @@
 							
 						ilines += newline[:-1] + '),'
 						
 						if batchcount > 500:
 							qry = isqlhdr + ilines[:-1]
 							batchcount = 0
 							ilines = ''
+							#print(qry)
+							#sys.exit(0)
 							self.execute(qry)
 
 		if batchcount > 0:
 			qry = isqlhdr + ilines[:-1]
 			batchcount = 0
 			ilines = ''
 			self.execute(qry)
@@ -430,14 +471,15 @@
 			return True
 
 	def close(self):
 		if self.dbconn:
 			self.dbconn.close()
 
 	def ask_for_database_details(self):
+		print('Asking about DSN: ' +  self.DSN)
 		self.db_conn_dets.DB_HOST = input('DB_HOST (localhost): ') or 'localhost'
 		self.db_conn_dets.DB_PORT = input('DB_PORT (1532): ') or '1532'
 		self.db_conn_dets.DB_NAME = input('DB_NAME (postgres): ') or 'postgres'
 		self.db_conn_dets.DB_SCHEMA = input('DB_SCHEMA (public): ') or 'public'
 		self.db_conn_dets.DB_USERNAME = input('DB_USERNAME (postgres): ') or 'postgres'
 		self.db_conn_dets.DB_USERPWD = input('DB_USERPWD: ') or '4165605869'
 
@@ -505,26 +547,9 @@
 			self.execute(select_one_fld)
 			retval=self.cur.fetchone()
 			return retval[0]
 		except Exception as e:
 			raise Exception("SQL ERROR:\n\n" + str(e))
 
 if __name__ == '__main__':
-	mydb = postgres_db()
-	mydb.connect()
-	print(mydb.dbstr())	
-
-	#print(mydb.does_table_exist('newtbl'))
-	#mydb.enable_logging = True
-	#mydb.logquery(mydb.db_conn_dets.dbconnectionstr())
-
-	#print('Connected to ' + mydb.dbversion())
-	#qry = """
-	#SELECT DISTINCT table_catalog as database_name, table_schema as schema 
-	#FROM INFORMATION_SCHEMA.TABLES
-	#"""
-	#print(mydb.export_query_to_str(qry,'\t'))
-
-	#mydb.load_csv_to_table('testcase1.csv','testcase1',True,',')
-
-	mydb.close()	
+	main()
```

### Comparing `postgresdave_package-1.8.0/LICENSE` & `postgresdave_package-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `postgresdave_package-1.8.0/pyproject.toml` & `postgresdave_package-2.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling","psycopg2","garbledave_package"]
 
 build-backend = "hatchling.build"
 
 [project]
 name = "postgresdave_package"
-version = "1.8.0"
+version = "2.0.3"
 dependencies = [
   'psycopg2 >= 2.9.5',
   'garbledave_package >= 1.0.0'
 ]
 authors = [
   { name="Dave Skura", email="dskura@gmail.com" },
 ]
```

### Comparing `postgresdave_package-1.8.0/PKG-INFO` & `postgresdave_package-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postgresdave_package
-Version: 1.8.0
+Version: 2.0.3
 Summary: A wrapper for simplified Postgres usage using psycopg2.
 Project-URL: Homepage, https://github.com/daveskura/postgresdave
 Project-URL: Author Linkedin, https://www.linkedin.com/in/2166883
 Author-email: Dave Skura <dskura@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

