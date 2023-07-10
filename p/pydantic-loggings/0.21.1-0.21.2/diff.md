# Comparing `tmp/pydantic-loggings-0.21.1.tar.gz` & `tmp/pydantic-loggings-0.21.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-loggings-0.21.1.tar", last modified: Wed Jul  5 16:40:17 2023, max compression
+gzip compressed data, was "pydantic-loggings-0.21.2.tar", last modified: Mon Jul 10 17:47:56 2023, max compression
```

## Comparing `pydantic-loggings-0.21.1.tar` & `pydantic-loggings-0.21.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:40:17.899483 pydantic-loggings-0.21.1/
--rw-r--r--   0 root         (0) root         (0)     3205 2023-07-05 16:40:17.899483 pydantic-loggings-0.21.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2441 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/README.md
--rw-r--r--   0 root         (0) root         (0)     2419 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 16:40:17.899483 pydantic-loggings-0.21.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:40:17.895483 pydantic-loggings-0.21.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:40:17.895483 pydantic-loggings-0.21.1/src/pydantic_loggings/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/src/pydantic_loggings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:40:17.899483 pydantic-loggings-0.21.1/src/pydantic_loggings/base/
--rw-r--r--   0 root         (0) root         (0)      241 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/src/pydantic_loggings/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/src/pydantic_loggings/base/filters.py
--rw-r--r--   0 root         (0) root         (0)      404 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/src/pydantic_loggings/base/formatters.py
--rw-r--r--   0 root         (0) root         (0)      392 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/src/pydantic_loggings/base/handlers.py
--rw-r--r--   0 root         (0) root         (0)      337 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/src/pydantic_loggings/base/loggers.py
--rw-r--r--   0 root         (0) root         (0)      557 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/src/pydantic_loggings/base/loggings.py
--rw-r--r--   0 root         (0) root         (0)     3706 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/src/pydantic_loggings/mixins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:40:17.899483 pydantic-loggings-0.21.1/src/pydantic_loggings/not_set/
--rw-r--r--   0 root         (0) root         (0)      241 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/src/pydantic_loggings/not_set/__init__.py
--rw-r--r--   0 root         (0) root         (0)      419 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/src/pydantic_loggings/not_set/filters.py
--rw-r--r--   0 root         (0) root         (0)     1417 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/src/pydantic_loggings/not_set/formatters.py
--rw-r--r--   0 root         (0) root         (0)      894 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/src/pydantic_loggings/not_set/handlers.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/src/pydantic_loggings/not_set/loggers.py
--rw-r--r--   0 root         (0) root         (0)     2515 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/src/pydantic_loggings/not_set/loggings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:40:17.899483 pydantic-loggings-0.21.1/src/pydantic_loggings/rich/
--rw-r--r--   0 root         (0) root         (0)      148 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/src/pydantic_loggings/rich/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/src/pydantic_loggings/rich/handlers.py
--rw-r--r--   0 root         (0) root         (0)      337 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/src/pydantic_loggings/rich/loggers.py
--rw-r--r--   0 root         (0) root         (0)      339 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/src/pydantic_loggings/rich/loggings.py
--rw-r--r--   0 root         (0) root         (0)      191 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/src/pydantic_loggings/types_.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-05 16:40:07.000000 pydantic-loggings-0.21.1/src/pydantic_loggings/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:40:17.899483 pydantic-loggings-0.21.1/src/pydantic_loggings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3205 2023-07-05 16:40:17.000000 pydantic-loggings-0.21.1/src/pydantic_loggings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1018 2023-07-05 16:40:17.000000 pydantic-loggings-0.21.1/src/pydantic_loggings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:40:17.000000 pydantic-loggings-0.21.1/src/pydantic_loggings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-07-05 16:40:17.000000 pydantic-loggings-0.21.1/src/pydantic_loggings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-05 16:40:17.000000 pydantic-loggings-0.21.1/src/pydantic_loggings.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:47:56.813249 pydantic-loggings-0.21.2/
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-07-10 17:47:56.813249 pydantic-loggings-0.21.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2441 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/README.md
+-rw-r--r--   0 root         (0) root         (0)     2419 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 17:47:56.813249 pydantic-loggings-0.21.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:47:56.809249 pydantic-loggings-0.21.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:47:56.809249 pydantic-loggings-0.21.2/src/pydantic_loggings/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/src/pydantic_loggings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:47:56.813249 pydantic-loggings-0.21.2/src/pydantic_loggings/base/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/src/pydantic_loggings/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/src/pydantic_loggings/base/filters.py
+-rw-r--r--   0 root         (0) root         (0)      404 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/src/pydantic_loggings/base/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      392 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/src/pydantic_loggings/base/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      337 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/src/pydantic_loggings/base/loggers.py
+-rw-r--r--   0 root         (0) root         (0)      557 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/src/pydantic_loggings/base/loggings.py
+-rw-r--r--   0 root         (0) root         (0)     3706 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/src/pydantic_loggings/mixins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:47:56.813249 pydantic-loggings-0.21.2/src/pydantic_loggings/not_set/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/src/pydantic_loggings/not_set/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/src/pydantic_loggings/not_set/filters.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/src/pydantic_loggings/not_set/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      894 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/src/pydantic_loggings/not_set/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/src/pydantic_loggings/not_set/loggers.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/src/pydantic_loggings/not_set/loggings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:47:56.813249 pydantic-loggings-0.21.2/src/pydantic_loggings/rich/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/src/pydantic_loggings/rich/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/src/pydantic_loggings/rich/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      337 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/src/pydantic_loggings/rich/loggers.py
+-rw-r--r--   0 root         (0) root         (0)      339 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/src/pydantic_loggings/rich/loggings.py
+-rw-r--r--   0 root         (0) root         (0)      191 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/src/pydantic_loggings/types_.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 17:47:46.000000 pydantic-loggings-0.21.2/src/pydantic_loggings/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:47:56.809249 pydantic-loggings-0.21.2/src/pydantic_loggings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-07-10 17:47:56.000000 pydantic-loggings-0.21.2/src/pydantic_loggings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-07-10 17:47:56.000000 pydantic-loggings-0.21.2/src/pydantic_loggings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 17:47:56.000000 pydantic-loggings-0.21.2/src/pydantic_loggings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-10 17:47:56.000000 pydantic-loggings-0.21.2/src/pydantic_loggings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-10 17:47:56.000000 pydantic-loggings-0.21.2/src/pydantic_loggings.egg-info/top_level.txt
```

### Comparing `pydantic-loggings-0.21.1/PKG-INFO` & `pydantic-loggings-0.21.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-loggings
-Version: 0.21.1
+Version: 0.21.2
 Author-email: m9810223 <m9810223@gmail.com>
 Project-URL: Homepage, https://github.com/m9810223/pydantic-logging-settings
 Project-URL: Source, https://github.com/m9810223/pydantic-logging-settings
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pydantic-loggings-0.21.1/README.md` & `pydantic-loggings-0.21.2/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.21.1/pyproject.toml` & `pydantic-loggings-0.21.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 authors = [
   { name = "m9810223", email = "m9810223@gmail.com" },
 ]
 name = "pydantic-loggings"
 readme = "README.md"
 requires-python = ">=3.9"
-version = "0.21.1"
+version = "0.21.2"
 
 classifiers = [
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3",
```

### Comparing `pydantic-loggings-0.21.1/src/pydantic_loggings/base/loggings.py` & `pydantic-loggings-0.21.2/src/pydantic_loggings/base/loggings.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.21.1/src/pydantic_loggings/mixins.py` & `pydantic-loggings-0.21.2/src/pydantic_loggings/mixins.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.21.1/src/pydantic_loggings/not_set/formatters.py` & `pydantic-loggings-0.21.2/src/pydantic_loggings/not_set/formatters.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.21.1/src/pydantic_loggings/not_set/handlers.py` & `pydantic-loggings-0.21.2/src/pydantic_loggings/not_set/handlers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.21.1/src/pydantic_loggings/not_set/loggers.py` & `pydantic-loggings-0.21.2/src/pydantic_loggings/not_set/loggers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.21.1/src/pydantic_loggings/not_set/loggings.py` & `pydantic-loggings-0.21.2/src/pydantic_loggings/not_set/loggings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 import logging
 import typing as t
-import warnings
 from logging.config import DictConfigurator
 
 from pydantic import field_validator
 from pydantic_core.core_schema import FieldValidationInfo
 from pydantic_settings import BaseSettings
 from pydantic_settings import SettingsConfigDict
 
@@ -68,14 +67,12 @@
     def configure(self):
         self.configurator(self.configuration).configure()
 
     def is_valid_logger_name(self, logger_name: str):
         return logger_name in ['', 'root', *(self.loggers or {}).keys()]
 
     def get_logger(self, logger_name: str = ''):
-        if not self.is_valid_logger_name(logger_name):
-            warnings.warn(f'Logger: `{logger_name}` is not found.')
         return logging.getLogger(name=logger_name)
 
     def configure_and_get_logger(self, logger_name: str = ''):
         self.configure()
         return self.get_logger(logger_name=logger_name)
```

### Comparing `pydantic-loggings-0.21.1/src/pydantic_loggings/rich/handlers.py` & `pydantic-loggings-0.21.2/src/pydantic_loggings/rich/handlers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.21.1/src/pydantic_loggings.egg-info/PKG-INFO` & `pydantic-loggings-0.21.2/src/pydantic_loggings.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-loggings
-Version: 0.21.1
+Version: 0.21.2
 Author-email: m9810223 <m9810223@gmail.com>
 Project-URL: Homepage, https://github.com/m9810223/pydantic-logging-settings
 Project-URL: Source, https://github.com/m9810223/pydantic-logging-settings
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pydantic-loggings-0.21.1/src/pydantic_loggings.egg-info/SOURCES.txt` & `pydantic-loggings-0.21.2/src/pydantic_loggings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

