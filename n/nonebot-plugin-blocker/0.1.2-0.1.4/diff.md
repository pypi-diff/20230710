# Comparing `tmp/nonebot-plugin-blocker-0.1.2.tar.gz` & `tmp/nonebot-plugin-blocker-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-blocker-0.1.2.tar", last modified: Mon Jul 10 15:26:52 2023, max compression
+gzip compressed data, was "nonebot-plugin-blocker-0.1.4.tar", last modified: Mon Jul 10 16:34:12 2023, max compression
```

## Comparing `nonebot-plugin-blocker-0.1.2.tar` & `nonebot-plugin-blocker-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:26:52.369463 nonebot-plugin-blocker-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-10 15:26:52.369463 nonebot-plugin-blocker-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-10 15:26:32.000000 nonebot-plugin-blocker-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:26:52.365463 nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-10 15:26:32.000000 nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-10 15:26:32.000000 nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-10 15:26:32.000000 nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:26:52.365463 nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-10 15:26:52.000000 nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-10 15:26:52.000000 nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 15:26:52.000000 nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 15:26:52.000000 nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 15:26:52.000000 nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-10 15:26:32.000000 nonebot-plugin-blocker-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 15:26:52.369463 nonebot-plugin-blocker-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:34:12.867934 nonebot-plugin-blocker-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-10 16:34:12.867934 nonebot-plugin-blocker-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-10 16:33:52.000000 nonebot-plugin-blocker-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:34:12.867934 nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-10 16:33:52.000000 nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-10 16:33:52.000000 nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-10 16:33:52.000000 nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:34:12.867934 nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-10 16:34:12.000000 nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-10 16:34:12.000000 nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:34:12.000000 nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 16:34:12.000000 nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 16:34:12.000000 nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-10 16:33:52.000000 nonebot-plugin-blocker-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 16:34:12.867934 nonebot-plugin-blocker-0.1.4/setup.cfg
```

### Comparing `nonebot-plugin-blocker-0.1.2/PKG-INFO` & `nonebot-plugin-blocker-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.1.2
+Version: 0.1.4
 Summary: Message Blocker
 Author-email: MerCuJerry <mercujerry@gmail.com>
 License: MIT
+Project-URL: homepage, https://github.com/MerCuJerry/nonebot-plugin-blocker
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
@@ -26,20 +27,17 @@
 <a href="https://pypi.python.org/pypi/nonebot-plugin-blocker">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-blocker.svg" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 </div>
 
-这是一个 nonebot2 插件项目，用于分群配置机器人的开启关闭
-
 ## 📖 介绍
 
-使用.bot on在该群开启bot
-使用.bot off在该群关闭bot
+这是一个 nonebot2 插件项目，用于分群配置机器人的开启关闭
 
 ## 💿 安装
 <details>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
 <details>
@@ -50,26 +48,35 @@
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
     plugins = ["nonebot-plugin-blocker"]
 
 </details>
 
-## 配置
-
-在 nonebot2 根目录下面的data目录里找到blocker 编辑里面的blocker_reply
+## ⚙️ 配置
 
+插件的配置文件位于 `data/blocker/blocker_reply.json` 里
+```jsonc
     {
         "reply_on":{
             "type":"text"
             "data":{
                 "text":"在本群开启"
             }
         },
         "reply_off":{
             "type":"text"
             "data":{
                 "text":"在本群关闭"
             }
         }
     }
-    
+```
+`data/blocker/blocklist.json` 里是已经设置关闭Bot的群号，可以在关闭nonebot之后手动编辑
+
+## 💬 指令
+
+指令只有管理员，群主以及Bot的SUPERUSER能够使用
+
+### .bot on在该群开启bot
+
+### .bot off在该群关闭bot
```

#### html2text {}

```diff
@@ -1,18 +1,22 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.4 Summary:
 Message Blocker Author-email: MerCuJerry
-gmail.com> License: MIT Requires-Python: <4.0,>=3.8 Description-Content-Type:
+gmail.com> License: MIT Project-URL: homepage, https://github.com/MerCuJerry/
+nonebot-plugin-blocker Requires-Python: <4.0,>=3.8 Description-Content-Type:
 text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
                                    [python]
-è¿æ¯ä¸ä¸ª nonebot2 æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­
-## ð ä»ç» ä½¿ç¨.bot onå¨è¯¥ç¾¤å¼å¯bot ä½¿ç¨.bot offå¨è¯¥ç¾¤å³é­bot
-## ð¿ å®è£  ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
+## ð ä»ç» è¿æ¯ä¸ä¸ª nonebot2
+æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­ ## ð¿ å®è£
+ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-blocker  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot-plugin-blocker"]  ## éç½® å¨ nonebot2
-æ ¹ç®å½ä¸é¢çdataç®å½éæ¾å°blocker ç¼è¾éé¢çblocker_reply
-{ "reply_on":{ "type":"text" "data":{ "text":"å¨æ¬ç¾¤å¼å¯" } },
-"reply_off":{ "type":"text" "data":{ "text":"å¨æ¬ç¾¤å³é­" } } }
+["nonebot-plugin-blocker"]  ## âï¸ éç½® æä»¶çéç½®æä»¶ä½äº `data/
+blocker/blocker_reply.json` é ```jsonc { "reply_on":{ "type":"text" "data":
+{ "text":"å¨æ¬ç¾¤å¼å¯" } }, "reply_off":{ "type":"text" "data":{ "text":
+"å¨æ¬ç¾¤å³é­" } } } ``` `data/blocker/blocklist.json`
+éæ¯å·²ç»è®¾ç½®å³é­Botçç¾¤å·ï¼å¯ä»¥å¨å³é­nonebotä¹åæå¨ç¼è¾
+## ð¬ æä»¤ æä»¤åªæç®¡çåï¼ç¾¤ä¸»ä»¥åBotçSUPERUSERè½å¤ä½¿ç¨
+### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot
```

### Comparing `nonebot-plugin-blocker-0.1.2/README.md` & `nonebot-plugin-blocker-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,20 +17,17 @@
 <a href="https://pypi.python.org/pypi/nonebot-plugin-blocker">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-blocker.svg" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 </div>
 
-这是一个 nonebot2 插件项目，用于分群配置机器人的开启关闭
-
 ## 📖 介绍
 
-使用.bot on在该群开启bot
-使用.bot off在该群关闭bot
+这是一个 nonebot2 插件项目，用于分群配置机器人的开启关闭
 
 ## 💿 安装
 <details>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
 <details>
@@ -41,26 +38,35 @@
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
     plugins = ["nonebot-plugin-blocker"]
 
 </details>
 
-## 配置
-
-在 nonebot2 根目录下面的data目录里找到blocker 编辑里面的blocker_reply
+## ⚙️ 配置
 
+插件的配置文件位于 `data/blocker/blocker_reply.json` 里
+```jsonc
     {
         "reply_on":{
             "type":"text"
             "data":{
                 "text":"在本群开启"
             }
         },
         "reply_off":{
             "type":"text"
             "data":{
                 "text":"在本群关闭"
             }
         }
     }
-    
+```
+`data/blocker/blocklist.json` 里是已经设置关闭Bot的群号，可以在关闭nonebot之后手动编辑
+
+## 💬 指令
+
+指令只有管理员，群主以及Bot的SUPERUSER能够使用
+
+### .bot on在该群开启bot
+
+### .bot off在该群关闭bot
```

#### html2text {}

```diff
@@ -1,14 +1,17 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
                                    [python]
-è¿æ¯ä¸ä¸ª nonebot2 æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­
-## ð ä»ç» ä½¿ç¨.bot onå¨è¯¥ç¾¤å¼å¯bot ä½¿ç¨.bot offå¨è¯¥ç¾¤å³é­bot
-## ð¿ å®è£  ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
+## ð ä»ç» è¿æ¯ä¸ä¸ª nonebot2
+æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­ ## ð¿ å®è£
+ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-blocker  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot-plugin-blocker"]  ## éç½® å¨ nonebot2
-æ ¹ç®å½ä¸é¢çdataç®å½éæ¾å°blocker ç¼è¾éé¢çblocker_reply
-{ "reply_on":{ "type":"text" "data":{ "text":"å¨æ¬ç¾¤å¼å¯" } },
-"reply_off":{ "type":"text" "data":{ "text":"å¨æ¬ç¾¤å³é­" } } }
+["nonebot-plugin-blocker"]  ## âï¸ éç½® æä»¶çéç½®æä»¶ä½äº `data/
+blocker/blocker_reply.json` é ```jsonc { "reply_on":{ "type":"text" "data":
+{ "text":"å¨æ¬ç¾¤å¼å¯" } }, "reply_off":{ "type":"text" "data":{ "text":
+"å¨æ¬ç¾¤å³é­" } } } ``` `data/blocker/blocklist.json`
+éæ¯å·²ç»è®¾ç½®å³é­Botçç¾¤å·ï¼å¯ä»¥å¨å³é­nonebotä¹åæå¨ç¼è¾
+## ð¬ æä»¤ æä»¤åªæç®¡çåï¼ç¾¤ä¸»ä»¥åBotçSUPERUSERè½å¤ä½¿ç¨
+### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot
```

### Comparing `nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker/__main__.py` & `nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,34 +4,35 @@
     from nonebot.adapters.onebot.v12 import GroupMessageEvent, MessageSegment, GROUP_ADMIN, GROUP_OWNER
 else:
     from nonebot.adapters.onebot.v11 import GroupMessageEvent, MessageSegment, GROUP_ADMIN, GROUP_OWNER
 
 from nonebot.permission import SUPERUSER
 from nonebot import on_regex, logger
 from nonebot.matcher import Matcher
+import re
 from nonebot.message import run_preprocessor
 from .config import BlockerList
 
 blockerlist: BlockerList
 
-blocker = on_regex(r"^.bot (on|off)$",permission= GROUP_ADMIN | GROUP_OWNER | SUPERUSER, priority=2)
+blocker = on_regex(r"^[.。]bot (on|off)$",permission= GROUP_ADMIN | GROUP_OWNER | SUPERUSER, priority=2)
 
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
-    if blockerlist.check_blocker(event.group_id) and event.get_plaintext().find(".bot") == -1:
+    if blockerlist.check_blocker(event.group_id) and re.match('[.。]bot (on|off)',event.get_plaintext()) is None:
         logger.info("[Blocker]Your Message is Blocked By Blocker.")
         await matcher.finish()
         
 @blocker.handle()
 async def blocker_msg_handle(matcher: Matcher,event: GroupMessageEvent):
     if event.get_plaintext().find('on') != -1:
         msg_type , msg_data = blockerlist.get_on_reply()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker/config.py` & `nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker.egg-info/PKG-INFO` & `nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.1.2
+Version: 0.1.4
 Summary: Message Blocker
 Author-email: MerCuJerry <mercujerry@gmail.com>
 License: MIT
+Project-URL: homepage, https://github.com/MerCuJerry/nonebot-plugin-blocker
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
@@ -26,20 +27,17 @@
 <a href="https://pypi.python.org/pypi/nonebot-plugin-blocker">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-blocker.svg" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 </div>
 
-这是一个 nonebot2 插件项目，用于分群配置机器人的开启关闭
-
 ## 📖 介绍
 
-使用.bot on在该群开启bot
-使用.bot off在该群关闭bot
+这是一个 nonebot2 插件项目，用于分群配置机器人的开启关闭
 
 ## 💿 安装
 <details>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
 <details>
@@ -50,26 +48,35 @@
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
     plugins = ["nonebot-plugin-blocker"]
 
 </details>
 
-## 配置
-
-在 nonebot2 根目录下面的data目录里找到blocker 编辑里面的blocker_reply
+## ⚙️ 配置
 
+插件的配置文件位于 `data/blocker/blocker_reply.json` 里
+```jsonc
     {
         "reply_on":{
             "type":"text"
             "data":{
                 "text":"在本群开启"
             }
         },
         "reply_off":{
             "type":"text"
             "data":{
                 "text":"在本群关闭"
             }
         }
     }
-    
+```
+`data/blocker/blocklist.json` 里是已经设置关闭Bot的群号，可以在关闭nonebot之后手动编辑
+
+## 💬 指令
+
+指令只有管理员，群主以及Bot的SUPERUSER能够使用
+
+### .bot on在该群开启bot
+
+### .bot off在该群关闭bot
```

#### html2text {}

```diff
@@ -1,18 +1,22 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.4 Summary:
 Message Blocker Author-email: MerCuJerry
-gmail.com> License: MIT Requires-Python: <4.0,>=3.8 Description-Content-Type:
+gmail.com> License: MIT Project-URL: homepage, https://github.com/MerCuJerry/
+nonebot-plugin-blocker Requires-Python: <4.0,>=3.8 Description-Content-Type:
 text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
                                    [python]
-è¿æ¯ä¸ä¸ª nonebot2 æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­
-## ð ä»ç» ä½¿ç¨.bot onå¨è¯¥ç¾¤å¼å¯bot ä½¿ç¨.bot offå¨è¯¥ç¾¤å³é­bot
-## ð¿ å®è£  ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
+## ð ä»ç» è¿æ¯ä¸ä¸ª nonebot2
+æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­ ## ð¿ å®è£
+ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-blocker  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot-plugin-blocker"]  ## éç½® å¨ nonebot2
-æ ¹ç®å½ä¸é¢çdataç®å½éæ¾å°blocker ç¼è¾éé¢çblocker_reply
-{ "reply_on":{ "type":"text" "data":{ "text":"å¨æ¬ç¾¤å¼å¯" } },
-"reply_off":{ "type":"text" "data":{ "text":"å¨æ¬ç¾¤å³é­" } } }
+["nonebot-plugin-blocker"]  ## âï¸ éç½® æä»¶çéç½®æä»¶ä½äº `data/
+blocker/blocker_reply.json` é ```jsonc { "reply_on":{ "type":"text" "data":
+{ "text":"å¨æ¬ç¾¤å¼å¯" } }, "reply_off":{ "type":"text" "data":{ "text":
+"å¨æ¬ç¾¤å³é­" } } } ``` `data/blocker/blocklist.json`
+éæ¯å·²ç»è®¾ç½®å³é­Botçç¾¤å·ï¼å¯ä»¥å¨å³é­nonebotä¹åæå¨ç¼è¾
+## ð¬ æä»¤ æä»¤åªæç®¡çåï¼ç¾¤ä¸»ä»¥åBotçSUPERUSERè½å¤ä½¿ç¨
+### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot
```

