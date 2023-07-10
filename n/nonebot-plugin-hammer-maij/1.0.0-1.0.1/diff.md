# Comparing `tmp/nonebot_plugin_hammer_maij-1.0.0.tar.gz` & `tmp/nonebot_plugin_hammer_maij-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_hammer_maij-1.0.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_hammer_maij-1.0.1.tar", max compression
```

## Comparing `nonebot_plugin_hammer_maij-1.0.0.tar` & `nonebot_plugin_hammer_maij-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11558 2022-08-01 04:54:18.632590 nonebot_plugin_hammer_maij-1.0.0/LICENSE
--rw-r--r--   0        0        0     1614 2023-07-10 10:43:55.171590 nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/__init__.py
--rw-r--r--   0        0        0      137 2022-08-20 09:34:04.927206 nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/config.py
--rw-r--r--   0        0        0      353 2023-07-09 12:41:09.897298 nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/const.py
--rw-r--r--   0        0        0     3812 2023-07-10 08:58:01.734256 nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/data_classes.py
--rw-r--r--   0        0        0      243 2023-07-09 12:25:43.042069 nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/handler/__init__.py
--rw-r--r--   0        0        0     1392 2023-07-10 09:38:23.751115 nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/handler/admin_handler.py
--rw-r--r--   0        0        0     3947 2023-07-10 09:37:38.523389 nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/handler/announcement_handler.py
--rw-r--r--   0        0        0     2307 2023-07-10 09:37:44.250082 nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/handler/handle_utils.py
--rw-r--r--   0        0        0     2051 2023-07-10 09:37:48.465740 nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/handler/log_handler.py
--rw-r--r--   0        0        0     4684 2023-07-10 09:37:52.997095 nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/handler/place_handler.py
--rw-r--r--   0        0        0        0 2022-08-21 06:11:13.597330 nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/http/__init__.py
--rw-r--r--   0        0        0      825 2023-07-10 09:37:57.041659 nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/http/http_client.py
--rw-r--r--   0        0        0      126 2023-07-09 11:36:07.424785 nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/http/http_utils.py
--rw-r--r--   0        0        0      321 2022-08-20 13:57:53.444975 nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/http/response_exception.py
--rw-r--r--   0        0        0     1308 2023-07-10 09:39:50.900640 nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/maij_config.py
--rw-r--r--   0        0        0      345 2023-07-10 08:58:01.720383 nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/utils.py
--rw-r--r--   0        0        0     1015 2023-07-10 10:42:38.811195 nonebot_plugin_hammer_maij-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5069 2023-07-10 10:50:00.875524 nonebot_plugin_hammer_maij-1.0.0/README.md
--rw-r--r--   0        0        0     5900 1970-01-01 00:00:00.000000 nonebot_plugin_hammer_maij-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11558 2022-08-01 04:54:18.632590 nonebot_plugin_hammer_maij-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1614 2023-07-10 10:43:55.171590 nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/__init__.py
+-rw-r--r--   0        0        0      137 2022-08-20 09:34:04.927206 nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/config.py
+-rw-r--r--   0        0        0      353 2023-07-09 12:41:09.897298 nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/const.py
+-rw-r--r--   0        0        0     3812 2023-07-10 08:58:01.734256 nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/data_classes.py
+-rw-r--r--   0        0        0      243 2023-07-09 12:25:43.042069 nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/handler/__init__.py
+-rw-r--r--   0        0        0     1392 2023-07-10 09:38:23.751115 nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/handler/admin_handler.py
+-rw-r--r--   0        0        0     3973 2023-07-10 13:36:56.836707 nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/handler/announcement_handler.py
+-rw-r--r--   0        0        0     2307 2023-07-10 09:37:44.250082 nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/handler/handle_utils.py
+-rw-r--r--   0        0        0     2051 2023-07-10 09:37:48.465740 nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/handler/log_handler.py
+-rw-r--r--   0        0        0     4684 2023-07-10 09:37:52.997095 nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/handler/place_handler.py
+-rw-r--r--   0        0        0        0 2022-08-21 06:11:13.597330 nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/http/__init__.py
+-rw-r--r--   0        0        0      825 2023-07-10 09:37:57.041659 nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/http/http_client.py
+-rw-r--r--   0        0        0      126 2023-07-09 11:36:07.424785 nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/http/http_utils.py
+-rw-r--r--   0        0        0      321 2022-08-20 13:57:53.444975 nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/http/response_exception.py
+-rw-r--r--   0        0        0     1308 2023-07-10 09:39:50.900640 nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/maij_config.py
+-rw-r--r--   0        0        0      345 2023-07-10 08:58:01.720383 nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/utils.py
+-rw-r--r--   0        0        0     1015 2023-07-10 13:39:53.654224 nonebot_plugin_hammer_maij-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5569 2023-07-10 13:39:42.848232 nonebot_plugin_hammer_maij-1.0.1/README.md
+-rw-r--r--   0        0        0     6387 1970-01-01 00:00:00.000000 nonebot_plugin_hammer_maij-1.0.1/PKG-INFO
```

### Comparing `nonebot_plugin_hammer_maij-1.0.0/LICENSE` & `nonebot_plugin_hammer_maij-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/__init__.py` & `nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/data_classes.py` & `nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/data_classes.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/handler/admin_handler.py` & `nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/handler/admin_handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/handler/announcement_handler.py` & `nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/handler/announcement_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         return
 
     ##########
     async def do():
         response = client.put(
             url=f'{consts.API_URL}/place/{location}/{place_name}/announcement/{announcement_id}/renewal',
             json={
-                "operator": event.user_id,
+                "operatorId": event.user_id,
             })
         data = Announcement(**json_dict_from_response(response))
         await matcher.send(
             reply_text(
                 f'''成功为{data.place.placeName}的第{data.announcementId}号公告续期一周，其内容如下：
 {await data.display_str(bot, event)}'''.strip(), event))
 
@@ -90,15 +90,16 @@
         announcement_id: int = int(r[1].strip())
     except ValueError:
         await matcher.send(reply_text('请输入正确的公告ID。', event))
         return
 
     ##########
     async def do():
-        response = client.delete(
+        response = client.request(
+            'DELETE',
             url=f'{consts.API_URL}/place/{location}/{place_name}/announcement/{announcement_id}',
             json={
                 "deleterId": event.user_id,
             })
         data = Announcement(**json_dict_from_response(response))
         await matcher.send(
             reply_text(f'''成功为{data.place.placeName}删除了第{data.announcementId}号公告，其内容如下：
```

### Comparing `nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/handler/handle_utils.py` & `nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/handler/handle_utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/handler/log_handler.py` & `nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/handler/log_handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/handler/place_handler.py` & `nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/handler/place_handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/http/http_client.py` & `nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/http/http_client.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_hammer_maij-1.0.0/nonebot_plugin_hammer_maij/maij_config.py` & `nonebot_plugin_hammer_maij-1.0.1/nonebot_plugin_hammer_maij/maij_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_hammer_maij-1.0.0/pyproject.toml` & `nonebot_plugin_hammer_maij-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_hammer_maij"
-version = "1.0.0"
+version = "1.0.1"
 description = "A Nonebot2 plugin implements MaiJ API, which helps MaimaiDX players share the information of game zones."
 authors = ["ArgonarioD <argonariod@outlook.com>"]
 repository = "https://github.com/ArgonarioD/nonebot-plugin-hammer-maij"
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_hammer_maij"}]
 classifiers = [
```

### Comparing `nonebot_plugin_hammer_maij-1.0.0/README.md` & `nonebot_plugin_hammer_maij-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,18 @@
   <img src="https://img.shields.io/badge/Onebot-v11-lightgrey" alt="onebot11">
   <img src="https://img.shields.io/badge/nonebot-2.0.0-orange" alt="nonebot2">
   <a href="https://github.com/ArgonarioD/nonebot-plugin-hammer-core">
     <img src="https://img.shields.io/badge/hammer--core-0.1.3-green" alt="hammer-core">
   </a>
 </p>
 
+## 前言
+本插件的本质是 [Hammer MaiJ API](https://docs.hammer-hfut.tk:233/maij) 的 Nonebot2 前端，
+可以令您的机器人与其它同样接入了 Hammer MaiJ API 的机器人以及机器人所面向的玩家共享该服务中已经存在的舞萌DX机厅信息。
+
 ## 使用本插件
 
 1. 用包管理器在你的 Bot 项目中安装本包，以 Poetry（Nonebot2.0.0 使用的默认包管理器）为例，在命令行中执行
 
 ```shell
 poetry add nonebot-plugin-hammer-maij
 ```
@@ -77,15 +81,24 @@
 
 - Python 3.9.7
 - go-cqhttp v1.1.0
 - nonebot 2.0.0
 
 ## 本插件所实现的API
 
-- [Hammer MaiJ API]("https://docs.hammer-hfut.tk:233/maij")
+- [Hammer MaiJ API](https://docs.hammer-hfut.tk:233/maij)
+
+## 更新日志
+
+### v1.0.1 (*2023-07-10*)
+#### Bugs Fixed
+- 修复了续期公告请求体参数名错误的问题
+- 修复了删除公告请求无法发送的问题
+### v1.0.0 (*2023-07-10*)
+发布本项目
 
 ## 鸣谢
 
 - [onebot](https://github.com/botuniverse/onebot)
 - [nonebot2](https://github.com/nonebot/nonebot2)
 - [go-cqhttp](https://github.com/Mrs4s/go-cqhttp)
```

#### html2text {}

```diff
@@ -1,11 +1,15 @@
                                    [hammer]
  # Nonebot Plugin Hammer MaiJ â¨ åºäº onebotãnonebot2 ä¸ Hammer MaiJ API
                    ç èèDXæºåä¿¡æ¯å±äº«æä»¶ â¨
      [license] [pypi] [python] [maij] [onebot11] [nonebot2] [hammer-core]
+## åè¨ æ¬æä»¶çæ¬è´¨æ¯ [Hammer MaiJ API](https://docs.hammer-hfut.tk:
+233/maij) ç Nonebot2 åç«¯ï¼
+å¯ä»¥ä»¤æ¨çæºå¨äººä¸å¶å®åæ ·æ¥å¥äº Hammer MaiJ API
+çæºå¨äººä»¥åæºå¨äººæé¢åçç©å®¶å±äº«è¯¥æå¡ä¸­å·²ç»å­å¨çèèDXæºåä¿¡æ¯ã
 ## ä½¿ç¨æ¬æä»¶ 1. ç¨åç®¡çå¨å¨ä½ ç Bot é¡¹ç®ä¸­å®è£æ¬åï¼ä»¥
 Poetryï¼Nonebot2.0.0
 ä½¿ç¨çé»è®¤åç®¡çå¨ï¼ä¸ºä¾ï¼å¨å½ä»¤è¡ä¸­æ§è¡ ```shell poetry
 add nonebot-plugin-hammer-maij ``` 2. ä¿®æ¹éç½®ï¼ä»¤ Nonebot2.0.0
 è½å¤å è½½æ¬æä»¶ï¼ 1. ä½¿ç¨ `pyproject.toml`
 ç®¡çæä»¶å è½½çæåµï¼ ä¿®æ¹ä½ ç `pyproject.toml` çä»¥ä¸å±æ§ï¼
 ```toml [tool.nonebot] plugin = ["nonebot_plugin_hammer_maij"] ``` 2. ä½¿ç¨
@@ -31,11 +35,15 @@
 æ¥è¯¢æå®æºåä»æ¥çå¡æ°åæ´è®°å½ | | å\[ä¸](æ¡/ä¸ª)å¬å
 <å°å> <åå®¹> |
 åéä¸æ¡å¬åï¼åå®¹æ¯ææ¢è¡ï¼å¨ä¸ç»­æçæåµä¸ä¸å¨åä¼è¢«èªå¨å é¤
 | | ç»­\[ä¸](ç»­/ å/ä¸)å¬å <å°å> <å¬åID> |
 ä¸ºæå®å¬åç»­æä¸å¨ | | å \[ä¸](æ¡/ä¸ª)å¬å <å°å> <å¬åID> |
 å é¤æå®çå¬åï¼åªæåå¸èå¯ä»¥å é¤ | ## æµè¯ç¯å¢ - Python
 3.9.7 - go-cqhttp v1.1.0 - nonebot 2.0.0 ## æ¬æä»¶æå®ç°çAPI - [Hammer
-MaiJ API]("https://docs.hammer-hfut.tk:233/maij") ## é¸£è°¢ - [onebot](https://
-github.com/botuniverse/onebot) - [nonebot2](https://github.com/nonebot/
-nonebot2) - [go-cqhttp](https://github.com/Mrs4s/go-cqhttp) --
+MaiJ API](https://docs.hammer-hfut.tk:233/maij) ## æ´æ°æ¥å¿ ### v1.0.1
+(*2023-07-10*) #### Bugs Fixed -
+ä¿®å¤äºç»­æå¬åè¯·æ±ä½åæ°åéè¯¯çé®é¢ -
+ä¿®å¤äºå é¤å¬åè¯·æ±æ æ³åéçé®é¢ ### v1.0.0 (*2023-07-10*)
+åå¸æ¬é¡¹ç® ## é¸£è°¢ - [onebot](https://github.com/botuniverse/onebot) -
+[nonebot2](https://github.com/nonebot/nonebot2) - [go-cqhttp](https://
+github.com/Mrs4s/go-cqhttp) --
 - ~~*å¦æè§å¾æç¨çè¯æ±ç¹ä¸ªStaråµQwQ*~~
```

### Comparing `nonebot_plugin_hammer_maij-1.0.0/PKG-INFO` & `nonebot_plugin_hammer_maij-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hammer-maij
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Nonebot2 plugin implements MaiJ API, which helps MaimaiDX players share the information of game zones.
 Home-page: https://github.com/ArgonarioD/nonebot-plugin-hammer-maij
 License: Apache-2.0
 Author: ArgonarioD
 Author-email: argonariod@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -44,14 +44,18 @@
   <img src="https://img.shields.io/badge/Onebot-v11-lightgrey" alt="onebot11">
   <img src="https://img.shields.io/badge/nonebot-2.0.0-orange" alt="nonebot2">
   <a href="https://github.com/ArgonarioD/nonebot-plugin-hammer-core">
     <img src="https://img.shields.io/badge/hammer--core-0.1.3-green" alt="hammer-core">
   </a>
 </p>
 
+## 前言
+本插件的本质是 [Hammer MaiJ API](https://docs.hammer-hfut.tk:233/maij) 的 Nonebot2 前端，
+可以令您的机器人与其它同样接入了 Hammer MaiJ API 的机器人以及机器人所面向的玩家共享该服务中已经存在的舞萌DX机厅信息。
+
 ## 使用本插件
 
 1. 用包管理器在你的 Bot 项目中安装本包，以 Poetry（Nonebot2.0.0 使用的默认包管理器）为例，在命令行中执行
 
 ```shell
 poetry add nonebot-plugin-hammer-maij
 ```
@@ -98,15 +102,24 @@
 
 - Python 3.9.7
 - go-cqhttp v1.1.0
 - nonebot 2.0.0
 
 ## 本插件所实现的API
 
-- [Hammer MaiJ API]("https://docs.hammer-hfut.tk:233/maij")
+- [Hammer MaiJ API](https://docs.hammer-hfut.tk:233/maij)
+
+## 更新日志
+
+### v1.0.1 (*2023-07-10*)
+#### Bugs Fixed
+- 修复了续期公告请求体参数名错误的问题
+- 修复了删除公告请求无法发送的问题
+### v1.0.0 (*2023-07-10*)
+发布本项目
 
 ## 鸣谢
 
 - [onebot](https://github.com/botuniverse/onebot)
 - [nonebot2](https://github.com/nonebot/nonebot2)
 - [go-cqhttp](https://github.com/Mrs4s/go-cqhttp)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hammer-maij Version: 1.0.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hammer-maij Version: 1.0.1 Summary:
 A Nonebot2 plugin implements MaiJ API, which helps MaimaiDX players share the
 information of game zones. Home-page: https://github.com/ArgonarioD/nonebot-
 plugin-hammer-maij License: Apache-2.0 Author: ArgonarioD Author-email:
 argonariod@outlook.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -10,14 +10,18 @@
 nonebot-plugin-hammer-core (>=0.3.2,<0.4.0) Requires-Dist: nonebot-plugin-
 localstore (>=0.5.0,<0.6.0) Project-URL: Repository, https://github.com/
 ArgonarioD/nonebot-plugin-hammer-maij Description-Content-Type: text/markdown
                                    [hammer]
  # Nonebot Plugin Hammer MaiJ â¨ åºäº onebotãnonebot2 ä¸ Hammer MaiJ API
                    ç èèDXæºåä¿¡æ¯å±äº«æä»¶ â¨
      [license] [pypi] [python] [maij] [onebot11] [nonebot2] [hammer-core]
+## åè¨ æ¬æä»¶çæ¬è´¨æ¯ [Hammer MaiJ API](https://docs.hammer-hfut.tk:
+233/maij) ç Nonebot2 åç«¯ï¼
+å¯ä»¥ä»¤æ¨çæºå¨äººä¸å¶å®åæ ·æ¥å¥äº Hammer MaiJ API
+çæºå¨äººä»¥åæºå¨äººæé¢åçç©å®¶å±äº«è¯¥æå¡ä¸­å·²ç»å­å¨çèèDXæºåä¿¡æ¯ã
 ## ä½¿ç¨æ¬æä»¶ 1. ç¨åç®¡çå¨å¨ä½ ç Bot é¡¹ç®ä¸­å®è£æ¬åï¼ä»¥
 Poetryï¼Nonebot2.0.0
 ä½¿ç¨çé»è®¤åç®¡çå¨ï¼ä¸ºä¾ï¼å¨å½ä»¤è¡ä¸­æ§è¡ ```shell poetry
 add nonebot-plugin-hammer-maij ``` 2. ä¿®æ¹éç½®ï¼ä»¤ Nonebot2.0.0
 è½å¤å è½½æ¬æä»¶ï¼ 1. ä½¿ç¨ `pyproject.toml`
 ç®¡çæä»¶å è½½çæåµï¼ ä¿®æ¹ä½ ç `pyproject.toml` çä»¥ä¸å±æ§ï¼
 ```toml [tool.nonebot] plugin = ["nonebot_plugin_hammer_maij"] ``` 2. ä½¿ç¨
@@ -43,11 +47,15 @@
 æ¥è¯¢æå®æºåä»æ¥çå¡æ°åæ´è®°å½ | | å\[ä¸](æ¡/ä¸ª)å¬å
 <å°å> <åå®¹> |
 åéä¸æ¡å¬åï¼åå®¹æ¯ææ¢è¡ï¼å¨ä¸ç»­æçæåµä¸ä¸å¨åä¼è¢«èªå¨å é¤
 | | ç»­\[ä¸](ç»­/ å/ä¸)å¬å <å°å> <å¬åID> |
 ä¸ºæå®å¬åç»­æä¸å¨ | | å \[ä¸](æ¡/ä¸ª)å¬å <å°å> <å¬åID> |
 å é¤æå®çå¬åï¼åªæåå¸èå¯ä»¥å é¤ | ## æµè¯ç¯å¢ - Python
 3.9.7 - go-cqhttp v1.1.0 - nonebot 2.0.0 ## æ¬æä»¶æå®ç°çAPI - [Hammer
-MaiJ API]("https://docs.hammer-hfut.tk:233/maij") ## é¸£è°¢ - [onebot](https://
-github.com/botuniverse/onebot) - [nonebot2](https://github.com/nonebot/
-nonebot2) - [go-cqhttp](https://github.com/Mrs4s/go-cqhttp) --
+MaiJ API](https://docs.hammer-hfut.tk:233/maij) ## æ´æ°æ¥å¿ ### v1.0.1
+(*2023-07-10*) #### Bugs Fixed -
+ä¿®å¤äºç»­æå¬åè¯·æ±ä½åæ°åéè¯¯çé®é¢ -
+ä¿®å¤äºå é¤å¬åè¯·æ±æ æ³åéçé®é¢ ### v1.0.0 (*2023-07-10*)
+åå¸æ¬é¡¹ç® ## é¸£è°¢ - [onebot](https://github.com/botuniverse/onebot) -
+[nonebot2](https://github.com/nonebot/nonebot2) - [go-cqhttp](https://
+github.com/Mrs4s/go-cqhttp) --
 - ~~*å¦æè§å¾æç¨çè¯æ±ç¹ä¸ªStaråµQwQ*~~
```

