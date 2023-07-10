# Comparing `tmp/nonebot-plugin-blocker-0.1.0.tar.gz` & `tmp/nonebot-plugin-blocker-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-blocker-0.1.0.tar", last modified: Thu Jul  6 03:30:50 2023, max compression
+gzip compressed data, was "nonebot-plugin-blocker-0.1.1.tar", last modified: Mon Jul 10 14:30:07 2023, max compression
```

## Comparing `nonebot-plugin-blocker-0.1.0.tar` & `nonebot-plugin-blocker-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:30:50.147082 nonebot-plugin-blocker-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-06 03:30:50.147082 nonebot-plugin-blocker-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-06 03:30:39.000000 nonebot-plugin-blocker-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:30:50.143082 nonebot-plugin-blocker-0.1.0/nonebot_plugin_blocker/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-06 03:30:39.000000 nonebot-plugin-blocker-0.1.0/nonebot_plugin_blocker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-06 03:30:39.000000 nonebot-plugin-blocker-0.1.0/nonebot_plugin_blocker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-06 03:30:39.000000 nonebot-plugin-blocker-0.1.0/nonebot_plugin_blocker/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:30:50.147082 nonebot-plugin-blocker-0.1.0/nonebot_plugin_blocker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-06 03:30:50.000000 nonebot-plugin-blocker-0.1.0/nonebot_plugin_blocker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-06 03:30:50.000000 nonebot-plugin-blocker-0.1.0/nonebot_plugin_blocker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 03:30:50.000000 nonebot-plugin-blocker-0.1.0/nonebot_plugin_blocker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-06 03:30:50.000000 nonebot-plugin-blocker-0.1.0/nonebot_plugin_blocker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 03:30:50.000000 nonebot-plugin-blocker-0.1.0/nonebot_plugin_blocker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-06 03:30:39.000000 nonebot-plugin-blocker-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 03:30:50.147082 nonebot-plugin-blocker-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:30:07.379492 nonebot-plugin-blocker-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-10 14:30:07.379492 nonebot-plugin-blocker-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-10 14:29:54.000000 nonebot-plugin-blocker-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:30:07.379492 nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-10 14:29:54.000000 nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-10 14:29:54.000000 nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-10 14:29:54.000000 nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:30:07.379492 nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-10 14:30:07.000000 nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-10 14:30:07.000000 nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:30:07.000000 nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 14:30:07.000000 nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 14:30:07.000000 nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-10 14:29:54.000000 nonebot-plugin-blocker-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 14:30:07.379492 nonebot-plugin-blocker-0.1.1/setup.cfg
```

### Comparing `nonebot-plugin-blocker-0.1.0/PKG-INFO` & `nonebot-plugin-blocker-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.1.0
+Version: 0.1.1
 Summary: Message Blocker
 Author-email: MerCuJerry <mercujerry@gmail.com>
 License: MIT
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 
 <div align="center">
@@ -17,18 +17,18 @@
 
 # nonebot-plugin-blocker
 
 _✨ NoneBot Plugin Blocker ✨_
 
 
 <a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-example.svg" alt="license">
+    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-blocker.svg" alt="license">
 </a>
-<a href="https://pypi.python.org/pypi/nonebot-plugin-example">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-example.svg" alt="pypi">
+<a href="https://pypi.python.org/pypi/nonebot-plugin-blocker">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-blocker.svg" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 </div>
 
 这是一个 nonebot2 插件项目，用于分群配置机器人的开启关闭
 
@@ -49,7 +49,27 @@
 </details>
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
     plugins = ["nonebot-plugin-blocker"]
 
 </details>
+
+## 配置
+
+在 nonebot2 根目录下面的data目录里找到blocker 编辑里面的blocker_reply
+
+    {
+        "reply_on":{
+            "type":"text"
+            "data":{
+                "text":"在本群开启"
+            }
+        },
+        "reply_off":{
+            "type":"text"
+            "data":{
+                "text":"在本群关闭"
+            }
+        }
+    }
+
```

#### html2text {}

```diff
@@ -1,15 +1,18 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.1 Summary:
 Message Blocker Author-email: MerCuJerry
 gmail.com> License: MIT Requires-Python: <4.0,>=3.8 Description-Content-Type:
 text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
                                    [python]
 è¿æ¯ä¸ä¸ª nonebot2 æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­
 ## ð ä»ç» ä½¿ç¨.bot onå¨è¯¥ç¾¤å¼å¯bot ä½¿ç¨.bot offå¨è¯¥ç¾¤å³é­bot
 ## ð¿ å®è£  ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-blocker  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot-plugin-blocker"]
+["nonebot-plugin-blocker"]  ## éç½® å¨ nonebot2
+æ ¹ç®å½ä¸é¢çdataç®å½éæ¾å°blocker ç¼è¾éé¢çblocker_reply
+{ "reply_on":{ "type":"text" "data":{ "text":"å¨æ¬ç¾¤å¼å¯" } },
+"reply_off":{ "type":"text" "data":{ "text":"å¨æ¬ç¾¤å³é­" } } }
```

### Comparing `nonebot-plugin-blocker-0.1.0/README.md` & `nonebot-plugin-blocker-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 # nonebot-plugin-blocker
 
 _✨ NoneBot Plugin Blocker ✨_
 
 
 <a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-example.svg" alt="license">
+    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-blocker.svg" alt="license">
 </a>
-<a href="https://pypi.python.org/pypi/nonebot-plugin-example">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-example.svg" alt="pypi">
+<a href="https://pypi.python.org/pypi/nonebot-plugin-blocker">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-blocker.svg" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 </div>
 
 这是一个 nonebot2 插件项目，用于分群配置机器人的开启关闭
 
@@ -40,7 +40,27 @@
 </details>
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
     plugins = ["nonebot-plugin-blocker"]
 
 </details>
+
+## 配置
+
+在 nonebot2 根目录下面的data目录里找到blocker 编辑里面的blocker_reply
+
+    {
+        "reply_on":{
+            "type":"text"
+            "data":{
+                "text":"在本群开启"
+            }
+        },
+        "reply_off":{
+            "type":"text"
+            "data":{
+                "text":"在本群关闭"
+            }
+        }
+    }
+
```

#### html2text {}

```diff
@@ -4,8 +4,11 @@
                                    [python]
 è¿æ¯ä¸ä¸ª nonebot2 æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­
 ## ð ä»ç» ä½¿ç¨.bot onå¨è¯¥ç¾¤å¼å¯bot ä½¿ç¨.bot offå¨è¯¥ç¾¤å³é­bot
 ## ð¿ å®è£  ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-blocker  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot-plugin-blocker"]
+["nonebot-plugin-blocker"]  ## éç½® å¨ nonebot2
+æ ¹ç®å½ä¸é¢çdataç®å½éæ¾å°blocker ç¼è¾éé¢çblocker_reply
+{ "reply_on":{ "type":"text" "data":{ "text":"å¨æ¬ç¾¤å¼å¯" } },
+"reply_off":{ "type":"text" "data":{ "text":"å¨æ¬ç¾¤å³é­" } } }
```

### Comparing `nonebot-plugin-blocker-0.1.0/nonebot_plugin_blocker.egg-info/PKG-INFO` & `nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.1.0
+Version: 0.1.1
 Summary: Message Blocker
 Author-email: MerCuJerry <mercujerry@gmail.com>
 License: MIT
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 
 <div align="center">
@@ -17,18 +17,18 @@
 
 # nonebot-plugin-blocker
 
 _✨ NoneBot Plugin Blocker ✨_
 
 
 <a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-example.svg" alt="license">
+    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-blocker.svg" alt="license">
 </a>
-<a href="https://pypi.python.org/pypi/nonebot-plugin-example">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-example.svg" alt="pypi">
+<a href="https://pypi.python.org/pypi/nonebot-plugin-blocker">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-blocker.svg" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 </div>
 
 这是一个 nonebot2 插件项目，用于分群配置机器人的开启关闭
 
@@ -49,7 +49,27 @@
 </details>
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
     plugins = ["nonebot-plugin-blocker"]
 
 </details>
+
+## 配置
+
+在 nonebot2 根目录下面的data目录里找到blocker 编辑里面的blocker_reply
+
+    {
+        "reply_on":{
+            "type":"text"
+            "data":{
+                "text":"在本群开启"
+            }
+        },
+        "reply_off":{
+            "type":"text"
+            "data":{
+                "text":"在本群关闭"
+            }
+        }
+    }
+
```

#### html2text {}

```diff
@@ -1,15 +1,18 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.1 Summary:
 Message Blocker Author-email: MerCuJerry
 gmail.com> License: MIT Requires-Python: <4.0,>=3.8 Description-Content-Type:
 text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
                                    [python]
 è¿æ¯ä¸ä¸ª nonebot2 æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­
 ## ð ä»ç» ä½¿ç¨.bot onå¨è¯¥ç¾¤å¼å¯bot ä½¿ç¨.bot offå¨è¯¥ç¾¤å³é­bot
 ## ð¿ å®è£  ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-blocker  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot-plugin-blocker"]
+["nonebot-plugin-blocker"]  ## éç½® å¨ nonebot2
+æ ¹ç®å½ä¸é¢çdataç®å½éæ¾å°blocker ç¼è¾éé¢çblocker_reply
+{ "reply_on":{ "type":"text" "data":{ "text":"å¨æ¬ç¾¤å¼å¯" } },
+"reply_off":{ "type":"text" "data":{ "text":"å¨æ¬ç¾¤å³é­" } } }
```

