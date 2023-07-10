# Comparing `tmp/nonebot-plugin-cfassistant-1.2.tar.gz` & `tmp/nonebot-plugin-cfassistant-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-cfassistant-1.2.tar", last modified: Mon Jul 10 02:01:04 2023, max compression
+gzip compressed data, was "nonebot-plugin-cfassistant-1.3.tar", last modified: Mon Jul 10 07:18:06 2023, max compression
```

## Comparing `nonebot-plugin-cfassistant-1.2.tar` & `nonebot-plugin-cfassistant-1.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 02:01:04.555825 nonebot-plugin-cfassistant-1.2/
--rw-rw-rw-   0        0        0      264 2023-07-10 02:01:04.555825 nonebot-plugin-cfassistant-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3184 2023-07-08 01:30:14.000000 nonebot-plugin-cfassistant-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 02:01:04.537855 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant/
--rw-rw-rw-   0        0        0     6503 2023-07-07 15:44:48.000000 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant/__init__.py
--rw-rw-rw-   0        0        0     3784 2023-07-08 12:01:28.000000 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant/changeRemind.py
--rw-rw-rw-   0        0        0    10451 2023-07-10 01:53:20.000000 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant/updateContest.py
--rw-rw-rw-   0        0        0     6043 2023-07-10 01:56:49.000000 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant/updateUser.py
-drwxrwxrwx   0        0        0        0 2023-07-10 02:01:04.552824 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant.egg-info/
--rw-rw-rw-   0        0        0      264 2023-07-10 02:01:04.000000 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      483 2023-07-10 02:01:04.000000 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 02:01:04.000000 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-10 02:00:54.000000 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      130 2023-07-10 02:01:04.000000 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-07-10 02:01:04.000000 nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 02:01:04.556825 nonebot-plugin-cfassistant-1.2/setup.cfg
--rw-rw-rw-   0        0        0      660 2023-07-10 01:57:44.000000 nonebot-plugin-cfassistant-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:18:06.888471 nonebot-plugin-cfassistant-1.3/
+-rw-rw-rw-   0        0        0      264 2023-07-10 07:18:06.887471 nonebot-plugin-cfassistant-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4528 2023-07-10 07:17:18.000000 nonebot-plugin-cfassistant-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 07:18:06.848349 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant/
+-rw-rw-rw-   0        0        0     6415 2023-07-10 06:57:00.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant/__init__.py
+-rw-rw-rw-   0        0        0     3784 2023-07-08 12:01:28.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant/changeRemind.py
+-rw-rw-rw-   0        0        0      110 2023-07-10 06:41:42.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant/randomProblems.py
+-rw-rw-rw-   0        0        0    10451 2023-07-10 01:53:20.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant/updateContest.py
+-rw-rw-rw-   0        0        0     6039 2023-07-10 06:54:58.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant/updateUser.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:18:06.881927 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant.egg-info/
+-rw-rw-rw-   0        0        0      264 2023-07-10 07:18:06.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-07-10 07:18:06.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 07:18:06.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-10 07:18:00.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      130 2023-07-10 07:18:06.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-07-10 07:18:06.000000 nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 07:18:06.889471 nonebot-plugin-cfassistant-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      660 2023-07-10 07:17:21.000000 nonebot-plugin-cfassistant-1.3/setup.py
```

### Comparing `nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant/__init__.py` & `nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,21 +24,21 @@
 
 
 data_path = './data/CFHelper/'
 if not os.path.exists(data_path):
     os.makedirs(data_path)
 
 timing = require("nonebot_plugin_apscheduler").scheduler
-getCF = on_command("CF", rule=to_me(), aliases={"查CF","查cf","cf"}, priority=10, block=True)
-PluginHelp=on_command("CFHELP", rule=to_me(), aliases={"cfhelp"}, priority=10, block=True)
-bind= on_command("绑定", rule=to_me(), aliases={"订阅","用户"}, priority=10, block=True)
-onGroupRemind = on_command("群提醒", rule=to_me(), priority=10, block=True)
-disGroupdRemind = on_command("取消群提醒", rule=to_me(), priority=10, block=True)
-onPrivateRemind = on_command("提醒", rule=to_me(), priority=10, block=True)
-disPrivateRemind = on_command("取消提醒", rule=to_me(), priority=10, block=True)
+getCF = on_command("CF",aliases={"查CF","查cf","cf","Cf","cF"}, priority=10, block=True)
+PluginHelp=on_command("CFHELP", aliases={"cfhelp"}, priority=10, block=True)
+bind= on_command("绑定", aliases={"订阅","用户"}, priority=10, block=True)
+onGroupRemind = on_command("群提醒", priority=10, block=True)
+disGroupdRemind = on_command("取消群提醒",  priority=10, block=True)
+onPrivateRemind = on_command("提醒", priority=10, block=True)
+disPrivateRemind = on_command("取消提醒", priority=10, block=True)
 
 
 @getCF.handle()
 async def getCF_fun():
     tasks_list = [
         asyncio.create_task(returnContestInfo())
     ]
```

### Comparing `nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant/changeRemind.py` & `nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant/changeRemind.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant/updateContest.py` & `nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant/updateContest.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cfassistant-1.2/nonebot_plugin_cfassistant/updateUser.py` & `nonebot-plugin-cfassistant-1.3/nonebot_plugin_cfassistant/updateUser.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,13 +152,13 @@
             output=f"当前时间：{datetime.datetime.now()}\n"
             await cursor.execute('SELECT now_rating,last_rating,QQ FROM User WHERE id = ?', (user.id,))
             row = await cursor.fetchone()
             if row is not None:
                 now_rating,last_rating,QQ = row
                 if last_rating!=now_rating:
                     change=now_rating-last_rating
-                    output+=f"检测到您的CF账号 {user.id} 分数发生变化，从{last_rating} → {now_rating}  变动了{change}分！\n"
+                    output+=f"检测到您的CF账号 {user.id} 分数发生变化，从{last_rating} → {now_rating}  变动了{change}分~"
                     outputlist.append({'QQ':QQ,'output':output})
             else:
                 continue
     return outputlist
```

### Comparing `nonebot-plugin-cfassistant-1.2/setup.py` & `nonebot-plugin-cfassistant-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = '1.2'
+VERSION = '1.3'
 
 setup(
     name='nonebot-plugin-cfassistant', 
     version=VERSION,  
     description='一个支持CF(codeforces)平台查询比赛/比赛提醒/监测分数变化的nonebot机器人插件', 
     packages=find_packages(),
     zip_safe=False,
```

