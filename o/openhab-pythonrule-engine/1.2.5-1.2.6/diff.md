# Comparing `tmp/openhab_pythonrule_engine-1.2.5.tar.gz` & `tmp/openhab_pythonrule_engine-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openhab_pythonrule_engine-1.2.5.tar", last modified: Mon Jul 10 15:29:41 2023, max compression
+gzip compressed data, was "dist/openhab_pythonrule_engine-1.2.6.tar", last modified: Mon Jul 10 15:32:47 2023, max compression
```

## Comparing `openhab_pythonrule_engine-1.2.5.tar` & `openhab_pythonrule_engine-1.2.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/cron_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/eventbus_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/item_change_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14294 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/item_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/loaded_rule_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/rule_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/rule_engine_webthing.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/source_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/cron_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/eventbus_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/item_change_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14294 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/item_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/loaded_rule_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/rule_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/rule_engine_webthing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/source_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 15:32:47.000000 openhab_pythonrule_engine-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-10 15:32:31.000000 openhab_pythonrule_engine-1.2.6/setup.py
```

### Comparing `openhab_pythonrule_engine-1.2.5/PKG-INFO` & `openhab_pythonrule_engine-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhab_pythonrule_engine
-Version: 1.2.5
+Version: 1.2.6
 Summary: Openhab python rule engine
 Home-page: https://github.com/grro/openhab_pythonrule_engine
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # OpenHAB python rule engine
         A python 3.x rule engine for OpenHAB. This rule engine allows defining rule by using python 3.x.
```

### Comparing `openhab_pythonrule_engine-1.2.5/README.md` & `openhab_pythonrule_engine-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/__init__.py` & `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/app.py` & `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/app.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/cache.py` & `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/cache.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/cron_processor.py` & `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/cron_processor.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/eventbus_consumer.py` & `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/eventbus_consumer.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/invoke.py` & `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/invoke.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/item_change_processor.py` & `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/item_change_processor.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/item_registry.py` & `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/item_registry.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/loaded_rule_processor.py` & `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/loaded_rule_processor.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/processor.py` & `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         triggers = self.trigger_by_module.get(trigger.module, set())
         triggers.add(trigger)
         self.trigger_by_module[trigger.module] = triggers
         self.on_add_trigger(trigger)
 
     def remove_triggers(self, module: str):
         if module in self.trigger_by_module.keys():
-            logging.info("removing all " + str(len(self.trigger_by_module[module])) + self.name + " trigger of '" + module + "'")
+            logging.info("removing all " + str(len(self.trigger_by_module[module])) + " " + self.name + " trigger of '" + module + "'")
             del self.trigger_by_module[module]
         self.on_remove_triggers(module)
 
     def process_trigger(self, trigger: Trigger):
         try:
             trigger.invoke(self.item_registry)
             self.last_executed = datetime.now().strftime("%H:%M:%S") + ' - ' + trigger.module + '.py  @when("' + trigger.expression + '")'
```

### Comparing `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/rule_engine.py` & `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/rule_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         self.listeners = set()
 
     def on_executed(self, source: Processor, success: bool):
         if success:
             self.last_executed = source.last_executed
         else:
             self.last_executed = source.last_error
+        self.__notify_listener()
 
     def __del__(self):
         self.stop()
 
     def add_listener(self, listener):
         self.listeners.add(listener)
         self.__notify_listener()
```

### Comparing `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/rule_engine_webthing.py` & `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/rule_engine_webthing.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/source_scanner.py` & `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/source_scanner.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/trigger.py` & `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine/trigger.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine.egg-info/PKG-INFO` & `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhab-pythonrule-engine
-Version: 1.2.5
+Version: 1.2.6
 Summary: Openhab python rule engine
 Home-page: https://github.com/grro/openhab_pythonrule_engine
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # OpenHAB python rule engine
         A python 3.x rule engine for OpenHAB. This rule engine allows defining rule by using python 3.x.
```

### Comparing `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine.egg-info/SOURCES.txt` & `openhab_pythonrule_engine-1.2.6/openhab_pythonrule_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.5/setup.py` & `openhab_pythonrule_engine-1.2.6/setup.py`

 * *Files identical despite different names*

