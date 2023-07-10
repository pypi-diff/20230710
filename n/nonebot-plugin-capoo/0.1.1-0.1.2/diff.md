# Comparing `tmp/nonebot_plugin_capoo-0.1.1.tar.gz` & `tmp/nonebot_plugin_capoo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_capoo-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_capoo-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_capoo-0.1.1.tar` & `nonebot_plugin_capoo-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-09 10:46:20.018078 nonebot_plugin_capoo-0.1.1/LICENSE
--rw-r--r--   0        0        0     3840 2023-07-09 10:46:20.018078 nonebot_plugin_capoo-0.1.1/README.md
--rw-r--r--   0        0        0     4478 2023-07-09 10:46:20.022078 nonebot_plugin_capoo-0.1.1/nonebot_plugin_capoo/__init__.py
--rw-r--r--   0        0        0      520 2023-07-09 10:46:20.022078 nonebot_plugin_capoo-0.1.1/nonebot_plugin_capoo/config.py
--rw-r--r--   0        0        0     2805 2023-07-09 10:46:20.022078 nonebot_plugin_capoo-0.1.1/nonebot_plugin_capoo/download.py
--rw-r--r--   0        0        0      469 2023-07-09 10:46:20.022078 nonebot_plugin_capoo-0.1.1/nonebot_plugin_capoo/sqlite.py
--rw-r--r--   0        0        0      599 2023-07-09 10:46:20.022078 nonebot_plugin_capoo-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4692 1970-01-01 00:00:00.000000 nonebot_plugin_capoo-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-10 14:29:30.893785 nonebot_plugin_capoo-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3840 2023-07-10 14:29:30.893785 nonebot_plugin_capoo-0.1.2/README.md
+-rw-r--r--   0        0        0     4478 2023-07-10 14:29:30.897786 nonebot_plugin_capoo-0.1.2/nonebot_plugin_capoo/__init__.py
+-rw-r--r--   0        0        0      520 2023-07-10 14:29:30.897786 nonebot_plugin_capoo-0.1.2/nonebot_plugin_capoo/config.py
+-rw-r--r--   0        0        0     2805 2023-07-10 14:29:30.897786 nonebot_plugin_capoo-0.1.2/nonebot_plugin_capoo/download.py
+-rw-r--r--   0        0        0      469 2023-07-10 14:29:30.897786 nonebot_plugin_capoo-0.1.2/nonebot_plugin_capoo/sqlite.py
+-rw-r--r--   0        0        0      603 2023-07-10 14:29:30.897786 nonebot_plugin_capoo-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4666 1970-01-01 00:00:00.000000 nonebot_plugin_capoo-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_capoo-0.1.1/LICENSE` & `nonebot_plugin_capoo-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_capoo-0.1.1/README.md` & `nonebot_plugin_capoo-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_capoo-0.1.1/nonebot_plugin_capoo/__init__.py` & `nonebot_plugin_capoo-0.1.2/nonebot_plugin_capoo/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_capoo-0.1.1/nonebot_plugin_capoo/config.py` & `nonebot_plugin_capoo-0.1.2/nonebot_plugin_capoo/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_capoo-0.1.1/nonebot_plugin_capoo/download.py` & `nonebot_plugin_capoo-0.1.2/nonebot_plugin_capoo/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_capoo-0.1.1/pyproject.toml` & `nonebot_plugin_capoo-0.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "nonebot-plugin-capoo"
-version = "0.1.1"
+version = "0.1.2"
 description = "一个发送 capoo 表情包的插件"
 authors = ["HuParry <huparry@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_capoo"}]
 homepage = "https://github.com/HuParry/nonebot-plugin-capoo"
 repository = "https://github.com/HuParry/nonebot-plugin-capoo"
 
 
 [tool.poetry.dependencies]
-python = "^3.8"
-nonebot2 = "^2.0.0"
-nonebot-adapter-onebot = "^2.2.3"
+python = ">=3.8"
+nonebot2 = ">=2.0.0"
+nonebot-adapter-onebot = ">=2.1.5"
 httpx = ">=0.20.0,<1.0.0"
-asyncio = "^3.4.3"
+asyncio = ">=3.4.3"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_capoo-0.1.1/PKG-INFO` & `nonebot_plugin_capoo-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-capoo
-Version: 0.1.1
+Version: 0.1.2
 Summary: 一个发送 capoo 表情包的插件
 Home-page: https://github.com/HuParry/nonebot-plugin-capoo
 License: MIT
 Author: HuParry
 Author-email: huparry@outlook.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: asyncio (>=3.4.3,<4.0.0)
+Requires-Dist: asyncio (>=3.4.3)
 Requires-Dist: httpx (>=0.20.0,<1.0.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
-Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.1.5)
+Requires-Dist: nonebot2 (>=2.0.0)
 Project-URL: Repository, https://github.com/HuParry/nonebot-plugin-capoo
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-capoo Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-capoo Version: 0.1.2 Summary:
 ä¸ä¸ªåé capoo è¡¨æåçæä»¶ Home-page: https://github.com/HuParry/
 nonebot-plugin-capoo License: MIT Author: HuParry Author-email:
-huparry@outlook.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: asyncio
-(>=3.4.3,<4.0.0) Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-Dist: nonebot-
-adapter-onebot (>=2.2.3,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
-Project-URL: Repository, https://github.com/HuParry/nonebot-plugin-capoo
-Description-Content-Type: text/markdown
+huparry@outlook.com Requires-Python: >=3.8 Classifier: License :: OSI Approved
+:: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Dist: asyncio (>=3.4.3)
+Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-Dist: nonebot-adapter-onebot
+(>=2.1.5) Requires-Dist: nonebot2 (>=2.0.0) Project-URL: Repository, https://
+github.com/HuParry/nonebot-plugin-capoo Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
        # nonebot-plugin-capoo _â¨ ä¸ä¸ªåéæä»¤å°±è½è®©ä½ ç bot
     ååºå¯ç±ç capoo çå¾ççæä»¶ â¨_ [license] [pypi] [python]
 ## ð ä»ç» capoo å®å¨æ¯å¤ªå¯ç±äºï¼æä»¥ææ¶éäºå ç¾å¼  capoo
 çè¡¨æåãè¿ä¸ªæä»¶ç¨äºè®© bot åé capoo çè¡¨æ¸åã
 ä¸å¼å§ççæ¬åªè½ç®åå°ä»æçå¾æºéåéè¡¨æåï¼å¨ v0.1.0
```

