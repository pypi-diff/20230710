# Comparing `tmp/tibis-1.0.9.tar.gz` & `tmp/tibis-1.0.9b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tibis-1.0.9.tar", max compression
+gzip compressed data, was "tibis-1.0.9b0.tar", max compression
```

## Comparing `tibis-1.0.9.tar` & `tibis-1.0.9b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1317 2022-05-04 07:11:06.352528 tibis-1.0.9/LICENSE
--rw-r--r--   0        0        0     3298 2023-03-07 15:28:13.653463 tibis-1.0.9/README.md
--rw-r--r--   0        0        0      517 2023-07-03 12:54:57.885545 tibis-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     1582 2023-06-26 08:37:09.179153 tibis-1.0.9/tibis/lib/args_parser.py
--rw-r--r--   0        0        0     7881 2023-07-03 12:44:33.559982 tibis-1.0.9/tibis/lib/common.py
--rw-r--r--   0        0        0      632 2023-07-03 12:42:59.349671 tibis-1.0.9/tibis/lib/config.py
--rw-r--r--   0        0        0     3028 2023-07-03 12:54:29.582039 tibis-1.0.9/tibis/lib/create.py
--rw-r--r--   0        0        0      940 2023-07-03 12:49:53.411034 tibis-1.0.9/tibis/lib/delete.py
--rw-r--r--   0        0        0     1267 2022-05-04 07:40:49.614937 tibis-1.0.9/tibis/lib/first_time.py
--rw-r--r--   0        0        0      562 2022-05-04 07:11:06.355861 tibis-1.0.9/tibis/lib/list.py
--rw-r--r--   0        0        0     1431 2023-06-05 07:02:14.055365 tibis-1.0.9/tibis/lib/lock.py
--rw-r--r--   0        0        0      540 2022-05-04 07:11:06.355861 tibis-1.0.9/tibis/lib/logger.py
--rw-r--r--   0        0        0     1203 2023-07-03 12:44:23.373282 tibis-1.0.9/tibis/lib/static.py
--rw-r--r--   0        0        0     1643 2023-03-07 09:14:53.679647 tibis-1.0.9/tibis/lib/unlock.py
--rw-r--r--   0        0        0      729 2022-05-04 07:28:38.614261 tibis-1.0.9/tibis/tibis.py
--rw-r--r--   0        0        0     4094 1970-01-01 00:00:00.000000 tibis-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1317 2022-05-04 07:11:06.352528 tibis-1.0.9b0/LICENSE
+-rw-r--r--   0        0        0     3298 2023-03-07 15:28:13.653463 tibis-1.0.9b0/README.md
+-rw-r--r--   0        0        0      518 2023-07-10 08:50:37.483493 tibis-1.0.9b0/pyproject.toml
+-rw-r--r--   0        0        0     1582 2023-06-26 08:37:09.179153 tibis-1.0.9b0/tibis/lib/args_parser.py
+-rw-r--r--   0        0        0     7881 2023-07-03 12:44:33.559982 tibis-1.0.9b0/tibis/lib/common.py
+-rw-r--r--   0        0        0      632 2023-07-03 12:42:59.349671 tibis-1.0.9b0/tibis/lib/config.py
+-rw-r--r--   0        0        0     3028 2023-07-03 13:25:44.310044 tibis-1.0.9b0/tibis/lib/create.py
+-rw-r--r--   0        0        0      932 2023-07-10 08:50:03.645574 tibis-1.0.9b0/tibis/lib/delete.py
+-rw-r--r--   0        0        0     1267 2022-05-04 07:40:49.614937 tibis-1.0.9b0/tibis/lib/first_time.py
+-rw-r--r--   0        0        0      562 2022-05-04 07:11:06.355861 tibis-1.0.9b0/tibis/lib/list.py
+-rw-r--r--   0        0        0     1431 2023-06-05 07:02:14.055365 tibis-1.0.9b0/tibis/lib/lock.py
+-rw-r--r--   0        0        0      540 2022-05-04 07:11:06.355861 tibis-1.0.9b0/tibis/lib/logger.py
+-rw-r--r--   0        0        0     1203 2023-07-03 12:44:23.373282 tibis-1.0.9b0/tibis/lib/static.py
+-rw-r--r--   0        0        0     1643 2023-03-07 09:14:53.679647 tibis-1.0.9b0/tibis/lib/unlock.py
+-rw-r--r--   0        0        0      729 2022-05-04 07:28:38.614261 tibis-1.0.9b0/tibis/tibis.py
+-rw-r--r--   0        0        0     4096 1970-01-01 00:00:00.000000 tibis-1.0.9b0/PKG-INFO
```

### Comparing `tibis-1.0.9/LICENSE` & `tibis-1.0.9b0/LICENSE`

 * *Files identical despite different names*

### Comparing `tibis-1.0.9/README.md` & `tibis-1.0.9b0/README.md`

 * *Files identical despite different names*

### Comparing `tibis-1.0.9/pyproject.toml` & `tibis-1.0.9b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tibis"
-version = "1.0.9"
+version = "1.0.9b"
 description = "Tibis is a secure storage manager"
 authors = ["shoxxdj <shoxx@shoxxdj.fr>"]
 readme = "README.md"
 homepage = "https://github.com/shoxxdj/tibis"
 
 [tool.poetry.dependencies]
 python = ">=3.6"
```

### Comparing `tibis-1.0.9/tibis/lib/args_parser.py` & `tibis-1.0.9b0/tibis/lib/args_parser.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.9/tibis/lib/common.py` & `tibis-1.0.9b0/tibis/lib/common.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.9/tibis/lib/config.py` & `tibis-1.0.9b0/tibis/lib/config.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.9/tibis/lib/create.py` & `tibis-1.0.9b0/tibis/lib/create.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.9/tibis/lib/delete.py` & `tibis-1.0.9b0/tibis/lib/delete.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,18 @@
    while answer not in ["y", "n"]:
     answer = input(chalk.red.bold("OK to push to continue [Y/N]? ")).lower()
    if(answer=="y"):
     #On vire la data  du storage
     if(common.isUnlocked(dirname)):
       mp=common.getMountPoint(dirname)
       log.warning("Your content was previously unlocked at "+ str(mp) +" you have to delete it by yourself")
-      try:
-       common.remove_dir(static.tibis_keys_location+"/"+dirname)
-      except:
-       log.warning("Keys are already gone")
+    try:
+      common.remove_dir(static.tibis_keys_location+"/"+dirname)
       common.deleteSQLEntry(dirname)
-      log.warning("Entry and keys removed")
+    except:
+     log.warning("Keys are already gone")
+     log.warning("Entry and keys removed")
    else:
     log.success("Leaves the things as it ...")     
 
 if __name__ == '__main__':
   deleteSQLEntry(dirname)
```

### Comparing `tibis-1.0.9/tibis/lib/first_time.py` & `tibis-1.0.9b0/tibis/lib/first_time.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.9/tibis/lib/list.py` & `tibis-1.0.9b0/tibis/lib/list.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.9/tibis/lib/lock.py` & `tibis-1.0.9b0/tibis/lib/lock.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.9/tibis/lib/logger.py` & `tibis-1.0.9b0/tibis/lib/logger.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.9/tibis/lib/static.py` & `tibis-1.0.9b0/tibis/lib/static.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.9/tibis/lib/unlock.py` & `tibis-1.0.9b0/tibis/lib/unlock.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.9/tibis/tibis.py` & `tibis-1.0.9b0/tibis/tibis.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.9/PKG-INFO` & `tibis-1.0.9b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tibis
-Version: 1.0.9
+Version: 1.0.9b0
 Summary: Tibis is a secure storage manager
 Home-page: https://github.com/shoxxdj/tibis
 Author: shoxxdj
 Author-email: shoxx@shoxxdj.fr
 Requires-Python: >=3.6
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

