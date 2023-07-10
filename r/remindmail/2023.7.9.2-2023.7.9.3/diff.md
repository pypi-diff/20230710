# Comparing `tmp/remindmail-2023.7.9.2.tar.gz` & `tmp/remindmail-2023.7.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remindmail-2023.7.9.2.tar", last modified: Mon Jul 10 04:26:06 2023, max compression
+gzip compressed data, was "remindmail-2023.7.9.3.tar", last modified: Mon Jul 10 04:27:26 2023, max compression
```

## Comparing `remindmail-2023.7.9.2.tar` & `remindmail-2023.7.9.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-10 04:26:06.457299 remindmail-2023.7.9.2/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1070 2022-10-19 22:48:49.000000 remindmail-2023.7.9.2/LICENSE.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    15502 2023-07-10 04:26:06.457299 remindmail-2023.7.9.2/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    15153 2023-06-22 04:24:04.000000 remindmail-2023.7.9.2/README.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2022-10-19 22:48:49.000000 remindmail-2023.7.9.2/pyproject.toml
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      751 2023-07-10 04:26:06.457299 remindmail-2023.7.9.2/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-10 04:26:06.457299 remindmail-2023.7.9.2/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-10 04:26:06.457299 remindmail-2023.7.9.2/src/remind/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2023-04-30 04:24:17.000000 remindmail-2023.7.9.2/src/remind/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     7621 2023-06-28 22:32:45.000000 remindmail-2023.7.9.2/src/remind/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2405 2023-04-30 04:24:17.000000 remindmail-2023.7.9.2/src/remind/reminder.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    26444 2023-07-10 04:21:17.000000 remindmail-2023.7.9.2/src/remind/remindmail.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    12881 2023-06-28 22:32:45.000000 remindmail-2023.7.9.2/src/remind/remindmail_utils.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6501 2023-06-22 04:24:04.000000 remindmail-2023.7.9.2/src/remind/trello_manager.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-10 04:26:06.457299 remindmail-2023.7.9.2/src/remindmail.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    15502 2023-07-10 04:26:06.000000 remindmail-2023.7.9.2/src/remindmail.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      392 2023-07-10 04:26:06.000000 remindmail-2023.7.9.2/src/remindmail.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-07-10 04:26:06.000000 remindmail-2023.7.9.2/src/remindmail.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2023-07-10 04:26:06.000000 remindmail-2023.7.9.2/src/remindmail.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2023-07-10 04:26:06.000000 remindmail-2023.7.9.2/src/remindmail.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-10 04:27:26.676341 remindmail-2023.7.9.3/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1070 2022-10-19 22:48:49.000000 remindmail-2023.7.9.3/LICENSE.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    15502 2023-07-10 04:27:26.676341 remindmail-2023.7.9.3/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    15153 2023-06-22 04:24:04.000000 remindmail-2023.7.9.3/README.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2022-10-19 22:48:49.000000 remindmail-2023.7.9.3/pyproject.toml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      751 2023-07-10 04:27:26.676341 remindmail-2023.7.9.3/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-10 04:27:26.676341 remindmail-2023.7.9.3/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-10 04:27:26.676341 remindmail-2023.7.9.3/src/remind/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2023-04-30 04:24:17.000000 remindmail-2023.7.9.3/src/remind/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     7621 2023-06-28 22:32:45.000000 remindmail-2023.7.9.3/src/remind/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2405 2023-04-30 04:24:17.000000 remindmail-2023.7.9.3/src/remind/reminder.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    26405 2023-07-10 04:27:04.000000 remindmail-2023.7.9.3/src/remind/remindmail.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    12881 2023-06-28 22:32:45.000000 remindmail-2023.7.9.3/src/remind/remindmail_utils.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6501 2023-06-22 04:24:04.000000 remindmail-2023.7.9.3/src/remind/trello_manager.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-10 04:27:26.676341 remindmail-2023.7.9.3/src/remindmail.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    15502 2023-07-10 04:27:26.000000 remindmail-2023.7.9.3/src/remindmail.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      392 2023-07-10 04:27:26.000000 remindmail-2023.7.9.3/src/remindmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-07-10 04:27:26.000000 remindmail-2023.7.9.3/src/remindmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2023-07-10 04:27:26.000000 remindmail-2023.7.9.3/src/remindmail.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2023-07-10 04:27:26.000000 remindmail-2023.7.9.3/src/remindmail.egg-info/top_level.txt
```

### Comparing `remindmail-2023.7.9.2/LICENSE.md` & `remindmail-2023.7.9.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `remindmail-2023.7.9.2/PKG-INFO` & `remindmail-2023.7.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2023.7.9.2
+Version: 2023.7.9.3
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `remindmail-2023.7.9.2/README.md` & `remindmail-2023.7.9.3/README.md`

 * *Files identical despite different names*

### Comparing `remindmail-2023.7.9.2/setup.cfg` & `remindmail-2023.7.9.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = remindmail
-version = 2023.07.09.2
+version = 2023.07.09.3
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily schedule reminders to be emailed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/remindmail
 project_urls =
```

### Comparing `remindmail-2023.7.9.2/src/remind/__main__.py` & `remindmail-2023.7.9.3/src/remind/__main__.py`

 * *Files identical despite different names*

### Comparing `remindmail-2023.7.9.2/src/remind/reminder.py` & `remindmail-2023.7.9.3/src/remind/reminder.py`

 * *Files identical despite different names*

### Comparing `remindmail-2023.7.9.2/src/remind/remindmail.py` & `remindmail-2023.7.9.3/src/remind/remindmail.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,15 +517,14 @@
                 query_time_formatted = parsed_date[0].strftime(
                     query_time_format)
 
             if manual_message:
                 query = manual_message
             else:
                 if len(parsed_date[1]) > 1:
-                    print(parsed_date)
                     query = ''.join(get_larger(
                         parsed_date[1][0], parsed_date[1][1]))
                     query = strip_to(''.join(query.rsplit(' on ', 1)) or query)
                 elif len(parsed_date) > 1:
                     parsed_date_formatted = strip_to(''.join(parsed_date[1]))
                     if parsed_date_formatted:
                         query = parsed_date_formatted
```

### Comparing `remindmail-2023.7.9.2/src/remind/remindmail_utils.py` & `remindmail-2023.7.9.3/src/remind/remindmail_utils.py`

 * *Files identical despite different names*

### Comparing `remindmail-2023.7.9.2/src/remind/trello_manager.py` & `remindmail-2023.7.9.3/src/remind/trello_manager.py`

 * *Files identical despite different names*

### Comparing `remindmail-2023.7.9.2/src/remindmail.egg-info/PKG-INFO` & `remindmail-2023.7.9.3/src/remindmail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2023.7.9.2
+Version: 2023.7.9.3
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

