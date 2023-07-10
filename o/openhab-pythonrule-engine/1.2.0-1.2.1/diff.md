# Comparing `tmp/openhab_pythonrule_engine-1.2.0.tar.gz` & `tmp/openhab_pythonrule_engine-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openhab_pythonrule_engine-1.2.0.tar", last modified: Mon Jul 10 05:32:38 2023, max compression
+gzip compressed data, was "dist/openhab_pythonrule_engine-1.2.1.tar", last modified: Mon Jul 10 05:41:54 2023, max compression
```

## Comparing `openhab_pythonrule_engine-1.2.0.tar` & `openhab_pythonrule_engine-1.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/cron_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/eventbus_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/item_change_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/item_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/loaded_rule_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/rule_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/rule_engine_webthing.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/source_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:41:54.000000 openhab_pythonrule_engine-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-10 05:41:54.000000 openhab_pythonrule_engine-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-10 05:41:41.000000 openhab_pythonrule_engine-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:41:54.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-10 05:41:41.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-10 05:41:41.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-10 05:41:41.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-10 05:41:41.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-10 05:41:41.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/cron_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-10 05:41:41.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/eventbus_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-10 05:41:41.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-10 05:41:41.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/item_change_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-07-10 05:41:41.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/item_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-10 05:41:41.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/loaded_rule_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-10 05:41:41.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-10 05:41:41.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/rule_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-10 05:41:41.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/rule_engine_webthing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-10 05:41:41.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/source_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-10 05:41:41.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:41:54.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-10 05:41:54.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-10 05:41:54.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 05:41:54.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 05:41:54.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-10 05:41:54.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 05:41:54.000000 openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 05:41:54.000000 openhab_pythonrule_engine-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-10 05:41:41.000000 openhab_pythonrule_engine-1.2.1/setup.py
```

### Comparing `openhab_pythonrule_engine-1.2.0/PKG-INFO` & `openhab_pythonrule_engine-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhab_pythonrule_engine
-Version: 1.2.0
+Version: 1.2.1
 Summary: Openhab python rule engine
 Home-page: https://github.com/grro/openhab_pythonrule_engine
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # OpenHAB python rule engine
         A python 3.x rule engine for OpenHAB. This rule engine allows defining rule by using python 3.x.
```

### Comparing `openhab_pythonrule_engine-1.2.0/README.md` & `openhab_pythonrule_engine-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/__init__.py` & `openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/app.py` & `openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/app.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/cache.py` & `openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/cache.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/cron_processor.py` & `openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/cron_processor.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/eventbus_consumer.py` & `openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/eventbus_consumer.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/invoke.py` & `openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/invoke.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/item_change_processor.py` & `openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/item_change_processor.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/item_registry.py` & `openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/item_registry.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/loaded_rule_processor.py` & `openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/loaded_rule_processor.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/processor.py` & `openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/processor.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/rule_engine.py` & `openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/rule_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
 import os
 import sys
 import importlib
-from source_scanner import visit
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler
 from openhab_pythonrule_engine.item_registry import ItemRegistry
 from openhab_pythonrule_engine.cron_processor import CronProcessor
 from openhab_pythonrule_engine.item_change_processor import ItemChangeProcessor
 from openhab_pythonrule_engine.loaded_rule_processor import RuleLoadedProcessor
+from openhab_pythonrule_engine.source_scanner import visit
 
 
 
 class FileSystemListener(FileSystemEventHandler):
 
     def __init__(self, rule_engine, dir):
         self.rule_engine = rule_engine
```

### Comparing `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/rule_engine_webthing.py` & `openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/rule_engine_webthing.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/source_scanner.py` & `openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/source_scanner.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/trigger.py` & `openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine/trigger.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine.egg-info/PKG-INFO` & `openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhab-pythonrule-engine
-Version: 1.2.0
+Version: 1.2.1
 Summary: Openhab python rule engine
 Home-page: https://github.com/grro/openhab_pythonrule_engine
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # OpenHAB python rule engine
         A python 3.x rule engine for OpenHAB. This rule engine allows defining rule by using python 3.x.
```

### Comparing `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine.egg-info/SOURCES.txt` & `openhab_pythonrule_engine-1.2.1/openhab_pythonrule_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.0/setup.py` & `openhab_pythonrule_engine-1.2.1/setup.py`

 * *Files identical despite different names*

