# Comparing `tmp/nonebot_plugin_stable_diffusion_diao-0.2.3.tar.gz` & `tmp/nonebot_plugin_stable_diffusion_diao-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.2.3.tar", last modified: Mon Jul  3 04:29:08 2023, max compression
+gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.tar", last modified: Mon Jul 10 13:22:58 2023, max compression
```

## Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3.tar` & `nonebot_plugin_stable_diffusion_diao-0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.2.3/LICENSE
--rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/__init__.py
--rw-r--r--   0        0        0    18642 2023-06-12 05:11:59.033569 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/aidraw.py
--rw-r--r--   0        0        0     6213 2023-05-30 17:03:22.535709 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
--rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
--rw-r--r--   0        0        0     3894 2023-06-12 05:12:59.000048 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
--rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
--rw-r--r--   0        0        0    15498 2023-07-03 03:48:52.147195 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/backend/base.py
--rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
--rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
--rw-r--r--   0        0        0     5947 2023-06-10 12:00:09.717111 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/backend/sd.py
--rw-r--r--   0        0        0    14062 2023-07-03 04:14:23.655776 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/config.py
--rw-r--r--   0        0        0     9229 2023-06-14 05:11:03.238536 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
--rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
--rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
--rw-r--r--   0        0        0     1102 2023-05-30 17:05:34.472127 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
--rw-r--r--   0        0        0     3751 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
--rw-r--r--   0        0        0    12146 2023-07-03 04:12:39.656129 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
--rw-r--r--   0        0        0     4139 2023-07-03 04:27:28.351334 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
--rw-r--r--   0        0        0    30352 2023-07-03 04:26:00.699128 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
--rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/translation.py
--rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/fifo.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/locales/en.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/locales/jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/locales/zh.py
--rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/manage.py
--rw-r--r--   0        0        0     1479 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
--rw-r--r--   0        0        0     2111 2023-07-03 03:51:06.635888 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/utils/data.py
--rw-r--r--   0        0        0     7756 2023-07-03 04:15:36.169943 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
--rw-r--r--   0        0        0      647 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
--rw-r--r--   0        0        0     1011 2023-07-02 13:09:21.904491 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/utils/save.py
--rw-r--r--   0        0        0     1994 2023-05-28 09:58:15.414188 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/version.py
--rw-r--r--   0        0        0      713 2023-07-03 04:29:08.255147 nonebot_plugin_stable_diffusion_diao-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      462 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3/LICENSE
+-rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/__init__.py
+-rw-r--r--   0        0        0    24757 2023-07-10 12:17:22.236100 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/aidraw.py
+-rw-r--r--   0        0        0     6213 2023-05-30 17:03:22.535709 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
+-rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
+-rw-r--r--   0        0        0     3894 2023-06-12 05:12:59.000048 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
+-rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
+-rw-r--r--   0        0        0    14048 2023-07-10 03:47:58.215732 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/backend/base.py
+-rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
+-rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
+-rw-r--r--   0        0        0     5756 2023-07-05 12:50:22.337153 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/backend/sd.py
+-rw-r--r--   0        0        0    17747 2023-07-10 13:05:32.558038 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/config.py
+-rw-r--r--   0        0        0     9229 2023-06-14 05:11:03.238536 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
+-rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
+-rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
+-rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
+-rw-r--r--   0        0        0     2754 2023-07-09 06:10:57.298081 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
+-rw-r--r--   0        0        0    11373 2023-07-10 03:48:14.234739 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
+-rw-r--r--   0        0        0     4139 2023-07-03 04:27:28.351334 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
+-rw-r--r--   0        0        0    37746 2023-07-10 13:21:35.094847 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
+-rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/translation.py
+-rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/fifo.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/locales/en.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/locales/jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/locales/zh.py
+-rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/manage.py
+-rw-r--r--   0        0        0     4417 2023-07-10 13:17:35.345221 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
+-rw-r--r--   0        0        0     2111 2023-07-03 03:51:06.635888 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/utils/data.py
+-rw-r--r--   0        0        0     7818 2023-07-10 12:44:00.159159 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
+-rw-r--r--   0        0        0      648 2023-07-09 16:19:12.987305 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
+-rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/utils/save.py
+-rw-r--r--   0        0        0     1985 2023-07-05 12:05:38.346774 nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/version.py
+-rw-r--r--   0        0        0      724 2023-07-10 13:22:58.012772 nonebot_plugin_stable_diffusion_diao-0.3/pyproject.toml
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3/PKG-INFO
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/LICENSE` & `nonebot_plugin_stable_diffusion_diao-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/amusement/vits.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/amusement/vits.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/backend/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/backend/base.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/backend/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import aiohttp
 from nonebot import get_driver
 from nonebot.log import logger
 from PIL import Image
 from nonebot.adapters.onebot.v11 import MessageEvent, PrivateMessageEvent
 
 from ..config import config, redis_client
-from ..utils import png2jpg
+from ..utils import png2jpg, unload_and_reload
 from ..utils.data import shapemap
 from ..utils.load_balance import sd_LoadBalance
 history_list = []
 
 
 class AIDRAW_BASE:
     max_resolution: int = 16
@@ -121,15 +121,16 @@
         self.control_net = {"control_net": False,
                            "controlnet_module": "",
                            "controlnet_model": ""
                            }
         self.backend_info: dict = None
         self.task_type: str = None
         self.img_hash = None
-        self.redis_client = redis_client
+        self.extra_info = ""
+        self.audit_info = ""
         
         # 数值合法检查
         if self.steps <= 0 or self.steps > (36 if config.novelai_paid else 28):
             self.steps = 28
         if self.strength < 0 or self.strength > 1:
             self.strength = 0.7
         if self.noise < 0 or self.noise > 1:
@@ -257,35 +258,17 @@
             global history_list
             async with session.post(post_api, json=payload) as resp:
                 if resp.status not in [200, 201]:
                     resp_dict = json.loads(await resp.text())
                     logger.error(resp_dict)
                     if resp_dict["error"] == "OutOfMemoryError":
                         logger.info("检测到爆显存，执行自动模型释放并加载")
-                        async with aiohttp.ClientSession() as session:
-                            async with session.post(url=f"http://{self.backend_site}/sdapi/v1/unload-checkpoint") as resp:
-                                if resp.status not in [200, 201]:
-                                    logger.error(f"释放模型失败，可能是webui版本太旧，未支持此API，错误:{await resp.text()}")
-                        async with aiohttp.ClientSession() as session:
-                            async with session.post(url=f"http://{self.backend_site}/sdapi/v1/reload-checkpoint") as resp:
-                                if resp.status not in [200, 201]:
-                                    logger.error(f"重载模型失败，错误:{await resp.text()}")
-                                logger.info("重载模型成功")
+                        await unload_and_reload(backend_site=self.backend_site)
                 spend_time = time.time() - self.start_time
                 self.spend_time = f"{spend_time:.2f}秒"
-                tmp_history_list = self.backend_info[self.backend_site][self.task_type]["info"]["history"]
-                tmp_history_list.append({self.start_time: spend_time})
-                tc = self.backend_info[self.backend_site][self.task_type]["info"]["tasks_count"]
-                tc -= 1
-                self.backend_info[self.backend_site][self.task_type]["info"]["tasks_count"] = tc
-                cur_status = "idel" if tc == 0 else self.task_type
-                self.backend_info["status"] = cur_status
-                self.backend_info[self.backend_site][self.task_type]["info"]["history"] = tmp_history_list
-                with open("data/novelai/load_balance.json", "w") as f:
-                    f.write(json.dumps(self.backend_info))
                 img = await self.fromresp(resp)
                 logger.debug(f"获取到返回图片，正在处理")
                 # 将图片转化为jpg
                 if config.novelai_save == 1:
                     image_new = await png2jpg(img)
                 else:
                     image_new = base64.b64decode(img)
@@ -321,15 +304,17 @@
             "control_net",
             "hiresfix",
             "hiresfix_scale",
             "super_res_after_generate",
             "spend_time",
             "vram",
             "backend_name",
-            "img_hash"
+            "img_hash",
+            "tags",
+            "ntags"
         )
 
     def __getitem__(self, item):
         return getattr(self, item)
 
     def format(self):
         dict_self = dict(self)
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/backend/naifu.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/backend/naifu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/backend/novelai.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/backend/novelai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/backend/sd.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/backend/sd.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         if self.control_net["control_net"]:
             self.task_type = "controlnet"
         elif self.img2img:
             self.task_type = "img2img"
         else:
             self.task_type = "txt2img"
         logger.info(f"任务类型:{self.task_type}")
-        resp_tuple = await sd_LoadBalance(task_type=self.task_type, state_dict=self.backend_info)
+        resp_tuple = await sd_LoadBalance()
         self.backend_name = resp_tuple[1][1]
         self.backend_site = resp_tuple[1][0]
         return resp_tuple
 
     async def post_parameters(self):
         '''
         获取post参数
@@ -92,24 +92,21 @@
                 parameters.update(config.novelai_ControlNet_payload[1])
                 parameters["controlnet_units"][0]["input_image"] = self.image           
         return header, post_api, parameters
 
     async def post(self):
         global defult_site
         defult_site = None # 所有后端失效后, 尝试使用默认后端
-        with open("data/novelai/load_balance.json", "r", encoding="utf-8") as f:
-            content = f.read()
-            self.backend_info = json.loads(content)
         # 失效自动重试 
         for retry_times in range(config.novelai_retry):
             try:
                 self.start_time = time.time()
                 parameters_tuple = await self.post_parameters()
                 await self.post_(*parameters_tuple)
-            except:
+            except Exception:
                 self.start_time: float = time.time()
                 logger.info(f"第{retry_times + 1}次尝试")
                 logger.error(traceback.print_exc())
                 await asyncio.sleep(2)
                 if retry_times >= 1: # 如果指定了后端, 重试两次仍然失败的话, 使用负载均衡重新获取可用后端
                     defult_site = config.novelai_site
                     self.backend_index = None
@@ -119,19 +116,19 @@
                     raise RuntimeError(f"重试{config.novelai_retry}次后仍然发生错误, 请检查服务器")
             else:
                 if config.novelai_load_balance is False:
                     try:
                         self.backend_name = (list(config.novelai_backend_url_dict.keys())[self.backend_index] 
                                              if self.backend_index 
                                              else self.backend_name)
-                    except:
+                    except Exception:
                         self.backend_name = ""
                 resp_list = await asyncio.gather(*[self.get_webui_config(self.backend_site), get_vram(self.backend_site)], return_exceptions=False)
                 resp_json = resp_list[0]
                 try:
                     self.model = resp_json["sd_model_checkpoint"]
-                except:
+                except Exception:
                     self.model = ""
                 self.vram = resp_list[1]
                 break
                 
         return self.result
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/config.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,82 +1,88 @@
 import json
 from pathlib import Path
+import aiohttp
+import ast
+import asyncio
 
 import aiofiles
 from nonebot import get_driver
 from nonebot.log import logger
 from pydantic import BaseSettings, validator
 from pydantic.fields import ModelField
-import os
-
 
 jsonpath = Path("data/novelai/config.json").resolve()
 lb_jsonpath = Path("data/novelai/load_balance.json").resolve()
+redis_client = None
+backend_emb, backend_lora = None, None
 
 nickname = list(get_driver().config.nickname)[0] if len(
-    get_driver().config.nickname) else "nonebot-plugin-stable-diffusion"
+    get_driver().config.nickname) else "nonebot-plugin-stable-diffusion-diao"
 
 
 class Config(BaseSettings):
     # 服务器设置
     lb_jsonpath
-    novelai_steps: int = None # 默认步数
+    novelai_steps: int = None  # 默认步数
     novelai_command_start: set = {"绘画", "咏唱", "召唤", "约稿", "aidraw", "画", "绘图", "AI绘图", "ai绘图"}
-    novelai_scale: int = 7 # CFG Scale 请你自己设置, 每个模型都有适合的值
-    novelai_retry: int = 3 # post失败后重试的次数
+    novelai_scale: int = 7  # CFG Scale 请你自己设置, 每个模型都有适合的值
+    novelai_retry: int = 4  # post失败后重试的次数
     novelai_token: str = ""  # 官网的token
     # novelai: dict = {"novelai":""}# 你的服务器地址（包含端口），不包含http头，例:127.0.0.1:6969
     novelai_mode: str = "sd"
     novelai_site: str = "la.iamdiao.lol:5938"
     # 后台设置
     novelai_save: int = 2  # 是否保存图片至本地,0为不保存，1保存，2同时保存追踪信息
-    novelai_save_png: bool = False # 是否保存为PNG格式
+    novelai_save_png: bool = False  # 是否保存为PNG格式
     novelai_paid: int = 3  # 0为禁用付费模式，1为点数制，2为不限制
     novelai_pure: bool = True  # 是否启用简洁返回模式（只返回图片，不返回tag等数据）
     novelai_limit: bool = False  # 是否开启限速
-    novelai_daylimit: int = 0  # 每日次数限制，0为禁用
+    novelai_daylimit: int = 24  # 每日次数限制，0为禁用
     novelai_h: int = 2  # 是否允许H, 0为不允许, 1为删除屏蔽词, 2允许
-    novelai_htype: int = 3 # 1为发现H后私聊用户返回图片, 2为返回群消息但是只返回图片url并且主人直接私吞H图(, 3发送二维码(无论参数如何都会保存图片到本地)
+    novelai_htype: int = 3  # 1为发现H后私聊用户返回图片, 2为返回群消息但是只返回图片url并且主人直接私吞H图(, 3发送二维码(无论参数如何都会保存图片到本地)
     novelai_antireport: bool = True  # 玄学选项。开启后，合并消息内发送者将会显示为调用指令的人而不是bot
     novelai_max: int = 3  # 每次能够生成的最大数量
     # 允许生成的图片最大分辨率，对应(值)^2.默认为1024（即1024*1024）。如果服务器比较寄，建议改成640（640*640）或者根据能够承受的情况修改。naifu和novelai会分别限制最大长宽为1024
     # 可运行更改的设置
     novelai_tags: str = ""  # 内置的tag
     novelai_ntags: str = ""  # 内置的反tag
     novelai_cd: int = 60  # 默认的cd
+    novelai_group_cd: int = 3  # 默认的群共享cd
     novelai_on: bool = True  # 是否全局开启
     novelai_revoke: int = 0  # 是否自动撤回，该值不为0时，则为撤回时间
-    novelai_random_ratio: bool = True # 是否开启随机比例
-    novelai_random_sampler: bool = False # 是否开启随机采样器
-    novelai_random_scale: bool = True # 是否开启随机CFG
+    novelai_random_ratio: bool = True  # 是否开启随机比例
+    novelai_random_sampler: bool = False  # 是否开启随机采样器
+    novelai_random_scale: bool = False  # 是否开启随机CFG
     novelai_random_ratio_list: list = [("p", 0.35), ("s", 0.10), ("l", 0.35), ("uw", 0.1), ("uwp", 0.1)] # 随机图片比例
-    novelai_random_sampler_list = [("Euler a", 0.25), ("Euler", 0.1), ("UniPC", 0.05), ("DDIM", 0.1), ("DPM++ 2S a Karras", 0.15), ("DPM++ SDE", 0.05), ("DPM++ 2S a", 0.1), ("DPM++ SDE Karras", 0.05), ("DPM++ 2M Karras", 0.15)]
+    novelai_random_sampler_list = [("Euler a", 0.35), ("DDIM", 0.3), ("DPM++ 2S a Karras", 0.05), ("DPM++ 2M Karras", 0.3)]
     novelai_random_scale_list = [(3, 0.05), (4, 0.2), (5, 0.05), (6, 0.4), (7, 0.1), (8, 0.18), (9, 0.02)]
-    novelai_load_balance: bool = True # 负载均衡, 使用前请先将队列限速关闭, 目前只支持stable-diffusion-webui, 所以目前只支持novelai_mode = "sd" 时可用, 目前已知问题, 很短很短时间内疯狂画图的话无法均匀分配任务
+    novelai_load_balance: bool = True  # 负载均衡, 使用前请先将队列限速关闭, 目前只支持stable-diffusion-webui, 所以目前只支持novelai_mode = "sd" 时可用, 目前已知问题, 很短很短时间内疯狂画图的话无法均匀分配任务
+    novelai_load_balance_mode: int = 1  # 负载均衡模式, 1为随机, 2为加权随机选择
+    novelai_load_balance_weight: list = []  # 设置列表, 列表长度为你的后端数量, 数值为随机权重, 例[0.2, 0.5, 0.3]
     novelai_backend_url_dict: dict = {"雕雕的后端": "la.iamdiao.lol:5938", "雕雕的后端2": "la.iamdiao.lol:1521"} # 你能用到的后端, 键为名称, 值为url, 例:backend_url_dict = {"NVIDIA P102-100": "192.168.5.197:7860","NVIDIA CMP 40HX": "127.0.0.1:7860"
-    novelai_sampler: str = None # 默认采样器,不写的话默认Euler a, Euler a系画人物可能比较好点, DDIM系, 如UniPC画出来的背景比较丰富, DPM系采样器一般速度较慢, 请你自己尝试(以上为个人感觉
-    novelai_hr: bool = True # 是否启动高清修复
-    novelai_hr_scale: float = 1.5 # 高清修复放大比例
+    novelai_sampler: str = None  # 默认采样器,不写的话默认Euler a, Euler a系画人物可能比较好点, DDIM系, 如UniPC画出来的背景比较丰富, DPM系采样器一般速度较慢, 请你自己尝试(以上为个人感觉
+    novelai_hr: bool = True  # 是否启动高清修复
+    novelai_hr_scale: float = 1.5  # 高清修复放大比例
     novelai_hr_payload: dict = {
         "enable_hr": "true", 
-        "denoising_strength": 0.55, # 重绘幅度
-        "hr_scale": novelai_hr_scale, # 高清修复比例, 1.5为长宽分辨率各X1.5
-        "hr_upscaler": "Lanczos", # 超分模型, 使用前请先确认此模型是否可用, 推荐使用R-ESRGAN 4x+ Anime6B
-        "hr_second_pass_steps": 7, # 高清修复步数, 个人建议7是个不错的选择, 速度质量都不错
+        "denoising_strength": 0.55,  # 重绘幅度
+        "hr_scale": novelai_hr_scale,  # 高清修复比例, 1.5为长宽分辨率各X1.5
+        "hr_upscaler": "Lanczos",  # 超分模型, 使用前请先确认此模型是否可用, 推荐使用R-ESRGAN 4x+ Anime6B
+        "hr_second_pass_steps": 7,  # 高清修复步数, 个人建议7是个不错的选择, 速度质量都不错
     } # 以上为个人推荐值
-    novelai_SuperRes_MaxPixels: int = 2000 # 超分最大像素值, 对应(值)^2, 为了避免有人用超高分辨率的图来超分导致爆显存(
-    novelai_SuperRes_generate: bool = False # 图片生成后是否再次进行一次超分
+    novelai_SuperRes_MaxPixels: int = 2000  # 超分最大像素值, 对应(值)^2, 为了避免有人用超高分辨率的图来超分导致爆显存(
+    novelai_SuperRes_generate: bool = False  # 图片生成后是否再次进行一次超分
     novelai_SuperRes_generate_payload: dict = {
-        "upscaling_resize": 1.2, # 超分倍率, 为长宽分辨率各X1.2
-        "upscaler_1": "Lanczos", # 第一次超分使用的方法
-        "upscaler_2": "R-ESRGAN 4x+ Anime6B", # 第二次超分使用的方法
-        "extras_upscaler_2_visibility": 0.7 # 第二层upscaler力度
+        "upscaling_resize": 1.2,  # 超分倍率, 为长宽分辨率各X1.2
+        "upscaler_1": "Lanczos",  # 第一次超分使用的方法
+        "upscaler_2": "R-ESRGAN 4x+ Anime6B",  # 第二次超分使用的方法
+        "extras_upscaler_2_visibility": 0.7  # 第二层upscaler力度
     } # 以上为个人推荐值
     novelai_ControlNet_post_method: int = 0
-    novelai_size_org: int = 640 # 最大分辨率
+    novelai_size_org: int = 640  # 最大分辨率
     if novelai_hr:
         novelai_size: int = novelai_size_org
     else:
         novelai_size: int = novelai_size_org * novelai_hr_payload["hr_scale"]
     '''post方法有 0: /sdapi/v1/txt2img 和 1: /controlnet/txt2img 
     个人使用第一种方法post显卡占用率反复横跳TAT 
     tips:使用/controlnet/txt2img会提示warning: consider using the '/sdapi/v1/txt2img' route with the 'alwayson_scripts' json property instead''' 
@@ -112,29 +118,32 @@
     ]
     
     novelai_cndm: dict = {"controlnet_module": "canny", 
                           "controlnet_processor_res": novelai_size, 
                           "controlnet_threshold_a": 100, 
                           "controlnet_threshold_b": 250}
     
-    novelai_picaudit: int = 4 # 1为百度云图片审核, 2为本地审核功能, 请去百度云免费领取 https://ai.baidu.com/tech/imagecensoring 3为关闭, 4为使用webui，api,地址为novelai_tagger_site设置的
+    novelai_picaudit: int = 4  # 1为百度云图片审核, 2为本地审核功能, 请去百度云免费领取 https://ai.baidu.com/tech/imagecensoring 3为关闭, 4为使用webui，api,地址为novelai_tagger_site设置的
     novelai_pic_audit_api_key: dict = {"SECRET_KEY": "",
-                                       "API_KEY": ""} # 你的百度云API Key
+                                       "API_KEY": ""}  # 你的百度云API Key
     openai_api_key: str = "" # 如果要使用ChatGPTprompt生成功能, 请填写你的OpenAI API Key
-    novelai_auto_icon: bool = True # 机器人自动换头像(没写呢！)
-    novelai_extra_pic_audit = True # 是否为二次元的我, chatgpt生成tag等功能添加审核功能
+    novelai_auto_icon: bool = True  # 机器人自动换头像(没写呢！)
+    novelai_extra_pic_audit = True  # 是否为二次元的我, chatgpt生成tag等功能添加审核功能
     # 翻译API设置
     bing_key: str = None  # bing的翻译key
     deepl_key: str = None  # deepL的翻译key
-    baidu_translate_key: dict = None # 例:{"SECRET_KEY": "", "API_KEY": ""} # https://console.bce.baidu.com/ai/?_=1685076516634#/ai/machinetranslation/overview/index
-    novelai_todaygirl = 1 # 可选值 1 和 2 两种不同的方式
-    novelai_tagger_site: str = "la.iamdiao.lol:25" # 分析功能的地址 例如 127.0.0.1:7860
+    baidu_translate_key: dict = None  # 例:{"SECRET_KEY": "", "API_KEY": ""} # https://console.bce.baidu.com/ai/?_=1685076516634#/ai/machinetranslation/overview/index
+    novelai_todaygirl = 1  # 可选值 1 和 2 两种不同的方式
+    novelai_tagger_site: str = "la.iamdiao.lol:25"  # 分析功能的地址 例如 127.0.0.1:7860
     vits_site: str = "la.iamdiao.lol:587"
-    run_screenshot = False # 获取服务器的屏幕截图
-
+    run_screenshot = False  # 获取服务器的屏幕截图
+    backend_name_list = list(novelai_backend_url_dict.keys())
+    bakcend_site_list = list(novelai_backend_url_dict.values())
+    is_redis_enable = True  # 是否启动redis, 启动redis以获得更多功能
+    auto_match = True  # 是否自动匹配
     # 允许单群设置的设置
     def keys(cls):
         return ("novelai_cd", "novelai_tags", "novelai_on", "novelai_ntags", "novelai_revoke", "novelai_h", "novelai_htype", "novelai_picaudit", "novelai_pure", "novelai_site")
 
     def __getitem__(cls, item):
         return getattr(cls, item)
 
@@ -239,47 +248,109 @@
                 await f.write(jsonnew)
             return True
         else:
             logger.debug(f"不正确的赋值,{arg_},{value},{type(value)}")
             return False
 
 
+async def get_(site: str, end_point="/sdapi/v1/prompt-styles") -> dict or None:
+    async with aiohttp.ClientSession() as session:
+        async with session.get(url=f"http://{site}{end_point}") as resp:
+            if resp.status in [200, 201]:
+                resp_json: list = await resp.json()
+                return resp_json
+            else:
+                return None
+
+
+async def this_is_a_func(end_point_index):
+    task_list = []
+    end_point_list = ["/sdapi/v1/prompt-styles", "/sdapi/v1/embeddings", "/sdapi/v1/loras"]
+    for site in config.bakcend_site_list:
+        task_list.append(get_(site, end_point_list[end_point_index]))
+    all_resp = await asyncio.gather(*task_list, return_exceptions=False)
+    return all_resp
+
 config = Config(**get_driver().config.dict())
 logger.info(f"加载config完成" + str(config))
-novelai_backend_url_dict = config.novelai_backend_url_dict
-state_dict = {}
-std_dict = {"status": "idle",
-            "start_time": None, 
-            "txt2img": {"info": {"history": [{None: None}], "history_avage_time": None, "eta_time": 30, "tasks_count": 0}}, 
-            "img2img": {"info": {"history": [{None: None}], "history_avage_time": None, "eta_time": 30, "tasks_count": 0}}, 
-            "controlnet": {"info": {"history": [{None: None}], "history_avage_time": None, "eta_time": 30, "tasks_count": 0}}
-            }
-if os.path.isfile(lb_jsonpath):
-    with open(lb_jsonpath, "r", encoding="utf-8") as f:
-        content = f.read()
-        state_dict: dict = json.loads(content)
-        
-for k, v in novelai_backend_url_dict.items():
-    if v not in state_dict.keys():
-        state_dict[v] = std_dict
-        logger.info(f"新添加后端{k}")
-
-if not lb_jsonpath.exists():
-    lb_jsonpath.parent.mkdir(parents=True, exist_ok=True)
-with open(lb_jsonpath, "w", encoding="utf-8") as f:
-    f.write(json.dumps(state_dict))
-
-logger.info(f"后端数据加载完成, 共有{len(list(novelai_backend_url_dict.keys()))}个后端被加载")
+logger.info(f"后端数据加载完成, 共有{len(config.backend_name_list)}个后端被加载")
 
 try:
     import tensorflow
 except ImportError:
-    logger.error("未能成功导入tensorflow")
-    logger.error("novelai_picaudit为2时本地图片审核不可用")
-redis_client = None
-# try:
-#     import redis
-# except ImportError:
-#     logger.error("未找到redis")
-# else:
-#     redis_client = redis.Redis(host='localhost', port=6379, db=4)
+    logger.warning("未能成功导入tensorflow")
+    logger.warning("novelai_picaudit为2时本地图片审核不可用")
+if config.is_redis_enable:
+    try:
+        import redis
+    except ImportError:
+        logger.error("未找到redis库, 请先pip install redis")
+    else:
+        async def main():
+            redis_client = []
+            r1 = redis.Redis(host='localhost', port=6379, db=7)
+            r2 = redis.Redis(host='localhost', port=6379, db=8)
+            r3 = redis.Redis(host='localhost', port=6379, db=9)
+            redis_client = [r1, r2, r3]
+            resp = r1.ping()
+            try:
+                if resp:
+                    logger.info("redis连接成功")
+                    logger.info("开始读取webui的预设")
+                    
+                    all_style_list, all_emb_list, all_lora_list = [], [], []
+                    backend_emb, backend_lora = {}, {}
+                    all_resp_style = await this_is_a_func(0)
+                    # all_resp_style = all_resp_style[0]
+                    for backend_style in all_resp_style:
+                        for style in backend_style:
+                            if style is not None:
+                                all_style_list.append(json.dumps(style))
+                    logger.info("读取webui的预设完成")
+                    logger.info("开始读取webui的embs")
+                    normal_backend_index = -1
+                    all_emb_list = await this_is_a_func(1)
+                    for back_emb in all_emb_list:
+                        normal_backend_index += 1
+                        if back_emb is not None:
+                            emb_dict = {}
+                            n = 0
+                            for emb in list(back_emb["loaded"].keys()):
+                                n += 1
+                                emb_dict[n] = emb
+                            backend_emb[config.backend_name_list[normal_backend_index]] = emb_dict
+                        else:
+                            backend_emb[config.backend_name_list[normal_backend_index]] = None
+                    logger.info("开始读取webui的loras")
+                    all_lora_list = await this_is_a_func(2)
+                    normal_backend_index = -1
+                    for back_lora in all_lora_list:
+                        normal_backend_index += 1
+                        if back_lora is not None:
+                            lora_dict = {}
+                            n = 0
+                            for lora in back_lora:
+                                lora_name = lora["name"]
+                                n += 1
+                                lora_dict[n] = lora_name
+                            backend_lora[config.backend_name_list[normal_backend_index]] = lora_dict
+                        else:
+                            backend_lora[config.backend_name_list[normal_backend_index]] = None
+                    logger.info("存入数据库...")
+                    if r2.exists("emb"):
+                        r2.delete(*["style", "emb", "lora"])
+                    pipe = r2.pipeline()
+                    pipe.rpush("style", *all_style_list)
+                    pipe.set("emb", str(backend_emb))
+                    pipe.set("lora", str(backend_lora))
+                    pipe.execute()
+                else:
+                    logger.error("redis连接失败")
+                    redis_client = None
+            except Exception:
+                logger.error("出现了意外错误, 已经暂停redis使用")
+                redis_client = None
+            return redis_client
+        redis_client = asyncio.run(main())
+
+
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/anlas.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/anlas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/control_net.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/control_net.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import base64
 from nonebot import on_command
 from nonebot.adapters.onebot.v11 import MessageEvent, MessageSegment, ActionFailed, Bot
 from nonebot.log import logger
 from .translation import translate
 from .safe_method import send_forward_msg, risk_control
 from ..config import config
+from ..utils import pic_audit_standalone
 
 deepdanbooru = on_command(".gettag", aliases={"鉴赏", "查书", "分析"})
 
 
 @deepdanbooru.handle()
 async def deepdanbooru_handle(event: MessageEvent, bot: Bot):
     h_ = None
@@ -22,38 +23,23 @@
         url = seg.data["url"]
     if url:
         async with aiohttp.ClientSession() as session:
             logger.info(f"正在获取图片")
             async with session.get(url) as resp:
                 bytes = await resp.read()
         str_img = str(base64.b64encode(bytes), "utf-8")
-        message = ""
         start = "data:image/jpeg;base64,"
         str0 = start+str_img
+        
         if config.novelai_tagger_site:
-            site = config.novelai_tagger_site
-            payload = {"image": str0, "model": "wd14-vit-v2-git", "threshold": 0.35 }
-            async with aiohttp.ClientSession() as session:
-                async with session.post(url=f"http://{site}/tagger/v1/interrogate", json=payload) as resp:
-                    if resp.status not in [200, 201]:
-                        resp_text = await resp.text()
-                        logger.error(f"API失败，错误信息:{resp.status, resp_text}")
-                        await deepdanbooru.finish(f"识别失败，错误代码为{resp.status}")
-                    else:
-                        resp_dict = await resp.json()
-                        tags = resp_dict["caption"]
-                        replace_list =  ["general", "sensitive", "questionable", "explicit"]
-                        possibilities = {}
-                        for i in replace_list:
-                            possibilities[i]=tags[i]
-                            del tags[i]
-                        value = list(possibilities.values())
-                        value.sort(reverse=True)
-                        h_ = f"这张图涩度{value[0] * 100}%"
-                        tags = ", ".join(list(tags.keys()))
+            resp_tuple = await pic_audit_standalone(str0, True)
+            if resp_tuple is None:
+                await deepdanbooru.finish("识别失败")
+            h_, tags = resp_tuple
+            tags = ", ".join(tags)
 
         else:
             async with aiohttp.ClientSession() as session:
                 async with session.post('https://mayhug-rainchan-anime-image-label.hf.space/api/predict/', json={"data": [str0, 0.6,"ResNet101"]}) as resp:
                     if resp.status != 200:
                         await deepdanbooru.finish(f"识别失败，错误代码为{resp.status}")
                     jsonresult = await resp.json()
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ..config import config, nickname
 from ..utils.save import save_img
-from ..utils import sendtosuperuser
+from ..utils import sendtosuperuser, pic_audit_standalone
 from io import BytesIO
 import base64
 import aiohttp, aiofiles
 import nonebot
 import os
 import urllib
 import re
@@ -56,15 +56,15 @@
                     logger.debug("超分API失效")
             if save_img_:
                 await save_img(fifo, i, fifo.group_id)
             message.append(MessageSegment.image(i))
             return message
         if await config.get_value(fifo.group_id, "picaudit") in [1, 2, 4] or config.novelai_picaudit in [1, 2, 4]:
             try:
-                label, h_value = await check_safe(i, fifo)
+                label, h_value, fifo.audit_info = await check_safe(i, fifo)
             except RuntimeError as e:
                 logger.error(f"NSFWAPI调用失败，错误代码为{e.args}")
                 label = "unknown"
             if label in ["safe", "general", "sensitive"]:
                 label = "_safe"
                 if config.novelai_SuperRes_generate:
                     try:
@@ -73,22 +73,22 @@
                         for i in resp_tuple:
                             i = resp_tuple[0]
                     except:
                         pass
                 message.append(MessageSegment.image(i))
             else:
                 label = "_explicit"
-                message.append(f"\n太涩了,让我先看, 这张图涩度{h_value}%")
+                message.append(f"\n太涩了,让我先看, 这张图涩度{h_value:.1f}%")
                 nsfw_count += 1
                 htype = await config.get_value(fifo.group_id, "htype") or config.novelai_htype
                 message_data = await sendtosuperuser(f"让我看看谁又画色图了{MessageSegment.image(i)}, 来自群{fifo.group_id}")
                 message_id = message_data["message_id"]
                 message_all = await bot.get_msg(message_id=message_id)
                 url_regex = r'http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+]|[!*\(\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+'
-                img_url = re.findall(url_regex, message_all["message"])
+                img_url = re.findall(url_regex, str(message_all["message"]))
                 if htype in [1, 2]:
                     if htype == 1:
                         try:
                             await bot.send_private_msg(user_id=fifo.user_id, 
                                                        message=f"悄悄给你看哦{MessageSegment.image(i)}\n{fifo.img_hash}"
                                                        )
                         except ActionFailed:
@@ -179,41 +179,26 @@
         file_obj = BytesIO(img_bytes)
         possibilities = await asyncio.get_event_loop().run_in_executor(None, main, file_obj)
         value = list(possibilities.values())
         value.sort(reverse=True)
         reverse_dict = {value: key for key, value in possibilities.items()}
         if is_check:
             return possibilities
-        return reverse_dict[value[0]], value[0] * 100
+        return reverse_dict[value[0]], value[0] * 100, ""
     
     elif picaudit == 4 or config.novelai_picaudit == 4:
         img_base64 = base64.b64encode(img_bytes).decode()
-
-        payload = {"image": img_base64, "model": "wd14-vit-v2-git", "threshold": 0.35 }
-
-        async with aiohttp.ClientSession() as session:
-            async with session.post(url=f"http://{config.novelai_tagger_site}/tagger/v1/interrogate", json=payload) as resp:
-                if resp.status not in [200, 201]:
-                    resp_text = await resp.text()
-                    logger.error(f"API失败，错误信息:{resp.status, resp_text}")
-                    return "unknown", 0
-                else:
-                    resp_dict = await resp.json()
-                    tags = resp_dict["caption"]
-                    replace_list =  ["general", "sensitive", "questionable", "explicit"]
-                    possibilities = {}
-                    for i in replace_list:
-                        possibilities[i]=tags[i]
-                    value = list(possibilities.values())
-                    value.sort(reverse=True)
-                    reverse_dict = {value: key for key, value in possibilities.items()}
-                    logger.info(f"审核结果:{reverse_dict}")
+        possibilities, message = await pic_audit_standalone(img_base64, False, True)
+        value = list(possibilities.values())
+        value.sort(reverse=True)
+        reverse_dict = {value: key for key, value in possibilities.items()}
+        logger.info(message)
         if is_check:
             return possibilities
-        return "explicit" if reverse_dict[value[0]] == "questionable" else reverse_dict[value[0]], value[0] * 100
+        return "explicit" if reverse_dict[value[0]] == "questionable" else reverse_dict[value[0]], value[0] * 100, message
 
     async def get_file_content_as_base64(path, urlencoded=False):
         # 不知道为啥, 不用这个函数处理的话API会报错图片格式不正确, 试过不少方法了,还是不行(
         """
         获取文件base64编码
         :param path: 文件路径
         :param urlencoded: 是否对结果进行urlencoded 
@@ -248,11 +233,11 @@
     async with aiohttp.ClientSession(headers=headers) as session:
         async with session.post(baidu_api, data=payload) as resp:
             result = await resp.json()
             logger.info(f"审核结果:{result}")
             if is_check:
                 return result
             if result['conclusionType'] == 1:
-                return "safe", result['data'][0]['probability'] * 100
+                return "safe", result['data'][0]['probability'] * 100, ""
             else:
                 return "", result['data'][0]['probability'] * 100
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,26 +6,30 @@
 import json, aiohttp, time, base64
 import base64
 import time
 import io
 import re
 import asyncio
 import aiofiles
-import datetime
+from datetime import datetime
 import os
 import traceback
 import random
+import ast
 
-from ..config import config, redis_client
+from ..config import config, redis_client, nickname
 from ..extension.translation import translate
 from ..extension.explicit_api import check_safe_method, check_safe
 from .translation import translate
 from ..backend import AIDRAW
+from ..utils import unload_and_reload, pic_audit_standalone
+from ..utils.save import save_img
 from ..utils.data import lowQuality, basetag
-from ..utils.load_balance import sd_LoadBalance
+from ..utils.load_balance import sd_LoadBalance, get_vram
+from ..utils.prepocess import prepocess_tags
 from .safe_method import send_forward_msg, risk_control
 from ..extension.daylimit import count
 
 from nonebot import on_command, on_shell_command
 from nonebot.adapters.onebot.v11 import Bot, MessageEvent, Message, MessageSegment, ActionFailed, PrivateMessageEvent
 from nonebot.params import CommandArg, Arg, ArgPlainText, ShellCommandArgs
 from nonebot.typing import T_State
@@ -43,14 +47,17 @@
     if isinstance(event, PrivateMessageEvent):
         site = config.novelai_site
     else:
         site = await config.get_value(event.group_id, "site") or config.novelai_site
     reverse_dict = {value: key for key, value in config.novelai_backend_url_dict.items()}
     return site, reverse_dict    
 
+reverse_dict = {value: key for key, value in config.novelai_backend_url_dict.items()}
+current_date = datetime.now().date()
+day: str = str(int(datetime.combine(current_date, datetime.min.time()).timestamp()))
 
 header = {
     "content-type": "application/json",
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36 Edg/108.0.1462.54"
 }
 
 get_models = on_command(
@@ -67,32 +74,104 @@
 get_backend_status = on_command("后端", aliases={"查看后端"})
 get_emb = on_command("emb", aliases={"embs"})
 get_lora = on_command("lora", aliases={"loras"})
 get_sampler = on_command("采样器", aliases={"获取采样器"})
 translate_ = on_command("翻译")
 hr_fix = on_command("高清修复") # 欸，还没写呢，就是玩
 random_tags = on_command("随机tag")
-find_pic = on_command("找图片")
+find_pic = on_command("找图片", aliases={"图片"})
 word_frequency_count = on_command("词频统计", aliases={"tag统计"})
 run_screen_shot = on_command("运行截图", aliases={"状态"}, block=False, priority=2)
 audit = on_command("审核")
 genera_aging = on_command("再来一张")
+reload_ = on_command("卸载模型", aliases={"释放显存"})
+style_ = on_command("预设")
 
-more_func_parser = ArgumentParser()
+more_func_parser, style_parser = ArgumentParser(), ArgumentParser()
 more_func_parser.add_argument("-i", "--index", type=int, help="设置索引", dest="index")
 more_func_parser.add_argument("-v", "--value", type=str, help="设置值", dest="value")
 more_func_parser.add_argument("-s", "--search", type=str, help="搜索设置名", dest="search")
+style_parser.add_argument("tags", type=str, nargs="*", help="正面提示词")
+style_parser.add_argument("-f", "--find", type=str, help="寻找预设", dest="find_style_name")
+style_parser.add_argument("-n", "--name", type=str, help="预设名", dest="style_name")
+style_parser.add_argument("-u", type=str, help="负面提示词", dest="style_ntags")
+style_parser.add_argument("-d", type=str, help="删除指定预设", dest="delete")
 
 set_sd_config = on_shell_command(
     "config",
     aliases={"设置"},
     parser=more_func_parser,
     priority=5
 )
 
+style_ = on_shell_command(
+    "预设",
+    parser=style_parser,
+    priority=5
+)
+
+
+async def get_and_process_lora(site, site_, text_msg=None):
+    loras_list = [f"这是来自webui:{site_}的lora,\t\n注使用例<lora:xxx:0.8>\t\n或者可以使用 -lora 数字索引 , 例如 -lora 1\n"]
+    n = 0
+    lora_dict = {}
+    get_lora_site = "http://" + site + "/sdapi/v1/loras"
+    resp_json = await aiohttp_func("get", get_lora_site)
+    for item in resp_json[0]:
+        i = item["name"]
+        n += 1
+        lora_dict[n] = i
+        if text_msg:
+            pattern = re.compile(f".*{text_msg}.*", re.IGNORECASE)
+            if pattern.match(i):
+                loras_list.append(f"{n}.{i}\t\n")
+        else:
+            loras_list.append(f"{n}.{i}\t\n")
+    if redis_client:
+        r2 = redis_client[1]
+        if r2.exists("lora"):
+            lora_dict_org = r2.get("lora")
+            lora_dict_org = ast.literal_eval(lora_dict_org.decode("utf-8"))
+            lora_dict = lora_dict_org[site_]
+            lora_dict_org[site_] = lora_dict
+            r2.set("lora", json.dumps(lora_dict_org))
+    else:
+        async with aiofiles.open("data/novelai/loras.json", "w", encoding="utf-8") as f:
+            await f.write(json.dumps(lora_dict))
+    return lora_dict, loras_list
+
+
+async def get_and_process_emb(site, site_, text_msg=None):
+    embs_list = [f"这是来自webui:{site_}的embeddings,\t\n注:直接把emb加到tags里即可使用\t\n中文emb可以使用 -nt 来排除, 例如 -nt 雕雕\n"]
+    n = 0
+    emb_dict = {}
+    get_emb_site = "http://" + site + "/sdapi/v1/embeddings"
+    resp_json = await aiohttp_func("get", get_emb_site)
+    all_embs = list(resp_json[0]["loaded"].keys())
+    for i in all_embs:
+        n += 1
+        emb_dict[n] = i
+        if text_msg:
+            pattern = re.compile(f".*{text_msg}.*", re.IGNORECASE)
+            if pattern.match(i):
+                embs_list.append(f"{n}.{i}\t\n")
+        else:
+            embs_list.append(f"{n}.{i}\t\n")
+    if redis_client:
+        r2 = redis_client[1]
+        emb_dict_org = r2.get("emb")
+        emb_dict_org = ast.literal_eval(emb_dict_org.decode("utf-8"))
+        emb_dict = emb_dict_org[site_]
+        emb_dict_org[site_] = emb_dict
+        r2.set("emb", json.dumps(emb_dict_org))
+    else:
+        async with aiofiles.open("data/novelai/embs.json", "w", encoding="utf-8") as f:
+            await f.write(json.dumps(emb_dict))
+    return emb_dict, embs_list 
+
 
 async def download_img(url):
     async with aiohttp.ClientSession() as session:
         async with session.get(url) as resp:
             img_bytes = await resp.read()
             img_base64 = base64.b64encode(img_bytes).decode("utf-8")
             return img_base64, img_bytes
@@ -225,19 +304,19 @@
                     backend_site_index
                     ):
     
     backend_site = list(config.novelai_backend_url_dict.values())[int(backend_site_index)]
     await func_init(event)
     try:
         site_ = reverse_dict[backend_site]
-    except:
+    except KeyError:
         site_ = await config(event.group_id, "site") or config.novelai_site
     try:
         site_index = list(config.novelai_backend_url_dict.keys()).index(site_)
-    except:
+    except KeyError:
         site_index = ""
     async with aiofiles.open("data/novelai/models.json", "r", encoding="utf-8") as f:
         content = await f.read()
         models_dict = json.loads(content)
     try:
         data = models_dict[model_index]
         await bot.send(event=event, message=f"收到指令，为后端{site_}更换模型中，后端索引-sd {site_index}，请等待,期间无法出图", at_sender=True)
@@ -250,15 +329,14 @@
         else:
             await bot.send(event=event, message="更换模型失败，错误代码%s" % str(code), at_sender=True)
     except KeyError:
         await get_models.finish("输入错误,索引错误")
 
 
 async def aiohttp_func(way, url, payload=""):
-    
     if way == "post":
         async with aiohttp.ClientSession() as session:
             async with session.post(url=url, json=payload) as resp:
                 resp_data = await resp.json()
                 return resp_data, resp.status
     else:
         async with aiohttp.ClientSession() as session:
@@ -280,19 +358,19 @@
         n += 1 
         if args.search:
             pattern = re.compile(f".*{args.search}.*", re.IGNORECASE)
             if pattern.match(i):
                 msg_list.append(f"{n}.设置项: {i},设置值: {v}" + "\n")
         else:
             msg_list.append(f"{n}.设置项: {i},设置值: {v}" + "\n")
-    if args.index == None and args.value == None:
+    if args.index is None and args.value == None:
         await risk_control(bot, event, msg_list, True)
-    elif args.index == None:
+    elif args.index is None:
         await set_sd_config.finish("你要设置啥啊!")
-    elif args.value == None:
+    elif args.value is None:
         await set_sd_config.finish("你的设置值捏?")
     else:
         payload = {
             index_list[args.index - 1]: args.value
         }
         try:
             await aiohttp_func("post", get_config_site, payload)
@@ -300,99 +378,44 @@
             await set_sd_config.finish(f"出现错误,{str(e)}")
         else:
             await bot.send(event=event, message=f"设置完成{payload}")
 
 
 @get_emb.handle()
 async def _(event: MessageEvent, bot: Bot, msg: Message = CommandArg()):
+    text_msg = None
     index = 0
-    text_msg = msg.extract_plain_text().strip()
+    msg = msg.extract_plain_text().strip()
     if msg:
-        list_len = len(list(config.novelai_backend_url_dict.values()))
-        try:
-            int(text_msg)
-        except:
-            pass
+        if "_" in msg:
+            index, text_msg = int(msg.split("_")[0]), msg.split("_")[1]
         else:
-            index = int(text_msg)
-            if 0 <= index < list_len:
-                pass
+            if msg.isdigit():
+                index = int(msg)
             else:
-                index = 0
-    if index is not None and isinstance(index, int):
-        site = list(config.novelai_backend_url_dict.values())[index]
-        msg = None
-    else:
-         site, rev = await func_init(event)
-    try:
-        site_ = reverse_dict[site]
-    except:
-        site_ = await config.get_value(event.group_id, "site") or config.novelai_site
-    embs_list = [f"这是来自webui:{site_}的embeddings,\t\n注:直接把emb加到tags里即可使用\t\n中文emb可以使用 -nt 来排除, 例如 -nt 雕雕\n"]
-    n = 0
-    emb_dict = {}
-    get_emb_site = "http://" + site + "/sdapi/v1/embeddings"
-    resp_json = await aiohttp_func("get", get_emb_site)
-    all_embs = list(resp_json[0]["loaded"].keys())
-    pattern = re.compile(f".*{text_msg}.*", re.IGNORECASE)
-    for i in all_embs:
-        n += 1
-        emb_dict[n] = i
-        if msg:
-            if pattern.match(i):
-                embs_list.append(f"{n}.{i}\t\n")
-        else:
-            embs_list.append(f"{n}.{i}\t\n")
-    async with aiofiles.open("data/novelai/embs.json", "w", encoding="utf-8") as f:
-        await f.write(json.dumps(emb_dict))
+                text_msg = msg
+    site_, site = config.backend_name_list[index], config.bakcend_site_list[index]
+    emb_dict, embs_list = await get_and_process_emb(site, site_, text_msg)
     await risk_control(bot, event, embs_list, True)
 
-
 @get_lora.handle()
 async def _(event: MessageEvent, bot: Bot, msg: Message = CommandArg()):
+    text_msg = None
     index = 0
-    text_msg = msg.extract_plain_text().strip()
-    try:
-        site_ = reverse_dict[site]
-    except:
-        site_ = await config.get_value(event.group_id, "site") or config.novelai_site
+    msg = msg.extract_plain_text().strip()
     if msg:
-        list_len = len(list(config.novelai_backend_url_dict.values()))
-        try:
-            int(text_msg)
-        except:
-            pass
+        if "_" in msg:
+            index, text_msg = int(msg.split("_")[0]), msg.split("_")[1]
         else:
-            index = int(text_msg)
-            if 0 <= index < list_len:
-                pass
+            if msg.isdigit():
+                index = int(msg)
             else:
-                index = 0
-    loras_list = [f"这是来自webui:{site_}的lora,\t\n注使用例<lora:xxx:0.8>\t\n或者可以使用 -lora 数字索引 , 例如 -lora 1\n"]
-    n = 0
-    lora_dict = {}
-    if index is not None and isinstance(index, int):
-        site = list(config.novelai_backend_url_dict.values())[index]
-        msg = None
-    else:
-         site, rev = await func_init(event)
-    get_lora_site = "http://" + site + "/sdapi/v1/loras"
-    resp_json = await aiohttp_func("get", get_lora_site)
-    pattern = re.compile(f".*{text_msg}.*", re.IGNORECASE)
-    for item in resp_json[0]:
-        i = item["name"]
-        n += 1
-        lora_dict[n] = i
-        if msg:
-            if pattern.match(i):
-                loras_list.append(f"{n}.{i}\t\n")
-        else:
-            loras_list.append(f"{n}.{i}\t\n")
-    async with aiofiles.open("data/novelai/loras.json", "w", encoding="utf-8") as f:
-        await f.write(json.dumps(lora_dict))
+                text_msg = msg
+    site_, site = config.backend_name_list[index], config.bakcend_site_list[index]
+    lora_dict, loras_list = await get_and_process_lora(site, site_, text_msg)
     await risk_control(bot, event, loras_list, True)
 
 
 @super_res.handle()
 async def pic_fix(state: T_State, super_res: Message = CommandArg()):
     if super_res:
         state['super_res'] = super_res
@@ -449,18 +472,20 @@
             state["net"] = net
         elif net[0].type == "image":
             state["net"] = net
             state["tag"] = net
     else:
         state["tag"] = net
 
+
 @control_net.got('tag', "请输入绘画的关键词")
 async def __():
     pass
 
+
 @control_net.got("net", "你的图图呢？")
 async def _(event: MessageEvent, bot: Bot, tag: str = ArgPlainText("tag"), msg: Message = Arg("net")):
     if config.novelai_daylimit and not await SUPERUSER(bot, event):
         left = await count(str(event.user_id), 2)
         if left == -1:
             await control_net.finish(f"今天你的次数不够了哦，明天再来找我玩吧")
     await func_init(event)
@@ -543,32 +568,32 @@
         sampler = i["name"]
         sampler_list.append(f"{sampler}\t\n")
     await risk_control(bot, event, sampler_list)
 
 
 @get_backend_status.handle()
 async def _(event: MessageEvent, bot: Bot):
-    async with aiofiles.open("data/novelai/load_balance.json", "r", encoding="utf-8") as f:
-        content = await f.read()
-        backend_info: dict = json.loads(content)
-    backend_info_task_type = ["txt2img", "img2img", "controlnet"]
+    # async with aiofiles.open("data/novelai/load_balance.json", "r", encoding="utf-8") as f:
+    #     content = await f.read()
+    #     backend_info: dict = json.loads(content)
+    # backend_info_task_type = ["txt2img", "img2img", "controlnet"]
     n = -1
     backend_list = list(config.novelai_backend_url_dict.keys())
     backend_site = list(config.novelai_backend_url_dict.values())
     message = []
     task_list = []
     fifo = AIDRAW(event=event)
     all_tuple = await fifo.load_balance_init()
     for i in backend_site:
         task_list.append(fifo.get_webui_config(i))
     resp_config = await asyncio.gather(*task_list, return_exceptions=True)
     resp_tuple = all_tuple[1][2]
-    today = str(datetime.date.today())
+    current_date = datetime.now().date()
+    day: str = str(int(datetime.combine(current_date, datetime.min.time()).timestamp()))
     for i, m in zip(resp_tuple, resp_config):
-        work_history_list = []
         today_task = 0
         n += 1
         if isinstance(i, (aiohttp.ContentTypeError, 
                           TypeError,
                           asyncio.exceptions.TimeoutError,
                           Exception)
                           ):
@@ -585,25 +610,32 @@
                     text_message += f"后端空闲中\t\n"
                 else:
                     eta = i[0]["eta_relative"]
                     text_message += f"后端繁忙捏,还需要{eta:.2f}秒完成任务\t\n"
                 message.append(text_message)
             else:
                 message.append(f"{n+1}.后端{backend_list[n]}掉线😭\t\n")
-        for t in backend_info_task_type:
-            history_list: list[dict] = backend_info[backend_site[n]][t]["info"]["history"]
-            for task in history_list:
-                work_history_list.append(list(task.keys()))
-        today = str(datetime.date.today())
-        for ts in work_history_list:
-            if ts[0] == "null":
-                continue
-            if time.strftime("%Y-%m-%d", time.localtime(float(ts[0]))) == today:
-                today_task += 1
+                
+        today_task = 0
+        if redis_client:
+            r = redis_client[2]
+            if r.exists(day):
+                today = r.get(day)
+                today = ast.literal_eval(today.decode("utf-8"))
+                today_task = today["gpu"][backend_list[n]]
+        else:
+            filename = "data/novelai/day_limit_data.json"
+            if os.path.exists():
+                async with aiofiles.open(filename, "r") as f:
+                    json_ = await f.read()
+                    json_ = json.loads(json_)
+                today_task = json_[day]["gpu"][backend_list[n]]
         message.append(f"今日此后端已画{today_task}张图\t\n")
+        vram = await get_vram(backend_site[n])
+        message.append(f"{vram}\t\n")
 
     await risk_control(bot, event, message, True)
 
 
 @control_net_list.handle()
 async def _(event: MessageEvent, bot: Bot, msg: Message = CommandArg()):
     await func_init(event)
@@ -643,15 +675,23 @@
     txt_msg = msg.extract_plain_text()
     en = await translate(txt_msg, "en")
     await risk_control(bot=bot, event=event, message=[en])
 
 
 @random_tags.handle()
 async def _(event: MessageEvent, bot: Bot, msg: Message = CommandArg()):
-    all_tags_list = await asyncio.get_event_loop().run_in_executor(None, get_tags_list)
+    if redis_client:
+        r = redis_client[0]
+        all_tags_list_str = [] 
+        all_tags_list = r.lrange("prompt", 0, -1)
+        for byte_tag in all_tags_list:
+            all_tags_list_str.append(ast.literal_eval(byte_tag.decode("utf-8")))
+        all_tags_list = all_tags_list_str
+    else:
+        all_tags_list = await asyncio.get_event_loop().run_in_executor(None, get_tags_list)
     chose_tags_list = random.sample(all_tags_list, 12)
     chose_tags = ', '.join(chose_tags_list)
 
     fifo = AIDRAW(user_id=event.user_id, 
                   tags=chose_tags, 
                   ntags=lowQuality, 
                   event=event
@@ -674,67 +714,81 @@
                        message=MessageSegment.image(fifo.result[0])+fifo.img_hash,
                        at_sender=True, 
                        reply_message=True)
 
 
 @find_pic.handle()
 async def _(event: MessageEvent, bot: Bot, msg: Message = CommandArg()):
+    txt_content = ""
+
     hash_id = msg.extract_plain_text()
     directory_path = "data/novelai/output"  # 指定目录路径
     filenames = await asyncio.get_event_loop().run_in_executor(None, get_all_filenames, directory_path)
     txt_file_name, img_file_name = f"{hash_id}.txt", f"{hash_id}.jpg"
     if txt_file_name in list(filenames.keys()):
         txt_content = await asyncio.get_event_loop().run_in_executor(None, extract_tags_from_file, filenames[txt_file_name])
         img_file_path = filenames[img_file_name]
         img_file_path = img_file_path if os.path.exists(img_file_path) else filenames[f"{hash_id}.png"]
+        
         async with aiofiles.open(img_file_path, "rb") as f:
             content = await f.read()
         msg_list = [f"这是你要找的{hash_id}的图\n", txt_content, MessageSegment.image(content)]
+    else:
+        await find_pic.finish("你要找的图不存在")
 
-        if config.novelai_extra_pic_audit:
-            fifo = AIDRAW(user_id=event.get_user_id,
-                          event=event 
-                        )
-            
-            await fifo.load_balance_init()
-            message_ = await check_safe_method(fifo, [content], [""], None, False)
-            if isinstance(message_[1], MessageSegment):
-                try:
-                    await send_forward_msg(bot, event, event.sender.nickname, str(event.user_id), msg_list)
-                except ActionFailed:
-                    await risk_control(bot, event, msg_list, True)
-            else:
-                await bot.send(event, message="哼！想看涩图，自己看私聊去！")
-        else:
+    if config.novelai_extra_pic_audit:
+        fifo = AIDRAW(user_id=event.get_user_id,
+                        event=event 
+                    )
+        await fifo.load_balance_init()
+        message_ = await check_safe_method(fifo, [content], [""], None, False)
+        if isinstance(message_[1], MessageSegment):
             try:
                 await send_forward_msg(bot, event, event.sender.nickname, str(event.user_id), msg_list)
             except ActionFailed:
                 await risk_control(bot, event, msg_list, True)
+        else:
+            await bot.send(event, message="哼！想看涩图，自己看私聊去！")
+    else:
+        try:
+            await send_forward_msg(bot, event, event.sender.nickname, str(event.user_id), msg_list)
+        except ActionFailed:
+            await risk_control(bot, event, msg_list, True)
 
 
 @word_frequency_count.handle()
 async def _(event: MessageEvent, bot: Bot, msg: Message = CommandArg()):
-    
     msg_list = []
-
+    if redis_client:
+        r = redis_client[0]
+        if r.exists("prompt"):
+            word_list_str = []
+            word_list = r.lrange("prompt", 0, -1)
+            for byte_word in word_list:
+                word_list_str.append(ast.literal_eval(byte_word.decode("utf-8")))
+            word_list = word_list_str
+        else:
+            await word_frequency_count.finish("画几张图图再来统计吧!")
+    else:
+        word_list = await asyncio.get_event_loop().run_in_executor(None, get_tags_list, False)
+        
     def count_word_frequency(word_list):
         word_frequency = Counter(word_list)
         return word_frequency
 
     def sort_word_frequency(word_frequency):
         sorted_frequency = sorted(word_frequency.items(), key=lambda x: x[1], reverse=True)
         return sorted_frequency
 
-    word_list = await asyncio.get_event_loop().run_in_executor(None, get_tags_list, False)
     word_frequency = count_word_frequency(word_list)
     sorted_frequency = sort_word_frequency(word_frequency)
     for word, frequency in sorted_frequency[0:240] if len(sorted_frequency) >= 240 else sorted_frequency:
         msg_list.append(f"prompt:{word},出现次数:{frequency}\t\n")
     await risk_control(bot, event, msg_list, True)
-        
+
 
 @run_screen_shot.handle()
 async def _(event: MessageEvent, bot: Bot):
     if config.run_screenshot:
         time_ = str(time.time())
         file_name = f"screenshot_{time_}.png"
         screenshot = ImageGrab.grab()
@@ -742,31 +796,132 @@
         with open(file_name, "rb") as f:
             pic_content = f.read()
             bytes_img = io.BytesIO(pic_content)
         await bot.send(event=event, message=MessageSegment.image(bytes_img))
         os.remove(file_name)
     else:
         await run_screen_shot.finish("未启动屏幕截图")
-        
-        
+
+
 @audit.handle()
 async def _(event: MessageEvent, bot: Bot):
     url = ""
     reply = event.reply
     if reply:
         for seg in reply.message['image']:
             url = seg.data["url"]
     for seg in event.message['image']:
         url = seg.data["url"]
     if url:
         async with aiohttp.ClientSession() as session:
             async with session.get(url) as resp:
                 bytes = await resp.read()
-        str_img = str(base64.b64encode(bytes), "utf-8")
-    # 应对不同的后端审核
-    
-    
+        img_base64 = str(base64.b64encode(bytes), "utf-8")
+        message = await pic_audit_standalone(img_base64)
+        await bot.send(event, message, at_sender=True, reply_message=True)
+
+
 @genera_aging.handle()
 async def _(event: MessageEvent, bot: Bot):
-    pass
     # 读取redis数据
-    redis_client
+    if redis_client:
+        r = redis_client[0]
+        if r.exists(str(event.user_id)):
+            fifo_info = r.lindex(str(event.user_id), -1)
+            fifo_info = fifo_info.decode("utf-8")
+            fifo_info = ast.literal_eval(fifo_info)
+            del fifo_info["seed"]
+            fifo = AIDRAW(**fifo_info)
+            try:
+                await fifo.post()
+            except Exception:
+                logger.error(traceback.print_exc())
+                await genera_aging.finish("出错惹, 快叫主人看控制台")
+            else:
+                img_msg = MessageSegment.image(fifo.result[0])
+                result = await check_safe_method(fifo, [fifo.result[0]], [""], None, True, "_agin")
+                if isinstance(result[1], MessageSegment):
+                    await bot.send(event=event,
+                                   message=f"{nickname}又给你画了一张哦!"+img_msg+f"\n{fifo.img_hash}",
+                                   at_sender=True,
+                                   reply_message=True
+                                   )
+                await save_img(fifo=fifo, img_bytes=fifo.result[0],extra=fifo.group_id+"_agin")
+        else:
+            await genera_aging.finish("你还没画过图, 这个功能用不了哦!")
+    else:
+        await genera_aging.finish("未连接redis, 此功能不可用")
+
+
+@reload_.handle()
+async def _(msg: Message = CommandArg()):
+    if not msg:
+        await reload_.finish("你要释放哪个后端的显存捏?")
+    text_msg = int(msg.extract_plain_text())
+    if not text_msg.isdigit():
+        await reload_.finish("笨蛋!后端编号是数字啦!!")
+    try:
+        await unload_and_reload(text_msg)
+    except Exception:
+        logger.error(traceback.print_exc())
+    else:
+        await reload_.finish(f"为后端{config.backend_name_list[text_msg]}重载成功啦!")
+        
+
+@style_.handle()
+async def _(event: MessageEvent, bot: Bot, args: Namespace = ShellCommandArgs()):
+    message_list = []
+    style_dict = {}
+    if redis_client:
+        r = redis_client[1]
+        if r.exists("style"):
+            style_list = r.lrange("style", 0, -1)
+            style_list = [ast.literal_eval(style.decode("utf-8")) for style in style_list]
+            if r.exists("user_style"):
+                user_style_list = r.lrange("user_style", 0, -1)
+                user_style_list = [ast.literal_eval(style.decode("utf-8")) for style in user_style_list]
+                style_list += user_style_list
+    else:
+        await style.finish("需要redis以使用此功能")
+    if args.delete:
+        delete_name = args.delete[0] if isinstance(args.delete, list) else args.delete
+        find_style = False
+        style_index = -1
+        for style in user_style_list:
+            style_index += 1
+            if style["name"] == delete_name:
+                pipe = r.pipeline()
+                r.lset("user_style", style_index, '__DELETED__')
+                r.lrem("user_style", style_index, '__DELETED__')
+                pipe.execute()
+                find_style = True
+                await style_.finish(f"删除预设{delete_name}成功!")
+        if not find_style:
+            await style_.finish(f"没有找到预设{delete_name},是不是打错了!\n另外不支持删除从webui中导入的预设")
+    if args.find_style_name:
+        find_style = False
+        for style in style_list:
+            if args.find_style_name == style["name"]:
+                name, tags, ntags = style["name"], style["prompt"], style["negative_prompt"]
+                find_style = True
+                await risk_control(bot, event, [f"预设名称: {name}\n正面提示词: {tags}\n负面提示词: {ntags}\n"], True)
+                break
+        if not find_style:
+            await style_.finish(f"没有找到预设{args.find_style_name}")
+    if len(args.tags) != 0:
+        args.ntags = ""
+        if args.tags and args.style_name:
+            tags = await prepocess_tags(args.tags)
+            ntags = await prepocess_tags(args.ntags)
+            style_dict["name"] = args.style_name
+            style_dict["prompt"] = tags
+            style_dict["negative_prompt"] = ntags
+            r.rpush("user_style", str(style_dict))
+            await style_.finish(f"添加预设: {args.style_name}成功!")
+        else:
+            await style_.finish("参数不完整, 请检查后重试")
+    else:
+        for style in style_list:
+            name, tags, ntags = style["name"], style["prompt"], style["negative_prompt"]
+            message_list.append(f"预设名称: {name}\n正面提示词: {tags}\n负面提示词: {ntags}\n")
+        await risk_control(bot, event, message_list, True)
+
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/translation.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/extension/translation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/manage.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/utils/data.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/utils/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,21 @@
-import aiohttp, asyncio, random
+import aiohttp
+import asyncio 
+import random
 from nonebot import logger
-from ..config import config
-import json
+from ..config import config, redis_client
 import time
-import aiofiles
-import traceback
 from tqdm import tqdm
+from datetime import datetime
 
-
-async def calc_avage_time(state_dict_: list):
-    spend_time_list = []
-    for date_time in state_dict_["info"]["history"]:
-        spend_time_list.append(list(date_time.values())[0])
-    spend_time_list.pop(0)
-    spend_time_list.sort()
-    spend_time_list.pop() and spend_time_list.pop(0)
-    return int(sum(spend_time_list) / (len(spend_time_list)) - 3)
+import ast
+import traceback
+import aiofiles
+import json
+import os
 
 
 async def get_progress(url):
     first_get = "http://" + url + "/sdapi/v1/memory" 
     api_url = "http://" + url + "/sdapi/v1/progress"
     async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=2)) as session1:
         async with session1.get(url=first_get) as resp1:
@@ -41,92 +37,41 @@
                 vram_used = int(all_memory_usage["cuda"]["system"]["used"]/1000000)
                 vram_usage = f"显存占用{vram_used}M/{vram_total}M"
     except Exception:
         vram_usage = ""
     return vram_usage
 
 
-async def chose_backend(state_dict, normal_backend, task_type):
-    backend_processtime: dict = {}
-    ava_url_dict: dict = {}
-    # n = -1
-    #         y = 0
-    #         normal_backend = list(status_dict.keys())
-    #         logger.info("没有空闲后端")
-    #         if len(normal_backend) == 0:
-    #             raise RuntimeError("没有可用后端")
-    #         else:
-    #             eta_list = list(status_dict.values())
-    #             for t, b in zip(eta_list, normal_backend):
-    #                 if int(t) < defult_eta:
-    #                     y += 1
-    #                     ava_url = b
-    #                     logger.info(f"已选择后端{reverse_dict[ava_url]}")
-    #                     break
-    #                 else:
-    #                     y +=0
-    #             if y == 0:
-    #                 reverse_sta_dict = {value: key for key, value in status_dict.items()}
-    #                 eta_list.sort()
-    #                 ava_url = reverse_sta_dict[eta_list[0]]
-    for i in normal_backend:
-        cur_state_dict = state_dict[i][task_type]
-        history_info_list: list = cur_state_dict["info"]
-        logger.debug(history_info_list)
-        if len(history_info_list["history"]) > 20: # 需要至少20次生成来确定此后端的平均工作时间
-            ava_time = (await calc_avage_time(cur_state_dict) if 
-                        history_info_list["history_avage_time"] is None 
-                        else i["history_avage_time"])
-        elif len(history_info_list["history"]) > 100:
-            # 重新计算平均时间, 并清空时间列表
-            pass
-        else: 
-            ava_time = cur_state_dict["info"]["eta_time"]
-        count = cur_state_dict["info"]["tasks_count"]
-        total_process_time = count * ava_time
-        backend_processtime.update({total_process_time: i})
-    # process_time_rev = {value: key for key, value in backend_process_time}
-    backend_process_time = list(backend_processtime.keys())
-    backend_process_time.sort()
-    logger.debug(backend_processtime[backend_process_time[0]])
-    logger.error(backend_processtime)
-    return backend_processtime[backend_process_time[0]]
-
-
-async def sd_LoadBalance(addtional_site=None, task_counts=None, task_type=None, state_dict=None):
+async def sd_LoadBalance():
     '''
     分别返回可用后端索引, 后端对应ip和名称(元组), 显存占用
     '''
+    current_date = datetime.now().date()
+    day: str = str(int(datetime.combine(current_date, datetime.min.time()).timestamp()))
     backend_url_dict = config.novelai_backend_url_dict
-    if state_dict is None:
-        with open("data/novelai/load_balance.json", "r", encoding="utf-8") as f:
-            content = f.read()
-            state_dict = json.loads(content)
-    else:
-        pass
-    if addtional_site:
-        backend_url_dict.update({"群专属后端": f"{addtional_site}"})
     reverse_dict = {value: key for key, value in backend_url_dict.items()}
     tasks = []
     is_avaiable = 0
     status_dict = {}
     ava_url = None
     n = -1
     e = -1
+    defult_eta = 20
     normal_backend = None
+    idle_backend = []
     for url in backend_url_dict.values():
         tasks.append(get_progress(url))
     # 获取api队列状态
     all_resp = await asyncio.gather(*tasks, return_exceptions=True)
     for resp_tuple in all_resp:
         e += 1 
-        if isinstance(resp_tuple, 
-                      (aiohttp.ContentTypeError, 
-                       asyncio.exceptions.TimeoutError, 
-                       aiohttp.ClientTimeout, 
+        if isinstance(resp_tuple,
+                      (aiohttp.ContentTypeError,
+                       asyncio.exceptions.TimeoutError,
+                       aiohttp.ClientTimeout,
                        Exception)
                        ):
             print(f"后端{list(config.novelai_backend_url_dict.keys())[e]}掉线")
         else:
             try:
                 if resp_tuple[3] in [200, 201]:
                     n += 1
@@ -137,42 +82,103 @@
             except RuntimeError or TypeError:
                 print(f"后端{list(config.novelai_backend_url_dict.keys())[e]}出错")
                 continue
             else:
                 # 更改判断逻辑
                 if resp_tuple[0]["progress"] in [0, 0.01, 0.0]:
                         is_avaiable += 1
-                        ava_url = normal_backend[n]
+                        idle_backend.append(normal_backend[n])
                 else:
                     pass
-                    # if state_dict[resp_tuple[2]]["status"] == "idle":
-                    #     logger.info("后端空闲")
-                    #     is_avaiable += 1
-                    #     ava_url = normal_backend[n]
-                    #     break
             total = 100
             progress = int(resp_tuple[0]["progress"]*100)
             show_str = f"{list(backend_url_dict.keys())[e]}"
-            show_str = show_str.ljust(22, "-")
-            with tqdm(total=total, desc=show_str + "-->", bar_format="{l_bar}{bar}|") as pbar:
+            show_str = show_str.ljust(25, "-")
+            with tqdm(total=total,
+                      desc=show_str + "-->",
+                      bar_format="{l_bar}{bar}|"
+                      ) as pbar:
                 pbar.update(progress)
                 time.sleep(0.1)
-    if normal_backend is None:
-        normal_backend_name = config.novelai_site or "127.0.0.1:7860"
-        normal_backend = [config.novelai_site, "127.0.0.1:7860"]
+    if config.novelai_load_balance_mode == 1:
+        if is_avaiable == 0:
+            n = -1
+            y = 0
+            normal_backend = list(status_dict.keys())
+            logger.info("没有空闲后端")
+            if len(normal_backend) == 0:
+                raise RuntimeError("没有可用后端")
+            else:
+                eta_list = list(status_dict.values())
+                for t, b in zip(eta_list, normal_backend):
+                    if int(t) < defult_eta:
+                        y += 1
+                        ava_url = b
+                        logger.info(f"已选择后端{reverse_dict[ava_url]}")
+                        break
+                    else:
+                        y += 0
+                if y == 0:
+                    reverse_sta_dict = {value: key for key, value in status_dict.items()}
+                    eta_list.sort()
+                    ava_url = reverse_sta_dict[eta_list[0]]
+        if len(idle_backend) >= 1:
+            ava_url = random.choice(idle_backend)
+    elif config.novelai_load_balance_mode == 2:
+        list_tuple = []
+        weight_list = config.novelai_load_balance_weight
+        backend_url_list = list(config.novelai_backend_url_dict.values())
+        weight_list_len = len(weight_list)
+        backend_url_list_len = len(backend_url_list)
+        normal_backend_len = len(normal_backend)
+        if weight_list_len != backend_url_list_len:
+            logger.warning("权重列表长度不一致, 请重新配置!")
+            ava_url = random.choice(normal_backend)
+        else:
+            from ..backend import AIDRAW
+            if weight_list_len != normal_backend_len:
+                multi = weight_list_len / (weight_list_len - normal_backend_len)
+                for weight, backend_site in zip(weight_list, backend_url_list):
+                    if backend_site in normal_backend:
+                        list_tuple.append((backend_site, weight*multi))
+            else:
+                for backend, weight in zip(normal_backend, weight_list):
+                    list_tuple.append((backend, weight))
+            print(list_tuple)
+            fifo = AIDRAW()
+            ava_url = fifo.weighted_choice(list_tuple)
+    if redis_client:
+        try:
+            r = redis_client[2]
+            if r.exists(day):
+                backend_info = r.get(day)
+                backend_info = backend_info.decode("utf-8")
+                backend_info = ast.literal_eval(backend_info)
+                if backend_info.get("gpu"):
+                    backend_dict = backend_info.get("gpu")
+                    backend_dict[reverse_dict[ava_url]] = backend_dict[reverse_dict[ava_url]] + 1
+                    backend_info["gpu"] = backend_dict
+                else:
+                    backend_dict = {}
+                    backend_info["gpu"] = {}
+                    for i in list(config.novelai_backend_url_dict.keys()):
+                        backend_dict[i] = 1
+                        backend_info["gpu"] = backend_dict
+                r.set(day, str(backend_info))
+        except Exception:
+            logger.warning("redis出错惹!不过问题不大")
+            logger.info(traceback.print_exc())
     else:
-        normal_backend_name = [i for i in normal_backend]
-    if is_avaiable == 0:
-        logger.debug("进入后端选择")
-        ava_url = await chose_backend(state_dict, normal_backend, task_type)
-
+        filename = "data/novelai/day_limit_data.json"
+        if os.path.exists(filename):
+            async with aiofiles.open(filename, "r") as f:
+                json_ = await f.read()
+                json_ = json.loads(json_)
+            json_[day]["gpu"][reverse_dict[ava_url]] = json_[day]["gpu"][reverse_dict[ava_url]] + 1
+            async with aiofiles.open(filename, "w") as f:
+                await f.write(json.dumps(json_))
+        else:
+            pass
     logger.info(f"已选择后端{reverse_dict[ava_url]}")
-    tc = int(state_dict[ava_url][task_type]["info"]["tasks_count"])
-    tc += 1
-    state_dict[ava_url]["status"] = task_type
-    state_dict[ava_url]["start_time"] = time.time()
-    state_dict[ava_url][task_type]["info"]["tasks_count"] = tc
-    with open("data/novelai/load_balance.json", "w", encoding="utf-8") as f:
-        f.write(json.dumps(state_dict))
     ava_url_index = list(backend_url_dict.values()).index(ava_url)
     ava_url_tuple = (ava_url, reverse_dict[ava_url], all_resp, len(normal_backend))
-    return ava_url_index, ava_url_tuple, normal_backend, state_dict
+    return ava_url_index, ava_url_tuple, normal_backend
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from ..extension.translation import translate
 
 
 async def prepocess_tags(tags: list[str]):
-    tags: str = "".join([i+" " for i in tags if isinstance(i,str)])
+    tags: str = "".join([i+", " for i in tags if isinstance(i,str)])
     # 去除CQ码
     tags = re.sub("\[CQ[^\s]*?]", "", tags)
     # 检测中文
     taglist = tags.split(",")
     tagzh = ""
     tags_ = ""
     for i in taglist:
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/version.py` & `nonebot_plugin_stable_diffusion_diao-0.3/nonebot_plugin_stable_diffusion_diao/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,46 +5,45 @@
 
 from .utils import check_last_version, sendtosuperuser, compare_version
 class Version():
     version: str  # 当前版本
     lastcheck: float = 0  # 上次检查时间
     ispushed: bool = True  # 是否已经推送
     latest: str = "0.0.0"  # 最新版本
-    package = "nonebot-plugin-novelai"
+    package = "nonebot-plugin-stable-diffusion-diao"
     url = "https://sena-nana.github.io/MutsukiDocs/update/novelai/"
 
     def __init__(self):
         # 初始化当前版本
         try:
             self.version = version(self.package)
         except:
-            self.version = "0.5.7"
+            self.version = "0.3.0"
 
     async def check_update(self):
         """检查更新，并推送"""
         # 每日检查
         if time.time() - self.lastcheck > 80000:
             update = await check_last_version(self.package)
             # 判断是否重复检查
             if await compare_version(self.latest, update):
                 self.latest = update
                 # 判断是否是新版本
                 if await compare_version(self.version, self.latest):
                     logger.info(self.push_txt())
                     self.ispushed = False
                 else:
-                    logger.info(f"novelai插件检查版本完成，当前版本{self.version}，最新版本{self.latest}")
+                    logger.info(f"插件检查版本完成，当前版本{self.version}，最新版本{self.latest}")
             else:
-                logger.info(f"novelai插件检查版本完成，当前版本{self.version}，最新版本{self.latest}")
+                logger.info(f"插件检查版本完成，当前版本{self.version}，最新版本{self.latest}")
             self.lastcheck = time.time()
         # 如果没有推送，则启动推送流程
         if not self.ispushed:
             await sendtosuperuser(self.push_txt())
             self.ispushed = True
 
     def push_txt(self):
         # 获取推送文本
         logger.debug(self.__dict__)
-        return f"novelai插件检测到新版本{self.latest},当前版本{self.version},请使用pip install --upgrade {self.package}命令升级,更新日志：{self.url}"
-
+        return f"插件检测到新版本{self.latest},当前版本{self.version},请使用pip install --upgrade {self.package}命令升级,更新日志：{self.url}"
 
 version = Version()
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.3/pyproject.toml` & `nonebot_plugin_stable_diffusion_diao-0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [project]
 name = "nonebot-plugin-stable-diffusion-diao"
-version = "0.2.3"
+version = "0.3"
 description = "主要面对stable-diffusion-webui-api的nonebot2插件"
 authors = [
     { name = "DiaoDaiaChan", email = "diaodaiachan@qq.com" },
 ]
 dependencies = [
     "aiofiles>=23.1.0",
     "aiohttp>=3.8.4",
     "nonebot-adapter-onebot>=2.1.3",
     "nonebot2>=2.0.0b4",
     "nonebot-plugin-htmlrender==0.2.0.3",
     "Pillow>=9.5.0",
     "qrcode>=7.4.2",
     "tqdm",
+    "redis",
 ]
 
 [tool.pdm.dependencies]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [tool.pdm.dependencies.tensorflow]
```

