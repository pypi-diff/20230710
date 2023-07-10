# Comparing `tmp/python_json_log_formatter-3.2.4.tar.gz` & `tmp/python_json_log_formatter-3.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_json_log_formatter-3.2.4.tar", last modified: Mon Jul 10 12:52:04 2023, max compression
+gzip compressed data, was "python_json_log_formatter-3.2.5.tar", last modified: Mon Jul 10 13:07:00 2023, max compression
```

## Comparing `python_json_log_formatter-3.2.4.tar` & `python_json_log_formatter-3.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-07-10 12:52:04.405762 python_json_log_formatter-3.2.4/
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)    11358 2022-11-24 16:19:23.000000 python_json_log_formatter-3.2.4/LICENSE
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)     3424 2023-07-10 12:52:04.405596 python_json_log_formatter-3.2.4/PKG-INFO
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)     2793 2023-06-02 13:54:12.000000 python_json_log_formatter-3.2.4/README.md
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)      945 2023-06-02 13:54:12.000000 python_json_log_formatter-3.2.4/pyproject.toml
-drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-07-10 12:52:04.404191 python_json_log_formatter-3.2.4/python_json_log_formatter/
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)     1195 2023-06-02 13:54:12.000000 python_json_log_formatter-3.2.4/python_json_log_formatter/__init__.py
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)       93 2023-06-02 13:54:12.000000 python_json_log_formatter-3.2.4/python_json_log_formatter/__init__.pyi
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)       21 2023-07-10 12:42:58.000000 python_json_log_formatter-3.2.4/python_json_log_formatter/_version.py
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)       16 2023-06-02 14:51:25.000000 python_json_log_formatter-3.2.4/python_json_log_formatter/_version.pyi
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)    13567 2023-07-10 12:48:01.000000 python_json_log_formatter-3.2.4/python_json_log_formatter/context_filter.py
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)      605 2023-07-10 12:48:10.000000 python_json_log_formatter-3.2.4/python_json_log_formatter/context_filter.pyi
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)        0 2022-12-13 12:36:44.000000 python_json_log_formatter-3.2.4/python_json_log_formatter/py.typed
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)     5425 2023-07-10 12:45:52.000000 python_json_log_formatter-3.2.4/python_json_log_formatter/python_json_log_formatter.py
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)      574 2023-06-02 14:51:06.000000 python_json_log_formatter-3.2.4/python_json_log_formatter/python_json_log_formatter.pyi
-drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-07-10 12:52:04.405376 python_json_log_formatter-3.2.4/python_json_log_formatter.egg-info/
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)     3424 2023-07-10 12:52:04.000000 python_json_log_formatter-3.2.4/python_json_log_formatter.egg-info/PKG-INFO
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)      617 2023-07-10 12:52:04.000000 python_json_log_formatter-3.2.4/python_json_log_formatter.egg-info/SOURCES.txt
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)        1 2023-07-10 12:52:04.000000 python_json_log_formatter-3.2.4/python_json_log_formatter.egg-info/dependency_links.txt
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)       26 2023-07-10 12:52:04.000000 python_json_log_formatter-3.2.4/python_json_log_formatter.egg-info/top_level.txt
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)       38 2023-07-10 12:52:04.405820 python_json_log_formatter-3.2.4/setup.cfg
+drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-07-10 13:07:00.543629 python_json_log_formatter-3.2.5/
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)    11358 2022-11-24 16:19:23.000000 python_json_log_formatter-3.2.5/LICENSE
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)     3424 2023-07-10 13:07:00.543489 python_json_log_formatter-3.2.5/PKG-INFO
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)     2793 2023-06-02 13:54:12.000000 python_json_log_formatter-3.2.5/README.md
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)      945 2023-06-02 13:54:12.000000 python_json_log_formatter-3.2.5/pyproject.toml
+drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-07-10 13:07:00.542553 python_json_log_formatter-3.2.5/python_json_log_formatter/
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)     1195 2023-06-02 13:54:12.000000 python_json_log_formatter-3.2.5/python_json_log_formatter/__init__.py
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)       93 2023-06-02 13:54:12.000000 python_json_log_formatter-3.2.5/python_json_log_formatter/__init__.pyi
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)       21 2023-07-10 13:05:58.000000 python_json_log_formatter-3.2.5/python_json_log_formatter/_version.py
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)       16 2023-06-02 14:51:25.000000 python_json_log_formatter-3.2.5/python_json_log_formatter/_version.pyi
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)    13571 2023-07-10 13:05:37.000000 python_json_log_formatter-3.2.5/python_json_log_formatter/context_filter.py
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)      605 2023-07-10 12:48:10.000000 python_json_log_formatter-3.2.5/python_json_log_formatter/context_filter.pyi
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)        0 2022-12-13 12:36:44.000000 python_json_log_formatter-3.2.5/python_json_log_formatter/py.typed
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)     5425 2023-07-10 12:45:52.000000 python_json_log_formatter-3.2.5/python_json_log_formatter/python_json_log_formatter.py
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)      574 2023-06-02 14:51:06.000000 python_json_log_formatter-3.2.5/python_json_log_formatter/python_json_log_formatter.pyi
+drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-07-10 13:07:00.543296 python_json_log_formatter-3.2.5/python_json_log_formatter.egg-info/
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)     3424 2023-07-10 13:07:00.000000 python_json_log_formatter-3.2.5/python_json_log_formatter.egg-info/PKG-INFO
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)      617 2023-07-10 13:07:00.000000 python_json_log_formatter-3.2.5/python_json_log_formatter.egg-info/SOURCES.txt
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)        1 2023-07-10 13:07:00.000000 python_json_log_formatter-3.2.5/python_json_log_formatter.egg-info/dependency_links.txt
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)       26 2023-07-10 13:07:00.000000 python_json_log_formatter-3.2.5/python_json_log_formatter.egg-info/top_level.txt
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)       38 2023-07-10 13:07:00.543675 python_json_log_formatter-3.2.5/setup.cfg
```

### Comparing `python_json_log_formatter-3.2.4/LICENSE` & `python_json_log_formatter-3.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_json_log_formatter-3.2.4/PKG-INFO` & `python_json_log_formatter-3.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_json_log_formatter
-Version: 3.2.4
+Version: 3.2.5
 Summary: Supplements a default formatter configuration for machine-readable JSON logging and applies it
 Author-email: Niels Korschinsky <niels.korschinsky@ibm.com>
 Project-URL: Homepage, https://github.com/IBM/python-json-log-formatter
 Project-URL: Bug Tracker, https://github.com/IBM/python-json-log-formatter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python_json_log_formatter Version: 3.2.4 Summary:
+Metadata-Version: 2.1 Name: python_json_log_formatter Version: 3.2.5 Summary:
 Supplements a default formatter configuration for machine-readable JSON logging
 and applies it Author-email: Niels Korschinsky
 korschinsky@ibm.com> Project-URL: Homepage, https://github.com/IBM/python-json-
 log-formatter Project-URL: Bug Tracker, https://github.com/IBM/python-json-log-
 formatter/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
```

### Comparing `python_json_log_formatter-3.2.4/README.md` & `python_json_log_formatter-3.2.5/README.md`

 * *Files identical despite different names*

### Comparing `python_json_log_formatter-3.2.4/pyproject.toml` & `python_json_log_formatter-3.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_json_log_formatter-3.2.4/python_json_log_formatter/__init__.py` & `python_json_log_formatter-3.2.5/python_json_log_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `python_json_log_formatter-3.2.4/python_json_log_formatter/context_filter.py` & `python_json_log_formatter-3.2.5/python_json_log_formatter/context_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     These structured JSON log lines are automatically parsed and indexed by LogDNA.
     """
 
     @property
     def message_key(self):
         return self.__message_key
 
-    __message_key: ClassVar[str] = "msg"
+    __message_key: ClassVar[str] = "message"
     """name of the key under which the msg will be saved"""
 
     __job_retry_limit_env = "JOB_RETRY_LIMIT"
     """ENV-Key of the retry limit per job, name defined by Code Engine"""
 
     __job_retry_count_env = "JOB_INDEX_RETRY_COUNT"
     """ENV-Key of the current re-try count per job, name defined by Code Engine"""
```

### Comparing `python_json_log_formatter-3.2.4/python_json_log_formatter/context_filter.pyi` & `python_json_log_formatter-3.2.5/python_json_log_formatter/context_filter.pyi`

 * *Files identical despite different names*

### Comparing `python_json_log_formatter-3.2.4/python_json_log_formatter/python_json_log_formatter.py` & `python_json_log_formatter-3.2.5/python_json_log_formatter/python_json_log_formatter.py`

 * *Files identical despite different names*

### Comparing `python_json_log_formatter-3.2.4/python_json_log_formatter/python_json_log_formatter.pyi` & `python_json_log_formatter-3.2.5/python_json_log_formatter/python_json_log_formatter.pyi`

 * *Files identical despite different names*

### Comparing `python_json_log_formatter-3.2.4/python_json_log_formatter.egg-info/PKG-INFO` & `python_json_log_formatter-3.2.5/python_json_log_formatter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-json-log-formatter
-Version: 3.2.4
+Version: 3.2.5
 Summary: Supplements a default formatter configuration for machine-readable JSON logging and applies it
 Author-email: Niels Korschinsky <niels.korschinsky@ibm.com>
 Project-URL: Homepage, https://github.com/IBM/python-json-log-formatter
 Project-URL: Bug Tracker, https://github.com/IBM/python-json-log-formatter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-json-log-formatter Version: 3.2.4 Summary:
+Metadata-Version: 2.1 Name: python-json-log-formatter Version: 3.2.5 Summary:
 Supplements a default formatter configuration for machine-readable JSON logging
 and applies it Author-email: Niels Korschinsky
 korschinsky@ibm.com> Project-URL: Homepage, https://github.com/IBM/python-json-
 log-formatter Project-URL: Bug Tracker, https://github.com/IBM/python-json-log-
 formatter/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
```

### Comparing `python_json_log_formatter-3.2.4/python_json_log_formatter.egg-info/SOURCES.txt` & `python_json_log_formatter-3.2.5/python_json_log_formatter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

