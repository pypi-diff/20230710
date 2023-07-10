# Comparing `tmp/nonebot_plugin_cp_broadcast-0.2.0.tar.gz` & `tmp/nonebot_plugin_cp_broadcast-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cp_broadcast-0.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_cp_broadcast-0.2.1.tar", max compression
```

## Comparing `nonebot_plugin_cp_broadcast-0.2.0.tar` & `nonebot_plugin_cp_broadcast-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2023-07-08 04:01:16.961115 nonebot_plugin_cp_broadcast-0.2.0/LICENSE
--rw-r--r--   0        0        0     4494 2023-07-08 04:01:16.961115 nonebot_plugin_cp_broadcast-0.2.0/README.md
--rw-r--r--   0        0        0     7431 2023-07-08 04:01:16.965115 nonebot_plugin_cp_broadcast-0.2.0/nonebot_plugin_cp_broadcast/__init__.py
--rw-r--r--   0        0        0     2503 2023-07-08 04:01:16.965115 nonebot_plugin_cp_broadcast-0.2.0/nonebot_plugin_cp_broadcast/atcoder.py
--rw-r--r--   0        0        0     1946 2023-07-08 04:01:16.965115 nonebot_plugin_cp_broadcast-0.2.0/nonebot_plugin_cp_broadcast/codeforces.py
--rw-r--r--   0        0        0      432 2023-07-08 04:01:16.965115 nonebot_plugin_cp_broadcast-0.2.0/nonebot_plugin_cp_broadcast/config.py
--rw-r--r--   0        0        0     2416 2023-07-08 04:01:16.965115 nonebot_plugin_cp_broadcast-0.2.0/nonebot_plugin_cp_broadcast/nowcoder.py
--rw-r--r--   0        0        0      766 2023-07-08 04:01:16.965115 nonebot_plugin_cp_broadcast-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5444 1970-01-01 00:00:00.000000 nonebot_plugin_cp_broadcast-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-10 14:24:36.954228 nonebot_plugin_cp_broadcast-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4494 2023-07-10 14:24:36.954228 nonebot_plugin_cp_broadcast-0.2.1/README.md
+-rw-r--r--   0        0        0     7505 2023-07-10 14:24:36.958228 nonebot_plugin_cp_broadcast-0.2.1/nonebot_plugin_cp_broadcast/__init__.py
+-rw-r--r--   0        0        0     2503 2023-07-10 14:24:36.958228 nonebot_plugin_cp_broadcast-0.2.1/nonebot_plugin_cp_broadcast/atcoder.py
+-rw-r--r--   0        0        0     1946 2023-07-10 14:24:36.958228 nonebot_plugin_cp_broadcast-0.2.1/nonebot_plugin_cp_broadcast/codeforces.py
+-rw-r--r--   0        0        0      432 2023-07-10 14:24:36.958228 nonebot_plugin_cp_broadcast-0.2.1/nonebot_plugin_cp_broadcast/config.py
+-rw-r--r--   0        0        0     2416 2023-07-10 14:24:36.958228 nonebot_plugin_cp_broadcast-0.2.1/nonebot_plugin_cp_broadcast/nowcoder.py
+-rw-r--r--   0        0        0      771 2023-07-10 14:24:36.958228 nonebot_plugin_cp_broadcast-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5503 1970-01-01 00:00:00.000000 nonebot_plugin_cp_broadcast-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_cp_broadcast-0.2.0/LICENSE` & `nonebot_plugin_cp_broadcast-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.2.0/README.md` & `nonebot_plugin_cp_broadcast-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.2.0/nonebot_plugin_cp_broadcast/__init__.py` & `nonebot_plugin_cp_broadcast-0.2.1/nonebot_plugin_cp_broadcast/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     supported_adapters = {"nonebot.adapters.onebot.v11"},
 )
 
 
 try:
     scheduler = require("nonebot_plugin_apscheduler").scheduler
 except BaseException:
+    logger.warning('未检测到定时插件，定时功能将不启用')
     scheduler = None
 ###列表下标0为比赛名称、下标1为比赛时间、下标2为比赛链接
 
 async def ans_today():  #today
     global cf
     global atc
     global nc
```

### Comparing `nonebot_plugin_cp_broadcast-0.2.0/nonebot_plugin_cp_broadcast/atcoder.py` & `nonebot_plugin_cp_broadcast-0.2.1/nonebot_plugin_cp_broadcast/atcoder.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.2.0/nonebot_plugin_cp_broadcast/codeforces.py` & `nonebot_plugin_cp_broadcast-0.2.1/nonebot_plugin_cp_broadcast/codeforces.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.2.0/nonebot_plugin_cp_broadcast/nowcoder.py` & `nonebot_plugin_cp_broadcast-0.2.1/nonebot_plugin_cp_broadcast/nowcoder.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.2.0/pyproject.toml` & `nonebot_plugin_cp_broadcast-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "nonebot-plugin-cp-broadcast"
-version = "0.2.0"
+version = "0.2.1"
 description = "Codeforces、牛客、AtCoder平台比赛查询，ACMer 必备"
 authors = ["HuParry <huparry@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_cp_broadcast"}]
 homepage = "https://github.com/HuParry/nonebot-plugin-cp-broadcast"
 repository = "https://github.com/HuParry/nonebot-plugin-cp-broadcast"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.8"
 nonebot2 = { version = "^2.0.0", extras = ["fastapi"] }
-nonebot-adapter-onebot = "^2.2.2"
+nonebot-adapter-onebot = ">=2.1.5"
 httpx = ">=0.20.0,<1.0.0"
-nonebot-plugin-apscheduler = "^0.3.0"
-fake-useragent = "^1.1.3"
-bs4 = "^0.0.1"
-asyncio = "^3.4.3"
+nonebot-plugin-apscheduler = ">=0.3.0"
+fake-useragent = ">=1.1.3"
+bs4 = ">=0.0.1"
+asyncio = ">=3.4.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_cp_broadcast-0.2.0/PKG-INFO` & `nonebot_plugin_cp_broadcast-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cp-broadcast
-Version: 0.2.0
+Version: 0.2.1
 Summary: Codeforces、牛客、AtCoder平台比赛查询，ACMer 必备
 Home-page: https://github.com/HuParry/nonebot-plugin-cp-broadcast
 License: MIT
 Author: HuParry
 Author-email: huparry@outlook.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: asyncio (>=3.4.3,<4.0.0)
-Requires-Dist: bs4 (>=0.0.1,<0.0.2)
-Requires-Dist: fake-useragent (>=1.1.3,<2.0.0)
+Requires-Dist: asyncio (>=3.4.3)
+Requires-Dist: bs4 (>=0.0.1)
+Requires-Dist: fake-useragent (>=1.1.3)
 Requires-Dist: httpx (>=0.20.0,<1.0.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0)
-Requires-Dist: nonebot-plugin-apscheduler (>=0.3.0,<0.4.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.1.5)
+Requires-Dist: nonebot-plugin-apscheduler (>=0.3.0)
 Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/HuParry/nonebot-plugin-cp-broadcast
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-cp-broadcast Version: 0.2.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-cp-broadcast Version: 0.2.1 Summary:
 Codeforcesãçå®¢ãAtCoderå¹³å°æ¯èµæ¥è¯¢ï¼ACMer å¿å¤ Home-page:
 https://github.com/HuParry/nonebot-plugin-cp-broadcast License: MIT Author:
-HuParry Author-email: huparry@outlook.com Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: asyncio
-(>=3.4.3,<4.0.0) Requires-Dist: bs4 (>=0.0.1,<0.0.2) Requires-Dist: fake-
-useragent (>=1.1.3,<2.0.0) Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-
-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0) Requires-Dist: nonebot-plugin-
-apscheduler (>=0.3.0,<0.4.0) Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
-Project-URL: Repository, https://github.com/HuParry/nonebot-plugin-cp-broadcast
-Description-Content-Type: text/markdown
+HuParry Author-email: huparry@outlook.com Requires-Python: >=3.8 Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Dist: asyncio (>=3.4.3) Requires-Dist: bs4 (>=0.0.1) Requires-Dist: fake-
+useragent (>=1.1.3) Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-Dist:
+nonebot-adapter-onebot (>=2.1.5) Requires-Dist: nonebot-plugin-apscheduler
+(>=0.3.0) Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0) Project-URL:
+Repository, https://github.com/HuParry/nonebot-plugin-cp-broadcast Description-
+Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-cp-broadcast _â¨ ä¸ä¸ª Codeforcesãçå®¢ç«èµãAtCoder
 å¹³å°çç¼ç¨ç«èµæ¥è¯¢æä»¶ï¼ACMerå¿å¤ â¨_ [license] [pypi] [python]
 ## ð ä»ç» å¯¹äºæ¯ä¸ä¸ª ACMer
 æ¥è¯´ï¼åå ç¼ç¨ç«èµæ¯å¿ä¸å¯å°çï¼è¿ä¸ªæä»¶å®ç°äº
 Codeforcesãçå®¢ç«èµãAtCoder
```

