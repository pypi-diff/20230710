# Comparing `tmp/nonebot-plugin-cfassistant-1.1.tar.gz` & `tmp/nonebot-plugin-cfassistant-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-cfassistant-1.1.tar", last modified: Sat Jul  8 16:36:12 2023, max compression
+gzip compressed data, was "nonebot-plugin-cfassistant-1.2.tar", last modified: Mon Jul 10 02:01:04 2023, max compression
```

## Comparing `nonebot-plugin-cfassistant-1.1.tar` & `nonebot-plugin-cfassistant-1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 16:36:12.468580 nonebot-plugin-cfassistant-1.1/
--rw-rw-rw-   0        0        0      264 2023-07-08 16:36:12.468580 nonebot-plugin-cfassistant-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3184 2023-07-08 01:30:14.000000 nonebot-plugin-cfassistant-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 16:36:12.455833 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant/
--rw-rw-rw-   0        0        0     6503 2023-07-07 15:44:48.000000 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant/__init__.py
--rw-rw-rw-   0        0        0     3784 2023-07-08 12:01:28.000000 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant/changeRemind.py
--rw-rw-rw-   0        0        0    10468 2023-07-08 12:12:18.000000 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant/updateContest.py
--rw-rw-rw-   0        0        0     6085 2023-07-08 12:34:24.000000 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant/updateUser.py
-drwxrwxrwx   0        0        0        0 2023-07-08 16:36:12.467074 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant.egg-info/
--rw-rw-rw-   0        0        0      264 2023-07-08 16:36:12.000000 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      483 2023-07-08 16:36:12.000000 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 16:36:12.000000 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-08 16:36:00.000000 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      115 2023-07-08 16:36:12.000000 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-07-08 16:36:12.000000 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 16:36:12.469589 nonebot-plugin-cfassistant-1.1/setup.cfg
--rw-rw-rw-   0        0        0      633 2023-07-08 16:35:38.000000 nonebot-plugin-cfassistant-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 02:01:04.555825 nonebot-plugin-cfassistant-1.2/
+-rw-rw-rw-   0        0        0      264 2023-07-10 02:01:04.555825 nonebot-plugin-cfassistant-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3184 2023-07-08 01:30:14.000000 nonebot-plugin-cfassistant-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 02:01:04.537855 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant/
+-rw-rw-rw-   0        0        0     6503 2023-07-07 15:44:48.000000 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant/__init__.py
+-rw-rw-rw-   0        0        0     3784 2023-07-08 12:01:28.000000 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant/changeRemind.py
+-rw-rw-rw-   0        0        0    10451 2023-07-10 01:53:20.000000 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant/updateContest.py
+-rw-rw-rw-   0        0        0     6043 2023-07-10 01:56:49.000000 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant/updateUser.py
+drwxrwxrwx   0        0        0        0 2023-07-10 02:01:04.552824 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant.egg-info/
+-rw-rw-rw-   0        0        0      264 2023-07-10 02:01:04.000000 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2023-07-10 02:01:04.000000 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 02:01:04.000000 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-10 02:00:54.000000 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      130 2023-07-10 02:01:04.000000 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-07-10 02:01:04.000000 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 02:01:04.556825 nonebot-plugin-cfassistant-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      660 2023-07-10 01:57:44.000000 nonebot-plugin-cfassistant-1.2/setup.py
```

### Comparing `nonebot-plugin-cfassistant-1.1/README.md` & `nonebot-plugin-cfassistant-1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant/__init__.py` & `nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant/changeRemind.py` & `nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant/changeRemind.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant/updateContest.py` & `nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant/updateContest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import requests
+import aiohttp
 import json
 import datetime
 import aiosqlite
 import asyncio 
 import os
 
 contest_url = "https://codeforces.com/api/contest.list?gym=false"
@@ -64,28 +64,27 @@
         self.relativeTimeShow=relativeTimeShow
         self.remindStatus=0
 
 
 async def updateContest():
     Contests=[]
     try:
-        response = requests.get(contest_url)
-        response.raise_for_status()  # 检查响应是否成功，如果不成功会抛出异常
-        data = json.loads(response.text)
-    except requests.RequestException as e:
+        async with aiohttp.ClientSession() as session:
+            async with session.get(contest_url) as response:
+                response.raise_for_status()  # 检查响应是否成功，如果不成功会抛出异常
+                data = await response.json()
+    except aiohttp.ClientError as e:
         print("请求错误:", e)
         return Contests
     except json.JSONDecodeError as e:
         print("JSON解析错误:", e)
         return Contests
-        # 处理JSON解析异常的情况
     except Exception as e:
         print("发生了其他错误:", e)
         return Contests
-        # 处理其他未预料到的异常情况
 
     # 检查API响应状态
     if data["status"] == "OK":
         # 获取result列表
         results = data["result"]
         # 遍历每个结果并储存键值
         for result in results:
```

### Comparing `nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant/updateUser.py` & `nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant/updateUser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import requests
+import aiohttp
 import json
 import datetime
 import aiosqlite
 import asyncio 
 import time
 user_info_baseurl="https://codeforces.com/api/user.info?handles="
 import os
@@ -38,28 +38,27 @@
         self.status=status if status is not None else 1
         self.last_rating=last_rating if last_rating is not None else 0
 
 
 async def addUser(id,QQ):
     user_info_url=user_info_baseurl+id
     try:
-        response = requests.get(user_info_url)
-        response.raise_for_status()  # 检查响应是否成功，如果不成功会抛出异常
-        data = json.loads(response.text)
-    except requests.RequestException as e:
+        async with aiohttp.ClientSession() as session:
+            async with session.get(user_info_url) as response:
+                response.raise_for_status()  # 检查响应是否成功，如果不成功会抛出异常
+                data = await response.json()
+    except aiohttp.ClientError as e:
         print("请求错误:", e)
-        return False 
+        return False
     except json.JSONDecodeError as e:
         print("JSON解析错误:", e)
         return False
-        # 处理JSON解析异常的情况
     except Exception as e:
         print("发生了其他错误:", e)
         return False
-        # 处理其他未预料到的异常情况
 
     # 检查API响应状态
     if data["status"] == "OK":
         # 获取result列表
         results = data["result"]
         
         # 遍历每个结果并储存键值
@@ -95,28 +94,27 @@
         if not RS:
             return Users
         for row in RS:
             Oid, Onow_rating, Oupdate_time, OQQ, Ostatus ,Olast_rating = row
             user_info_url=user_info_baseurl+Oid
             time.sleep(0.3)
             try:
-                response = requests.get(user_info_url)
-                response.raise_for_status()  # 检查响应是否成功，如果不成功会抛出异常
-                data = json.loads(response.text)
-            except requests.RequestException as e:
+                async with aiohttp.ClientSession() as session:
+                    async with session.get(user_info_url) as response:
+                        response.raise_for_status()  # 检查响应是否成功，如果不成功会抛出异常
+                        data = await response.json()
+            except aiohttp.ClientError as e:
                 print("请求错误:", e)
                 continue
             except json.JSONDecodeError as e:
                 print("JSON解析错误:", e)
                 continue
-                # 处理JSON解析异常的情况
             except Exception as e:
                 print("发生了其他错误:", e)
                 continue
-                # 处理其他未预料到的异常情况
 
             # 检查API响应状态
             if data["status"] == "OK":
                 # 获取result列表
                 results = data["result"]
                 
                 # 遍历每个结果并储存键值
```

### Comparing `nonebot-plugin-cfassistant-1.1/setup.py` & `nonebot-plugin-cfassistant-1.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = '1.1'
+VERSION = '1.2'
 
 setup(
     name='nonebot-plugin-cfassistant', 
     version=VERSION,  
     description='一个支持CF(codeforces)平台查询比赛/比赛提醒/监测分数变化的nonebot机器人插件', 
     packages=find_packages(),
     zip_safe=False,
     url='https://github.com/coyude/nonebot-plugin-cfassistant',
     author="coyude",
     install_requires=[
         "requests>=2.23.0",
         "nonebot_plugin_apscheduler>=0.3.0",
         "nonebot2>=2.0.0",
         "nonebot-adapter-onebot>=2.2.3",
-        "aiosqlite>=0.17.0"
+        "aiosqlite>=0.17.0",
+        "aiohttp>=3.8.0"
     ],
 )
```

