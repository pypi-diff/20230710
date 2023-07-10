# Comparing `tmp/rsxml-2.0.1.tar.gz` & `tmp/rsxml-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsxml-2.0.1.tar", last modified: Thu Jul  6 17:32:17 2023, max compression
+gzip compressed data, was "rsxml-2.0.2.tar", last modified: Mon Jul 10 19:32:25 2023, max compression
```

## Comparing `rsxml-2.0.1.tar` & `rsxml-2.0.2.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-06 17:32:17.296512 rsxml-2.0.1/
--rw-r--r--   0 matt       (501) staff       (20)     1072 2023-07-05 23:12:54.000000 rsxml-2.0.1/LICENSE
--rw-r--r--   0 matt       (501) staff       (20)     7076 2023-07-06 17:32:17.296594 rsxml-2.0.1/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)     6578 2023-07-05 23:39:56.000000 rsxml-2.0.1/README.md
--rw-r--r--   0 matt       (501) staff       (20)      864 2023-07-05 23:36:34.000000 rsxml-2.0.1/pyproject.toml
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-06 17:32:17.290009 rsxml-2.0.1/rsxml/
--rw-r--r--   0 matt       (501) staff       (20)      385 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)       22 2023-07-06 17:31:48.000000 rsxml-2.0.1/rsxml/__version__.py
--rw-r--r--   0 matt       (501) staff       (20)    13856 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/api.py
--rw-r--r--   0 matt       (501) staff       (20)      151 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/constants.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-06 17:32:17.291997 rsxml-2.0.1/rsxml/debug/
--rw-r--r--   0 matt       (501) staff       (20)      102 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/debug/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)     7973 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/debug/debug_proc.py
--rw-r--r--   0 matt       (501) staff       (20)     3120 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/debug/loop_timer.py
--rw-r--r--   0 matt       (501) staff       (20)     1906 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/debug/timer.py
--rw-r--r--   0 matt       (501) staff       (20)     8508 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/debug/timer_buckets.py
--rw-r--r--   0 matt       (501) staff       (20)     3081 2023-07-06 15:41:36.000000 rsxml-2.0.1/rsxml/dotenv.py
--rw-r--r--   0 matt       (501) staff       (20)     1741 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/etag.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-06 17:32:17.292468 rsxml-2.0.1/rsxml/logging/
--rw-r--r--   0 matt       (501) staff       (20)        0 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/logging/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)     8209 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/logging/logger.py
--rw-r--r--   0 matt       (501) staff       (20)     3716 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/logging/progress_bar.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-06 17:32:17.294700 rsxml-2.0.1/rsxml/project_xml/
--rw-r--r--   0 matt       (501) staff       (20)     3135 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/project_xml/Analysis.py
--rw-r--r--   0 matt       (501) staff       (20)    15552 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/project_xml/Dataset.py
--rw-r--r--   0 matt       (501) staff       (20)     5988 2023-07-06 16:53:46.000000 rsxml-2.0.1/rsxml/project_xml/MetaData.py
--rw-r--r--   0 matt       (501) staff       (20)     9850 2023-07-06 16:32:25.000000 rsxml-2.0.1/rsxml/project_xml/Project.py
--rw-r--r--   0 matt       (501) staff       (20)     3712 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/project_xml/ProjectBounds.py
--rw-r--r--   0 matt       (501) staff       (20)     3455 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/project_xml/QAQCEvent.py
--rw-r--r--   0 matt       (501) staff       (20)     5518 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/project_xml/RSObj.py
--rw-r--r--   0 matt       (501) staff       (20)     3091 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/project_xml/Realization.py
--rw-r--r--   0 matt       (501) staff       (20)      236 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/project_xml/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)      463 2023-07-06 17:31:21.000000 rsxml-2.0.1/rsxml/project_xml/common.py
--rw-r--r--   0 matt       (501) staff       (20)      766 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/rspaths.py
--rw-r--r--   0 matt       (501) staff       (20)     7339 2023-07-06 15:22:35.000000 rsxml-2.0.1/rsxml/util.py
--rw-r--r--   0 matt       (501) staff       (20)     1999 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/validation.py
--rw-r--r--   0 matt       (501) staff       (20)      371 2023-07-05 23:12:54.000000 rsxml-2.0.1/rsxml/xml.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-06 17:32:17.291022 rsxml-2.0.1/rsxml.egg-info/
--rw-r--r--   0 matt       (501) staff       (20)     7076 2023-07-06 17:32:17.000000 rsxml-2.0.1/rsxml.egg-info/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)     1050 2023-07-06 17:32:17.000000 rsxml-2.0.1/rsxml.egg-info/SOURCES.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2023-07-06 17:32:17.000000 rsxml-2.0.1/rsxml.egg-info/dependency_links.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2023-05-23 16:11:44.000000 rsxml-2.0.1/rsxml.egg-info/not-zip-safe
--rw-r--r--   0 matt       (501) staff       (20)       59 2023-07-06 17:32:17.000000 rsxml-2.0.1/rsxml.egg-info/requires.txt
--rw-r--r--   0 matt       (501) staff       (20)        6 2023-07-06 17:32:17.000000 rsxml-2.0.1/rsxml.egg-info/top_level.txt
--rw-r--r--   0 matt       (501) staff       (20)       79 2023-07-06 17:32:17.296833 rsxml-2.0.1/setup.cfg
--rw-r--r--   0 matt       (501) staff       (20)     1257 2023-07-06 15:45:55.000000 rsxml-2.0.1/setup.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-06 17:32:17.296234 rsxml-2.0.1/tests/
--rw-r--r--   0 matt       (501) staff       (20)     2302 2023-07-05 23:12:54.000000 rsxml-2.0.1/tests/test_dotenv.py
--rw-r--r--   0 matt       (501) staff       (20)     1131 2023-07-05 23:12:54.000000 rsxml-2.0.1/tests/test_etags.py
--rw-r--r--   0 matt       (501) staff       (20)      679 2023-07-05 23:12:54.000000 rsxml-2.0.1/tests/test_load_samples.py
--rw-r--r--   0 matt       (501) staff       (20)     1327 2023-07-05 23:12:54.000000 rsxml-2.0.1/tests/test_paths.py
--rw-r--r--   0 matt       (501) staff       (20)     8861 2023-07-06 17:31:31.000000 rsxml-2.0.1/tests/test_project_xml.py
--rw-r--r--   0 matt       (501) staff       (20)     7503 2023-07-05 23:12:54.000000 rsxml-2.0.1/tests/test_timers.py
--rw-r--r--   0 matt       (501) staff       (20)     3204 2023-07-05 23:27:33.000000 rsxml-2.0.1/tests/test_util.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-10 19:32:25.555820 rsxml-2.0.2/
+-rw-r--r--   0 matt       (501) staff       (20)     1072 2023-07-05 23:12:54.000000 rsxml-2.0.2/LICENSE
+-rw-r--r--   0 matt       (501) staff       (20)     7076 2023-07-10 19:32:25.555911 rsxml-2.0.2/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)     6578 2023-07-05 23:39:56.000000 rsxml-2.0.2/README.md
+-rw-r--r--   0 matt       (501) staff       (20)      864 2023-07-05 23:36:34.000000 rsxml-2.0.2/pyproject.toml
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-10 19:32:25.547584 rsxml-2.0.2/rsxml/
+-rw-r--r--   0 matt       (501) staff       (20)      385 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)       22 2023-07-10 19:31:56.000000 rsxml-2.0.2/rsxml/__version__.py
+-rw-r--r--   0 matt       (501) staff       (20)    13856 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/api.py
+-rw-r--r--   0 matt       (501) staff       (20)      151 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/constants.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-10 19:32:25.550208 rsxml-2.0.2/rsxml/debug/
+-rw-r--r--   0 matt       (501) staff       (20)      102 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/debug/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)     8354 2023-07-07 15:26:31.000000 rsxml-2.0.2/rsxml/debug/debug_proc.py
+-rw-r--r--   0 matt       (501) staff       (20)     3120 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/debug/loop_timer.py
+-rw-r--r--   0 matt       (501) staff       (20)     1906 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/debug/timer.py
+-rw-r--r--   0 matt       (501) staff       (20)     8508 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/debug/timer_buckets.py
+-rw-r--r--   0 matt       (501) staff       (20)     3081 2023-07-06 15:41:36.000000 rsxml-2.0.2/rsxml/dotenv.py
+-rw-r--r--   0 matt       (501) staff       (20)     1741 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/etag.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-10 19:32:25.550791 rsxml-2.0.2/rsxml/logging/
+-rw-r--r--   0 matt       (501) staff       (20)        0 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/logging/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)     9170 2023-07-07 16:12:54.000000 rsxml-2.0.2/rsxml/logging/logger.py
+-rw-r--r--   0 matt       (501) staff       (20)     3716 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/logging/progress_bar.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-10 19:32:25.553953 rsxml-2.0.2/rsxml/project_xml/
+-rw-r--r--   0 matt       (501) staff       (20)     3871 2023-07-10 16:15:20.000000 rsxml-2.0.2/rsxml/project_xml/Analysis.py
+-rw-r--r--   0 matt       (501) staff       (20)     9317 2023-07-10 19:19:25.000000 rsxml-2.0.2/rsxml/project_xml/Dataset.py
+-rw-r--r--   0 matt       (501) staff       (20)     9370 2023-07-10 19:18:19.000000 rsxml-2.0.2/rsxml/project_xml/Geopackage.py
+-rw-r--r--   0 matt       (501) staff       (20)     6502 2023-07-10 15:33:03.000000 rsxml-2.0.2/rsxml/project_xml/MetaData.py
+-rw-r--r--   0 matt       (501) staff       (20)    10537 2023-07-10 18:51:44.000000 rsxml-2.0.2/rsxml/project_xml/Project.py
+-rw-r--r--   0 matt       (501) staff       (20)     3712 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/project_xml/ProjectBounds.py
+-rw-r--r--   0 matt       (501) staff       (20)     3462 2023-07-07 18:42:13.000000 rsxml-2.0.2/rsxml/project_xml/ProjectValidation.py
+-rw-r--r--   0 matt       (501) staff       (20)     3852 2023-07-10 15:40:00.000000 rsxml-2.0.2/rsxml/project_xml/QAQCEvent.py
+-rw-r--r--   0 matt       (501) staff       (20)     6170 2023-07-10 15:36:29.000000 rsxml-2.0.2/rsxml/project_xml/RSObj.py
+-rw-r--r--   0 matt       (501) staff       (20)     7317 2023-07-10 19:14:21.000000 rsxml-2.0.2/rsxml/project_xml/Realization.py
+-rw-r--r--   0 matt       (501) staff       (20)     1174 2023-07-10 18:52:07.000000 rsxml-2.0.2/rsxml/project_xml/Warehouse.py
+-rw-r--r--   0 matt       (501) staff       (20)      320 2023-07-10 18:40:08.000000 rsxml-2.0.2/rsxml/project_xml/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)      421 2023-07-10 16:10:03.000000 rsxml-2.0.2/rsxml/project_xml/common.py
+-rw-r--r--   0 matt       (501) staff       (20)     1329 2023-07-07 19:16:00.000000 rsxml-2.0.2/rsxml/rspaths.py
+-rw-r--r--   0 matt       (501) staff       (20)     7339 2023-07-06 15:22:35.000000 rsxml-2.0.2/rsxml/util.py
+-rw-r--r--   0 matt       (501) staff       (20)     2059 2023-07-07 18:19:48.000000 rsxml-2.0.2/rsxml/validation.py
+-rw-r--r--   0 matt       (501) staff       (20)      371 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/xml.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-10 19:32:25.548956 rsxml-2.0.2/rsxml.egg-info/
+-rw-r--r--   0 matt       (501) staff       (20)     7076 2023-07-10 19:32:25.000000 rsxml-2.0.2/rsxml.egg-info/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)     1152 2023-07-10 19:32:25.000000 rsxml-2.0.2/rsxml.egg-info/SOURCES.txt
+-rw-r--r--   0 matt       (501) staff       (20)        1 2023-07-10 19:32:25.000000 rsxml-2.0.2/rsxml.egg-info/dependency_links.txt
+-rw-r--r--   0 matt       (501) staff       (20)        1 2023-05-23 16:11:44.000000 rsxml-2.0.2/rsxml.egg-info/not-zip-safe
+-rw-r--r--   0 matt       (501) staff       (20)       59 2023-07-10 19:32:25.000000 rsxml-2.0.2/rsxml.egg-info/requires.txt
+-rw-r--r--   0 matt       (501) staff       (20)        6 2023-07-10 19:32:25.000000 rsxml-2.0.2/rsxml.egg-info/top_level.txt
+-rw-r--r--   0 matt       (501) staff       (20)       79 2023-07-10 19:32:25.556175 rsxml-2.0.2/setup.cfg
+-rw-r--r--   0 matt       (501) staff       (20)     1257 2023-07-06 15:45:55.000000 rsxml-2.0.2/setup.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-10 19:32:25.555568 rsxml-2.0.2/tests/
+-rw-r--r--   0 matt       (501) staff       (20)     2302 2023-07-05 23:12:54.000000 rsxml-2.0.2/tests/test_dotenv.py
+-rw-r--r--   0 matt       (501) staff       (20)     1131 2023-07-05 23:12:54.000000 rsxml-2.0.2/tests/test_etags.py
+-rw-r--r--   0 matt       (501) staff       (20)     1837 2023-07-10 16:11:30.000000 rsxml-2.0.2/tests/test_load_samples.py
+-rw-r--r--   0 matt       (501) staff       (20)     2952 2023-07-07 19:18:01.000000 rsxml-2.0.2/tests/test_paths.py
+-rw-r--r--   0 matt       (501) staff       (20)    15389 2023-07-07 22:57:09.000000 rsxml-2.0.2/tests/test_project_xml.py
+-rw-r--r--   0 matt       (501) staff       (20)     7503 2023-07-05 23:12:54.000000 rsxml-2.0.2/tests/test_timers.py
+-rw-r--r--   0 matt       (501) staff       (20)     3204 2023-07-05 23:27:33.000000 rsxml-2.0.2/tests/test_util.py
```

### Comparing `rsxml-2.0.1/LICENSE` & `rsxml-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.1/PKG-INFO` & `rsxml-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsxml
-Version: 2.0.1
+Version: 2.0.2
 Summary: Riverscapes XML helpers for use across Python3 open-source GIS Stack
 Home-page: https://github.com/Riverscapes/RiverscapesXML
 Author: Matt Reimer
 Author-email: info@northarrowresearch.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rsxml-2.0.1/README.md` & `rsxml-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.1/pyproject.toml` & `rsxml-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.1/rsxml/api.py` & `rsxml-2.0.2/rsxml/api.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.1/rsxml/debug/debug_proc.py` & `rsxml-2.0.2/rsxml/debug/debug_proc.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         """_summary_
 
         Args:
             imgpath (str): _description_
         """
         log = Logger('write_plot')
         if not plt:
-            log.error('You need Matplotlib to run write_plot')
+            log.warning('No plot written. You need Matplotlib to run write_plot.')
             return
         x = []
         data = {}
         with open(self.filepath, encoding='utf8') as csvfile:
             reader = csv.DictReader(csvfile)
             for row in reader:
                 for key in row.keys():
@@ -215,17 +215,19 @@
         callback (function): _description_
         memlogfile (str): _description_
 
     Returns:
         _type_: _description_
     """
     log = Logger('Debug')
+    log.setlevel('DEBUG')
+    log.debug('Starting thread_run')
     if not psutil:
         log.error('You need "psutil" to run the debug tools')
-        return
+        raise Exception('Missing psutil')
 
     memmon = MemoryMonitor(memlogfile, 1)
     result = None
     max_obj = None
     try:
         with ThreadPoolExecutor() as executor:
             mem_thread = executor.submit(memmon.measure_usage)
@@ -237,14 +239,19 @@
             finally:
                 memmon.keep_measuring = False
                 max_obj = mem_thread.result()
                 log.debug(f'MaxStats: {max_obj}')
     except Exception as err_out:
         # Make sure we always return so that we don't have to debug our debugger
         log.error(err_out)
+    log.debug(f'Resource plot CSV written to {memlogfile}')
     try:
-        memmon.write_plot(os.path.splitext(memlogfile)[0] + '.png')
+        if plt:
+            memmon.write_plot(os.path.splitext(memlogfile)[0] + '.png')
+            log.debug(f'Resource plot written to {os.path.splitext(memlogfile)[0] + ".png"}')
+        else:
+            log.warning('No plot written. You need Matplotlib to run write_plot.')
     except Exception as err:
         log.error(f'Error Writing memory plot: {err}')
 
     ret_val = max_obj.toString() if max_obj is not None else "process no longer exists"
     return result, ret_val
```

### Comparing `rsxml-2.0.1/rsxml/debug/loop_timer.py` & `rsxml-2.0.2/rsxml/debug/loop_timer.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.1/rsxml/debug/timer.py` & `rsxml-2.0.2/rsxml/debug/timer.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.1/rsxml/debug/timer_buckets.py` & `rsxml-2.0.2/rsxml/debug/timer_buckets.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.1/rsxml/dotenv.py` & `rsxml-2.0.2/rsxml/dotenv.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.1/rsxml/etag.py` & `rsxml-2.0.2/rsxml/etag.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.1/rsxml/logging/logger.py` & `rsxml-2.0.2/rsxml/logging/logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,29 +32,31 @@
 
         def __init__(self):
             self.initialized = False
             self.verbose = False
             self.logpath = None
             self.handler = None
             self.logger = logging.getLogger("LOGGER")
+            logging.addLevelName(25, 'TITLE')
+            self.loglevels = logging.getLevelNamesMapping()
 
-        def setup(self, log_path=None, verbose=False, log_level: str = None):
+        def setup(self, log_path=None, verbose=False, log_level: int = None):
             """_summary_
 
             Args:
                 logPath (_type_, optional): _description_. Defaults to None.
                 verbose (bool, optional): _description_. Defaults to False.
             """
             self.initialized = True
-            self.verbose = verbose
 
             if verbose is True and log_level is not None:
                 raise ValueError("Cannot set both verbose and log_level")
 
-            loglevel = logging.INFO if not verbose else logging.DEBUG
+            self.verbose = verbose if verbose else log_level >= logging.DEBUG
+            loglevel = log_level if log_level else logging.INFO if not verbose else logging.DEBUG
 
             self.logger = logging.getLogger("LOGGER")
             self.logger.setLevel(loglevel)
 
             # Make sure we capture osgeo warnigns if we need to
             osgeo_logger = logging.getLogger("osgeo")
             osgeo_logger.setLevel(logging.WARNING)
@@ -72,74 +74,77 @@
                 self.handler.setFormatter(logging.Formatter('%(asctime)s %(levelname)-8s [%(curmethod)-15s] %(message)s'))
                 self.handler.datefmt = '%Y-%m-%d %H:%M:%S'
 
                 self.logger.addHandler(self.handler)
 
                 osgeo_logger.addHandler(self.handler)
 
-        def logprint(self, message, method="", severity="info", exception=None):
+        def logprint(self, message, method="", severity="INFO", exception=None):
             """
             Logprint logs things 3 different ways: 1) stdout 2) log txt file 3) xml
             :param message:
             :param method:
             :param severity:
             :param exception:
             :return:
             """
+            msg_log_level = self.loglevels[severity.upper()]
 
-            # Verbose logs don't get written until we ask for them
-            if severity == 'debug' and not self.verbose:
+            # If we're not verbose and the log level is less than info then don't print
+            if msg_log_level < self.logger.level:
                 return
 
             # dateStr = datetime.datetime.now().strftime('%Y-%m-%dT%H:%M:%S%z')
             msg_arr = []
             if exception is not None:
                 txtmsg = f'{message}  Exception: {str(exception)}'
                 msg = f'[{severity}] [{method}] {message} : {str(exception)}'
-            elif severity == 'title':
+            elif msg_log_level == self.loglevels['TITLE']:
                 buffer = 15
                 buffer_str = buffer * ' '
                 spcrbar = (len(message) + (buffer * 2)) * '='
                 msg_arr = [
                     spcrbar, f'{buffer_str}{message}{buffer_str}', spcrbar, ' '
                 ]
-                msg = '\n'.join([f'[info] [{method}] {m}' for m in msg_arr])
+                msg = '\n'.join([f'[INFO] [{method}] {m}' for m in msg_arr])
             else:
                 txtmsg = message
                 msg = f'[{severity}] [{method}] {message}'
 
             # Print to stdout
             if not NO_UI or colored is None:
-                if severity == 'debug':
+                if msg_log_level == self.loglevels['DEBUG']:
                     msg = colored(msg, 'cyan')
-                if severity == 'warning':
+                if msg_log_level == self.loglevels['WARNING']:
                     msg = colored(msg, 'yellow')
-                if severity == 'error':
+                if msg_log_level == self.loglevels['ERROR']:
                     msg = colored(msg, 'red')
-                if severity == 'title':
+                if msg_log_level == self.loglevels['CRITICAL']:
+                    msg = colored(msg, 'red', attrs=['bold', 'reverse'])
+                if msg_log_level == self.loglevels['TITLE']:
                     msg = colored(msg, 'magenta')
 
             print(msg)
 
-            # If we haven't set up a logger then we're done here. Don't write to any files
+            # If we haven't set up a log file then we're done here. Don't write to any files
             if not self.initialized:
                 return
 
             # Write to log file
-            if severity == 'info':
+            if msg_log_level == self.loglevels['INFO']:
                 self.logger.info(txtmsg, extra={'curmethod': method})
-            elif severity == 'warning':
+            elif msg_log_level == self.loglevels['WARNING']:
                 self.logger.warning(txtmsg, extra={'curmethod': method})
-            elif severity == 'error':
+            elif msg_log_level == self.loglevels['ERROR']:
                 self.logger.error(txtmsg, extra={'curmethod': method})
-            elif severity == 'critical':
+            elif msg_log_level == self.loglevels['CRITICAL']:
                 self.logger.critical(txtmsg, extra={'curmethod': method})
-            elif severity == 'debug':
+            elif msg_log_level == self.loglevels['DEBUG']:
                 self.logger.debug(txtmsg, extra={'curmethod': method})
-            elif severity == 'title':
+            elif msg_log_level == self.loglevels['TITLE']:
                 for msg_it in msg_arr:
                     self.logger.info(msg_it, extra={'curmethod': method})
 
     def __init__(self, **kwargs):
         if not _LoggerSingleton.instance:
             _LoggerSingleton.instance = _LoggerSingleton.__Logger(**kwargs)
 
@@ -184,71 +189,79 @@
     def setlevel(self, log_level: str):
         """Set the level of the logger
 
         Args:
             level (_type_): _description_
         """
         self.instance.logger.setLevel(logging.getLevelName(log_level))
+        if self.instance.handler is not None:
+            self.instance.handler.setLevel(logging.getLevelName(log_level))
 
-    def debug(self, *args):
+    def debug(self, *args, **kwargs):
         """
         This works a little differently. You can basically throw anything you want into it.
         :param message:
         :return:
         """
         msgarr = []
         for arg in args:
             if isinstance(arg, str):
                 msgarr.append(arg)
             else:
                 msgarr.append(pformat(arg))
+        for key, value in kwargs.items():
+            if isinstance(value, str):
+                msgarr.append(f'{key}: {value}')
+            else:
+                msgarr.append(f'{key}: {pformat(value)}')
+
         finalmessage = '\n'.join(msgarr).replace('\n', '\n              ')
-        self.instance.logprint(finalmessage, self.method, "debug")
+        self.instance.logprint(finalmessage, self.method, "DEBUG")
 
     def destroy(self):
         """_summary_
         """
         self.instance = None
         self.method = None
 
     def info(self, message):
         """_summary_
 
         Args:
             message (_type_): _description_
         """
-        self.instance.logprint(message, self.method, "info")
+        self.instance.logprint(message, self.method, "INFO")
 
     def error(self, message, exception=None):
         """_summary_
 
         Args:
             message (_type_): _description_
             exception (_type_, optional): _description_. Defaults to None.
         """
-        self.instance.logprint(message, self.method, "error", exception)
+        self.instance.logprint(message, self.method, "ERROR", exception)
 
     def critical(self, message, exception=None):
         """_summary_
 
         Args:
             message (_type_): _description_
             exception (_type_, optional): _description_. Defaults to None.
         """
-        self.instance.logprint(message, self.method, "critical", exception)
+        self.instance.logprint(message, self.method, "CRITICAL", exception)
 
     def warning(self, message, exception=None):
         """_summary_
 
         Args:
             message (_type_): _description_
             exception (_type_, optional): _description_. Defaults to None.
         """
-        self.instance.logprint(message, self.method, "warning", exception)
+        self.instance.logprint(message, self.method, "WARNING", exception)
 
     def title(self, message):
         """_summary_
 
         Args:
             message (_type_): _description_
         """
-        self.instance.logprint(message, self.method, "title")
+        self.instance.logprint(message, self.method, "TITLE")
```

### Comparing `rsxml-2.0.1/rsxml/logging/progress_bar.py` & `rsxml-2.0.2/rsxml/logging/progress_bar.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.1/rsxml/project_xml/Analysis.py` & `rsxml-2.0.2/rsxml/project_xml/Analysis.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,16 @@
     """
 from __future__ import annotations
 from typing import List
 import xml.etree.cElementTree as ET
 
 from rsxml.project_xml.RSObj import RSObj
 from rsxml.project_xml.MetaData import MetaData
-from rsxml.project_xml.Dataset import Dataset
+from rsxml.project_xml.Geopackage import Geopackage
+from rsxml.project_xml.Dataset import Dataset, RefDataset
 
 
 class Analysis(RSObj):
     """_summary_
 
     Args:
         RSObj (_type_): _description_
@@ -46,21 +47,37 @@
                          )
 
         self.metrics = MetaData(metrics._values, inner_tag='Metric', container_tag='Metrics') if metrics else None
         self.configuration = configuration
         self.products = products
 
     @staticmethod
+    def datasets_from_xml(xml_node: ET.Element, ds_type: str, common_datasets: List[Dataset] = []) -> List[Dataset | RefDataset]:
+        """This works across a dataset container AND accounts for the possibility of RefDatasets
+        """
+        retvals = []
+        found = xml_node.find(ds_type)
+        if found:
+            for ds in found:
+                if ds.tag == 'CommonDatasetRef':
+                    retvals.append(RefDataset.from_xml(ds, common_datasets))
+                elif ds.tag == 'Geopackage':
+                    retvals.append(Geopackage.from_xml(ds))
+                else:
+                    retvals.append(Dataset.from_xml(ds))
+        return retvals
+
+    @staticmethod
     def from_xml(xml_node: ET.Element) -> Analysis:
-        rsobj = super.from_xml(xml_node)
+        rsobj = RSObj.from_xml(xml_node)
 
         metrics = MetaData.from_xml(xml_node.find('Metrics'))
 
-        configuration = [Dataset.from_xml(d) for d in xml_node.findall('Configuration/*')]
-        products = [Dataset.from_xml(d) for d in xml_node.findall('Products/*')]
+        configuration = Analysis.datasets_from_xml(xml_node, 'Configuration')
+        products = Analysis.datasets_from_xml(xml_node, 'Products')
 
         return Analysis(xml_id=rsobj.xml_id,
                         name=rsobj.name,
                         metrics=metrics,
                         configuration=configuration,
                         products=products,
                         summary=rsobj.summary,
```

### Comparing `rsxml-2.0.1/rsxml/project_xml/MetaData.py` & `rsxml-2.0.2/rsxml/project_xml/MetaData.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,46 +139,61 @@
 
     def remove_meta(self, name: str) -> None:
         """
         Remove an existing metadata item by name.
         """
         self._values = [s for s in self._values if s.name != name]
 
+    def __eq__(self, other: MetaData) -> bool:
+
+        if not isinstance(other, MetaData):
+            return False
+
+        return self.container_tag == other.container_tag and \
+            self.inner_tag == other.inner_tag and \
+            len(self._values) == len(other._values) and \
+            all([a == b for a, b in zip(self._values, other._values)])
+
     @staticmethod
-    def from_xml(xml_node: ET.Element, parent: ET.Element) -> MetaData:
+    def from_xml(xml_node: ET.Element) -> MetaData:
         """
         Create an instance of the MetaData class from an xml node.
 
         Args:
             xml_node (ET.Element): _description_
 
         Returns:
             MetaData: _description_
         """
+        if xml_node is None:
+            return MetaData()
         container_tag = xml_node.tag
         inner_tag_find = xml_node.find('*')
         inner_tag = xml_node.find('*').tag if inner_tag_find is not None else None
 
         meta_data = MetaData(container_tag=container_tag, inner_tag=inner_tag)
 
         for meta in xml_node.findall('*'):
             meta_data.add_meta(
                 meta.get('name'),
-                meta.get('value'),
+                meta.text.strip() if meta.text else "",
                 meta.get('type'),
+                meta.get('ext')
             )
         return meta_data
 
     def to_xml(self) -> ET.Element:
         """
         Serialize a MetaData item to an xml node ready to be written to a project.rs.xml file.
 
         Returns:
             ET.Element: XML node representing the MetaData item.
         """
+        if len(self._values) == 0:
+            return None
         meta_data = ET.Element(self.container_tag)
         for meta in self._values:
             meta_node = ET.Element(self.inner_tag, {
                 'name': meta.name,
             })
             if meta.type is not None:
                 meta_node.set('type', meta.type)
```

### Comparing `rsxml-2.0.1/rsxml/project_xml/Project.py` & `rsxml-2.0.2/rsxml/project_xml/Project.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 
 Use this class to instantiate a project with associated metadata, bounds, datasets, and analysis.
 You can then write the project to an XML file.
 """
 from __future__ import annotations
 from typing import List
 import xml.etree.cElementTree as ET
+import os
 
 from rsxml.project_xml.MetaData import MetaData
 from rsxml.project_xml.RSObj import RSObj
 from rsxml.project_xml.ProjectBounds import ProjectBounds
 from rsxml.project_xml.Realization import Realization
-from rsxml.project_xml.Dataset import Dataset
+from rsxml.project_xml.Geopackage import Geopackage
+from rsxml.project_xml.Dataset import Dataset, RefDataset
 from rsxml.project_xml.QAQCEvent import QAQCEvent
+from rsxml.project_xml.Warehouse import Warehouse
 
 from rsxml.logging.logger import Logger
 
 
 class Project(RSObj):
     """
     Represents a project with associated metadata, bounds, datasets, and analysis.
@@ -99,49 +102,82 @@
         Returns:
             Project: initialized project object
         """
         xml_node = ET.parse(xml_file_path).getroot()
         return Project.from_xml(xml_node, xml_file_path)
 
     @staticmethod
-    def from_xml(xml_node: ET.Element, proj_path: str) -> Project:
+    def datasets_from_xml(xml_node: ET.Element, ds_type: str) -> List[Dataset | RefDataset]:
+        """This works across a dataset container AND accounts for the possibility of RefDatasets
+        """
+        retvals = []
+        found = xml_node.find(ds_type)
+        if found:
+            for ds in found:
+                if ds.tag == 'Geopackage':
+                    retvals.append(Geopackage.from_xml(ds))
+                else:
+                    retvals.append(Dataset.from_xml(ds))
+        return retvals
+
+    @staticmethod
+    def from_xml(xml_node: ET.Element, proj_path: str = None) -> Project:
         """
         Initializes a Project instance from an XML node.
         Typically only used within the load_project method.
 
         Args:
             xml_node (ET.Element): Root node from project XML file.
 
         Returns:
             Project: loaded project object
         """
 
         rsobj = RSObj.from_xml(xml_node)
         warehouse_find = xml_node.find('Warehouse')
+        warehouse = Warehouse.from_xml(warehouse_find) if warehouse_find is not None else None
+
         project_bounds_find = xml_node.find('ProjectBounds')
         if project_bounds_find is None:
             log = Logger('Project')
             log.warning("""WARNING: No ProjectBounds.
                 The project will load into the Riverscapes Data Exchange, but will be easier to discover if you add a ProjectBounds.""")
 
+        # We need to find common datasets before realizations, because realizations reference common datasets
+        common_datasets = Project.datasets_from_xml(xml_node, 'CommonDatasets')
+
+        realizations = []
+        realization_nodes = xml_node.find('Realizations')
+        if realization_nodes:
+            for realization_node in realization_nodes:
+                if realization_node:
+                    realizations.append(Realization.from_xml(realization_node, common_datasets))
+
+        qaqc_events = []
+        qaqc_events_nodes = xml_node.find('QAQCEvents')
+        if qaqc_events_nodes:
+            for qaqc_event_node in qaqc_events_nodes:
+                if qaqc_event_node:
+                    qaqc_events.append(QAQCEvent.from_xml(qaqc_event_node))
+
         project = Project(
             name=rsobj.name,
             project_type=xml_node.find('ProjectType').text,
             bounds=ProjectBounds.from_xml(project_bounds_find) if project_bounds_find else None,
             proj_path=proj_path,
             summary=rsobj.summary,
             description=rsobj.description,
             citation=rsobj.citation,
             meta_data=rsobj.meta_data,
-            warehouse=Warehouse.from_xml(warehouse_find) if warehouse_find else None,
+            warehouse=warehouse,
 
             # List comprehension on the result of find() will iterate over all the children of the node. Do not wildcard!
-            common_datasets=[Dataset.from_xml(dataset_node) for dataset_node in xml_node.find('CommonDatasets')] if xml_node.find('CommonDatasets') else None,
-            realizations=[Realization.from_xml(realization_node) for realization_node in xml_node.find('Realizations')]if xml_node.find('Realizations') else None,
-            qaqc_events=[QAQCEvent.from_xml(qaqc_event_node) for qaqc_event_node in xml_node.find('QAQCEvents')]if xml_node.find('QAQCEvents') else None,
+            common_datasets=common_datasets,
+            realizations=realizations,
+            qaqc_events=qaqc_events
         )
 
         return project
 
     def to_xml(self) -> ET.Element:
         """
         Serialize an instance of this class to an XML node.
@@ -149,14 +185,17 @@
         Returns:
             ET.Element: XML node representing this project.
         """
         xml_node = super().to_xml()
 
         ET.SubElement(xml_node, 'ProjectType').text = self.project_type
 
+        if self.warehouse:
+            xml_node.append(self.warehouse.to_xml())
+
         # If there's no Model Version then throw a warning
         if not self.meta_data.find_meta('ModelVersion'):
             self.log.warning(f'WARNING: No ModelVersion found for {self.name}')
 
         if self.qaqc_events and len(self.qaqc_events) > 0:
             qaqc_node = ET.SubElement(xml_node, 'QAQCEvents')
             for qaqc_event in self.qaqc_events:
@@ -173,74 +212,44 @@
         realizations_node = ET.SubElement(xml_node, 'Realizations')
 
         for realization in self.realizations:
             realizations_node.append(realization.to_xml())
 
         return xml_node
 
-    def write(self):
+    def write(self, new_path: str = None):
         """
         Serialize the project to an XML file on disk.
         Call this method once you have finished modifying the project and want to save it to disk.
 
         https://stackoverflow.com/questions/28813876/how-do-i-get-pythons-elementtree-to-pretty-print-to-an-xml-file
         """
+        log = Logger('Project Writer')
+        final_path = new_path if new_path else self.proj_path
+
+        if not final_path:
+            raise ValueError('Project path is not set. Cannot write project.')
+        path_dir = os.path.dirname(final_path)
+        if not os.path.exists(path_dir) or not os.path.isdir(path_dir):
+            raise ValueError(f'Project path {path_dir} does not exist or is not a directory. Cannot write project.')
+        if os.path.exists(final_path):
+            log.warning(f'Project path {final_path} already exists. Overwriting.')
+
         xml_node = self.to_xml()
         encoding = 'UTF-8'
 
         # Set the attributes
         xml_node.set("xmlns:xsi", "http://www.w3.org/2001/XMLSchema-instance")
         xml_node.set("xsi:noNamespaceSchemaLocation", "https://xml.riverscapes.net/Projects/XSD/V2/RiverscapesProject.xsd")
 
         # Create a copy of the input element: Convert to string, then parse again
-        copy = ET.fromstring(ET.tostring(xml_node, encoding='utf8'))
+        copy = ET.fromstring(ET.tostring(xml_node, encoding='utf-8'))
 
         # Format copy. This needs Python 3.9+
-        ET.indent(copy, space="    ", level=0)
+        ET.indent(copy, space="  ", level=0)
 
         # tostring() returns a binary, so we need to decode it to get a string
         xml_string = ET.tostring(copy, encoding=encoding).decode(encoding)
 
-        with open(self.proj_path, 'w', encoding=encoding) as f:
+        with open(final_path, 'w', encoding=encoding) as f:
             f.write('<?xml version="1.0" ?>\n')
             f.write(xml_string)
-
-
-class Warehouse:
-    """
-    Represents a Riverscapes Warehouse where the project is stored.
-    Only use this class if the project is already stored in a warehouse.
-    """
-    guid: str
-    api_url: str
-
-    def __init__(self, guid, api_url) -> None:
-        self.guid = guid
-        self.api_url = api_url
-
-    @staticmethod
-    def from_xml(xml_node: ET.Element) -> Warehouse:
-        """
-        Load an instance of this class from an XML node.
-
-        Args:
-            xml_node (ET.Element): XML node representing this warehouse.
-
-        Returns:
-            Warehouse: Initialized warehouse object.
-        """
-        return Warehouse(
-            guid=xml_node.attrib['id'],
-            api_url=xml_node.attrib['apiUrl']
-        )
-
-    def to_xml(self) -> ET.Element:
-        """
-        Serialize an instance of this class to an XML node.
-
-        Returns:
-            str: XML node representing this warehouse, ready to be written to disk.
-        """
-        root = ET.Element('Warehouse')
-        root.set('id', self.guid)
-        root.set('apiUrl', self.api_url)
-        return root
```

### Comparing `rsxml-2.0.1/rsxml/project_xml/ProjectBounds.py` & `rsxml-2.0.2/rsxml/project_xml/ProjectBounds.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.1/rsxml/project_xml/QAQCEvent.py` & `rsxml-2.0.2/rsxml/project_xml/QAQCEvent.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,38 +4,38 @@
         NotImplementedError: _description_
 
     Returns:
         _type_: _description_
     """
 from __future__ import annotations
 from typing import Dict
-from datetime import date
+from datetime import datetime
 import xml.etree.cElementTree as ET
 
 from rsxml.project_xml.RSObj import RSObj
 from rsxml.project_xml.MetaData import MetaData
-
+from rsxml.logging.logger import Logger
 
 ALLOWED_STATES = [
     'passed',
     'failed',
     'provisional',
 ]
 
 
 class QAQCEvent(RSObj):
     """_summary_
     """
-    date_performed: date
+    date_performed: datetime
     state: str
     performed_by: str
     links: Dict[str, str]
 
     def __init__(self,
-                 date_performed: date,
+                 date_performed: datetime,
                  performed_by: str,
                  state: str,
                  name: str,
                  summary: str = None,
                  description: str = None,
                  citation: str = None,
                  meta_data: MetaData = None,
@@ -71,16 +71,24 @@
 
         Args:
             xml_node (ET.Element): _description_
 
         Returns:
             QAQCEvent: _description_
         """
+        log = Logger()
         rs_obj = RSObj.from_xml(xml_node)
-        date_performed = xml_node.get('datePerformed')
+
+        try:
+            date_performed_node = xml_node.get('datePerformed')
+            date_performed = datetime.fromisoformat(date_performed_node)
+        except ValueError as err:
+            log.error(f'QAQC: datePerformed is not a valid ISO 8601 date like "{datetime.now().isoformat()}". Got: "{date_performed_node}"')
+            raise err
+
         performed_by = xml_node.find('PerformedBy').text
         state = xml_node.get('state')
 
         links = {}
         links_node = xml_node.find('Links')
         if links_node:
             for link_node in links_node.findall('URL'):
@@ -100,14 +108,15 @@
 
     def to_xml(self) -> ET.Element:
         """_summary_
 
         Returns:
             str: _description_
         """
+        log = Logger('QAQC')
         xml_node = super().to_xml()
         xml_node.set('datePerformed', self.date_performed.isoformat())
         xml_node.set('state', self.state)
 
         ET.SubElement(xml_node, 'PerformedBy').text = self.performed_by
 
         if self.links:
```

### Comparing `rsxml-2.0.1/rsxml/project_xml/RSObj.py` & `rsxml-2.0.2/rsxml/project_xml/RSObj.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def __init__(self,
                  xml_tag: str,
                  xml_id: str,
                  name: str,
                  summary: str = None,
                  description: str = None,
                  citation: str = None,
-                 meta_data: MetaData = None,
+                 meta_data: MetaData = MetaData(),
                  mandatory_id: bool = True
                  ) -> None:
         """
         Initializes an instance of RSObj, the base class for several other types.
 
         Args:
             xml_tag (str): The XML tag associated with the instance.
@@ -89,49 +89,65 @@
         self.xml_tag = xml_tag
         self.xml_id = xml_id.strip() if xml_id else None
         self.name = name.strip() if name else None
 
         self.summary = summary.strip() if summary else None
         self.description = description.strip() if description else None
         self.citation = citation.strip() if citation else None
-        self.meta_data = meta_data
+        self.meta_data = meta_data if meta_data else MetaData()
 
     @staticmethod
     def from_xml(xml_node: ET.Element) -> RSObj:
         """ parse XML and return an RSOBj """
 
         xml_id = xml_node.get('id')
         xml_tag = xml_node.tag
-        name = xml_node.find('Name').text
+        name_find = xml_node.find('Name')
+        if name_find is None:
+            raise ValueError('Name is mandatory')
+        name = name_find.text
 
         summary_find = xml_node.find('Summary')
         summary = summary_find.text if summary_find is not None else None
 
         description_find = xml_node.find('Description')
         description = description_find.text if description_find is not None else None
 
         citation_find = xml_node.find('Citation')
         citation = citation_find.text if citation_find is not None else None
 
         meta_data_find = xml_node.find('MetaData')
-        meta_data = MetaData.from_xml(meta_data_find, xml_node) if meta_data_find is not None else None
+        meta_data = MetaData.from_xml(meta_data_find) if meta_data_find is not None else MetaData()
 
         mandatory_id = xml_id is not None
 
         return RSObj(
             xml_tag=xml_tag,
             xml_id=xml_id,
             name=name,
             summary=summary,
             description=description,
             citation=citation,
             meta_data=meta_data,
             mandatory_id=mandatory_id
         )
 
+    def __eq__(self, other: RSObj) -> bool:
+        """ Equality operator """
+
+        if not isinstance(other, RSObj):
+            return False
+
+        return self.xml_id == other.xml_id and \
+            self.name == other.name and \
+            self.summary == other.summary and \
+            self.description == other.description and \
+            self.citation == other.citation and \
+            self.meta_data == other.meta_data
+
     def to_xml(self) -> ET.Element:
         """
          Serializes the object into an XML node
         """
 
         xml_node = ET.Element(self.xml_tag)
 
@@ -143,10 +159,12 @@
             ET.SubElement(xml_node, 'Summary').text = self.summary
         if self.description:
             ET.SubElement(xml_node, 'Description').text = self.description
         if self.citation:
             ET.SubElement(xml_node, 'Citation').text = self.citation
 
         if self.meta_data is not None:
-            xml_node.append(self.meta_data.to_xml())
+            new_node = self.meta_data.to_xml()
+            if new_node is not None:
+                xml_node.append(new_node)
 
         return xml_node
```

### Comparing `rsxml-2.0.1/rsxml/util.py` & `rsxml-2.0.2/rsxml/util.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.1/rsxml/validation.py` & `rsxml-2.0.2/rsxml/validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """_summary_"""
+from __future__ import annotations
+from typing import List
 import requests
 from io import BytesIO
 try:
     from lxml import etree
 except ImportError:
     etree = None
 from rsxml import Logger
@@ -74,7 +76,8 @@
         with open(project_file_path, 'r') as f:
             xml = f.read()
     except Exception as e:
         log.error(f'Could not read XML file {project_file_path}')
         raise e
 
     return validate_xml(xml, xsd)
+
```

### Comparing `rsxml-2.0.1/rsxml.egg-info/PKG-INFO` & `rsxml-2.0.2/rsxml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsxml
-Version: 2.0.1
+Version: 2.0.2
 Summary: Riverscapes XML helpers for use across Python3 open-source GIS Stack
 Home-page: https://github.com/Riverscapes/RiverscapesXML
 Author: Matt Reimer
 Author-email: info@northarrowresearch.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rsxml-2.0.1/rsxml.egg-info/SOURCES.txt` & `rsxml-2.0.2/rsxml.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -25,20 +25,23 @@
 rsxml/debug/timer.py
 rsxml/debug/timer_buckets.py
 rsxml/logging/__init__.py
 rsxml/logging/logger.py
 rsxml/logging/progress_bar.py
 rsxml/project_xml/Analysis.py
 rsxml/project_xml/Dataset.py
+rsxml/project_xml/Geopackage.py
 rsxml/project_xml/MetaData.py
 rsxml/project_xml/Project.py
 rsxml/project_xml/ProjectBounds.py
+rsxml/project_xml/ProjectValidation.py
 rsxml/project_xml/QAQCEvent.py
 rsxml/project_xml/RSObj.py
 rsxml/project_xml/Realization.py
+rsxml/project_xml/Warehouse.py
 rsxml/project_xml/__init__.py
 rsxml/project_xml/common.py
 tests/test_dotenv.py
 tests/test_etags.py
 tests/test_load_samples.py
 tests/test_paths.py
 tests/test_project_xml.py
```

### Comparing `rsxml-2.0.1/setup.py` & `rsxml-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.1/tests/test_dotenv.py` & `rsxml-2.0.2/tests/test_dotenv.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.1/tests/test_etags.py` & `rsxml-2.0.2/tests/test_etags.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.1/tests/test_timers.py` & `rsxml-2.0.2/tests/test_timers.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.1/tests/test_util.py` & `rsxml-2.0.2/tests/test_util.py`

 * *Files identical despite different names*

