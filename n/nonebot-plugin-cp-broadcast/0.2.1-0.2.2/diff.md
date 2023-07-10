# Comparing `tmp/nonebot_plugin_cp_broadcast-0.2.1.tar.gz` & `tmp/nonebot_plugin_cp_broadcast-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cp_broadcast-0.2.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_cp_broadcast-0.2.2.tar", max compression
```

## Comparing `nonebot_plugin_cp_broadcast-0.2.1.tar` & `nonebot_plugin_cp_broadcast-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2023-07-10 14:24:36.954228 nonebot_plugin_cp_broadcast-0.2.1/LICENSE
--rw-r--r--   0        0        0     4494 2023-07-10 14:24:36.954228 nonebot_plugin_cp_broadcast-0.2.1/README.md
--rw-r--r--   0        0        0     7505 2023-07-10 14:24:36.958228 nonebot_plugin_cp_broadcast-0.2.1/nonebot_plugin_cp_broadcast/__init__.py
--rw-r--r--   0        0        0     2503 2023-07-10 14:24:36.958228 nonebot_plugin_cp_broadcast-0.2.1/nonebot_plugin_cp_broadcast/atcoder.py
--rw-r--r--   0        0        0     1946 2023-07-10 14:24:36.958228 nonebot_plugin_cp_broadcast-0.2.1/nonebot_plugin_cp_broadcast/codeforces.py
--rw-r--r--   0        0        0      432 2023-07-10 14:24:36.958228 nonebot_plugin_cp_broadcast-0.2.1/nonebot_plugin_cp_broadcast/config.py
--rw-r--r--   0        0        0     2416 2023-07-10 14:24:36.958228 nonebot_plugin_cp_broadcast-0.2.1/nonebot_plugin_cp_broadcast/nowcoder.py
--rw-r--r--   0        0        0      771 2023-07-10 14:24:36.958228 nonebot_plugin_cp_broadcast-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5503 1970-01-01 00:00:00.000000 nonebot_plugin_cp_broadcast-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-10 15:31:10.955522 nonebot_plugin_cp_broadcast-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4488 2023-07-10 15:31:10.955522 nonebot_plugin_cp_broadcast-0.2.2/README.md
+-rw-r--r--   0        0        0     7505 2023-07-10 15:31:10.955522 nonebot_plugin_cp_broadcast-0.2.2/nonebot_plugin_cp_broadcast/__init__.py
+-rw-r--r--   0        0        0     2503 2023-07-10 15:31:10.955522 nonebot_plugin_cp_broadcast-0.2.2/nonebot_plugin_cp_broadcast/atcoder.py
+-rw-r--r--   0        0        0     1946 2023-07-10 15:31:10.955522 nonebot_plugin_cp_broadcast-0.2.2/nonebot_plugin_cp_broadcast/codeforces.py
+-rw-r--r--   0        0        0      438 2023-07-10 15:31:10.955522 nonebot_plugin_cp_broadcast-0.2.2/nonebot_plugin_cp_broadcast/config.py
+-rw-r--r--   0        0        0     2416 2023-07-10 15:31:10.955522 nonebot_plugin_cp_broadcast-0.2.2/nonebot_plugin_cp_broadcast/nowcoder.py
+-rw-r--r--   0        0        0      732 2023-07-10 15:31:10.955522 nonebot_plugin_cp_broadcast-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5445 1970-01-01 00:00:00.000000 nonebot_plugin_cp_broadcast-0.2.2/PKG-INFO
```

### Comparing `nonebot_plugin_cp_broadcast-0.2.1/LICENSE` & `nonebot_plugin_cp_broadcast-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.2.1/README.md` & `nonebot_plugin_cp_broadcast-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | cp_broadcast_list | 否 | [ ] | 开启早晨自动播报今日比赛的群聊，填 QQ 群号，注意以字符串形式填入 |
 | cp_broadcast_botname | 否 | "bot" | 填入你 bot 的名字，在 `help` 指令下会使用到你的 bot 的名字 |
 | cp_broadcast_time | 否 | {"hour":"7", "minute":"20"} | 每日在群聊播报比赛信息的时间，默认是早上 7 点 20，你可以在配置文件中按默认值格式修改成你想要的时间 |
 | cp_broadcast_updatetime | 否 | {"hour":"0", "minute":"0"} | 每天自动更新比赛数据的时间，默认是 0 点 0 分，你可以在配置文件中按默认值格式修改成你想要的时间 |
 
-该插件依赖 [nonebot_plugin_apscheduler](https://github.com/nonebot/plugin-apscheduler) 实现定时发送功能，如果你是通过下载项目源码安装插件的话，请注意安装好依赖。
+该插件依赖 [nonebot_plugin_apscheduler](https://github.com/nonebot/plugin-apscheduler) 实现定时发送功能，如果你未安装此依赖的话，将无法触发与定时相关的功能。
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | `cf` | 群员 | 否 | 群聊 | 发送最近三场 Codeforces 比赛的信息 |
 | `牛客` or `nc` | 群员 | 否 | 群聊 | 发送最近三场牛客比赛的信息 |
```

#### html2text {}

```diff
@@ -35,15 +35,15 @@
 æ¯æ¥å¨ç¾¤èæ­æ¥æ¯èµä¿¡æ¯çæ¶é´ï¼é»è®¤æ¯æ©ä¸ 7 ç¹
 20ï¼ä½ å¯ä»¥å¨éç½®æä»¶ä¸­æé»è®¤å¼æ ¼å¼ä¿®æ¹æä½ æ³è¦çæ¶é´ |
 | cp_broadcast_updatetime | å¦ | {"hour":"0", "minute":"0"} |
 æ¯å¤©èªå¨æ´æ°æ¯èµæ°æ®çæ¶é´ï¼é»è®¤æ¯ 0 ç¹ 0
 åï¼ä½ å¯ä»¥å¨éç½®æä»¶ä¸­æé»è®¤å¼æ ¼å¼ä¿®æ¹æä½ æ³è¦çæ¶é´
 | è¯¥æä»¶ä¾èµ [nonebot_plugin_apscheduler](https://github.com/nonebot/
 plugin-apscheduler)
-å®ç°å®æ¶åéåè½ï¼å¦æä½ æ¯éè¿ä¸è½½é¡¹ç®æºç å®è£æä»¶çè¯ï¼è¯·æ³¨æå®è£å¥½ä¾èµã
+å®ç°å®æ¶åéåè½ï¼å¦æä½ æªå®è£æ­¤ä¾èµçè¯ï¼å°æ æ³è§¦åä¸å®æ¶ç¸å³çåè½ã
 ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:
 -----:|:----:|:----:|:----:|:----:| | `cf` | ç¾¤å | å¦ | ç¾¤è |
 åéæè¿ä¸åº Codeforces æ¯èµçä¿¡æ¯ | | `çå®¢` or `nc` | ç¾¤å |
 å¦ | ç¾¤è | åéæè¿ä¸åºçå®¢æ¯èµçä¿¡æ¯ | | `atc` | ç¾¤å | å¦
 | ç¾¤è | åéæè¿ä¸¤åº AtCoder æ¯èµçä¿¡æ¯ | | `today` | ç¾¤å |
 å¦ | ç¾¤è | åéä»å¤©çæ¯èµä¿¡æ¯ | | `next` | ç¾¤å | å¦ | ç¾¤è |
 åéä»å¤©åçé¨åæ¯èµä¿¡æ¯ | | `help` | ç¾¤å | æ¯ | ç¾¤è |
```

### Comparing `nonebot_plugin_cp_broadcast-0.2.1/nonebot_plugin_cp_broadcast/__init__.py` & `nonebot_plugin_cp_broadcast-0.2.2/nonebot_plugin_cp_broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.2.1/nonebot_plugin_cp_broadcast/atcoder.py` & `nonebot_plugin_cp_broadcast-0.2.2/nonebot_plugin_cp_broadcast/atcoder.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.2.1/nonebot_plugin_cp_broadcast/codeforces.py` & `nonebot_plugin_cp_broadcast-0.2.2/nonebot_plugin_cp_broadcast/codeforces.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.2.1/nonebot_plugin_cp_broadcast/nowcoder.py` & `nonebot_plugin_cp_broadcast-0.2.2/nonebot_plugin_cp_broadcast/nowcoder.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.2.1/pyproject.toml` & `nonebot_plugin_cp_broadcast-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "nonebot-plugin-cp-broadcast"
-version = "0.2.1"
+version = "0.2.2"
 description = "Codeforces、牛客、AtCoder平台比赛查询，ACMer 必备"
 authors = ["HuParry <huparry@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_cp_broadcast"}]
 homepage = "https://github.com/HuParry/nonebot-plugin-cp-broadcast"
 repository = "https://github.com/HuParry/nonebot-plugin-cp-broadcast"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 nonebot2 = { version = "^2.0.0", extras = ["fastapi"] }
 nonebot-adapter-onebot = ">=2.1.5"
 httpx = ">=0.20.0,<1.0.0"
-nonebot-plugin-apscheduler = ">=0.3.0"
 fake-useragent = ">=1.1.3"
 bs4 = ">=0.0.1"
 asyncio = ">=3.4.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_cp_broadcast-0.2.1/PKG-INFO` & `nonebot_plugin_cp_broadcast-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cp-broadcast
-Version: 0.2.1
+Version: 0.2.2
 Summary: Codeforces、牛客、AtCoder平台比赛查询，ACMer 必备
 Home-page: https://github.com/HuParry/nonebot-plugin-cp-broadcast
 License: MIT
 Author: HuParry
 Author-email: huparry@outlook.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncio (>=3.4.3)
 Requires-Dist: bs4 (>=0.0.1)
 Requires-Dist: fake-useragent (>=1.1.3)
 Requires-Dist: httpx (>=0.20.0,<1.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.5)
-Requires-Dist: nonebot-plugin-apscheduler (>=0.3.0)
 Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/HuParry/nonebot-plugin-cp-broadcast
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
@@ -110,15 +109,15 @@
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | cp_broadcast_list | 否 | [ ] | 开启早晨自动播报今日比赛的群聊，填 QQ 群号，注意以字符串形式填入 |
 | cp_broadcast_botname | 否 | "bot" | 填入你 bot 的名字，在 `help` 指令下会使用到你的 bot 的名字 |
 | cp_broadcast_time | 否 | {"hour":"7", "minute":"20"} | 每日在群聊播报比赛信息的时间，默认是早上 7 点 20，你可以在配置文件中按默认值格式修改成你想要的时间 |
 | cp_broadcast_updatetime | 否 | {"hour":"0", "minute":"0"} | 每天自动更新比赛数据的时间，默认是 0 点 0 分，你可以在配置文件中按默认值格式修改成你想要的时间 |
 
-该插件依赖 [nonebot_plugin_apscheduler](https://github.com/nonebot/plugin-apscheduler) 实现定时发送功能，如果你是通过下载项目源码安装插件的话，请注意安装好依赖。
+该插件依赖 [nonebot_plugin_apscheduler](https://github.com/nonebot/plugin-apscheduler) 实现定时发送功能，如果你未安装此依赖的话，将无法触发与定时相关的功能。
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | `cf` | 群员 | 否 | 群聊 | 发送最近三场 Codeforces 比赛的信息 |
 | `牛客` or `nc` | 群员 | 否 | 群聊 | 发送最近三场牛客比赛的信息 |
```

#### html2text {}

```diff
@@ -1,21 +1,20 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-cp-broadcast Version: 0.2.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-cp-broadcast Version: 0.2.2 Summary:
 Codeforcesãçå®¢ãAtCoderå¹³å°æ¯èµæ¥è¯¢ï¼ACMer å¿å¤ Home-page:
 https://github.com/HuParry/nonebot-plugin-cp-broadcast License: MIT Author:
 HuParry Author-email: huparry@outlook.com Requires-Python: >=3.8 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: asyncio (>=3.4.3) Requires-Dist: bs4 (>=0.0.1) Requires-Dist: fake-
 useragent (>=1.1.3) Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-Dist:
-nonebot-adapter-onebot (>=2.1.5) Requires-Dist: nonebot-plugin-apscheduler
-(>=0.3.0) Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0) Project-URL:
-Repository, https://github.com/HuParry/nonebot-plugin-cp-broadcast Description-
-Content-Type: text/markdown
+nonebot-adapter-onebot (>=2.1.5) Requires-Dist: nonebot2[fastapi]
+(>=2.0.0,<3.0.0) Project-URL: Repository, https://github.com/HuParry/nonebot-
+plugin-cp-broadcast Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-cp-broadcast _â¨ ä¸ä¸ª Codeforcesãçå®¢ç«èµãAtCoder
 å¹³å°çç¼ç¨ç«èµæ¥è¯¢æä»¶ï¼ACMerå¿å¤ â¨_ [license] [pypi] [python]
 ## ð ä»ç» å¯¹äºæ¯ä¸ä¸ª ACMer
 æ¥è¯´ï¼åå ç¼ç¨ç«èµæ¯å¿ä¸å¯å°çï¼è¿ä¸ªæä»¶å®ç°äº
 Codeforcesãçå®¢ç«èµãAtCoder
@@ -49,15 +48,15 @@
 æ¯æ¥å¨ç¾¤èæ­æ¥æ¯èµä¿¡æ¯çæ¶é´ï¼é»è®¤æ¯æ©ä¸ 7 ç¹
 20ï¼ä½ å¯ä»¥å¨éç½®æä»¶ä¸­æé»è®¤å¼æ ¼å¼ä¿®æ¹æä½ æ³è¦çæ¶é´ |
 | cp_broadcast_updatetime | å¦ | {"hour":"0", "minute":"0"} |
 æ¯å¤©èªå¨æ´æ°æ¯èµæ°æ®çæ¶é´ï¼é»è®¤æ¯ 0 ç¹ 0
 åï¼ä½ å¯ä»¥å¨éç½®æä»¶ä¸­æé»è®¤å¼æ ¼å¼ä¿®æ¹æä½ æ³è¦çæ¶é´
 | è¯¥æä»¶ä¾èµ [nonebot_plugin_apscheduler](https://github.com/nonebot/
 plugin-apscheduler)
-å®ç°å®æ¶åéåè½ï¼å¦æä½ æ¯éè¿ä¸è½½é¡¹ç®æºç å®è£æä»¶çè¯ï¼è¯·æ³¨æå®è£å¥½ä¾èµã
+å®ç°å®æ¶åéåè½ï¼å¦æä½ æªå®è£æ­¤ä¾èµçè¯ï¼å°æ æ³è§¦åä¸å®æ¶ç¸å³çåè½ã
 ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:
 -----:|:----:|:----:|:----:|:----:| | `cf` | ç¾¤å | å¦ | ç¾¤è |
 åéæè¿ä¸åº Codeforces æ¯èµçä¿¡æ¯ | | `çå®¢` or `nc` | ç¾¤å |
 å¦ | ç¾¤è | åéæè¿ä¸åºçå®¢æ¯èµçä¿¡æ¯ | | `atc` | ç¾¤å | å¦
 | ç¾¤è | åéæè¿ä¸¤åº AtCoder æ¯èµçä¿¡æ¯ | | `today` | ç¾¤å |
 å¦ | ç¾¤è | åéä»å¤©çæ¯èµä¿¡æ¯ | | `next` | ç¾¤å | å¦ | ç¾¤è |
 åéä»å¤©åçé¨åæ¯èµä¿¡æ¯ | | `help` | ç¾¤å | æ¯ | ç¾¤è |
```

