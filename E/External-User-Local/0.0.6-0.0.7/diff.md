# Comparing `tmp/External-User-Local-0.0.6.tar.gz` & `tmp/External-User-Local-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "External-User-Local-0.0.6.tar", last modified: Mon Jul 10 07:35:54 2023, max compression
+gzip compressed data, was "External-User-Local-0.0.7.tar", last modified: Mon Jul 10 10:41:23 2023, max compression
```

## Comparing `External-User-Local-0.0.6.tar` & `External-User-Local-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:35:54.844751 External-User-Local-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:35:54.840751 External-User-Local-0.0.6/External_User_Local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-10 07:35:54.000000 External-User-Local-0.0.6/External_User_Local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-10 07:35:54.000000 External-User-Local-0.0.6/External_User_Local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 07:35:54.000000 External-User-Local-0.0.6/External_User_Local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 07:35:54.000000 External-User-Local-0.0.6/External_User_Local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-10 07:35:54.844751 External-User-Local-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-10 07:35:40.000000 External-User-Local-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:35:54.844751 External-User-Local-0.0.6/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 07:35:40.000000 External-User-Local-0.0.6/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-10 07:35:40.000000 External-User-Local-0.0.6/db/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-07-10 07:35:40.000000 External-User-Local-0.0.6/db/library_DB.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 07:35:54.844751 External-User-Local-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-10 07:35:40.000000 External-User-Local-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:35:54.844751 External-User-Local-0.0.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 07:35:40.000000 External-User-Local-0.0.6/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-10 07:35:40.000000 External-User-Local-0.0.6/src/library.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:35:54.844751 External-User-Local-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-10 07:35:40.000000 External-User-Local-0.0.6/tests/test_insertExternal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:41:23.790332 External-User-Local-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:41:23.786332 External-User-Local-0.0.7/External_User_Local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-10 10:41:23.000000 External-User-Local-0.0.7/External_User_Local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-10 10:41:23.000000 External-User-Local-0.0.7/External_User_Local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:41:23.000000 External-User-Local-0.0.7/External_User_Local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 10:41:23.000000 External-User-Local-0.0.7/External_User_Local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-10 10:41:23.790332 External-User-Local-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-10 10:41:09.000000 External-User-Local-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:41:23.786332 External-User-Local-0.0.7/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:41:09.000000 External-User-Local-0.0.7/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-10 10:41:09.000000 External-User-Local-0.0.7/db/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-07-10 10:41:09.000000 External-User-Local-0.0.7/db/library_DB.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 10:41:23.790332 External-User-Local-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-10 10:41:09.000000 External-User-Local-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:41:23.786332 External-User-Local-0.0.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:41:09.000000 External-User-Local-0.0.7/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-10 10:41:09.000000 External-User-Local-0.0.7/src/library.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:41:23.790332 External-User-Local-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-10 10:41:09.000000 External-User-Local-0.0.7/tests/test_insertExternal.py
```

### Comparing `External-User-Local-0.0.6/README.md` & `External-User-Local-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `External-User-Local-0.0.6/db/library_DB.py` & `External-User-Local-0.0.7/db/library_DB.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,29 +18,31 @@
             res = cursor.fetchone()
             cursor.close()
             max_id = res[0] + 1
             cursor = self.conn.cursor() 
             query_insert_external = "INSERT INTO external_user.external_user_table (id,system_id,username,token) VALUES (%s,1,%s,%s)"
             values=(max_id,user_name,access_token)
             cursor.execute(query_insert_external, values)
-            self.conn.commit()
-            cursor.fetchall()
+            
             cursor.close()
             cursor = self.conn.cursor()
             query_max_id = "SELECT MAX(id) FROM external_user_profile.external_user_profile_table"
             cursor.execute(query_max_id)
             res = cursor.fetchone()
             cursor.close()
-            max_id_new = res[0] + 1
+            if(res[0]):
+                max_id_new = res[0] + 1
+            else:
+                max_id_new=1
             cursor = self.conn.cursor() 
             values=(max_id_new,max_id,profile_id)
             query_insert_external_user_profile= "INSERT INTO external_user_profile.external_user_profile_table (id,external_user_id,profile_id) VALUES (%s,%s,%s)"
             cursor.execute(query_insert_external_user_profile,values)
-            res = cursor.fetchone()
             cursor.close()
+            self.conn.commit()
             locallgr.info("END insert access token to db")
         except mysql.connector.Error as error:
             locallgr.error(error.msg)
             
     def get(self,user_name):
         try:
             locallgr.info("start get access token for "+user_name) 
@@ -62,15 +64,15 @@
             select_query = """
                 SELECT * 
                 FROM external_user.external_user_table AS eu 
                 JOIN external_user_profile.external_user_profile_table AS eup ON eu.id = eup.external_user_id 
                 WHERE eup.profile_id = %s
             """
             cursor.execute(select_query, (profile_id,))
-            result = cursor.fetchall()
+            result = cursor.fetchone()
             cursor.close()
             locallgr.info("END get access token from db")
             return result
         except mysql.connector.Error as error:
             locallgr.error(error.msg)
 
         # Fetch all the rows returned by the query
@@ -114,28 +116,24 @@
             locallgr.error(error.msg)
         
     def delete_by_profile_id(self,profile_id):
         try:
             locallgr.info("start delete user external access token ")
             # Create a cursor object to execute queries
             cursor = self.conn.cursor()
-
-            # Execute the delete query
             delete_query = """
                 UPDATE external_user.external_user_table AS eu
                 JOIN external_user_profile.external_user_profile_table AS eup ON eu.id = eup.external_user_id
                 SET eu.id = NULL, eu.system_id = NULL, eu.username = NULL, eu.token = NULL, eup.profile_id = NULL
                 WHERE eup.profile_id = %s
             """
             cursor.execute(delete_query, (profile_id,))
 
-            # Commit the changes to the database
             self.conn.commit()
 
-            # Close the cursor and database connection
             cursor.close()
             locallgr.info("END delete access token from db")
         except mysql.connector.Error as error:
             locallgr.error(error.msg)
```

### Comparing `External-User-Local-0.0.6/setup.py` & `External-User-Local-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      # TODO: Please update the name and delete this line i.e. XXX-local or XXX-remote (without the -python-package suffix)
      name='External-User-Local',  
-     version='0.0.6',
+     version='0.0.7',
      author="Circles",
      author_email="info@circles.life",
      # TODO: Please update the description and delete this line
      description="PyPI Package for Circles access token library Local/Remote Python",
      # TODO: Please update the long description and delete this line    
      long_description="This is a package for sharing common access tokens function used in different repositories",
      long_description_content_type="text/markdown",
```

### Comparing `External-User-Local-0.0.6/src/library.py` & `External-User-Local-0.0.7/src/library.py`

 * *Files identical despite different names*

### Comparing `External-User-Local-0.0.6/tests/test_insertExternal.py` & `External-User-Local-0.0.7/tests/test_insertExternal.py`

 * *Files identical despite different names*

