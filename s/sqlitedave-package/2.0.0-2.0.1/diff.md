# Comparing `tmp/sqlitedave_package-2.0.0.tar.gz` & `tmp/sqlitedave_package-2.0.1.tar.gz`

## Comparing `sqlitedave_package-2.0.0.tar` & `sqlitedave_package-2.0.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.0/src/sqlitedave_package/.schemawiz_config3
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.0/src/sqlitedave_package/__init__.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.0/src/sqlitedave_package/a.csv
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.0/src/sqlitedave_package/complexdata.csv
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.0/src/sqlitedave_package/execute.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.0/src/sqlitedave_package/postgres_data.tsv
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.0/src/sqlitedave_package/query.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.0/src/sqlitedave_package/select.sql
--rw-r--r--   0        0        0    13433 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.0/src/sqlitedave_package/sqlitedave.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.0/src/sqlitedave_package/testcase1.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.0/src/sqlitedave_package/that_db
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.0/src/sqlitedave_package/this_db
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.0/tests/create_tables.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.0/tests/create_tesla.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.0/tests/select_from_sqlite_db.py
--rw-r--r--   0        0        0    50392 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.0/tests/tesla.csv
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.0/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.0/LICENSE
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.0/README.md
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/src/sqlitedave_package/.schemawiz_config3
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/src/sqlitedave_package/__init__.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/src/sqlitedave_package/a.csv
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/src/sqlitedave_package/complexdata.csv
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/src/sqlitedave_package/execute.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/src/sqlitedave_package/postgres_data.tsv
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/src/sqlitedave_package/query.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/src/sqlitedave_package/select.sql
+-rw-r--r--   0        0        0    13894 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/src/sqlitedave_package/sqlitedave.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/src/sqlitedave_package/testcase1.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/src/sqlitedave_package/that_db
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/src/sqlitedave_package/this_db
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/src/sqlitedave_package/z.testcase1.ddl
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/tests/create_tables.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/tests/create_tesla.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/tests/select_from_sqlite_db.py
+-rw-r--r--   0        0        0    50392 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/tests/tesla.csv
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/LICENSE
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/README.md
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 sqlitedave_package-2.0.1/PKG-INFO
```

### Comparing `sqlitedave_package-2.0.0/src/sqlitedave_package/execute.py` & `sqlitedave_package-2.0.1/src/sqlitedave_package/execute.py`

 * *Files identical despite different names*

### Comparing `sqlitedave_package-2.0.0/src/sqlitedave_package/query.py` & `sqlitedave_package-2.0.1/src/sqlitedave_package/query.py`

 * *Files identical despite different names*

### Comparing `sqlitedave_package-2.0.0/src/sqlitedave_package/sqlitedave.py` & `sqlitedave_package-2.0.1/src/sqlitedave_package/sqlitedave.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,29 +26,39 @@
 
 	mydb = sqlite_db()
 	mydb.connect()
 	print(mydb.dbstr())
 	#mydb.execute(qry)
 	
 	#mydb.load_csv_to_table('testcase1.csv','testcase1',True,',')
-	#print(mydb.queryone('SELECT COUNT(*) FROM testcase1'))
+	#data = mydb.query('SELECT * FROM testcase1')
+	#print(str(data.colcount))
+	#print(str(data.rowcount))
+	#print(str(data.column_names))
+
+	#for row in data:
+	#	for i in range(0,data.colcount):
+	#		print(row[i])
+
 
 	#print(mydb.export_query_to_str('SELECT count(*) FROM testcase1'))
 
 	#csvfilename = 'Station.tsv'
 	#tblname = 'Station'
 	
 	#mydb.load_csv_to_table('a.csv','tablea',True,',')
 	#mydb.export_table_to_csv(csvfilename,tblname)
 
 class disconnected_cursor:
 	def __init__(self,datacursor):
 		self.data = []
+		self.column_names = []
 		inputTuple = ()
 		for k in (i[0] for i in datacursor.description):
+			self.column_names.append(k)
 			col = (k,None,None,None,None,None,None)
 			inputTuple += col
 
 		self.description = tuple(splitTupleandGroup(7, inputTuple))
 		self.rowcount = 0
 		self.colcount = 0
 		for row in datacursor:
@@ -114,14 +124,18 @@
 		self.data_type = ''
 		self.Need_Quotes = ''
 		self.ordinal_position = -1
 		self.comment = '' # dateformat in csv [%Y/%m/%d]
 
 class sqlite_db:
 	def __init__(self,DB_NAME=''):
+		self.rowcount = -1
+		self.colcount = -1
+		self.column_names = []
+
 		self.delimiter = ''
 		self.delimiter_replace = '^~^'
 		self.enable_logging = False
 		self.max_loglines = 500
 		self.db_conn_dets = dbconnection_details(DB_NAME)
 		self.dbconn = None
 		self.cur = None
@@ -481,17 +495,21 @@
 
 			raise Exception(str(e))
 
 	def query(self,qry):
 		if not self.chk_conn():
 			self.connect()
 
-		all_rows_of_data = disconnected_cursor(self.dbconn.execute(qry))
+		self.all_rows_of_data = disconnected_cursor(self.dbconn.execute(qry))
+		self.rowcount = self.all_rows_of_data.rowcount
+		self.colcount = self.all_rows_of_data.colcount
+		self.column_names = self.all_rows_of_data.column_names
+
 		self.close()
-		return all_rows_of_data
+		return self.all_rows_of_data
 
 	def commit(self):
 		if self.chk_conn():
 			self.dbconn.commit()
 
 	def execute(self,qry):
 		try:
```

### Comparing `sqlitedave_package-2.0.0/tests/create_tables.py` & `sqlitedave_package-2.0.1/tests/create_tables.py`

 * *Files identical despite different names*

### Comparing `sqlitedave_package-2.0.0/tests/tesla.csv` & `sqlitedave_package-2.0.1/tests/tesla.csv`

 * *Files identical despite different names*

### Comparing `sqlitedave_package-2.0.0/LICENSE` & `sqlitedave_package-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlitedave_package-2.0.0/README.md` & `sqlitedave_package-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlitedave_package-2.0.0/pyproject.toml` & `sqlitedave_package-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling","garbledave_package"]
 
 build-backend = "hatchling.build"
 
 [project]
 name = "sqlitedave_package"
-version = "2.0.0"
+version = "2.0.1"
 dependencies = [
   'garbledave_package >= 1.0.0'
 ]
 authors = [
   { name="Dave Skura", email="dskura@gmail.com" },
 ]
 description = "A wrapper for simplified sqlite usage using sqlite3."
```

### Comparing `sqlitedave_package-2.0.0/PKG-INFO` & `sqlitedave_package-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlitedave_package
-Version: 2.0.0
+Version: 2.0.1
 Summary: A wrapper for simplified sqlite usage using sqlite3.
 Project-URL: Homepage, https://github.com/daveskura/sqlitedave
 Project-URL: Author Linkedin, https://www.linkedin.com/in/2166883
 Author-email: Dave Skura <dskura@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

