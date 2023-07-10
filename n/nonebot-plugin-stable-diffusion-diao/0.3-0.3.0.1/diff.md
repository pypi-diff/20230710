# Comparing `tmp/nonebot_plugin_stable_diffusion_diao-0.3.tar.gz` & `tmp/nonebot_plugin_stable_diffusion_diao-0.3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.tar", last modified: Mon Jul 10 13:22:58 2023, max compression
+gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.0.1.tar", last modified: Mon Jul 10 13:54:48 2023, max compression
```

## Comparing `nonebot_plugin_stable_diffusion_diao-0.3.tar` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3/LICENSE
--rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/__init__.py
--rw-r--r--   0        0        0    24757 2023-07-10 12:17:22.236100 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/aidraw.py
--rw-r--r--   0        0        0     6213 2023-05-30 17:03:22.535709 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
--rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
--rw-r--r--   0        0        0     3894 2023-06-12 05:12:59.000048 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
--rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
--rw-r--r--   0        0        0    14048 2023-07-10 03:47:58.215732 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/backend/base.py
--rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
--rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
--rw-r--r--   0        0        0     5756 2023-07-05 12:50:22.337153 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/backend/sd.py
--rw-r--r--   0        0        0    17747 2023-07-10 13:05:32.558038 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/config.py
--rw-r--r--   0        0        0     9229 2023-06-14 05:11:03.238536 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
--rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
--rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
--rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
--rw-r--r--   0        0        0     2754 2023-07-09 06:10:57.298081 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
--rw-r--r--   0        0        0    11373 2023-07-10 03:48:14.234739 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
--rw-r--r--   0        0        0     4139 2023-07-03 04:27:28.351334 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
--rw-r--r--   0        0        0    37746 2023-07-10 13:21:35.094847 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
--rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/translation.py
--rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/fifo.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/locales/en.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/locales/jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/locales/zh.py
--rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/manage.py
--rw-r--r--   0        0        0     4417 2023-07-10 13:17:35.345221 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
--rw-r--r--   0        0        0     2111 2023-07-03 03:51:06.635888 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/utils/data.py
--rw-r--r--   0        0        0     7818 2023-07-10 12:44:00.159159 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
--rw-r--r--   0        0        0      648 2023-07-09 16:19:12.987305 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
--rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/utils/save.py
--rw-r--r--   0        0        0     1985 2023-07-05 12:05:38.346774 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/version.py
--rw-r--r--   0        0        0      724 2023-07-10 13:22:58.012772 nonebot_plugin_stable_diffusion_diao-0.3/pyproject.toml
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3.0.1/LICENSE
+-rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/__init__.py
+-rw-r--r--   0        0        0    24757 2023-07-10 12:17:22.236100 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/aidraw.py
+-rw-r--r--   0        0        0     6213 2023-05-30 17:03:22.535709 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
+-rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
+-rw-r--r--   0        0        0     3894 2023-06-12 05:12:59.000048 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
+-rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
+-rw-r--r--   0        0        0    14048 2023-07-10 03:47:58.215732 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/backend/base.py
+-rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
+-rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
+-rw-r--r--   0        0        0     5756 2023-07-05 12:50:22.337153 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/backend/sd.py
+-rw-r--r--   0        0        0    17924 2023-07-10 13:46:44.820439 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/config.py
+-rw-r--r--   0        0        0     9229 2023-06-14 05:11:03.238536 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
+-rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
+-rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
+-rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
+-rw-r--r--   0        0        0     2754 2023-07-09 06:10:57.298081 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
+-rw-r--r--   0        0        0    11373 2023-07-10 03:48:14.234739 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
+-rw-r--r--   0        0        0     4139 2023-07-03 04:27:28.351334 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
+-rw-r--r--   0        0        0    37746 2023-07-10 13:38:05.015879 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
+-rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/extension/translation.py
+-rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/fifo.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/locales/en.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/locales/jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/locales/zh.py
+-rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/manage.py
+-rw-r--r--   0        0        0     4417 2023-07-10 13:38:19.527767 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
+-rw-r--r--   0        0        0     2111 2023-07-03 03:51:06.635888 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/utils/data.py
+-rw-r--r--   0        0        0     7818 2023-07-10 12:44:00.159159 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
+-rw-r--r--   0        0        0      648 2023-07-09 16:19:12.987305 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
+-rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/utils/save.py
+-rw-r--r--   0        0        0     1985 2023-07-05 12:05:38.346774 nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/version.py
+-rw-r--r--   0        0        0      728 2023-07-10 13:54:48.493191 nonebot_plugin_stable_diffusion_diao-0.3.0.1/pyproject.toml
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3.0.1/PKG-INFO
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/LICENSE` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/aidraw.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/aidraw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/amusement/vits.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/amusement/vits.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/backend/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/backend/base.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/backend/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/backend/naifu.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/backend/naifu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/backend/novelai.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/backend/novelai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/backend/sd.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/backend/sd.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/config.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from pathlib import Path
 import aiohttp
 import ast
 import asyncio
+import traceback
 
 import aiofiles
 from nonebot import get_driver
 from nonebot.log import logger
 from pydantic import BaseSettings, validator
 from pydantic.fields import ModelField
 
@@ -132,18 +133,18 @@
     bing_key: str = None  # bing的翻译key
     deepl_key: str = None  # deepL的翻译key
     baidu_translate_key: dict = None  # 例:{"SECRET_KEY": "", "API_KEY": ""} # https://console.bce.baidu.com/ai/?_=1685076516634#/ai/machinetranslation/overview/index
     novelai_todaygirl = 1  # 可选值 1 和 2 两种不同的方式
     novelai_tagger_site: str = "la.iamdiao.lol:25"  # 分析功能的地址 例如 127.0.0.1:7860
     vits_site: str = "la.iamdiao.lol:587"
     run_screenshot = False  # 获取服务器的屏幕截图
-    backend_name_list = list(novelai_backend_url_dict.keys())
-    bakcend_site_list = list(novelai_backend_url_dict.values())
     is_redis_enable = True  # 是否启动redis, 启动redis以获得更多功能
     auto_match = True  # 是否自动匹配
+    backend_name_list = []
+    backend_site_list = []
     # 允许单群设置的设置
     def keys(cls):
         return ("novelai_cd", "novelai_tags", "novelai_on", "novelai_ntags", "novelai_revoke", "novelai_h", "novelai_htype", "novelai_picaudit", "novelai_pure", "novelai_site")
 
     def __getitem__(cls, item):
         return getattr(cls, item)
 
@@ -249,34 +250,37 @@
             return True
         else:
             logger.debug(f"不正确的赋值,{arg_},{value},{type(value)}")
             return False
 
 
 async def get_(site: str, end_point="/sdapi/v1/prompt-styles") -> dict or None:
-    async with aiohttp.ClientSession() as session:
-        async with session.get(url=f"http://{site}{end_point}") as resp:
-            if resp.status in [200, 201]:
-                resp_json: list = await resp.json()
-                return resp_json
-            else:
-                return None
+    try:
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url=f"http://{site}{end_point}") as resp:
+                if resp.status in [200, 201]:
+                    resp_json: list = await resp.json()
+                    return resp_json
+                else:
+                    return None
+    except Exception:
+        return None
 
 
 async def this_is_a_func(end_point_index):
     task_list = []
     end_point_list = ["/sdapi/v1/prompt-styles", "/sdapi/v1/embeddings", "/sdapi/v1/loras"]
-    for site in config.bakcend_site_list:
+    for site in config.backend_site_list:
         task_list.append(get_(site, end_point_list[end_point_index]))
     all_resp = await asyncio.gather(*task_list, return_exceptions=False)
     return all_resp
 
 config = Config(**get_driver().config.dict())
-logger.info(f"加载config完成" + str(config))
-logger.info(f"后端数据加载完成, 共有{len(config.backend_name_list)}个后端被加载")
+config.backend_name_list = list(config.novelai_backend_url_dict.keys())
+config.backend_site_list = list(config.novelai_backend_url_dict.values())
 
 try:
     import tensorflow
 except ImportError:
     logger.warning("未能成功导入tensorflow")
     logger.warning("novelai_picaudit为2时本地图片审核不可用")
 if config.is_redis_enable:
@@ -296,18 +300,17 @@
                 if resp:
                     logger.info("redis连接成功")
                     logger.info("开始读取webui的预设")
                     
                     all_style_list, all_emb_list, all_lora_list = [], [], []
                     backend_emb, backend_lora = {}, {}
                     all_resp_style = await this_is_a_func(0)
-                    # all_resp_style = all_resp_style[0]
                     for backend_style in all_resp_style:
-                        for style in backend_style:
-                            if style is not None:
+                        if backend_style is not None:
+                            for style in backend_style:
                                 all_style_list.append(json.dumps(style))
                     logger.info("读取webui的预设完成")
                     logger.info("开始读取webui的embs")
                     normal_backend_index = -1
                     all_emb_list = await this_is_a_func(1)
                     for back_emb in all_emb_list:
                         normal_backend_index += 1
@@ -343,14 +346,16 @@
                     pipe.set("emb", str(backend_emb))
                     pipe.set("lora", str(backend_lora))
                     pipe.execute()
                 else:
                     logger.error("redis连接失败")
                     redis_client = None
             except Exception:
+                logger.error(traceback.print_exc())
                 logger.error("出现了意外错误, 已经暂停redis使用")
                 redis_client = None
             return redis_client
         redis_client = asyncio.run(main())
 
-
+logger.info(f"加载config完成" + str(config))
+logger.info(f"后端数据加载完成, 共有{len(config.backend_name_list)}个后端被加载")
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/anlas.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/extension/anlas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/control_net.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/extension/control_net.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,15 +389,15 @@
         if "_" in msg:
             index, text_msg = int(msg.split("_")[0]), msg.split("_")[1]
         else:
             if msg.isdigit():
                 index = int(msg)
             else:
                 text_msg = msg
-    site_, site = config.backend_name_list[index], config.bakcend_site_list[index]
+    site_, site = config.backend_name_list[index], config.backend_site_list[index]
     emb_dict, embs_list = await get_and_process_emb(site, site_, text_msg)
     await risk_control(bot, event, embs_list, True)
 
 @get_lora.handle()
 async def _(event: MessageEvent, bot: Bot, msg: Message = CommandArg()):
     text_msg = None
     index = 0
@@ -406,15 +406,15 @@
         if "_" in msg:
             index, text_msg = int(msg.split("_")[0]), msg.split("_")[1]
         else:
             if msg.isdigit():
                 index = int(msg)
             else:
                 text_msg = msg
-    site_, site = config.backend_name_list[index], config.bakcend_site_list[index]
+    site_, site = config.backend_name_list[index], config.backend_site_list[index]
     lora_dict, loras_list = await get_and_process_lora(site, site_, text_msg)
     await risk_control(bot, event, loras_list, True)
 
 
 @super_res.handle()
 async def pic_fix(state: T_State, super_res: Message = CommandArg()):
     if super_res:
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/translation.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/extension/translation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/manage.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/utils/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     img_PIL.save(image_new, format="JPEG", quality=95)
     image_new=image_new.getvalue()
     return image_new
 
 
 async def unload_and_reload(backend_index: int=None, backend_site=None):
     if backend_index is not None and isinstance(backend_index, int):
-        backend_site = config.bakcend_site_list[backend_index]
+        backend_site = config.backend_site_list[backend_index]
     async with aiohttp.ClientSession() as session:
         async with session.post(url=f"http://{backend_site}/sdapi/v1/unload-checkpoint") as resp:
             if resp.status not in [200, 201]:
                 logger.error(f"释放模型失败，可能是webui版本太旧，未支持此API，错误:{await resp.text()}")
     async with aiohttp.ClientSession() as session:
         async with session.post(url=f"http://{backend_site}/sdapi/v1/reload-checkpoint") as resp:
             if resp.status not in [200, 201]:
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/utils/data.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/utils/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/utils/save.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/utils/save.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/version.py` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/nonebot_plugin_stable_diffusion_diao/version.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3/pyproject.toml` & `nonebot_plugin_stable_diffusion_diao-0.3.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-stable-diffusion-diao"
-version = "0.3"
+version = "0.3.0.1"
 description = "主要面对stable-diffusion-webui-api的nonebot2插件"
 authors = [
     { name = "DiaoDaiaChan", email = "diaodaiachan@qq.com" },
 ]
 dependencies = [
     "aiofiles>=23.1.0",
     "aiohttp>=3.8.4",
```

