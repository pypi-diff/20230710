# Comparing `tmp/openhab_pythonrule_engine-1.1.9.tar.gz` & `tmp/openhab_pythonrule_engine-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openhab_pythonrule_engine-1.1.9.tar", last modified: Sat Mar 26 20:57:32 2022, max compression
+gzip compressed data, was "dist/openhab_pythonrule_engine-1.2.0.tar", last modified: Mon Jul 10 05:32:38 2023, max compression
```

## Comparing `openhab_pythonrule_engine-1.1.9.tar` & `openhab_pythonrule_engine-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 20:57:32.000000 openhab_pythonrule_engine-1.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)     4719 2022-03-26 20:57:32.000000 openhab_pythonrule_engine-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3596 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 20:57:32.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/
--rw-r--r--   0 runner    (1001) docker     (121)     3327 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5443 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      537 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     3195 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/condition.py
--rw-r--r--   0 runner    (1001) docker     (121)     2108 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/eventbus_consumer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1712 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/invoke.py
--rw-r--r--   0 runner    (1001) docker     (121)    11429 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/item_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)    13613 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/rule_engine.py
--rw-r--r--   0 runner    (1001) docker     (121)     3031 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/rule_engine_webthing.py
--rw-r--r--   0 runner    (1001) docker     (121)     5118 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 20:57:32.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4719 2022-03-26 20:57:31.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-03-26 20:57:31.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-26 20:57:31.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-03-26 20:57:31.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-03-26 20:57:31.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-03-26 20:57:31.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-26 20:57:32.000000 openhab_pythonrule_engine-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1414 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/cron_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/eventbus_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/item_change_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/item_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/loaded_rule_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/rule_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/rule_engine_webthing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/source_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 05:32:38.000000 openhab_pythonrule_engine-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-10 05:32:23.000000 openhab_pythonrule_engine-1.2.0/setup.py
```

### Comparing `openhab_pythonrule_engine-1.1.9/PKG-INFO` & `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openhab_pythonrule_engine
-Version: 1.1.9
+Name: openhab-pythonrule-engine
+Version: 1.2.0
 Summary: Openhab python rule engine
 Home-page: https://github.com/grro/openhab_pythonrule_engine
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # OpenHAB python rule engine
         A python 3.x rule engine for OpenHAB. This rule engine allows defining rule by using python 3.x.
```

### Comparing `openhab_pythonrule_engine-1.1.9/README.md` & `openhab_pythonrule_engine-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/__init__.py` & `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,15 +45,16 @@
         return "--openhab_uri http://localhost:8080 --python_rule_directory /etc/openhab/automation/rules/python --user me --pwd secret"
 
     def do_process_command(self, command:str, port: int, verbose: bool, args) -> bool:
         if command == 'listen' and (args.openhab_uri is not None) \
                                and (args.python_rule_directory is not None) \
                                and (args.user is not None) \
                                and (args.pwd is not None):
-            rule_engine = RuleEngine.start_singleton(args.openhab_uri, args.python_rule_directory, args.user, args.pwd)
+            rule_engine = RuleEngine(args.openhab_uri, args.python_rule_directory, args.user, args.pwd)
+            rule_engine.start()
             run_server(port, self.description, rule_engine)
             return True
         elif args.command == 'register' and \
              args.openhab_uri is not None and \
              args.python_rule_directory is not None and \
              args.user is not None and \
              args.pwd is not None:
```

### Comparing `openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/app.py` & `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,23 +75,34 @@
 
 
 class Unit:
 
     def __init__(self, packagename: str):
         self.packagename = packagename
 
+    def __print_status(self, service: str):
+        try:
+            status = subprocess.check_output("sudo systemctl is-active " + service, shell=True, stderr=subprocess.STDOUT)
+            if status.decode('ascii').strip() == 'active':
+                print(service + " is running (print log by calling " + "sudo journalctl -n 20 -u " + service + ")")
+                return
+        except subprocess.CalledProcessError as e:
+            pass
+        print("Warning: " + service + " is not running")
+        system("sudo journalctl -n 20 -u " + service)
+
     def register(self, port: int, unit: str):
         service = self.servicename(port)
         unit_file_fullname = str(pathlib.Path("/", "etc", "systemd", "system", service))
         with open(unit_file_fullname, "w") as file:
             file.write(unit)
         system("sudo systemctl daemon-reload")
         system("sudo systemctl enable " + service)
         system("sudo systemctl restart " + service)
-        system("sudo systemctl status " + service)
+        self.__print_status(service)
 
     def deregister(self, port: int):
         service = self.servicename(port)
         unit_file_fullname = str(pathlib.Path("/", "etc", "systemd", "system", service))
         system("sudo systemctl stop " + service)
         system("sudo systemctl disable " + service)
         system("sudo systemctl daemon-reload")
```

### Comparing `openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/cache.py` & `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/cache.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/eventbus_consumer.py` & `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/eventbus_consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def start(self):
         self.thread = Thread(target=self.__listen, daemon=True)
         self.thread.start()
 
     def __listen(self):
         while self.is_running:
             try:
-                logging.debug("opening sse stream (" + self.event_uri + ")")
+                logging.info("opening sse stream (" + self.event_uri + ")")
                 response = requests.get(self.event_uri, stream=True)
                 client = sseclient.SSEClient(response)
 
                 try:
                     for event in client.events():
                         data = json.loads(event.data)
                         self.event_listener.on_event(data)
```

### Comparing `openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/invoke.py` & `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/invoke.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/item_registry.py` & `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/item_registry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import requests
 import logging
 from logging import INFO
 from dateutil import parser
 from datetime import datetime
 from dataclasses import dataclass
+from requests import Session
+from threading import RLock
 from requests.auth import HTTPBasicAuth
 from typing import Optional, List, Dict, Any
 from openhab_pythonrule_engine.cache import Cache
 
 
 logging = logging.getLogger(__name__)
 
@@ -65,14 +66,16 @@
         if value_to_serialize is None:
             return None
         elif type(value_to_serialize) == bool:
             return "ON" if value_to_serialize else "OFF"
         elif type(value_to_serialize) == datetime:
             return value_to_serialize.strftime('%Y-%m-%dT%H:%M:%S')
         elif type(value_to_serialize) == int:
+            return str(int(value_to_serialize))
+        elif type(value_to_serialize) == float:
             return str(float(value_to_serialize))
         else:
             return str(value_to_serialize)
 
 
 @dataclass
 class NumericItem(Item):
@@ -166,126 +169,175 @@
             item = TextItem(data['name'], read_only, group_names, None if (state == 'NULL' or state == 'UNDEF') else state)
         return item
     except Exception as e:
         logging.warning("error occurred mapping " + str(data) + " to item", e)
         return None
 
 
-
-
 class ItemRegistry:
-    __instance = None
-
-    @staticmethod
-    def new_singleton(openhab_uri: str, user: str, pwd: str):
-        item_registry = ItemRegistry(openhab_uri, user, pwd)
-        ItemRegistry.__instance = item_registry
-        return item_registry
-
-    @staticmethod
-    def instance():
-        return ItemRegistry.__instance
 
     def __init__(self, openhab_uri: str, user: str, pwd: str):
+        self.__last_updates = []
+        self.__last_failed_updates = []
         self.cache = Cache()
         self.credentials = HTTPBasicAuth(user, pwd)
+        self.__session = Session()
+        self.__lock = RLock()
         if openhab_uri.endswith("/"):
             self.openhab_uri = openhab_uri
         else:
             self.openhab_uri = openhab_uri + "/"
 
+    def __renew_session(self):
+        self.__session = Session()
+
+    @property
+    def last_updates(self) -> List[str]:
+        return self.__last_updates
+
+    @property
+    def last_update(self) -> Optional[str]:
+        if len(self.last_updates) > 0:
+            return self.last_updates[-1]
+        else:
+            return None
+
+    @property
+    def last_failed_updates(self) -> List[str]:
+        return self.__last_failed_updates
+
+    @property
+    def last_failed_update(self) -> Optional[str]:
+        if len(self.last_failed_updates) > 0:
+            return self.last_failed_updates[-1]
+        else:
+            return None
+
     def on_event(self, event):
         if event.get("type", "") == "ThingUpdatedEvent":
-            logging.info("config change. reset cache")
+            logging.debug("config change. reset cache")
             self.cache.clear()
 
     def get_items(self, use_cache: bool = False) -> Dict[str, Item]:
         items = self.cache.read_entry("items", 24 * 60 * 60)
         if items is not None:
             return items
         else:
-            uri = self.openhab_uri+ "rest/items"
+            with self.__lock:
+                uri = self.openhab_uri+ "rest/items"
+                try:
+                    response = self.__session.get(uri, headers={"Accept": "application/json"}, auth = self.credentials)
+                    if response.status_code == 200:
+                        items = {}
+                        for entry in response.json():
+                            item = to_item(entry)
+                            if item is not None:
+                                items[item.item_name] = item
+                        self.cache.add_enry("items", items)
+                        return items
+                    elif response.status_code == 404:
+                        raise Exception("item " +   uri + " not exists " + response.text)
+                    else:
+                        raise Exception("could not read item state " +   uri +  " got error " + response.text)
+                except Exception as e:
+                    self.__renew_session()
+                    logging.warning("error occurred by calling " + uri, e)
+
+    def get_item(self, item_name: str) -> Optional[Item]:
+        with self.__lock:
+            uri = self.openhab_uri+ "rest/items/" + item_name
             try:
-                response = requests.get(uri, headers={"Accept": "application/json"}, auth = self.credentials)
+                response = self.__session.get(uri, headers={"Accept": "application/json"}, auth = self.credentials)
                 if response.status_code == 200:
-                    items = {}
-                    for entry in response.json():
-                        item = to_item(entry)
-                        if item is not None:
-                            items[item.item_name] = item
-                    self.cache.add_enry("items", items)
-                    return items
+                    data = response.json()
+                    return to_item(data)
                 elif response.status_code == 404:
                     raise Exception("item " +   uri + " not exists " + response.text)
+                elif response.status_code == 401:
+                    raise Exception("auth error. user=" + self.credentials.username)
                 else:
-                    raise Exception("could not read item state " +   uri +  " got error " + response.text)
+                    raise Exception("could not read item state " +  uri +  " got error " + response.text)
             except Exception as e:
+                self.__renew_session()
                 logging.warning("error occurred by calling " + uri, e)
 
-    def get_item(self, item_name: str) -> Optional[Item]:
-        uri = self.openhab_uri+ "rest/items/" + item_name
-        try:
-            response = requests.get(uri, headers={"Accept": "application/json"}, auth = self.credentials)
-            if response.status_code == 200:
-                data = response.json()
-                return to_item(data)
-            elif response.status_code == 404:
-                raise Exception("item " +   uri + " not exists " + response.text)
-            elif response.status_code == 401:
-                raise Exception("auth error. user=" + self.credentials.username)
-            else:
-                raise Exception("could not read item state " +  uri +  " got error " + response.text)
-        except Exception as e:
-            logging.warning("error occurred by calling " + uri, e)
-
     def has_item(self, item_name: str) -> bool:
         if item_name is None:
             return False
         else:
             return self.get_item(item_name) != None
 
     def get_group_membernames(self, group_name) -> List[str]:
         return [item.item_name for item in self.get_items().values() if group_name in item.group_names]
 
+    def __on_last_update(self, item_name: str, value):
+        self.__last_updates.append("[" + datetime.now().strftime("%Y-%m-%dT%H:%M:%S") + "] new value " + item_name + ": " + str(value))
+        while len(self.__last_updates) > 20:
+            self.__last_updates.pop(0)
+
+    def __on_last_failed_update(self, item_name: str, value, error_message: str):
+        self.__last_failed_updates.append("[" + datetime.now().strftime("%Y-%m-%dT%H:%M:%S") + "] error occured by setting " + item_name + " with " + str(value) + "  " + error_message)
+        while len(self.__last_failed_updates) > 20:
+            self.__last_failed_updates.pop(0)
+
     def set_item_state(self, item_name: str, value: str):
-        uri = self.openhab_uri+ "rest/items/" + item_name
-        try:
-            response = requests.post(uri, data=value, headers={"Content-type": "text/plain"}, auth = self.credentials)
-            if response.status_code == 200:
-                return
-            elif response.status_code == 404:
-                raise Exception("item " +   uri + " not exists " + response.text)
-            elif response.status_code == 401:
-                raise Exception("auth error. user=" + self.credentials.username)
-            else:
-                raise Exception("could not update item state " +   uri +  " got error " + response.text)
-        except Exception as e:
-            logging.warning("error occurred by performing put on " + uri, e)
+        with self.__lock:
+            uri = self.openhab_uri+ "rest/items/" + item_name
+            try:
+                response = self.__session.post(uri, data=value, headers={"Content-type": "text/plain"}, auth = self.credentials)
+                if response.status_code == 200:
+                    self.__on_last_update(item_name, value)
+                    return
+                elif response.status_code == 404:
+                    txt = "item " +   uri + " not exists " + response.text
+                    self.__on_last_failed_update(item_name, value, txt)
+                    raise Exception(txt)
+                elif response.status_code == 401:
+                    txt = "auth error. user=" + self.credentials.username
+                    self.__on_last_failed_update(item_name, value, txt)
+                    raise Exception(txt)
+                else:
+                    txt = "could not update item state " +   uri +  " got error " + response.text
+                    self.__on_last_failed_update(item_name, value, txt)
+                    raise Exception(txt)
+            except Exception as e:
+                self.__renew_session()
+                logging.warning("error occurred by performing put on " + uri, e)
 
     def get_item_metadata(self, item_name: str) -> Optional[Item]:
         items_meta_data = self.get_items(use_cache=True)
         for name in items_meta_data.keys():
             if item_name == name:
                 return items_meta_data[item_name]
         return None
 
+    def __get_item_metadata_or_throw_error(self, item_name: str) -> Item:
+        item_metadata = self.get_item_metadata(item_name)
+        if item_metadata is None:
+            raise Exception("item " + item_name + " not exists")
+        else:
+            return item_metadata
+
     def get_state(self, item_name: str, dflt):
         state = self.get_item(item_name)
         if state is None or state.value is None:
             return dflt
         else:
             return state.get_state()
 
     def get_state_as_numeric(self, item_name: str, dflt: float=-1) -> float:
         state = self.get_item(item_name)
         if state is None or state.value is None:
             return dflt
         else:
             return state.get_state_as_numeric()
 
+    def get_state_as_int(self, item_name: str, dflt: float=-1) -> int:
+        return int(self.get_state_as_numeric(item_name, dflt))
+
     def get_state_as_boolean(self, item_name: str, dflt: bool=False) -> bool:
         state = self.get_item(item_name)
         if state is None or state.value is None:
             return dflt
         else:
             return state.get_state_as_boolean()
 
@@ -299,27 +351,35 @@
     def get_state_as_datetime(self, item_name: str, datetime_string: str="1970-01-01") -> datetime:
         state = self.get_item(item_name)
         if state is None or state.value is None:
             return parser.parse(datetime_string)
         else:
             return state.get_state_as_datetime()
 
+    def is_equals(self, state1: str, state2: str):
+        return state1 == state2
 
-    def set_state(self, item_name: str, new_state, reason: str = "", log_level: int = INFO) -> bool:
+    def __state_not_equals(self, item_name: str, new_state) -> bool:
+        try:
+            old_state = self.get_state(item_name, None)
+            item_metadata = self.__get_item_metadata_or_throw_error(item_name)
+            return item_metadata.serialize(old_state) != item_metadata.serialize(new_state)
+        except Exception as e:
+            logging.warning("error occurred fetching state of " + item_name + " " + str(e))
+            return True
+
+    def set_state(self, item_name: str, new_state, reason: str = "", log_level: int = INFO, force: bool = False) -> bool:
         if new_state is None:
             logging.warning("try to set " + item_name + " = None. ignoring it")
         else:
-            item_metadata = self.get_item_metadata(item_name)
-            if item_metadata is None:
-                raise Exception("item " + item_name + " not exists")
-            else:
-                old_state = self.get_state(item_name, None)
-                serialized_old_sate = item_metadata.serialize(old_state)
-                serialized_new_state = item_metadata.serialize(new_state)
-                if serialized_old_sate != serialized_new_state:
+            if force or self.__state_not_equals(item_name, new_state):
+                try:
+                    serialized_new_state = self.__get_item_metadata_or_throw_error(item_name).serialize(new_state)
                     try:
                         self.set_item_state(item_name, serialized_new_state)
                         logging.log(log_level, "set " + item_name + " = " + serialized_new_state + " " + reason)
                         return True
                     except Exception as e:
-                        logging.warning("could not set " + item_name + " = " + serialized_new_state, e)
+                        logging.warning("could not set " + item_name + " = " + str(serialized_new_state) + " " + str(e))
+                except Exception as e:
+                    logging.warning("could not serialized value " + str(new_state) + " to update " + item_name + " " + str(e))
         return False
```

### Comparing `openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/rule_engine_webthing.py` & `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine/rule_engine_webthing.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,70 @@
 from webthing import (Value, Property, Thing, SingleThing, WebThingServer)
 import tornado.ioloop
 import logging
-from openhab_pythonrule_engine.rule_engine import RuleEngine, Rule
+from openhab_pythonrule_engine.rule_engine import RuleEngine
 
 
 class RuleEngineThing(Thing):
 
     def __init__(self, description: str, rule_engine: RuleEngine):
         Thing.__init__(
             self,
             'urn:dev:ops:pythonrule_engine-1',
             'python_rule',
             [],
             description
         )
 
         self.rule_engine = rule_engine
-        rule_engine.add_event_listener(self.on_event)
-        rule_engine.add_cron_listener(self.on_cron)
 
-        self.last_events = Value("")
+        self.openhab_uri = Value(self.rule_engine.openhab_uri)
         self.add_property(
             Property(self,
-                     'last_events',
-                     self.last_events,
+                     'openhab_uri',
+                     self.openhab_uri,
                      metadata={
-                         'title': 'last_events',
+                         'title': 'openhab URI',
                          'type': 'string',
-                         'description': 'the line break delimited newest events',
+                         'description': 'the connected openhab instance',
                          'readOnly': True
                      }))
 
-        self.last_handled_events = Value("")
+        self.loaded_modules = Value("")
         self.add_property(
             Property(self,
-                     'last_handled_events',
-                     self.last_handled_events,
+                     'loaded_modules',
+                     self.loaded_modules,
                      metadata={
-                         'title': 'last_handled_events',
+                         'title': 'loaded modules',
                          'type': 'string',
-                         'description': 'the line break delimited newest handled events',
-                         'readOnly': True
-                     }))
-
-        self.last_crons = Value("")
-        self.add_property(
-            Property(self,
-                     'last_crons',
-                     self.last_crons,
-                     metadata={
-                         'title': 'last_crons',
-                         'type': 'string',
-                         'description': 'the line break delimited newest cron executions',
+                         'description': 'the list of loaded modules',
                          'readOnly': True
                      }))
 
         self.ioloop = tornado.ioloop.IOLoop.current()
 
 
     def on_event(self):
-        self.ioloop.add_callback(self.__handle_event)
-
-    def __handle_event(self):
-        self.last_events.notify_of_external_update('\r\n'.join(self.rule_engine.last_events))
-        self.last_handled_events.notify_of_external_update('\r\n'.join(self.rule_engine.last_handled_events))
+        self.ioloop.add_callback(self.__handle)
 
     def on_cron(self):
-        self.ioloop.add_callback(self.__handle_cron)
-
-    def __handle_cron(self):
-        self.last_crons.notify_of_external_update('\r\n'.join(self.rule_engine.last_crons))
-
+        self.ioloop.add_callback(self.__handle)
 
+    def __handle(self):
+        self.loaded_modules.notify_of_external_update(", ".join(sorted(list(self.rule_engine.loaded_modules))))
 
 
 def run_server(port: int, description: str, rule_engine: RuleEngine):
     rule_engine_webthing = RuleEngineThing(description, rule_engine)
     server = WebThingServer(SingleThing(rule_engine_webthing), port=port, disable_host_validation=True)
 
     try:
         # start webthing server
         logging.info('starting the server listing on ' + str(port))
         server.start()
     except KeyboardInterrupt:
         logging.info('stopping the server')
         server.stop()
+        rule_engine.stop()
         logging.info('done')
```

### Comparing `openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine.egg-info/PKG-INFO` & `openhab_pythonrule_engine-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openhab-pythonrule-engine
-Version: 1.1.9
+Name: openhab_pythonrule_engine
+Version: 1.2.0
 Summary: Openhab python rule engine
 Home-page: https://github.com/grro/openhab_pythonrule_engine
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # OpenHAB python rule engine
         A python 3.x rule engine for OpenHAB. This rule engine allows defining rule by using python 3.x.
```

### Comparing `openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine.egg-info/SOURCES.txt` & `openhab_pythonrule_engine-1.2.0/openhab_pythonrule_engine.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 README.md
 setup.py
 openhab_pythonrule_engine/__init__.py
 openhab_pythonrule_engine/app.py
 openhab_pythonrule_engine/cache.py
 openhab_pythonrule_engine/condition.py
+openhab_pythonrule_engine/cron_processor.py
 openhab_pythonrule_engine/eventbus_consumer.py
 openhab_pythonrule_engine/invoke.py
+openhab_pythonrule_engine/item_change_processor.py
 openhab_pythonrule_engine/item_registry.py
+openhab_pythonrule_engine/loaded_rule_processor.py
+openhab_pythonrule_engine/processor.py
 openhab_pythonrule_engine/rule_engine.py
 openhab_pythonrule_engine/rule_engine_webthing.py
+openhab_pythonrule_engine/source_scanner.py
 openhab_pythonrule_engine/trigger.py
 openhab_pythonrule_engine.egg-info/PKG-INFO
 openhab_pythonrule_engine.egg-info/SOURCES.txt
 openhab_pythonrule_engine.egg-info/dependency_links.txt
 openhab_pythonrule_engine.egg-info/entry_points.txt
 openhab_pythonrule_engine.egg-info/requires.txt
 openhab_pythonrule_engine.egg-info/top_level.txt
```

### Comparing `openhab_pythonrule_engine-1.1.9/setup.py` & `openhab_pythonrule_engine-1.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             ENTRY_POINT + '=' + PACKAGENAME + ':main'
         ]
     },
     keywords=[
         'webthings', 'home automation', 'openhab', 'python3', 'python', 'rules'
     ],
     install_requires=[
-        'webthing==0.15.0', 'requests==2.26.0', 'sseclient-py==1.7.2', 'watchdog==2.1.6', 'pycron==3.0.0', 'python-dateutil==2.8.2'
+        'webthing', 'requests', 'sseclient-py>=1.7.2', 'watchdog>=2.1.6', 'pycron>=3.0.0', 'python-dateutil>=2.8.2'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Development Status :: 3 - Alpha"
     ],
```

