# Comparing `tmp/nonebot-plugin-blocker-0.1.6.tar.gz` & `tmp/nonebot-plugin-blocker-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-blocker-0.1.6.tar", last modified: Mon Jul 10 17:02:09 2023, max compression
+gzip compressed data, was "nonebot-plugin-blocker-0.1.7.tar", last modified: Mon Jul 10 20:07:14 2023, max compression
```

## Comparing `nonebot-plugin-blocker-0.1.6.tar` & `nonebot-plugin-blocker-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:02:09.145594 nonebot-plugin-blocker-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-10 17:02:09.145594 nonebot-plugin-blocker-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-10 17:01:50.000000 nonebot-plugin-blocker-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:02:09.145594 nonebot-plugin-blocker-0.1.6/nonebot_plugin_blocker/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-10 17:01:50.000000 nonebot-plugin-blocker-0.1.6/nonebot_plugin_blocker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-10 17:01:50.000000 nonebot-plugin-blocker-0.1.6/nonebot_plugin_blocker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-10 17:01:50.000000 nonebot-plugin-blocker-0.1.6/nonebot_plugin_blocker/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:02:09.145594 nonebot-plugin-blocker-0.1.6/nonebot_plugin_blocker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-10 17:02:09.000000 nonebot-plugin-blocker-0.1.6/nonebot_plugin_blocker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-10 17:02:09.000000 nonebot-plugin-blocker-0.1.6/nonebot_plugin_blocker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 17:02:09.000000 nonebot-plugin-blocker-0.1.6/nonebot_plugin_blocker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 17:02:09.000000 nonebot-plugin-blocker-0.1.6/nonebot_plugin_blocker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 17:02:09.000000 nonebot-plugin-blocker-0.1.6/nonebot_plugin_blocker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-10 17:01:50.000000 nonebot-plugin-blocker-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 17:02:09.145594 nonebot-plugin-blocker-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:07:14.371394 nonebot-plugin-blocker-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-10 20:07:14.367393 nonebot-plugin-blocker-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-10 20:06:57.000000 nonebot-plugin-blocker-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:07:14.367393 nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-10 20:06:57.000000 nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-10 20:06:57.000000 nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-10 20:06:57.000000 nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:07:14.367393 nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-10 20:07:14.000000 nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-10 20:07:14.000000 nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:07:14.000000 nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 20:07:14.000000 nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 20:07:14.000000 nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-10 20:06:57.000000 nonebot-plugin-blocker-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 20:07:14.371394 nonebot-plugin-blocker-0.1.7/setup.cfg
```

### Comparing `nonebot-plugin-blocker-0.1.6/PKG-INFO` & `nonebot-plugin-blocker-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.1.6
+Version: 0.1.7
 Summary: Message Blocker
 Author-email: MerCuJerry <mercujerry@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/MerCuJerry/nonebot-plugin-blocker
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.7 Summary:
 Message Blocker Author-email: MerCuJerry
 gmail.com> License: MIT Project-URL: homepage, https://github.com/MerCuJerry/
 nonebot-plugin-blocker Requires-Python: <4.0,>=3.8 Description-Content-Type:
 text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
```

### Comparing `nonebot-plugin-blocker-0.1.6/README.md` & `nonebot-plugin-blocker-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-blocker-0.1.6/nonebot_plugin_blocker/__main__.py` & `nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,37 +10,40 @@
 from nonebot.matcher import Matcher
 import re
 from nonebot.message import run_preprocessor
 from .config import BlockerList
 
 blockerlist: BlockerList
 
-blocker = on_regex(r"^[.。]bot (on|off)$",permission= GROUP_ADMIN | GROUP_OWNER | SUPERUSER, priority=2)
+blocker = on_regex(r"^[.。]bot (on|off)$",permission= GROUP_ADMIN | GROUP_OWNER | SUPERUSER, priority=2,block=True)
 
 @driver.on_startup
 async def load_blocker_on_start():
     global blockerlist
     blockerlist = BlockerList()
 
 @driver.on_shutdown
 async def save_blocker_on_shut():
     global blockerlist
     del blockerlist
 
 @run_preprocessor
 async def blocker_hook(matcher: Matcher,event: GroupMessageEvent):
-    if blockerlist.check_blocker(event.group_id) and re.match('[.。]bot (on|off)',event.get_plaintext()) is None:
+    if blockerlist.check_blocker(event.group_id, event.self_id) and re.match('[.。]bot (on|off)',event.get_plaintext()) is None:
         logger.info("[Blocker]Your Message is Blocked By Blocker.")
         await matcher.finish()
         
 @blocker.handle()
 async def blocker_msg_handle(matcher: Matcher,event: GroupMessageEvent):
     if event.get_plaintext().find('on') != -1:
         msg_type , msg_data = blockerlist.get_on_reply()
-        blockerlist.del_blocker(event.group_id)
+        blockerlist.del_blocker(event.group_id, event.self_id)
         logger.info("[Blocker]Delete Blocker Successful.")
-        await matcher.finish(MessageSegment(type=msg_type,data=msg_data))
+        if msg_type is None:
+            await matcher.finish('在本群开启')
     elif event.get_plaintext().find('off') != -1:
         msg_type , msg_data = blockerlist.get_off_reply()
-        blockerlist.add_blocker(event.group_id)
+        blockerlist.add_blocker(event.group_id, event.self_id)
         logger.info("[Blocker]Add Blocker Successful.")
-        await matcher.finish(MessageSegment(type=msg_type,data=msg_data))
+        if msg_type is None:
+            await matcher.finish('在本群关闭')
+    await matcher.finish(MessageSegment(type=msg_type,data=msg_data))
```

### Comparing `nonebot-plugin-blocker-0.1.6/nonebot_plugin_blocker/config.py` & `nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,55 +3,67 @@
 
 DATA_PATH = Path.cwd() / "data" / "blocker"
 if not DATA_PATH.exists():
     DATA_PATH.mkdir(parents=True)
 
 BLOCKLIST_JSON_PATH = DATA_PATH / "blocklist.json"
 if not BLOCKLIST_JSON_PATH.exists():
-    BLOCKLIST_JSON_PATH.write_text('[]',encoding='u8')
+    BLOCKLIST_JSON_PATH.write_text('{}',encoding='u8')
 
 REPLY_JSON_PATH = DATA_PATH / "blocker_reply.json"
 if not REPLY_JSON_PATH.exists():
     tmp_dict = {}
     tmp_dict['reply_on']={'type':'text','data':{'text':'在本群开启'}}
     tmp_dict['reply_off']={'type':'text','data':{'text':'在本群关闭'}}
     with REPLY_JSON_PATH.open('w', encoding='UTF-8') as file:
             json.dump(tmp_dict, file, ensure_ascii=False)
 
 class BlockerList:
     blocker_reply : dict
-    blocklist : list[int]
+    blocklist : dict[str,list[int]]
 
     def __init__(self):
         with BLOCKLIST_JSON_PATH.open('r', encoding='UTF-8') as file:
             self.blocklist = json.load(file)
+            if type(self.blocklist) != dict:
+                self.blocklist = {}
         with REPLY_JSON_PATH.open('r', encoding='UTF-8') as file:
             self.blocker_reply = json.load(file)
+            if type(self.blocker_reply) != dict:
+                self.blocker_reply = {}
             
     def get_on_reply(self):
-        return self.blocker_reply['reply_on']['type'],self.blocker_reply['reply_on']['data']
+        try:
+            return self.blocker_reply['reply_on']['type'], self.blocker_reply['reply_on']['data']
+        except:
+            return None, None
     
     def get_off_reply(self):
-        return self.blocker_reply['reply_off']['type'],self.blocker_reply['reply_off']['data']    
+        try:
+            return self.blocker_reply['reply_off']['type'], self.blocker_reply['reply_off']['data'] 
+        except:
+            return None, None 
     
-    def add_blocker(self,gid: int):
+    def add_blocker(self,gid: int, qid: int):
         try:
-            self.blocklist.index(gid)
+            self.blocklist[str(qid)].index(gid)
         except ValueError:
-            self.blocklist.append(gid)
+            self.blocklist[str(qid)].append(gid)
+        except KeyError:
+            self.blocklist.setdefault(str(qid),[gid])
         
-    def del_blocker(self,gid: int):
+    def del_blocker(self,gid: int, qid: int):
         try:
-            self.blocklist.remove(gid)
+            self.blocklist[str(qid)].remove(gid)
         except ValueError:
             pass
         
-    def check_blocker(self,gid: int) -> bool:
+    def check_blocker(self,gid: int, qid: int) -> bool:
         try:
-            self.blocklist.index(gid)
+            self.blocklist[str(qid)].index(gid)
         except:
             return False
         else:
             return True
 
     def __del__(self):
         with BLOCKLIST_JSON_PATH.open('w', encoding='UTF-8') as file:
```

### Comparing `nonebot-plugin-blocker-0.1.6/nonebot_plugin_blocker.egg-info/PKG-INFO` & `nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.1.6
+Version: 0.1.7
 Summary: Message Blocker
 Author-email: MerCuJerry <mercujerry@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/MerCuJerry/nonebot-plugin-blocker
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.7 Summary:
 Message Blocker Author-email: MerCuJerry
 gmail.com> License: MIT Project-URL: homepage, https://github.com/MerCuJerry/
 nonebot-plugin-blocker Requires-Python: <4.0,>=3.8 Description-Content-Type:
 text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
```

