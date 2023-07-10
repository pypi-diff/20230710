# Comparing `tmp/tableau_utilities-2.0.4.tar.gz` & `tmp/tableau_utilities-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableau_utilities-2.0.4.tar", last modified: Fri Jul  7 14:44:49 2023, max compression
+gzip compressed data, was "tableau_utilities-2.0.5.tar", last modified: Mon Jul 10 18:52:32 2023, max compression
```

## Comparing `tableau_utilities-2.0.4.tar` & `tableau_utilities-2.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-07 14:44:49.567978 tableau_utilities-2.0.4/
--rw-r--r--   0 justin     (502) staff       (20)     1062 2022-05-25 18:48:01.000000 tableau_utilities-2.0.4/LICENSE
--rw-r--r--   0 justin     (502) staff       (20)     8420 2023-07-07 14:44:49.567362 tableau_utilities-2.0.4/PKG-INFO
--rw-r--r--   0 justin     (502) staff       (20)     8116 2023-06-28 16:57:49.000000 tableau_utilities-2.0.4/README.md
--rw-r--r--   0 justin     (502) staff       (20)       38 2023-07-07 14:44:49.568167 tableau_utilities-2.0.4/setup.cfg
--rw-r--r--   0 justin     (502) staff       (20)     1107 2023-07-07 14:44:23.000000 tableau_utilities-2.0.4/setup.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-07 14:44:49.544654 tableau_utilities-2.0.4/tableau_utilities/
--rw-r--r--   0 justin     (502) staff       (20)      272 2023-06-28 16:57:49.000000 tableau_utilities-2.0.4/tableau_utilities/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)     2441 2023-06-28 16:57:49.000000 tableau_utilities-2.0.4/tableau_utilities/fetch_all_cols.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-07 14:44:49.551724 tableau_utilities-2.0.4/tableau_utilities/general/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.4/tableau_utilities/general/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)     2235 2023-06-28 16:57:49.000000 tableau_utilities-2.0.4/tableau_utilities/general/cli_styling.py
--rw-r--r--   0 justin     (502) staff       (20)     3497 2023-06-28 16:57:49.000000 tableau_utilities-2.0.4/tableau_utilities/general/config_column_persona.py
--rw-r--r--   0 justin     (502) staff       (20)     2278 2023-06-28 16:57:49.000000 tableau_utilities-2.0.4/tableau_utilities/general/funcs.py
--rw-r--r--   0 justin     (502) staff       (20)     2874 2023-06-28 16:57:49.000000 tableau_utilities-2.0.4/tableau_utilities/scripted_testing.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-07 14:44:49.559550 tableau_utilities-2.0.4/tableau_utilities/scripts/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.4/tableau_utilities/scripts/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)    23247 2023-06-28 16:57:49.000000 tableau_utilities-2.0.4/tableau_utilities/scripts/cli.py
--rw-r--r--   0 justin     (502) staff       (20)     1772 2023-06-28 16:57:49.000000 tableau_utilities-2.0.4/tableau_utilities/scripts/csv_config.py
--rw-r--r--   0 justin     (502) staff       (20)     7174 2023-07-07 14:44:23.000000 tableau_utilities-2.0.4/tableau_utilities/scripts/datasource.py
--rw-r--r--   0 justin     (502) staff       (20)    13151 2023-06-28 16:57:49.000000 tableau_utilities-2.0.4/tableau_utilities/scripts/gen_config.py
--rw-r--r--   0 justin     (502) staff       (20)     8539 2023-06-28 16:57:49.000000 tableau_utilities-2.0.4/tableau_utilities/scripts/merge_config.py
--rw-r--r--   0 justin     (502) staff       (20)     1867 2023-06-28 16:57:49.000000 tableau_utilities-2.0.4/tableau_utilities/scripts/server_info.py
--rw-r--r--   0 justin     (502) staff       (20)     4531 2023-06-28 16:57:49.000000 tableau_utilities-2.0.4/tableau_utilities/scripts/server_operate.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-07 14:44:49.562433 tableau_utilities-2.0.4/tableau_utilities/tableau_file/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.4/tableau_utilities/tableau_file/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)    11142 2023-06-29 22:18:13.000000 tableau_utilities-2.0.4/tableau_utilities/tableau_file/tableau_file.py
--rw-r--r--   0 justin     (502) staff       (20)    35162 2023-07-07 14:44:23.000000 tableau_utilities-2.0.4/tableau_utilities/tableau_file/tableau_file_objects.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-07 14:44:49.566127 tableau_utilities-2.0.4/tableau_utilities/tableau_server/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.4/tableau_utilities/tableau_server/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)    31778 2023-06-28 16:57:49.000000 tableau_utilities-2.0.4/tableau_utilities/tableau_server/tableau_server.py
--rw-r--r--   0 justin     (502) staff       (20)    13195 2023-06-28 16:57:49.000000 tableau_utilities-2.0.4/tableau_utilities/tableau_server/tableau_server_objects.py
--rw-r--r--   0 justin     (502) staff       (20)    10765 2023-07-07 14:44:23.000000 tableau_utilities-2.0.4/tableau_utilities/test_tableau_utilities.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-07 14:44:49.548988 tableau_utilities-2.0.4/tableau_utilities.egg-info/
--rw-r--r--   0 justin     (502) staff       (20)     8420 2023-07-07 14:44:49.000000 tableau_utilities-2.0.4/tableau_utilities.egg-info/PKG-INFO
--rw-r--r--   0 justin     (502) staff       (20)     1205 2023-07-07 14:44:49.000000 tableau_utilities-2.0.4/tableau_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 justin     (502) staff       (20)        1 2023-07-07 14:44:49.000000 tableau_utilities-2.0.4/tableau_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 justin     (502) staff       (20)       73 2023-07-07 14:44:49.000000 tableau_utilities-2.0.4/tableau_utilities.egg-info/entry_points.txt
--rw-r--r--   0 justin     (502) staff       (20)      112 2023-07-07 14:44:49.000000 tableau_utilities-2.0.4/tableau_utilities.egg-info/requires.txt
--rw-r--r--   0 justin     (502) staff       (20)       18 2023-07-07 14:44:49.000000 tableau_utilities-2.0.4/tableau_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-10 18:52:32.142441 tableau_utilities-2.0.5/
+-rw-r--r--   0 justin     (502) staff       (20)     1062 2022-05-25 18:48:01.000000 tableau_utilities-2.0.5/LICENSE
+-rw-r--r--   0 justin     (502) staff       (20)     8420 2023-07-10 18:52:32.141781 tableau_utilities-2.0.5/PKG-INFO
+-rw-r--r--   0 justin     (502) staff       (20)     8116 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/README.md
+-rw-r--r--   0 justin     (502) staff       (20)       38 2023-07-10 18:52:32.142865 tableau_utilities-2.0.5/setup.cfg
+-rw-r--r--   0 justin     (502) staff       (20)     1107 2023-07-10 18:51:08.000000 tableau_utilities-2.0.5/setup.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-10 18:52:32.123024 tableau_utilities-2.0.5/tableau_utilities/
+-rw-r--r--   0 justin     (502) staff       (20)      272 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)     2441 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/fetch_all_cols.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-10 18:52:32.129172 tableau_utilities-2.0.5/tableau_utilities/general/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/general/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)     2235 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/general/cli_styling.py
+-rw-r--r--   0 justin     (502) staff       (20)     3497 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/general/config_column_persona.py
+-rw-r--r--   0 justin     (502) staff       (20)     2278 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/general/funcs.py
+-rw-r--r--   0 justin     (502) staff       (20)     2874 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/scripted_testing.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-10 18:52:32.135174 tableau_utilities-2.0.5/tableau_utilities/scripts/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/scripts/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)    23247 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/scripts/cli.py
+-rw-r--r--   0 justin     (502) staff       (20)     1772 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/scripts/csv_config.py
+-rw-r--r--   0 justin     (502) staff       (20)     7647 2023-07-10 18:51:08.000000 tableau_utilities-2.0.5/tableau_utilities/scripts/datasource.py
+-rw-r--r--   0 justin     (502) staff       (20)    13151 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/scripts/gen_config.py
+-rw-r--r--   0 justin     (502) staff       (20)     8539 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/scripts/merge_config.py
+-rw-r--r--   0 justin     (502) staff       (20)     1867 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/scripts/server_info.py
+-rw-r--r--   0 justin     (502) staff       (20)     4531 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/scripts/server_operate.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-10 18:52:32.137055 tableau_utilities-2.0.5/tableau_utilities/tableau_file/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/tableau_file/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)    11705 2023-07-10 18:51:08.000000 tableau_utilities-2.0.5/tableau_utilities/tableau_file/tableau_file.py
+-rw-r--r--   0 justin     (502) staff       (20)    37816 2023-07-10 18:51:08.000000 tableau_utilities-2.0.5/tableau_utilities/tableau_file/tableau_file_objects.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-10 18:52:32.140457 tableau_utilities-2.0.5/tableau_utilities/tableau_server/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/tableau_server/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)    31778 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/tableau_server/tableau_server.py
+-rw-r--r--   0 justin     (502) staff       (20)    13195 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/tableau_server/tableau_server_objects.py
+-rw-r--r--   0 justin     (502) staff       (20)    10765 2023-07-10 18:39:33.000000 tableau_utilities-2.0.5/tableau_utilities/test_tableau_utilities.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-10 18:52:32.126708 tableau_utilities-2.0.5/tableau_utilities.egg-info/
+-rw-r--r--   0 justin     (502) staff       (20)     8420 2023-07-10 18:52:32.000000 tableau_utilities-2.0.5/tableau_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 justin     (502) staff       (20)     1205 2023-07-10 18:52:32.000000 tableau_utilities-2.0.5/tableau_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 justin     (502) staff       (20)        1 2023-07-10 18:52:32.000000 tableau_utilities-2.0.5/tableau_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 justin     (502) staff       (20)       73 2023-07-10 18:52:32.000000 tableau_utilities-2.0.5/tableau_utilities.egg-info/entry_points.txt
+-rw-r--r--   0 justin     (502) staff       (20)      112 2023-07-10 18:52:32.000000 tableau_utilities-2.0.5/tableau_utilities.egg-info/requires.txt
+-rw-r--r--   0 justin     (502) staff       (20)       18 2023-07-10 18:52:32.000000 tableau_utilities-2.0.5/tableau_utilities.egg-info/top_level.txt
```

### Comparing `tableau_utilities-2.0.4/LICENSE` & `tableau_utilities-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.4/PKG-INFO` & `tableau_utilities-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableau_utilities
-Version: 2.0.4
+Version: 2.0.5
 Summary: Utility for maintaining Tableau objects
 Home-page: http://pypi.python.org/pypi/tableau-utilities/
 Author: Justin Grilli
 Author-email: justin.grilli@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tableau_utilities-2.0.4/README.md` & `tableau_utilities-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.4/setup.py` & `tableau_utilities-2.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     author_email="justin.grilli@gmail.com",
     license='MIT',
     url='http://pypi.python.org/pypi/tableau-utilities/',
     description='Utility for maintaining Tableau objects',
     long_description=readme,
     long_description_content_type='text/markdown',
     name="tableau_utilities",
-    version="2.0.4",
+    version="2.0.5",
     packages=[
         'tableau_utilities',
         'tableau_utilities.general',
         'tableau_utilities.tableau_file',
         'tableau_utilities.tableau_server',
         'tableau_utilities.scripts'
     ],
```

### Comparing `tableau_utilities-2.0.4/tableau_utilities/fetch_all_cols.py` & `tableau_utilities-2.0.5/tableau_utilities/fetch_all_cols.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.4/tableau_utilities/general/cli_styling.py` & `tableau_utilities-2.0.5/tableau_utilities/general/cli_styling.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.4/tableau_utilities/general/config_column_persona.py` & `tableau_utilities-2.0.5/tableau_utilities/general/config_column_persona.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.4/tableau_utilities/general/funcs.py` & `tableau_utilities-2.0.5/tableau_utilities/general/funcs.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.4/tableau_utilities/scripted_testing.py` & `tableau_utilities-2.0.5/tableau_utilities/scripted_testing.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.4/tableau_utilities/scripts/cli.py` & `tableau_utilities-2.0.5/tableau_utilities/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.4/tableau_utilities/scripts/csv_config.py` & `tableau_utilities-2.0.5/tableau_utilities/scripts/csv_config.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.4/tableau_utilities/scripts/datasource.py` & `tableau_utilities-2.0.5/tableau_utilities/scripts/datasource.py`

 * *Files 20% similar despite different names*

```diff
@@ -55,28 +55,28 @@
     # Print Styling
     color = Color()
     symbol = Symbol()
 
     # Downloads the datasource from Tableau Server if the datasource is not local
     if location == 'online':
         d = server.get_datasource(datasource_id, datasource_name, project_name)
-        datasource_path = server.download_datasource(d.id, include_extract)
+        datasource_path = server.download_datasource(d.id, include_extract=include_extract)
         print(f'{color.fg_green}{symbol.success}  Downloaded Datasource:', f'{color.fg_yellow}{datasource_path}{color.reset}', '\n')
 
     datasource_file_name = os.path.basename(datasource_path)
     ds = Datasource(datasource_path)
 
     if save_tds:
         save_folder = f'{datasource_file_name} - BEFORE'
         os.makedirs(save_folder, exist_ok=True)
         if ds.extension == 'tds':
             xml_path = os.path.join(save_folder, datasource_file_name)
             shutil.copy(datasource_path, xml_path)
         else:
-            xml_path = ds.unzip(extract_to=save_folder)
+            xml_path = ds.unzip(extract_to=save_folder, unzip_all=True)
         if debugging_logs:
             print(f'{color.fg_green}{symbol.success}  BEFORE - TDS SAVED TO: {color.fg_yellow}{xml_path}{color.reset}')
 
     # List each of the objects specified to list
     if list_objects:
         print(f'{color.fg_cyan}{list_objects}:{color.reset}')
     if list_objects == 'Columns':
@@ -143,32 +143,35 @@
     if delete == 'folder':
         ds.folders_common.folder.delete(folder_name)
 
     # Enforce Connection
     if enforce_connection:
         if debugging_logs:
             print(f'Updating the datasource connection: {color.fg_cyan}{conn_type}{color.reset}')
-        ds.connection.update(tfo.Connection(
-            class_name=conn_type,
-            server=conn_host,
-            username=conn_user,
-            service=conn_role,
-            dbname=conn_db,
-            schema=conn_schema,
-            warehouse=conn_warehouse
-        ))
+        connection = ds.connection.get(conn_type)
+        if not connection and debugging_logs:
+            print(f'Datasource does not contain a connection of type: {conn_type}')
+        else:
+            connection.class_name = conn_type or connection.class_name
+            connection.server = conn_host or connection.server
+            connection.username = conn_user or connection.username
+            connection.service = conn_role or connection.service
+            connection.dbname = conn_db or connection.dbname
+            connection.schema = conn_schema or connection.schema
+            connection.warehouse = conn_warehouse or connection.warehouse
+            ds.connection.update(connection)
 
     # Save the datasource if an edit may have happened
     if column_name or folder_name or delete or enforce_connection:
         ds.save()
         print(f'{color.fg_green}{symbol.success}  Saved changes to: {color.fg_yellow}{datasource_path}{color.reset}')
 
     if save_tds:
         save_folder = f'{datasource_file_name} - AFTER'
         os.makedirs(save_folder, exist_ok=True)
         if ds.extension == 'tds':
             xml_path = os.path.join(save_folder, datasource_file_name)
             shutil.copy(datasource_path, xml_path)
         else:
-            xml_path = ds.unzip(extract_to=save_folder)
+            xml_path = ds.unzip(extract_to=save_folder, unzip_all=True)
         if debugging_logs:
             print(f'{color.fg_green}{symbol.success}  AFTER - TDS SAVED TO: {color.fg_yellow}{xml_path}{color.reset}')
```

### Comparing `tableau_utilities-2.0.4/tableau_utilities/scripts/gen_config.py` & `tableau_utilities-2.0.5/tableau_utilities/scripts/gen_config.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.4/tableau_utilities/scripts/merge_config.py` & `tableau_utilities-2.0.5/tableau_utilities/scripts/merge_config.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.4/tableau_utilities/scripts/server_info.py` & `tableau_utilities-2.0.5/tableau_utilities/scripts/server_info.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.4/tableau_utilities/scripts/server_operate.py` & `tableau_utilities-2.0.5/tableau_utilities/scripts/server_operate.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.4/tableau_utilities/tableau_file/tableau_file.py` & `tableau_utilities-2.0.5/tableau_utilities/tableau_file/tableau_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,21 +83,30 @@
                     tableau_file_path = os.path.join(file_dir, z.filename)
         return tableau_file_path
 
     def save(self):
         """ Save/Update the Tableau file with the XML changes made """
 
         if self.extension in ['tdsx', 'twbx']:
-            with ZipFile(self.file_path, 'r') as zr, ZipFile(self.file_path, 'w') as zw:
+            # Rebuild the TDSX / TWBX archive file, with the updated archived TDS / TWB
+            directory = os.path.dirname(self.file_path)
+            file_name = os.path.basename(self.file_path)
+            temp_path = os.path.join(directory, f'__temp_{file_name}')
+            with ZipFile(self.file_path, 'r') as zr, ZipFile(temp_path, 'w') as zw:
                 for file in zr.filelist:
                     if file.filename.split('.')[-1] in ['tds', 'twb']:
-                        self._tree.write(zw.open(file.filename, 'w'))
+                        self._tree.write(zw.open(file.filename, 'w'),
+                                         encoding="utf-8", xml_declaration=True)
+                    else:
+                        zw.writestr(file, zr.read(file.filename))
+            os.remove(self.file_path)
+            os.rename(temp_path, self.file_path)
         else:
             # Update the Tableau file's contents
-            self._tree.write(self.file_path)
+            self._tree.write(self.file_path, encoding="utf-8", xml_declaration=True)
 
 
 class Datasource(TableauFile):
     """
         A class representation of a Tableau Datasource.
         Used to update a Tableau Datasource by interacting with various elements,
         such as Columns, Folders, Connections, Metadata, etc.
@@ -151,17 +160,17 @@
                 new_item = transform_tableau_object(item)
                 try:
                     section.append(obj(**new_item))
                 except TypeError as err:
                     raise TableauFileError(f'{err}\n\nPre-transform {obj.tag} attributes: {item}') from err
         if len(section) > 1 or len(section) == 1 and enforce_list:
             return tfo.TableauFileObjects(section, item_class=obj, tag=obj.tag)
-        elif len(section) == 1:
+        if len(section) == 1:
             return section[0]
-        elif enforce_list:
+        if enforce_list:
             return tfo.TableauFileObjects(item_class=obj, tag=obj.tag)
         return obj()
 
     def enforce_column(self, column, folder_name=None, remote_name=None):
         """
             Enforces a column by:
                 - Adding the column if it doesn't exist, otherwise updating it to match the column
```

### Comparing `tableau_utilities-2.0.4/tableau_utilities/tableau_file/tableau_file_objects.py` & `tableau_utilities-2.0.5/tableau_utilities/tableau_file/tableau_file_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import sys
 import re
 import xml.etree.ElementTree as ET
 import xmltodict
+from datetime import datetime
 from dataclasses import dataclass, astuple
 from typing import Literal
 from tableau_utilities.general.funcs import transform_tableau_object
 
 @dataclass
 class TableauFileObject:
     """
@@ -46,14 +47,23 @@
             Set the attribute to a boolean,
             if the class has the attribute,
             and if the attribute is a string.
         """
         if self.__existing_str_attr(attr):
             setattr(self, attr, getattr(self, attr).lower() in ['true', 'yes'])
 
+    def __to_datetime(self, attr: str):
+        """
+            Set the attribute to a datetime,
+            if the class has the attribute,
+            and if the attribute is a string.
+        """
+        if self.__existing_str_attr(attr):
+            setattr(self, attr, datetime.strptime(getattr(self, attr), '%Y-%m-%d %H:%M:%S.%f'))
+
     def __post_init__(self):
         # Convert to Boolean
         self.__to_bool('contains_null')
         self.__to_bool('datatype_customized')
         self.__to_bool('extract_engine')
         self.__to_bool('enabled')
         self.__to_bool('hidden')
@@ -64,14 +74,16 @@
         self.__to_int('collation_flag')
         self.__to_int('count')
         self.__to_int('ordinal')
         self.__to_int('port')
         self.__to_int('precision')
         self.__to_int('scale')
         self.__to_int('width')
+        # Convert to Datetime
+        self.__to_datetime('timestamp_start')
 
     def dict(self):
         pass
 
     def xml(self):
         """ Returns the FileObject as an XML Element """
         return ET.fromstring(xmltodict.unparse({self.tag: self.dict()}, pretty=True))
@@ -333,14 +345,15 @@
             output['@visual-totals'] = self.visual_totals
 
         return output
 
 
 @dataclass
 class Relation(TableauFileObject):
+    """ The Relation Tableau file object """
     type: str
     tag: str = 'relation'
     name: str = None
     table: str = None
     text: str = None
     connection: str = None
     relation: TableauFileObjects = None
@@ -358,14 +371,15 @@
         return False
 
     def __post_init__(self):
         if self.relation is not None:
             self.relation = TableauFileObjects(self.relation, item_class=Relation, tag=self.tag)
         else:
             self.relation = TableauFileObjects(item_class=Relation, tag=self.tag)
+        super().__post_init__()
 
     def dict(self):
         dictionary = {'@type': self.type}
         if self.name is not None:
             dictionary['@name'] = self.name
         if self.connection is not None:
             dictionary['@connection'] = self.connection
@@ -376,14 +390,15 @@
         if self.relation is not None:
             dictionary['relation'] = [r.dict() for r in self.relation]
         return dictionary
 
 
 @dataclass
 class MappingCol(TableauFileObject):
+    """ The mapping Col Tableau file object """
     key: str
     value: str
     tag: str = 'map'
 
     def __post_init__(self):
         if not re.match(r'^\[.+]$', self.key):
             self.key = f'[{self.key}]'
@@ -445,14 +460,15 @@
     folder_item: TableauFileObjects[FolderItem] = None
 
     def __post_init__(self):
         if self.folder_item is not None:
             self.folder_item = TableauFileObjects(self.folder_item, item_class=FolderItem, tag='folder-item')
         else:
             self.folder_item = TableauFileObjects(item_class=FolderItem, tag='folder-item')
+        super().__post_init__()
 
     def __hash__(self):
         return hash(str(astuple(self)))
 
     def __eq__(self, other):
         if isinstance(other, str):
             return self.name == other
@@ -477,22 +493,24 @@
             for folder_item in self.folder_item:
                 output['folder-item'].append(folder_item.dict())
         return output
 
 
 @dataclass
 class FoldersCommon(TableauFileObject):
+    """ The FoldersCommon Tableau file object """
     folder: TableauFileObjects[Folder] = None
     tag: str = 'folders-common'
 
     def __post_init__(self):
         if self.folder is not None:
             self.folder = TableauFileObjects(self.folder, item_class=Folder, tag='folder')
         else:
             self.folder = TableauFileObjects(item_class=Folder, tag='folder')
+        super().__post_init__()
 
     def __getitem__(self, item):
         return self.folder[item]
 
     def __setitem__(self, key, value):
         self.folder[key] = value
 
@@ -552,15 +570,15 @@
 
     def dict(self):
         return {'folder': [f.dict() for f in self.folder]}
 
 
 @dataclass
 class DrillPath(TableauFileObject):
-    """ The drill paths """
+    """ The DrillPath Tableau file object """
     name: str
     field: list[str] = None
     tag: str = 'drill-path'
 
     def __hash__(self):
         return hash(str(astuple(self)))
 
@@ -577,22 +595,24 @@
         if self.field:
             output['field'] = self.field
         return output
 
 
 @dataclass
 class DrillPaths(TableauFileObject):
+    """ The DrillPaths Tableau file object """
     drill_path: TableauFileObjects[DrillPath] = None
     tag: str = 'drill-paths'
 
     def __post_init__(self):
         if self.drill_path is not None:
             self.drill_path = TableauFileObjects(self.drill_path, item_class=DrillPath, tag='drill-path')
         else:
             self.drill_path = TableauFileObjects(item_class=DrillPath, tag='drill-path')
+        super().__post_init__()
 
     def __getitem__(self, item):
         return self.drill_path[item]
 
     def __setitem__(self, key, value):
         self.drill_path[key] = value
 
@@ -652,14 +672,15 @@
 
     def dict(self):
         return {'drill-path': [f.dict() for f in self.drill_path]}
 
 
 @dataclass
 class Connection(TableauFileObject):
+    """ The Connection Tableau file object """
     tag: str = 'connection'
     authentication: str = None
     class_name: str = None
     dbname: str = None
     schema: str = None
     server: str = None
     service: str = None
@@ -730,23 +751,24 @@
         if self.port is not None:
             output['@port'] = str(self.port)
         return output
 
 
 @dataclass
 class NamedConnection(TableauFileObject):
-    """ The Connection Tableau file object """
+    """ The NamedConnection Tableau file object """
     name: str
     tag: str = 'named-connection'
     caption: str = None
     connection: Connection = None
 
     def __post_init__(self):
         if self.connection:
             self.connection = Connection(**transform_tableau_object(self.connection))
+        super().__post_init__()
 
     def __hash__(self):
         return hash(str(astuple(self)))
 
     def __eq__(self, other):
         if isinstance(other, str):
             return self.connection.class_name == other
@@ -764,34 +786,34 @@
             '@name': self.name,
             'connection': self.connection.dict()
         }
 
 
 @dataclass
 class MetadataRecord(TableauFileObject):
-    """ The MetadataColumn Tableau file object """
+    """ The MetadataRecord Tableau file object """
     class_name: str
     remote_name: str
     remote_type: str
     parent_name: str
     remote_alias: str
     tag: str = 'metadata-record'
-    local_name: str = None
+    ordinal: int = None
+    family: str = None
     local_type: str = None
-    object_id: str = None
+    local_name: str = None
     aggregation: str = None
-    family: str = None
-    collation: dict = None
-    contains_null: bool = None
     approx_count: int = None
-    ordinal: int = None
+    width: int = None
     precision: int = None
     scale: int = None
-    width: int = None
+    contains_null: bool = None
+    collation: dict = None
     attributes: list = None
+    object_id: str = None
 
     def __post_init__(self):
         if self.attributes and isinstance(self.attributes, dict):
             self.attributes = self.attributes['attribute']
         super().__post_init__()
 
     def __hash__(self):
@@ -840,30 +862,66 @@
         if self.attributes is not None:
             output['attributes'] = dict()
             output['attributes']['attribute'] = self.attributes
         return output
 
 
 @dataclass
+class RefreshEvent(TableauFileObject):
+    """ The RefreshEvent Tableau file object """
+    add_from_file_path: str = None
+    increment_value: str = None
+    refresh_type: str = None
+    rows_inserted: str = None
+    timestamp_start: datetime = None
+
+    def dict(self):
+        dictionary = dict()
+        if self.add_from_file_path is not None:
+            dictionary['@add-from-file-path'] = self.add_from_file_path
+        if self.increment_value is not None:
+            dictionary['@increment-value'] = self.increment_value
+        if self.refresh_type is not None:
+            dictionary['@refresh-type'] = self.refresh_type
+        if self.rows_inserted is not None:
+            dictionary['@rows-inserted'] = self.rows_inserted
+        if isinstance(self.timestamp_start, datetime):
+            dictionary['@timestamp-start'] = self.timestamp_start.strftime('%Y-%m-%d %H:%M:%S.%f')
+        return dictionary
+
+
+@dataclass
 class Refresh(TableauFileObject):
+    """ The Refresh Tableau file object """
     tag: str = 'refresh'
-    refresh_event: dict = None
+    refresh_event: RefreshEvent = None
     increment_key: str = None
     incremental_updates: bool = None
 
+    def __post_init__(self):
+        if isinstance(self.refresh_event, dict):
+            self.refresh_event = RefreshEvent(**transform_tableau_object(self.refresh_event))
+        super().__post_init__()
+
     def dict(self):
-        return {
-            '@refresh-event': self.refresh_event,
-            '@increment-key': self.increment_key,
-            '@incremental-updates': str(self.incremental_updates).lower()
-        }
+        dictionary = dict()
+        if isinstance(self.increment_key, str):
+            dictionary['@increment-key'] = self.increment_key
+        if isinstance(self.incremental_updates, bool):
+            dictionary['@incremental-updates'] = str(self.incremental_updates).lower()
+        if isinstance(self.refresh_event, RefreshEvent):
+            dictionary['refresh-event'] = self.refresh_event.dict()
+        else:
+            dictionary['@refresh-event'] = self.refresh_event
+        return dictionary
 
 
 @dataclass
 class ParentConnection(TableauFileObject):
+    """ The parent Connection Tableau file object """
     tag: str = 'connection'
     class_name: str = None
     authentication: str = None
     access_mode: str = None
     author_locale: str = None
     dbname: str = None
     schema: str = None
@@ -895,14 +953,15 @@
             self.cols = TableauFileObjects(item_class=MappingCol, tag='cols')
         if self.metadata_records is not None:
             self.metadata_records = TableauFileObjects(
                 self.metadata_records['metadata-record'], item_class=MetadataRecord, tag='metadata-records'
             )
         else:
             self.metadata_records = TableauFileObjects(item_class=MetadataRecord, tag='metadata-records')
+        super().__post_init__()
 
     def __getitem__(self, item):
         if item in self.named_connections:
             return self.named_connections[item].connection
 
     def __setitem__(self, key, value):
         self.named_connections[key].connection = value
@@ -931,15 +990,15 @@
         """
         if item.class_name in self.named_connections:
             self.named_connections[item.class_name].caption = item.server
             self.named_connections[item.class_name].connection = item
 
     def dict(self):
         dictionary = {'@class': self.class_name}
-        if self.named_connections is not None:
+        if self.named_connections:
             dictionary['named-connections'] = {'named-connection': [nc.dict() for nc in self.named_connections]}
         if self.relation is not None:
             dictionary['relation'] = self.relation.dict()
         if self.cols is not None:
             dictionary['cols'] = {'map': [c.dict() for c in self.cols]}
         if self.refresh is not None:
             dictionary['refresh'] = self.refresh.dict()
@@ -966,25 +1025,27 @@
         if self.extract_engine is not None:
             dictionary['@extract-engine'] = str(self.extract_engine).lower()
         return dictionary
 
 
 @dataclass
 class Extract(TableauFileObject):
+    """ The Extract Tableau file object """
     object_id: str = None
     user_specific: bool = None
     count: int = None
     enabled: bool = None
     units: str = None
     connection: ParentConnection = None
     tag: str = 'extract'
 
     def __post_init__(self):
         if self.connection is not None:
             self.connection = ParentConnection(**transform_tableau_object(self.connection))
+        super().__post_init__()
 
     def dict(self):
         dictionary = dict()
         if self.object_id is not None:
             dictionary['@object-id'] = self.object_id
         if self.user_specific is not None:
             dictionary['@user-specific'] = str(self.user_specific).lower()
@@ -997,36 +1058,41 @@
         if self.connection is not None:
             dictionary['connection'] = self.connection.dict()
         return dictionary
 
 
 @dataclass
 class Aliases(TableauFileObject):
+    """ The Aliases Tableau file object """
     enabled: bool = True
     tag: str = 'aliases'
 
     def dict(self):
         return {'@enabled': 'yes' if self.enabled else 'no'}
 
+
 @dataclass
 class DateOptions(TableauFileObject):
+    """ The DateOptions Tableau file object """
     fiscal_year_start: str = None
     start_of_week: str = None
     tag: str = 'date-options'
 
     def dict(self):
         dictionary = dict()
         if self.fiscal_year_start is not None:
             dictionary['@fiscal-year-start'] = self.fiscal_year_start
         if self.fiscal_year_start is not None:
             dictionary['@start-of-week'] = self.start_of_week
         return dictionary
 
+
 @dataclass
 class ColumnInstance(TableauFileObject):
+    """ The ColumnInstance Tableau file object """
     column: str = None
     derivation: str = None
     name: str = None
     pivot: str = None
     type: str = None
     tag: str = 'column-instance'
```

### Comparing `tableau_utilities-2.0.4/tableau_utilities/tableau_server/tableau_server.py` & `tableau_utilities-2.0.5/tableau_utilities/tableau_server/tableau_server.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.4/tableau_utilities/tableau_server/tableau_server_objects.py` & `tableau_utilities-2.0.5/tableau_utilities/tableau_server/tableau_server_objects.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.4/tableau_utilities/test_tableau_utilities.py` & `tableau_utilities-2.0.5/tableau_utilities/test_tableau_utilities.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.4/tableau_utilities.egg-info/PKG-INFO` & `tableau_utilities-2.0.5/tableau_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableau-utilities
-Version: 2.0.4
+Version: 2.0.5
 Summary: Utility for maintaining Tableau objects
 Home-page: http://pypi.python.org/pypi/tableau-utilities/
 Author: Justin Grilli
 Author-email: justin.grilli@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tableau_utilities-2.0.4/tableau_utilities.egg-info/SOURCES.txt` & `tableau_utilities-2.0.5/tableau_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

