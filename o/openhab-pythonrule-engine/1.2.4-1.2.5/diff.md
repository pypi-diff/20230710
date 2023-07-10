# Comparing `tmp/openhab_pythonrule_engine-1.2.4.tar.gz` & `tmp/openhab_pythonrule_engine-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openhab_pythonrule_engine-1.2.4.tar", last modified: Mon Jul 10 14:56:39 2023, max compression
+gzip compressed data, was "dist/openhab_pythonrule_engine-1.2.5.tar", last modified: Mon Jul 10 15:29:41 2023, max compression
```

## Comparing `openhab_pythonrule_engine-1.2.4.tar` & `openhab_pythonrule_engine-1.2.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:56:39.000000 openhab_pythonrule_engine-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-10 14:56:39.000000 openhab_pythonrule_engine-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-10 14:56:27.000000 openhab_pythonrule_engine-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:56:39.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-10 14:56:27.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-10 14:56:27.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-10 14:56:27.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-10 14:56:27.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-10 14:56:27.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/cron_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-10 14:56:27.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/eventbus_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-10 14:56:27.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-10 14:56:27.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/item_change_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14294 2023-07-10 14:56:27.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/item_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-10 14:56:27.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/loaded_rule_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-10 14:56:27.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-07-10 14:56:27.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/rule_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-10 14:56:27.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/rule_engine_webthing.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-10 14:56:27.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/source_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-10 14:56:27.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:56:39.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-10 14:56:38.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-10 14:56:39.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:56:38.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 14:56:38.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-10 14:56:38.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 14:56:38.000000 openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 14:56:39.000000 openhab_pythonrule_engine-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-10 14:56:27.000000 openhab_pythonrule_engine-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/cron_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/eventbus_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/item_change_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14294 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/item_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/loaded_rule_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/rule_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/rule_engine_webthing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/source_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 15:29:41.000000 openhab_pythonrule_engine-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-10 15:29:26.000000 openhab_pythonrule_engine-1.2.5/setup.py
```

### Comparing `openhab_pythonrule_engine-1.2.4/PKG-INFO` & `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openhab_pythonrule_engine
-Version: 1.2.4
+Name: openhab-pythonrule-engine
+Version: 1.2.5
 Summary: Openhab python rule engine
 Home-page: https://github.com/grro/openhab_pythonrule_engine
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # OpenHAB python rule engine
         A python 3.x rule engine for OpenHAB. This rule engine allows defining rule by using python 3.x.
```

### Comparing `openhab_pythonrule_engine-1.2.4/README.md` & `openhab_pythonrule_engine-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/__init__.py` & `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/app.py` & `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/app.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/cache.py` & `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/cache.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/cron_processor.py` & `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/cron_processor.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/eventbus_consumer.py` & `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/eventbus_consumer.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/invoke.py` & `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/invoke.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/item_change_processor.py` & `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/item_change_processor.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/item_registry.py` & `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/item_registry.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/loaded_rule_processor.py` & `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/loaded_rule_processor.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/processor.py` & `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/processor.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/rule_engine.py` & `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/rule_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 class RuleEngine:
 
     def __init__(self, openhab_uri:str, python_rule_directory: str, user: str, pwd: str):
         self.is_running = False
         self.openhab_uri = openhab_uri
         logging.info("connecting " + openhab_uri)
-        self.loaded_modules = set()
+        self.loaded_modules = dict()
         self.last_executed = ""
         self.last_error = ""
         self.__item_registry = ItemRegistry(openhab_uri, user, pwd)
         self.__processors = [ItemChangeProcessor(openhab_uri, self.__item_registry, self.on_executed),
                              CronProcessor(self.__item_registry, self.on_executed),
                              RuleLoadedProcessor(self.__item_registry, self.on_executed)]
         self.file_system_listener = FileSystemListener(self, python_rule_directory)
@@ -113,31 +113,31 @@
                 if modulename in sys.modules:
                     [processor.remove_triggers(modulename) for processor in self.__processors]
                     importlib.reload(sys.modules[modulename])
                     msg = "'" + filename + "' reloaded"
                 else:
                     importlib.import_module(modulename)
                     msg = "'" + filename + "' loaded for the first time"
-                self.loaded_modules.add(filename)
-                self.__notify_listener()
                 num_annotations = visit(modulename, [processor.parser() for processor in self.__processors])
+                self.loaded_modules[filename] = num_annotations
                 if num_annotations > 0:
                     logging.info(msg)
+                self.__notify_listener()
             except Exception as e:
                 logging.warning("error occurred by (re)loading " + filename + " " + str(e), e)
 
     def unload_module(self, filename: str, silent: bool = False):
         if filename.endswith(".py"):
             try:
                 modulename = self.__filename_to_modulename(filename)
                 if modulename in sys.modules:
                     if not silent:
                         logging.info("\"unloading\" '" + filename + "'")
                     [processor.remove_triggers(modulename) for processor in self.__processors]
                     del sys.modules[modulename]
-                self.loaded_modules.remove(filename)
+                del self.loaded_modules[filename]
                 self.__notify_listener()
             except Exception as e:
                 logging.warning("error occurred by unloading " + filename + " " + str(e), e)
 
     def __filename_to_modulename(self, filename):
         return filename[:-3]
```

### Comparing `openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/rule_engine_webthing.py` & `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/rule_engine_webthing.py`

 * *Files 11% similar despite different names*

```diff
@@ -70,16 +70,16 @@
 
     def on_update(self):
         self.ioloop.add_callback(self.__handle)
 
     def __handle(self):
         self.last_executed.notify_of_external_update(self.rule_engine.last_executed)
         self.last_failed.notify_of_external_update(self.rule_engine.last_error)
-        self.loaded_modules.notify_of_external_update(", ".join(sorted(list(self.rule_engine.loaded_modules))))
-
+        modulenames = sorted(list(self.rule_engine.loaded_modules.keys()))
+        self.loaded_modules.notify_of_external_update(", ".join([modulename + " (" + str(self.rule_engine.loaded_modules[modulename]) + ")" for modulename in modulenames if self.rule_engine.loaded_modules[modulename] > 0]))
 
 def run_server(port: int, description: str, rule_engine: RuleEngine):
     rule_engine_webthing = RuleEngineThing(description, rule_engine)
     server = WebThingServer(SingleThing(rule_engine_webthing), port=port, disable_host_validation=True)
 
     try:
         # start webthing server
```

### Comparing `openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/source_scanner.py` & `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/source_scanner.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine/trigger.py` & `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine/trigger.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine.egg-info/PKG-INFO` & `openhab_pythonrule_engine-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openhab-pythonrule-engine
-Version: 1.2.4
+Name: openhab_pythonrule_engine
+Version: 1.2.5
 Summary: Openhab python rule engine
 Home-page: https://github.com/grro/openhab_pythonrule_engine
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # OpenHAB python rule engine
         A python 3.x rule engine for OpenHAB. This rule engine allows defining rule by using python 3.x.
```

### Comparing `openhab_pythonrule_engine-1.2.4/openhab_pythonrule_engine.egg-info/SOURCES.txt` & `openhab_pythonrule_engine-1.2.5/openhab_pythonrule_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.2.4/setup.py` & `openhab_pythonrule_engine-1.2.5/setup.py`

 * *Files identical despite different names*

