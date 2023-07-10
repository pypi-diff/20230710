# Comparing `tmp/rin_proj1-1.0.tar.gz` & `tmp/rin_proj1-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rin_proj1-1.0.tar", max compression
+gzip compressed data, was "rin_proj1-1.1.tar", max compression
```

## Comparing `rin_proj1-1.0.tar` & `rin_proj1-1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1764 2023-07-07 19:54:15.068469 rin_proj1-1.0/README.md
--rw-r--r--   0        0        0      403 2023-07-07 20:07:03.822864 rin_proj1-1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-04 16:49:14.718478 rin_proj1-1.0/rin_proj1/__init__.py
--rw-r--r--   0        0        0     1214 2023-07-05 11:43:12.438622 rin_proj1-1.0/rin_proj1/db_insert.py
--rw-r--r--   0        0        0      311 2023-07-07 19:40:41.269360 rin_proj1-1.0/rin_proj1/get_yaml.py
--rw-r--r--   0        0        0     1817 2023-07-07 19:52:15.242093 rin_proj1-1.0/rin_proj1/logerror.py
--rw-r--r--   0        0        0     1965 2023-07-07 19:50:32.419534 rin_proj1-1.0/rin_proj1/main.py
--rw-r--r--   0        0        0     2224 1970-01-01 00:00:00.000000 rin_proj1-1.0/PKG-INFO
+-rw-r--r--   0        0        0     1836 2023-07-10 07:16:57.819910 rin_proj1-1.1/README.md
+-rw-r--r--   0        0        0      406 2023-07-10 07:12:55.002078 rin_proj1-1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-04 16:49:14.718478 rin_proj1-1.1/rin_proj1/__init__.py
+-rw-r--r--   0        0        0     1214 2023-07-05 11:43:12.438622 rin_proj1-1.1/rin_proj1/db_insert.py
+-rw-r--r--   0        0        0      311 2023-07-07 19:40:41.269360 rin_proj1-1.1/rin_proj1/get_yaml.py
+-rw-r--r--   0        0        0     1870 2023-07-10 07:17:54.202478 rin_proj1-1.1/rin_proj1/logerror.py
+-rw-r--r--   0        0        0     1965 2023-07-07 19:50:32.419534 rin_proj1-1.1/rin_proj1/main.py
+-rw-r--r--   0        0        0     2299 1970-01-01 00:00:00.000000 rin_proj1-1.1/PKG-INFO
```

### Comparing `rin_proj1-1.0/README.md` & `rin_proj1-1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 <h1> command usage (CLI) </h1>
 See list of commands with
 
 ```
 rin_proj1 --help
 ```
-Error logging is only compatible with `exec-based-on-env`<br>
+
+<b style="color:red">Error logging is only compatible with `exec-based-on-env`</b><br><br>
 <b>read_csv_and_insert_to_db :</b> Adds contents of provided csv to a .db file<br>
 <b>export_db_to_csv :</b> Adds contents of provided db to a .csv file
+
 <h2>set-config</h2>
 Executes read_csv_and_insert_to_db and export_db_to_csv functions with the given config file.
 If no path is provided, tries to open config.yaml in the current directory.<br>
 
 ```commandline
  rin_proj1 set-config --path path/to/config.yaml
 ```
-for default/config in current directory, use ```main1```
+
+for default/config in current directory, use ```rin_proj1 set-config```
 
 <hr>
 <h2>set-db</h2>
 Executes read_csv_and_insert_to_db and export_db_to_csv functions with the db_name provided by user.<br>
 
 ```rin_proj1 set-db``` saves data.db in current directory<br>
 ```rin_proj1 set-db db_name``` saves to db_name in current directory. Will create a file if not present<br>
@@ -26,37 +29,40 @@
 <hr>
 <h2>exec-based-on-env</h2>
 Executes read_csv_and_insert_to_db and export_db_to_csv functions with csv file depending on the environment type<br>
 
 ```bash
 rin_proj1 exec-based-on-env
 ```
-If you want to run the command in a different environment,
+
+If you want to run the command in a different environment, open/spawn the shell where command is to be run:
+
 ```bash
-poetry shell
 export APP_MODE=env_name
 rin_proj1 exec-based-on-env
 ```
+
 > <b>env_name options:</b>
-    development,
-    testing,
-    production
+> development,
+> testing,
+> production
 
 <hr>
 
 Successful execution should print confirmation message in terminal. If there is no output, check for a `mpj1_error.log` file to determine the error.<br><br>
 Expected yaml file layout (minimum):
 
 ```yaml
 LOG_LEVEL: log_level (see below for valid options)
 
-APP_MODE:
+env_name:
   csv_file: path/to/data.csv
   db_file: path/to/data.db
   table_file: your_table_name
 ```
+
 > <b>log_level options:</b>
-    critical,
-    error,
-    warning,
-    info,
-    debug
+> critical,
+> error,
+> warning,
+> info,
+> debug
```

### Comparing `rin_proj1-1.0/rin_proj1/db_insert.py` & `rin_proj1-1.1/rin_proj1/db_insert.py`

 * *Files identical despite different names*

### Comparing `rin_proj1-1.0/rin_proj1/logerror.py` & `rin_proj1-1.1/rin_proj1/logerror.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     elif isinstance(e, AttributeError):
         logging.error("config.yaml can't be read. Is the config file empty?")
     elif isinstance(e, KeyError):
         logging.error(f"KEY {e.args[0]} doesn't exist. Check config file")
     elif isinstance(e, TypeError):
         logging.error("Check values in csv/db file. TypeError encountered.")
     else:
-        logging.error(f"Encountered error with message {e}")
+        logging.error(f"Encountered error with message: {e}")
 
 
 def log_error(func) -> Callable[[...], None]:
     @wraps(func)
     def wrapper(*args, **kwargs) -> None:
         try:
             log_lvl = get_yaml("config.yaml").get("LOG_LEVEL", "")
@@ -43,11 +43,11 @@
             return
 
         try:
             logging.basicConfig(filename='mpj1_error.log', format='%(asctime)s - %(message)s',
                                 encoding='utf-8', level=log_map[log_lvl])
             func(*args, **kwargs)
         except Exception as e:
-            print(e)
+            print("Ended abruptly. Check mpj1_error.log for more info.")
             error_branch(e)
             return
     return wrapper
```

### Comparing `rin_proj1-1.0/rin_proj1/main.py` & `rin_proj1-1.1/rin_proj1/main.py`

 * *Files identical despite different names*

### Comparing `rin_proj1-1.0/PKG-INFO` & `rin_proj1-1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: rin-proj1
-Version: 1.0
-Summary: CLI tool convert .csv files to .db files and vice-versa
+Version: 1.1
+Summary: CLI tool to convert .csv files to .db files and vice-versa
 Author: Harine
 Author-email: haariinee@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyyaml (>=6.0,<7.0)
@@ -14,25 +14,28 @@
 
 <h1> command usage (CLI) </h1>
 See list of commands with
 
 ```
 rin_proj1 --help
 ```
-Error logging is only compatible with `exec-based-on-env`<br>
+
+<b style="color:red">Error logging is only compatible with `exec-based-on-env`</b><br><br>
 <b>read_csv_and_insert_to_db :</b> Adds contents of provided csv to a .db file<br>
 <b>export_db_to_csv :</b> Adds contents of provided db to a .csv file
+
 <h2>set-config</h2>
 Executes read_csv_and_insert_to_db and export_db_to_csv functions with the given config file.
 If no path is provided, tries to open config.yaml in the current directory.<br>
 
 ```commandline
  rin_proj1 set-config --path path/to/config.yaml
 ```
-for default/config in current directory, use ```main1```
+
+for default/config in current directory, use ```rin_proj1 set-config```
 
 <hr>
 <h2>set-db</h2>
 Executes read_csv_and_insert_to_db and export_db_to_csv functions with the db_name provided by user.<br>
 
 ```rin_proj1 set-db``` saves data.db in current directory<br>
 ```rin_proj1 set-db db_name``` saves to db_name in current directory. Will create a file if not present<br>
@@ -40,37 +43,41 @@
 <hr>
 <h2>exec-based-on-env</h2>
 Executes read_csv_and_insert_to_db and export_db_to_csv functions with csv file depending on the environment type<br>
 
 ```bash
 rin_proj1 exec-based-on-env
 ```
-If you want to run the command in a different environment,
+
+If you want to run the command in a different environment, open/spawn the shell where command is to be run:
+
 ```bash
-poetry shell
 export APP_MODE=env_name
 rin_proj1 exec-based-on-env
 ```
+
 > <b>env_name options:</b>
-    development,
-    testing,
-    production
+> development,
+> testing,
+> production
 
 <hr>
 
 Successful execution should print confirmation message in terminal. If there is no output, check for a `mpj1_error.log` file to determine the error.<br><br>
 Expected yaml file layout (minimum):
 
 ```yaml
 LOG_LEVEL: log_level (see below for valid options)
 
-APP_MODE:
+env_name:
   csv_file: path/to/data.csv
   db_file: path/to/data.db
   table_file: your_table_name
 ```
+
 > <b>log_level options:</b>
-    critical,
-    error,
-    warning,
-    info,
-    debug
+> critical,
+> error,
+> warning,
+> info,
+> debug
+
```

