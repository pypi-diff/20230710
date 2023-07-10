# Comparing `tmp/davex-2.1.6.tar.gz` & `tmp/davex-2.1.7.tar.gz`

## Comparing `davex-2.1.6.tar` & `davex-2.1.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 davex-2.1.6/.gitattributes
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/.schemawiz_config2
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/.schemawiz_config3
--rw-r--r--   0        0        0     7582 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/MySQLTableAnalysis.py
--rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/PostgresTableAnalysis.py
--rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/SimpleAnalysis.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/TableAnalysis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/__init__.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/cache_chart_counts.py
--rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/help.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/mysql_export.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/mysql_extract.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/mysql_import.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/postgres_export.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/postgres_extract.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/postgres_import.py
--rw-r--r--   0        0        0    16310 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/run.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/sp_analyze.sql
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/sp_setup.sql
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/sqlite_export.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/sqlite_extract.py
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/sqlite_import.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/sqliter.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 davex-2.1.6/src/davex/test.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 davex-2.1.6/tests/.schemawiz_config1
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 davex-2.1.6/tests/.schemawiz_config3
--rwxr-xr-x   0        0        0       28 2020-02-02 00:00:00.000000 davex-2.1.6/tests/BasicTest.bat
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 davex-2.1.6/tests/Untitled1.bat
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 davex-2.1.6/.gitignore
--rw-r--r--   0        0        0    18431 2020-02-02 00:00:00.000000 davex-2.1.6/LICENSE
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 davex-2.1.6/README.md
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 davex-2.1.6/pyproject.toml
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 davex-2.1.6/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 davex-2.1.7/.gitattributes
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/.schemawiz_config2
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/.schemawiz_config3
+-rw-r--r--   0        0        0     7582 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/MySQLTableAnalysis.py
+-rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/PostgresTableAnalysis.py
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/SimpleAnalysis.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/TableAnalysis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/__init__.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/cache_chart_counts.py
+-rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/help.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/mysql_export.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/mysql_extract.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/mysql_import.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/postgres_export.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/postgres_extract.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/postgres_import.py
+-rw-r--r--   0        0        0    16318 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/run.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/sp_analyze.sql
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/sp_setup.sql
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/sqlite_export.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/sqlite_extract.py
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/sqlite_import.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/sqliter.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 davex-2.1.7/src/davex/test.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 davex-2.1.7/tests/.schemawiz_config1
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 davex-2.1.7/tests/.schemawiz_config3
+-rwxr-xr-x   0        0        0       28 2020-02-02 00:00:00.000000 davex-2.1.7/tests/BasicTest.bat
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 davex-2.1.7/tests/Untitled1.bat
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 davex-2.1.7/.gitignore
+-rw-r--r--   0        0        0    18431 2020-02-02 00:00:00.000000 davex-2.1.7/LICENSE
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 davex-2.1.7/README.md
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 davex-2.1.7/pyproject.toml
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 davex-2.1.7/PKG-INFO
```

### Comparing `davex-2.1.6/src/davex/MySQLTableAnalysis.py` & `davex-2.1.7/src/davex/MySQLTableAnalysis.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.6/src/davex/PostgresTableAnalysis.py` & `davex-2.1.7/src/davex/PostgresTableAnalysis.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.6/src/davex/SimpleAnalysis.py` & `davex-2.1.7/src/davex/SimpleAnalysis.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.6/src/davex/TableAnalysis.py` & `davex-2.1.7/src/davex/TableAnalysis.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.6/src/davex/cache_chart_counts.py` & `davex-2.1.7/src/davex/cache_chart_counts.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.6/src/davex/help.py` & `davex-2.1.7/src/davex/help.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.6/src/davex/mysql_export.py` & `davex-2.1.7/src/davex/mysql_export.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.6/src/davex/mysql_extract.py` & `davex-2.1.7/src/davex/mysql_extract.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.6/src/davex/mysql_import.py` & `davex-2.1.7/src/davex/mysql_import.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.6/src/davex/postgres_export.py` & `davex-2.1.7/src/davex/postgres_export.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.6/src/davex/postgres_extract.py` & `davex-2.1.7/src/davex/postgres_extract.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.6/src/davex/postgres_import.py` & `davex-2.1.7/src/davex/postgres_import.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.6/src/davex/run.py` & `davex-2.1.7/src/davex/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
   Dave Skura, Dec,2022
 """
 from sqlitedave_package.sqlitedave import sqlite_db 
 from postgresdave_package.postgresdave import postgres_db 
 from mysqldave_package.mysqldave import mysql_db 
 
-from dbx.PostgresTableAnalysis import runner as Postgres_runner
-from dbx.MySQLTableAnalysis import runner as MySQL_runner
-import dbx.SimpleAnalysis as SimpleAnalysis
+from davex.PostgresTableAnalysis import runner as Postgres_runner
+from davex.MySQLTableAnalysis import runner as MySQL_runner
+import davex.SimpleAnalysis as SimpleAnalysis
 
 from querychart_package.querychart import charter
 
 import readchar
 
 import logging
-from dbx import help
+from davex import help
 import sys
 
 logging.basicConfig(level=logging.INFO)
 
 def main():
 	selected_schema = ''
 	selected_table = ''
```

### Comparing `davex-2.1.6/src/davex/sp_analyze.sql` & `davex-2.1.7/src/davex/sp_analyze.sql`

 * *Files identical despite different names*

### Comparing `davex-2.1.6/src/davex/sp_setup.sql` & `davex-2.1.7/src/davex/sp_setup.sql`

 * *Files identical despite different names*

### Comparing `davex-2.1.6/src/davex/sqlite_export.py` & `davex-2.1.7/src/davex/sqlite_export.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.6/src/davex/sqlite_extract.py` & `davex-2.1.7/src/davex/sqlite_extract.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.6/src/davex/sqlite_import.py` & `davex-2.1.7/src/davex/sqlite_import.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.6/src/davex/sqliter.py` & `davex-2.1.7/src/davex/sqliter.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.6/src/davex/test.py` & `davex-2.1.7/src/davex/test.py`

 * *Files identical despite different names*

### Comparing `davex-2.1.6/LICENSE` & `davex-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `davex-2.1.6/pyproject.toml` & `davex-2.1.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
-requires = ["hatchling","schemawizard_package","postgresdave_package","mysqldave_package","garbledave_package","sqlitedave_package"]
+requires = ["hatchling","querychart_package","schemawizard_package","postgresdave_package","mysqldave_package","garbledave_package","sqlitedave_package"]
 
 build-backend = "hatchling.build"
 
 [project]
 name = "davex"
-version = "2.1.6"
+version = "2.1.7"
 dependencies = [
-	'querychart_package >= 2.0.3',
+  'querychart_package >= 2.0.3',
   'schemawizard_package >= 2.5.1',
   'postgresdave_package >= 2.0.3',
   'mysqldave_package >= 2.0.3',
   'sqlitedave_package >= 2.0.1',
   'garbledave_package >= 1.0.0 '
 ]
 authors = [
```

### Comparing `davex-2.1.6/PKG-INFO` & `davex-2.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: davex
-Version: 2.1.6
+Version: 2.1.7
 Summary: Command line Data Profiling for Postgres, MySQL and sqlite.
 Project-URL: Homepage, https://github.com/daveskura/davex
 Project-URL: Author Linkedin, https://www.linkedin.com/in/2166883
 Author-email: Dave Skura <dskura@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

