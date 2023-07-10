# Comparing `tmp/nonebot_plugin_gachalogs-0.2.8.tar.gz` & `tmp/nonebot_plugin_gachalogs-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_gachalogs-0.2.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_gachalogs-0.2.9.tar", max compression
```

## Comparing `nonebot_plugin_gachalogs-0.2.8.tar` & `nonebot_plugin_gachalogs-0.2.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-01-05 10:23:39.429682 nonebot_plugin_gachalogs-0.2.8/LICENSE
--rw-r--r--   0        0        0     9509 2023-01-05 10:23:39.429682 nonebot_plugin_gachalogs-0.2.8/README.md
--rw-r--r--   0        0        0    14612 2023-01-05 10:23:39.741681 nonebot_plugin_gachalogs-0.2.8/nonebot_plugin_gachalogs/__init__.py
--rw-r--r--   0        0        0     3974 2023-01-05 10:23:39.741681 nonebot_plugin_gachalogs-0.2.8/nonebot_plugin_gachalogs/__meta__.py
--rw-r--r--   0        0        0     7734 2023-01-05 10:23:39.741681 nonebot_plugin_gachalogs-0.2.8/nonebot_plugin_gachalogs/data_export.py
--rw-r--r--   0        0        0    14162 2023-01-05 10:23:39.741681 nonebot_plugin_gachalogs-0.2.8/nonebot_plugin_gachalogs/data_import.py
--rw-r--r--   0        0        0    26720 2023-01-05 10:23:39.741681 nonebot_plugin_gachalogs-0.2.8/nonebot_plugin_gachalogs/data_render.py
--rw-r--r--   0        0        0    24153 2023-01-05 10:23:39.741681 nonebot_plugin_gachalogs-0.2.8/nonebot_plugin_gachalogs/data_source.py
--rw-r--r--   0        0        0    17121 2023-01-05 10:23:39.741681 nonebot_plugin_gachalogs-0.2.8/nonebot_plugin_gachalogs/gacha_achieve.py
--rw-r--r--   0        0        0      741 2023-01-05 10:23:39.741681 nonebot_plugin_gachalogs-0.2.8/pyproject.toml
--rw-r--r--   0        0        0    10481 1970-01-01 00:00:00.000000 nonebot_plugin_gachalogs-0.2.8/setup.py
--rw-r--r--   0        0        0    10492 1970-01-01 00:00:00.000000 nonebot_plugin_gachalogs-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-01-14 06:18:59.526821 nonebot_plugin_gachalogs-0.2.9/LICENSE
+-rw-r--r--   0        0        0     9940 2023-01-14 06:18:59.526821 nonebot_plugin_gachalogs-0.2.9/README.md
+-rw-r--r--   0        0        0    14433 2023-01-14 06:18:59.818824 nonebot_plugin_gachalogs-0.2.9/nonebot_plugin_gachalogs/__init__.py
+-rw-r--r--   0        0        0     4008 2023-01-14 06:18:59.818824 nonebot_plugin_gachalogs-0.2.9/nonebot_plugin_gachalogs/__meta__.py
+-rw-r--r--   0        0        0     7738 2023-01-14 06:18:59.818824 nonebot_plugin_gachalogs-0.2.9/nonebot_plugin_gachalogs/data_export.py
+-rw-r--r--   0        0        0    14282 2023-01-14 06:18:59.818824 nonebot_plugin_gachalogs-0.2.9/nonebot_plugin_gachalogs/data_import.py
+-rw-r--r--   0        0        0    27064 2023-01-14 06:18:59.818824 nonebot_plugin_gachalogs-0.2.9/nonebot_plugin_gachalogs/data_render.py
+-rw-r--r--   0        0        0    23969 2023-01-14 06:18:59.818824 nonebot_plugin_gachalogs-0.2.9/nonebot_plugin_gachalogs/data_source.py
+-rw-r--r--   0        0        0    17371 2023-01-14 06:18:59.818824 nonebot_plugin_gachalogs-0.2.9/nonebot_plugin_gachalogs/gacha_achieve.py
+-rw-r--r--   0        0        0     1191 2023-01-14 06:18:59.822824 nonebot_plugin_gachalogs-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0    10918 1970-01-01 00:00:00.000000 nonebot_plugin_gachalogs-0.2.9/setup.py
+-rw-r--r--   0        0        0    10921 1970-01-01 00:00:00.000000 nonebot_plugin_gachalogs-0.2.9/PKG-INFO
```

### Comparing `nonebot_plugin_gachalogs-0.2.8/LICENSE` & `nonebot_plugin_gachalogs-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gachalogs-0.2.8/README.md` & `nonebot_plugin_gachalogs-0.2.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 <h1 align="center">NoneBot Plugin GachaLogs</h1></br>
 
 
 <p align="center">🤖 用于分析与管理原神祈愿记录的 NoneBot2 插件</p></br>
 
 
-<p align="center"><b>现已支持祈愿历史记录链接自动更新！</b></p></br>
-
-
 <p align="center">
   <a href="https://github.com/monsterxcn/nonebot-plugin-gachalogs/actions">
-    <img src="https://img.shields.io/github/actions/workflow/status/monsterxcn/nonebot-plugin-gachalogs/publish.yml?branch=main&style=flat-square" alt="actions">
+    <img src="https://img.shields.io/github/actions/workflow/status/monsterxcn/nonebot-plugin-gachalogs/publish.yml?branch=main" alt="actions">
   </a>
   <a href="https://raw.githubusercontent.com/monsterxcn/nonebot-plugin-gachalogs/master/LICENSE">
-    <img src="https://img.shields.io/github/license/monsterxcn/nonebot-plugin-gachalogs?style=flat-square" alt="license">
+    <img src="https://img.shields.io/github/license/monsterxcn/nonebot-plugin-gachalogs" alt="license">
   </a>
   <a href="https://pypi.python.org/pypi/nonebot-plugin-gachalogs">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-gachalogs?style=flat-square" alt="pypi">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-gachalogs" alt="pypi">
+  </a>
+  <a href="https://www.python.org/">
+    <img src="https://img.shields.io/badge/python-3.8+-blue" alt="python" />
+  </a><br />
+  <a href="https://github.com/psf/black">
+    <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black" />
+  </a>
+  <a href="https://pycqa.github.io/isort">
+    <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?&labelColor=ef8336" alt="Imports: isort" />
+  </a>
+  <a href="https://results.pre-commit.ci/latest/github/monsterxcn/nonebot-plugin-gachalogs/main">
+    <img src="https://results.pre-commit.ci/badge/github/monsterxcn/nonebot-plugin-gachalogs/main.svg" alt="pre-commit" />
   </a>
-  <img src="https://img.shields.io/badge/python-3.8+-blue?style=flat-square" alt="python"><br />
 </p></br>
 
 
 | ![祈愿统计图](https://user-images.githubusercontent.com/22407052/198547014-469865b5-a298-4b91-beb2-645e028a4721.PNG) | ![成就示意图](https://user-images.githubusercontent.com/22407052/210336667-ecb56bcb-42dc-4235-ab17-1e30bea04362.PNG) |
 |:--:|:--:|
 
 
 ## 安装方法
 
 
-如果你正在使用 2.0.0.beta1 以上版本 NoneBot，推荐使用以下命令安装：
+如果你正在使用 2.0.0.beta1 以上版本 NoneBot2，推荐使用以下命令安装：
 
 
 ```bash
 # 从 nb_cli 安装
 python -m nb_cli plugin install nonebot-plugin-gachalogs
 
 # 或从 PyPI 安装
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
                     ****** NoneBot Plugin GachaLogs ******
         ð¤ ç¨äºåæä¸ç®¡çåç¥ç¥æ¿è®°å½ç NoneBot2 æä»¶
-              ç°å·²æ¯æç¥æ¿åå²è®°å½é¾æ¥èªå¨æ´æ°ï¼
                       [actions] [license] [pypi] [python]
+               [Code_style:_black] [Imports:_isort] [pre-commit]
 | ![ç¥æ¿ç»è®¡å¾](https://user-images.githubusercontent.com/22407052/
 198547014-469865b5-a298-4b91-beb2-645e028a4721.PNG) | ![æå°±ç¤ºæå¾](https:
 //user-images.githubusercontent.com/22407052/210336667-ecb56bcb-42dc-4235-ab17-
 1e30bea04362.PNG) | |:--:|:--:| ## å®è£æ¹æ³ å¦æä½ æ­£å¨ä½¿ç¨
-2.0.0.beta1 ä»¥ä¸çæ¬ NoneBotï¼æ¨èä½¿ç¨ä»¥ä¸å½ä»¤å®è£ï¼ ```bash #
+2.0.0.beta1 ä»¥ä¸çæ¬ NoneBot2ï¼æ¨èä½¿ç¨ä»¥ä¸å½ä»¤å®è£ï¼ ```bash #
 ä» nb_cli å®è£ python -m nb_cli plugin install nonebot-plugin-gachalogs #
 æä» PyPI å®è£ python -m pip install nonebot-plugin-gachalogs ``` ##
 ä½¿ç¨é¡»ç¥ - åæ¬¡ä½¿ç¨ `æ½å¡è®°å½`
 å½ä»¤æ¶ï¼è¦æ±è¾å¥ç¥æ¿åå²è®°å½é¾æ¥æç±³åæ¸¸éè¡è¯
 Cookieãå¦æåæ¬¡ä½¿ç¨è¾å¥é¾æ¥ï¼åªè¦åå¤çåå®¹ä¸­å«æå³å¯ï¼ä¸å¿æå¨æªååç¡®çé¾æ¥ï¼ï¼å¨è¯¥é¾æ¥ç
 AuthKey è¿æï¼24 å°æ¶ï¼åéè¦éæ°è¾å¥é¾æ¥æ Cookie
 æè½å·æ°æ°æ®ãå¦æåæ¬¡ä½¿ç¨è¾å¥ Cookieï¼åªè¦ Cookie
```

### Comparing `nonebot_plugin_gachalogs-0.2.8/nonebot_plugin_gachalogs/__init__.py` & `nonebot_plugin_gachalogs-0.2.9/nonebot_plugin_gachalogs/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,34 @@
-from pathlib import Path
 from typing import Dict
+from pathlib import Path
 
-from nonebot import on_command, on_notice
-from nonebot.adapters import Bot as rBot
-from nonebot.adapters import Event as rEvent
-from nonebot.log import logger
 from nonebot.rule import Rule
+from nonebot.log import logger
 from nonebot.typing import T_State
-
-try:
-    from nonebot.adapters.onebot.v11 import ActionFailed, Bot, Message, MessageSegment
-    from nonebot.adapters.onebot.v11.event import (
-        GroupMessageEvent,
-        MessageEvent,
-        NoticeEvent,
-    )
-except ImportError:
-    from nonebot.adapters.cqhttp import ActionFailed, Bot, Message, MessageSegment  # type: ignore
-    from nonebot.adapters.cqhttp.event import GroupMessageEvent, MessageEvent, NoticeEvent  # type: ignore
+from nonebot.adapters import Bot as rBot
+from nonebot import on_notice, on_command
+from nonebot.adapters import Event as rEvent
+from nonebot.adapters.onebot.v11.exception import ActionFailed
+from nonebot.adapters.onebot.v11 import Bot, Message, MessageSegment
+from nonebot.adapters.onebot.v11.event import (
+    NoticeEvent,
+    MessageEvent,
+    GroupMessageEvent,
+)
 
 from .__meta__ import SAFE_GROUP
 from .data_export import gnrtGachaFile
 from .data_import import importGachaFile
-from .data_render import gnrtGachaArchieve, gnrtGachaInfo
+from .data_render import gnrtGachaInfo, gnrtGachaArchieve
 from .data_source import (
+    logsHelper,
     checkAuthKey,
     configHelper,
-    getFullGachaLogs,
-    logsHelper,
     updateLogsUrl,
+    getFullGachaLogs,
 )
 
 
 async def _OFFLINE_FILE(bot: "rBot", event: "rEvent") -> bool:
     if isinstance(event, NoticeEvent):
         if event.notice_type in ["offline_file", "group_upload"]:  # type: ignore
             if hasattr(event, "user_id") and hasattr(event, "file"):
@@ -62,15 +58,17 @@
         if "command_arg" in list(state.get("_prefix", {}))
         else str(event.get_plaintext()).strip()
     ).split(" ")
     args = [arg.strip() for arg in args if ("[CQ:" not in arg) and arg]  # 阻止 CQ 码入参
     state["force"] = any(arg in ["-f", "--force", "刷新"] for arg in args)
     logger.debug(f"QQ{qq} {'' if state['force'] else '未'}要求刷新\n触发传入参数：{args}")
     # 检查当前消息来源是否安全
-    unsafe = isinstance(event, GroupMessageEvent) and (event.group_id not in SAFE_GROUP)  # type: ignore
+    unsafe = isinstance(event, GroupMessageEvent) and (
+        event.group_id not in SAFE_GROUP
+    )  # type: ignore
     # 读取配置数据
     cfg = await configHelper(qq)
     if cfg.get("error"):
         if any(s in " ".join(args) for s in ["https://", "stoken", "login_ticket"]):
             # 无缓存、触发时可能存在有效输入，跳过下一步输入
             state["args"] = " ".join(args)
         elif unsafe:
@@ -186,15 +184,17 @@
     imgB64 = await gnrtGachaArchieve(logs, uid)
     await aMatcher.finish(MessageSegment.image(imgB64))
 
 
 @eMatcher.handle()
 async def gachaExport(bot: Bot, event: MessageEvent, state: T_State):
     qq = event.get_user_id()
-    unsafe = isinstance(event, GroupMessageEvent) and (event.group_id not in SAFE_GROUP)  # type: ignore
+    unsafe = isinstance(event, GroupMessageEvent) and (
+        event.group_id not in SAFE_GROUP
+    )  # type: ignore
     # 提取导出目标 QQ 及导出方式
     target = {"qq": qq, "type": "xlsx"}
     for msgSeg in event.message:
         if msgSeg.type == "at":
             target["qq"] = msgSeg.data["qq"]
         elif msgSeg.type == "text":
             text = str(msgSeg.data["text"]).replace("ckjldc", "").lower()
```

### Comparing `nonebot_plugin_gachalogs-0.2.8/nonebot_plugin_gachalogs/__meta__.py` & `nonebot_plugin_gachalogs-0.2.9/nonebot_plugin_gachalogs/__meta__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
-from datetime import datetime
 from pathlib import Path
+from datetime import datetime
 
 from httpx import stream
-from nonebot import get_driver
 from pytz import timezone
+from nonebot import get_driver
 
 cfg = get_driver().config
 
 # 安全群组
 SAFE_GROUP = (
     list(cfg.gachalogs_safe_group) if hasattr(cfg, "gachalogs_safe_group") else []
 )
@@ -41,15 +41,17 @@
 PIE_FONT = (
     (Path(cfg.gachalogs_pie_font))
     if hasattr(cfg, "gachalogs_pie_font")
     else (LOCAL_DIR / "LXGW-Bold-minipie.ttf")
 )
 if not PIE_FONT.exists():
     with stream(
-        "GET", "https://cdn.monsterx.cn/bot/gachalogs/LXGW-Bold-minipie.ttf", verify=False
+        "GET",
+        "https://cdn.monsterx.cn/bot/gachalogs/LXGW-Bold-minipie.ttf",
+        verify=False,
     ) as r:
         with open(PIE_FONT, "wb") as f:
             for chunk in r.iter_bytes():
                 f.write(chunk)
 
 # 成就绘图资源
 ACHIEVE_FONT = (
@@ -63,15 +65,17 @@
     ) as r:
         with open(ACHIEVE_FONT, "wb") as f:
             for chunk in r.iter_bytes():
                 f.write(chunk)
 ACHIEVE_BG = LOCAL_DIR / "achieve-nodetail.png"
 if not ACHIEVE_BG.exists():
     with stream(
-        "GET", "https://cdn.monsterx.cn/bot/gachalogs/achieve-nodetail.png", verify=False
+        "GET",
+        "https://cdn.monsterx.cn/bot/gachalogs/achieve-nodetail.png",
+        verify=False,
     ) as r:
         with open(ACHIEVE_BG, "wb") as f:
             for chunk in r.iter_bytes():
                 f.write(chunk)
 ACHIEVE_BG_DETAIL = LOCAL_DIR / "achieve-detail.png"
 if not ACHIEVE_BG_DETAIL.exists():
     with stream(
```

### Comparing `nonebot_plugin_gachalogs-0.2.8/nonebot_plugin_gachalogs/data_export.py` & `nonebot_plugin_gachalogs-0.2.9/nonebot_plugin_gachalogs/data_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 # Modified from @sunfkny/genshin-gacha-export
 # https://github.com/sunfkny/genshin-gacha-export/blob/main/UIGF_converter.py
 # https://github.com/sunfkny/genshin-gacha-export/blob/main/writeXLSX.py
 
 import json
 from pathlib import Path
-from time import localtime, strftime, time
-from typing import Dict, Generator, List, Literal
+from time import time, strftime, localtime
+from typing import Dict, List, Literal, Generator
 
 from nonebot.log import logger
 from xlsxwriter import Workbook
 
-from .__meta__ import GACHA_TYPE, GACHA_TYPE_FULL, LOCAL_DIR
 from .data_source import logsHelper
+from .__meta__ import LOCAL_DIR, GACHA_TYPE, GACHA_TYPE_FULL
 
 
 def gnrtId() -> Generator[str, None, None]:
     """生成物品 ID"""
+
     id = 1000000000000000000
     while True:
         id = id + 1
         yield str(id)
 
 
 async def transUIGF(uid: str, gachaLogs: Dict) -> Dict:
     """
     转换原始请求结果为 UIGF JSON
 
     * ``param uid: str`` 抽卡记录所属 UID
     * ``param gachaLogs: dict`` 原始请求结果
     - ``return: Dict`` UIGF 格式数据
     """
+
     uigf = {
         "info": {
             "uid": uid,
             "lang": "zh-cn",
             "export_time": strftime("%Y-%m-%d %H:%M:%S", localtime()),
             "export_timestamp": int(time()),
             "export_app": "nonebot-plugin-gachalogs",
@@ -65,14 +67,15 @@
     转换原始请求结果为 UIGF XLSX
 
     * ``param uid: str`` 抽卡记录所属 UID
     * ``param gachaLogs: dict`` 原始请求结果
     * ``param uigfList: list`` UIGF 格式数据，由 ``transUIGF()`` 生成
     - ``return: Path`` XLSX 文件路径
     """
+
     exportTime = strftime("%Y%m%d%H%M%S", localtime())
     wbPath = LOCAL_DIR / f"Wish-{uid}-{exportTime}.xlsx"
     wb = Workbook(wbPath)
     # 重排顺序为 301 302 200 100（角色、武器、常驻、新手
     writeOrder = sorted(GACHA_TYPE.keys(), key=lambda t: t[0], reverse=True)
     for banner in writeOrder:
         # 新建页面
@@ -191,14 +194,15 @@
     """
     导出抽卡数据
 
     * ``param config: Dict`` 配置文件
     * ``param outFormat: Literal["xlsx", "json"]`` 导出格式
     - ``return: Dict`` 导出结果，出错时返回 ``{"error": "错误信息"}``
     """
+
     # 无抽卡记录数据直接返回
     if not config.get("logs"):
         return {"error": "没有抽卡记录可供导出哦！"}
     # 读取抽卡记录缓存
     uid, gachaLogs = await logsHelper(config["logs"])
     if not uid.isdigit():
         return {"error": uid}
```

### Comparing `nonebot_plugin_gachalogs-0.2.8/nonebot_plugin_gachalogs/data_import.py` & `nonebot_plugin_gachalogs-0.2.9/nonebot_plugin_gachalogs/data_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
-from datetime import datetime
 from pathlib import Path
-from typing import Any, Dict, Literal, Optional, Set, Tuple, Union
+from datetime import datetime
+from typing import Any, Set, Dict, Tuple, Union, Literal, Optional
 
-from httpx import AsyncClient, NetworkError
 from nonebot.log import logger
 from nonebot.utils import run_sync
+from httpx import AsyncClient, NetworkError
 
-from .__meta__ import GACHA_TYPE, LOCAL_DIR
 from .data_render import gnrtGachaInfo
-from .data_source import configHelper, logsHelper
+from .__meta__ import LOCAL_DIR, GACHA_TYPE
+from .data_source import logsHelper, configHelper
 
 
 @run_sync
 def analysisData(data: Dict[str, Any]) -> Tuple[int, str, Literal["inner", "uigf"]]:
     """
     分析导入数据
 
@@ -97,15 +97,15 @@
     """
     获取导入目标初始配置
 
     * ``param qq: str`` 导入动作触发 QQ
     * ``param uid: str`` 抽卡数据归属 UID
     * ``param isSuperuser: bool`` 导入动作触发 QQ 是否为超级用户
     - ``return: Tuple[Optional[Path], str, Dict[str, Any]]`` 导入目标本地记录文件、导入目标 QQ、导入目标初始配置（出错时返回 ``{"error": "}``）
-    """
+    """  # noqa: E501
 
     configKey, config = qq, (await configHelper(qq))
 
     # 非超级用户只能新增或更新自己
     if not isSuperuser:
         # 没有抽卡记录配置视为新增
         if config.get("error"):
@@ -116,15 +116,17 @@
                 "time": 0,
                 "game_biz": "hk4e_cn",
                 "game_uid": uid,
                 "region": "cn_gf01" if uid[0] in ["1", "2"] else "cn_qd01",
             }
         if uid != config["game_uid"]:
             config = {
-                "error": f"QQ{qq} 已经有 UID{config['game_uid']} 的抽卡记录，不能导入属于 UID{uid} 的抽卡记录"
+                "error": "QQ{} 已经有 UID{} 的抽卡记录，不能导入属于 UID{} 的抽卡记录".format(
+                    qq, config["game_uid"], uid
+                )
             }
     # 超级用户可以新增或更新自己，也可以更新别人
     else:
         # 超级用户没有抽卡记录配置 / 导入记录归属 UID 与抽卡记录配置不符
         if config.get("error") or uid != config["game_uid"]:
             # 先找一遍当前 UID 是否属于别人
             allConfig = await configHelper("0")
@@ -173,15 +175,15 @@
 
     * ``param inner: Dict`` 内部格式抽卡数据
     * ``param config: Dict`` 导入目标配置
     * ``param qq: str`` 导入目标 QQ
     * ``param uid: str`` 抽卡数据归属 UID
     * ``param timestamp: int`` 抽卡数据时间戳
     - ``return: Tuple[Dict[str, list], Dict[str, str]]`` 内部格式抽卡数据、导入结果（``{"error": "", "msg": ""}``）
-    """
+    """  # noqa: E501
 
     config["logs"] = config["logs"] or str(LOCAL_DIR / f"gachalogs-{uid}.json")
     config["time"] = timestamp
 
     # 写入 gachalogs-{uid}.json
     res, _ = await logsHelper(config["logs"], inner)
     if not res.isdigit():
@@ -202,15 +204,15 @@
 
     * ``param uigf: Dict`` UIGF 格式抽卡数据
     * ``param config: Dict`` 导入目标配置
     * ``param qq: str`` 导入目标 QQ
     * ``param uid: str`` 抽卡数据归属 UID
     * ``param timestamp: int`` 抽卡数据时间戳
     - ``return: Tuple[Dict[str, list], Dict[str, str]]`` 内部格式抽卡数据、导入结果（``{"error": "", "msg": ""}``）
-    """
+    """  # noqa: E501
     # TODO: 优化
     # 当前写的比较臃肿，主要基于以下思路：
     # 1. 导入和本地所有 id 非官方生成的都不可信任
     # 2. 无论本地记录还是要导入的 UIGF 格式数据，
     #    某时刻的数据只能是单抽或完整的十连
     # 3. 导入后按时间顺序将记录分别插入卡池单独的列表中
     # 4. 合并过程中所有记录的顺序均保证新数据在前，旧数据在后
@@ -254,15 +256,17 @@
             if str(log["id"]).startswith("1000"):
                 log["id"] = ""
             # 内部格式数据分离为单抽和十连
             if log["time"] in localDict:
                 localDict[log["time"]].append(log)
             else:
                 localDict[log["time"]] = [log]
-    assert all(len(subList) == 1 or len(subList) == 10 for subList in localDict.values())
+    assert all(
+        len(subList) == 1 or len(subList) == 10 for subList in localDict.values()
+    )
 
     # 合并中间态
     counters = {}
     for logsTime, logs in uigfDict.items():
         banner = "301" if logs[0]["gacha_type"] == "400" else logs[0]["gacha_type"]
         if logsTime not in localDict:
             localDict[logsTime] = logs
@@ -305,15 +309,15 @@
     """
     导入抽卡数据
 
     * ``param qq: str`` 发送者 QQ
     * ``param file: Dict[str, str]`` 导入文件数据
     * ``param superusers: Set[str]`` 超级用户集合
     - ``return: Dict[str, str]`` 导入结果，``{"error": "", "bak": "", "msg": "", "img": bytes}``
-    """
+    """  # noqa: E501
 
     # 获取导入文件数据
     data = await getFileData(file["url"])
     # 文件数据获取出错返回错误消息
     if data.get("error"):
         return data
```

### Comparing `nonebot_plugin_gachalogs-0.2.8/nonebot_plugin_gachalogs/data_render.py` & `nonebot_plugin_gachalogs-0.2.9/nonebot_plugin_gachalogs/data_render.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-from copy import deepcopy
-from datetime import datetime
 from io import BytesIO
 from math import floor
-from time import localtime, strftime
-from typing import Dict, List, Literal, Tuple
+from copy import deepcopy
+from datetime import datetime
+from time import strftime, localtime
+from typing import Dict, List, Tuple, Literal
 
+from pytz import timezone
 import matplotlib.pyplot as plt
-from matplotlib import font_manager as fm
 from nonebot.log import logger
 from nonebot.utils import run_sync
+from matplotlib import font_manager as fm
 from PIL import Image, ImageDraw, ImageFont
-from pytz import timezone
 
+from .gacha_achieve import calcAchievement
 from .__meta__ import (
-    ACHIEVE_BG,
-    ACHIEVE_BG_DETAIL,
-    ACHIEVE_FONT,
-    GACHA_TYPE,
     PIE_FONT,
     PIL_FONT,
     POOL_INFO,
+    ACHIEVE_BG,
+    GACHA_TYPE,
+    ACHIEVE_FONT,
+    ACHIEVE_BG_DETAIL,
 )
-from .gacha_achieve import calcAchievement
 
 
 def percent(a: int, b: int, rt: Literal["pct", "rgb"] = "pct") -> str:
     """
     概率百分数字符串或根据概率生成的 RGB 颜色生成
     ref: https://github.com/voderl/genshin-gacha-analyzer/blob/main/src/pages/ShowPage/AnalysisChart/utils.ts
 
     * ``param a: int`` 数值
     * ``param b: int`` 基准值
     * ``param rt: Literal["pct", "rgb"] = "pct"`` 返回类型，默认返回概率百分数字符串
     - ``return: str`` 概率百分数字符串（格式为 ``23.33%``）或根据概率生成的 RGB 颜色（格式为 ``#FFFFFF``）
-    """
+    """  # noqa: E501
+
     if rt == "pct":
         return str(round(a / b * 100, 2)) + "%"
     # 由概率生成 RGB 颜色
     percentColors = [
         {"pct": 0.0, "color": {"r": 46, "g": 200, "b": 5}},
         {"pct": 0.77, "color": {"r": 67, "g": 93, "b": 250}},
         {"pct": 1.0, "color": {"r": 255, "g": 0, "b": 0}},
@@ -50,27 +51,28 @@
             prevPct = percentColors[prevKey]["pct"]
             upPct = (pct - prevPct) / (level["pct"] - prevPct)
             lowPct = 1 - upPct
             nowCl = level["color"]
             clR = floor(lowPct * prevCl["r"] + upPct * nowCl["r"])
             clG = floor(lowPct * prevCl["g"] + upPct * nowCl["g"])
             clB = floor(lowPct * prevCl["b"] + upPct * nowCl["b"])
-            return "#{:02X}{:02X}{:02X}".format(clR, clG, clB)
+            return f"#{clR:02X}{clG:02X}{clB:02X}"
             # return "rgb({},{},{})".format(clR, clG, clB)
     return "#FF5652"
 
 
 def getPoolTag(num: int) -> Tuple[str, str, str]:
     """
     卡池运势标签
     ref: https://github.com/vikiboss/genshin-helper/blob/main/src/render/pages/gacha/components/Overview/index.tsx
 
     * ``param num: int`` 卡池五星平均抽数
     - ``return: Tuple[str, str, str]`` 卡池运势、字体背景色、字体边缘色
-    """
+    """  # noqa: E501
+
     if num == 0:
         return "无", "#759abf", "#4d8ccb"
     if num >= 72:
         return "非", "#6c6c6c", "#505a6d"
     if num >= 68:
         return "愁", "#b8b8b8", "#9a9fa8"
     if num >= 60:
@@ -84,14 +86,15 @@
     """
     Pillow 绘制字体设置
 
     * ``param size: int`` 字体大小
     * ``param achieve: bool = False`` 是否为抽卡成就绘图（成就绘图建议使用原神字体）
     - ``return: ImageFont.FreeTypeFont`` Pillow 字体对象
     """
+
     return ImageFont.truetype(str(ACHIEVE_FONT if achieve else PIL_FONT), size=size)
 
 
 @run_sync
 def colorfulFive(
     star5Data: List, fontSize: int, maxWidth: int, isWeapon: bool = False
 ) -> Image.Image:
@@ -100,14 +103,15 @@
 
     * ``param star5Data: List`` 五星历史记录列表
     * ``param fontSize: int`` 字体大小
     * ``param maxWidth: int`` 最大宽度
     * ``param isWeapon: bool = False`` 是否为武器祈愿活动
     - ``return: Image.Image`` Pillow 图片对象
     """
+
     ImageSize = (maxWidth, 1000)
     coordX, coordY = 0, 0  # 绘制坐标
     fontPadding = 10  # 字体行间距
     result = Image.new("RGBA", ImageSize, "#f9f9f9")
     tDraw = ImageDraw.Draw(result)
     # 首行固定文本绘制
     text1st = "五星历史记录："
@@ -129,15 +133,17 @@
                     word,
                     font=fs(fontSize),
                     fill=color,
                     stroke_width=int(item["up"]),
                     stroke_fill=color,
                 )
                 # 偏移 X 轴绘制坐标使物品名称与自己的抽数间隔 1/4 个空格、抽数与下一个物品名称间隔一个空格
-                coordX += (wordW + spaceW) if word[0] == "[" else int(wordW + spaceW / 4)
+                coordX += (
+                    (wordW + spaceW) if word[0] == "[" else int(wordW + spaceW / 4)
+                )
             elif word[0] == "[":
                 # 当前行绘制超过最大宽度限制，且当前绘制为抽数，换行绘制（保证 [ 与数字不分离）
                 coordX, coordY = 0, (coordY + stepY)  # 偏移绘制坐标至下行行首
                 tDraw.text(
                     (coordX, coordY),
                     word,
                     font=fs(fontSize),
@@ -227,14 +233,15 @@
 def calcStat(gachaLogs: Dict) -> Dict:
     """
     统计数据提取
 
     * ``param gachaLogs: Dict`` 原始抽卡记录数据
     - ``return: Dict`` 统计数据
     """
+
     single = {
         "total": 0,  # 总抽数
         "cntNot5": 0,  # 未出五星抽数
         "cntStar3": 0,  # 三星物品总数
         "cntChar4": 0,  # 四星角色总数
         "cntWeapon4": 0,  # 四星武器总数
         "cntChar5": 0,  # 五星角色总数
@@ -247,15 +254,15 @@
     renderOrder = sorted(GACHA_TYPE.keys(), key=lambda k: k[0], reverse=True)
     stat = {}  # 待返回统计数据
     for banner in renderOrder:
         if not gachaLogs.get(banner):
             continue
         gachaStat = deepcopy(single)
         gachaList = gachaLogs[banner]
-        gachaList.reverse()  # 千万不可以 gachaList.sort(key=lambda item: item["time"], reverse=False)
+        gachaList.reverse()
         counter, pityCounter = 0, 0  # 总抽数计数器、保底计数器
         upCounter = {}  # UP 物品计数器
         for item in gachaList:
             counter += 1  # 总抽数计数器递增
             pityCounter += 1  # 保底计数器递增
             rankType = int(item["rank_type"])
             itemName, itemType = item["name"], item["item_type"]
@@ -320,14 +327,15 @@
 def drawPie(stat: Dict) -> Tuple[Image.Image, bool]:
     """
     单个饼图绘制
 
     * ``param stat: Dict`` 统计数据，由 ``calcStat()`` 生成
     - ``return: Tuple[Image.Image, bool]`` 返回饼图、是否展示三星物品数据
     """
+
     partMap = [
         {"label": "三星武器", "color": "#73c0de", "total": stat["cntStar3"]},
         {"label": "四星武器", "color": "#91cc75", "total": stat["cntWeapon4"]},
         {"label": "四星角色", "color": "#5470c6", "total": stat["cntChar4"]},
         {"label": "五星武器", "color": "#ee6666", "total": stat["cntWeapon5"]},
         {"label": "五星角色", "color": "#fac858", "total": stat["cntChar5"]},
     ]
@@ -338,15 +346,16 @@
         showStar3 = False
     # 提取数据
     labels = [p["label"] for p in partMap if p["total"]]
     colors = [p["color"] for p in partMap if p["total"]]
     sizes = [p["total"] for p in partMap if p["total"]]
     explode = [(0.05 if "五星" in p["label"] else 0) for p in partMap if p["total"]]
     # 绘制饼图
-    textprops = {"fontproperties": fm.FontProperties(fname=PIE_FONT, size=18)}  # type: ignore
+    fontproperties = fm.FontProperties(fname=PIE_FONT, size=18)  # type: ignore
+    textprops = {"fontproperties": fontproperties}
     fig, ax = plt.subplots()
     ax.pie(
         sizes,
         labels=labels,
         colors=colors,
         autopct="%0.2f%%",
         labeldistance=1.1,
@@ -374,14 +383,15 @@
     """
     抽卡统计信息图片生成，通过 pillow 和 matplotlib 绘制图片
 
     * ``param rawData: Dict`` 抽卡记录数据
     * ``param uid: str`` 用户 UID
     - ``return: bytes`` 图片字节数据
     """
+
     wishStat = await calcStat(rawData)
     gotPool = [key for key in wishStat if wishStat[key]["total"] > 0]
     imageList = []
     for banner in gotPool:
         poolName, poolStat = GACHA_TYPE[banner], wishStat[banner]
         isWeapon = True if banner == "302" else False  # 是否为武器祈愿
         pityCnt = 80 if isWeapon else 90
@@ -418,15 +428,17 @@
             timeStat,
             font=fs(20),
             fill="#808080",
         )
         # 绘制卡池运势
         star5Data: List[Dict] = poolStat["star5"]
         star5Avg = (
-            sum(item["count"] for item in star5Data) / len(star5Data) if star5Data else 0
+            sum(item["count"] for item in star5Data) / len(star5Data)
+            if star5Data
+            else 0
         )
         poolTag, poolTagBg, poolTagEdge = getPoolTag(round(star5Avg))
         tDraw.rounded_rectangle(
             (500 - 13 - 80, poolImgH - 13 - 80, 500 - 13, poolImgH - 13),
             fill=poolTagBg,
             radius=15,
             width=0,
@@ -470,15 +482,17 @@
                 startW = 20
                 continue
             color = (
                 (
                     "#1890ff"
                     if txtIdx in [1, 3]
                     else percent(
-                        (pityCnt - int(text)) if int(text) < 91 else (pityCnt - notStar5),
+                        (pityCnt - int(text))
+                        if int(text) < 91
+                        else (pityCnt - notStar5),
                         pityCnt,
                         "rgb",
                     )
                 )
                 if text.isdigit()
                 else "black"
             )
@@ -558,14 +572,15 @@
     """
     抽卡成就图片生成，通过 pillow 绘制图片
 
     * ``param rawData: Dict`` 抽卡记录数据
     * ``param uid: str`` 用户 UID
     - ``return: bytes`` 图片字节数据
     """
+
     scope, achievements = await calcAchievement(rawData)
     result = Image.new("RGBA", (720, 110 * len(achievements) + 10 + 100), "#f9f9f9")
     drawer = ImageDraw.Draw(result)
 
     # 标题
     title = f"UID{uid} 抽卡成就"
     drawer.text(
@@ -585,43 +600,46 @@
 
     bgPure = Image.open(ACHIEVE_BG)
     bgDetail = Image.open(ACHIEVE_BG_DETAIL)
     for aIdx, achievement in enumerate(achievements):
         startHeight = 110 * (aIdx + 1)
         bg = bgDetail if achievement.get("value") else bgPure
         result.paste(bg, (10, startHeight), bg)
-        # 名称
-        drawer.text(
-            (115, startHeight + 18),
-            achievement["title"],
-            font=fs(22, True),
-            fill="#585757",
-        )
-        # 描述
+        # 描述分行，超过三行需要调整后面 名称 描述 绘制位置
         multilineText, tmpText, tmpLength = [], "", 0
         maxLength = 445 if achievement.get("value") else 565
         for s in achievement["info"]:
             length = fs(16, True).getlength(s)
             if tmpLength + length <= maxLength:
                 tmpText += s
                 tmpLength += length
             else:
                 multilineText.append(tmpText)
                 tmpText = s
                 tmpLength = length
         if tmpText.strip():
             multilineText.append(tmpText)
         multilineText = [s.strip() for s in multilineText if s.strip()]
-        spacing = (0.3 if len(multilineText) < 3 else 0.1) * 16
+        tooMany = len(multilineText) >= 3
+        # 名称
+        drawer.text(
+            (115, startHeight + 18 - (11 if tooMany else 0)),
+            achievement["title"],
+            font=fs(22, True),
+            fill="#585757",
+        )
+        # 描述
+        spacing = (0.3 if tooMany else 0.1) * 16
         drawer.multiline_text(
             (
                 125,
                 startHeight
                 + 100
                 - 18
+                + (11 if tooMany else 0)
                 - 16 * len(multilineText)
                 - spacing * (len(multilineText) - 1),
             ),
             "\n".join(multilineText),
             font=fs(16, True),
             fill="#988B81",
             spacing=spacing,
@@ -646,15 +664,16 @@
                     fill="#988B81",
                 )
             if achievement["value"] != "达成":
                 # 绘制 总计 等数据
                 drawer.text(
                     (
                         int(
-                            582 + (128 - fs(20, True).getlength(achievement["value"])) / 2
+                            582
+                            + (128 - fs(20, True).getlength(achievement["value"])) / 2
                         ),
                         int(
                             startHeight
                             + (5 if hasAchieve else 0)
                             + (100 - fs(20, True).getbbox(achievement["value"])[-1]) / 2
                         ),
                     ),
@@ -663,20 +682,22 @@
                     fill="#84603D",
                 )
             # 绘制 时间 等数据
             drawer.text(
                 (
                     int(
                         582
-                        + (128 - fs(15, True).getlength(achievement["achievedTime"])) / 2
+                        + (128 - fs(15, True).getlength(achievement["achievedTime"]))
+                        / 2
                     ),
                     int(
                         startHeight
                         + 76
-                        + (20 - fs(15, True).getbbox(achievement["achievedTime"])[-1]) / 2
+                        + (20 - fs(15, True).getbbox(achievement["achievedTime"])[-1])
+                        / 2
                     ),
                 ),
                 achievement["achievedTime"],
                 font=fs(15, True),
                 fill="#988B81",
             )
```

### Comparing `nonebot_plugin_gachalogs-0.2.8/nonebot_plugin_gachalogs/data_source.py` & `nonebot_plugin_gachalogs-0.2.9/nonebot_plugin_gachalogs/data_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 import json
+import uuid
 import random
 import string
-import uuid
-from asyncio import sleep as asyncsleep
+from re import search
 from hashlib import md5
 from pathlib import Path
-from re import search
-from time import localtime, strftime, time
-from typing import Dict, List, Literal, Tuple, Union
 from urllib import parse
+from asyncio import sleep as asyncsleep
+from time import time, strftime, localtime
+from typing import Dict, List, Tuple, Union, Literal
 
 from httpx import AsyncClient
 from nonebot.log import logger
 
 from .__meta__ import (
+    POOL_API,
+    ROLE_API,
+    ROOT_URL,
+    LOCAL_DIR,
+    TOKEN_API,
+    EXPIRE_SEC,
+    GACHA_TYPE,
     AUTHKEY_API,
     CLIENT_SALT,
     CLIENT_TYPE,
     CLIENT_VERSION,
-    EXPIRE_SEC,
-    GACHA_TYPE,
-    LOCAL_DIR,
-    POOL_API,
-    ROLE_API,
     ROOT_OVERSEA_URL,
-    ROOT_URL,
-    TOKEN_API,
 )
 
 
 def formatInput(input: str, find: Literal["url", "cookie"]) -> Dict:
     """
     输入内容格式化，可根据输入内容提取抽卡记录链接或米游社 Cookie
 
     * ``param input: str`` 输入内容
     * ``param find: Literal["url", "cookie"]`` 提取内容类型
     - ``return: Dict`` 提取结果，格式为 ``{"url": "链接"}`` 或 ``{"login_ticket": "xx", "stoken": "xx", ...}``，出错时返回 ``{}``
-    """
+    """  # noqa: E501
+
     if find == "cookie":
         if not input:
             return {}
         cookieDict = {}
         params = [
             "account_id",
             "cookie_token",
@@ -63,15 +64,15 @@
                 for p in ["account_id", "login_uid", "stuid", "ltuid"]:
                     cookieDict[p] = cookieDict[param]
                 break
         # return "; ".join([f"{k}={v}" for k, v in cookieDict.items()])
         return cookieDict
     elif find == "url":
         # ref: https://ihateregex.io/expr/url
-        urlReg = r"https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()!@:%_\+.~#?&\/\/=]*)"
+        urlReg = r"https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()!@:%_\+.~#?&\/\/=]*)"  # noqa: E501
         matchUrl = search(urlReg, input.replace("&amp;", "&"))
         if matchUrl:
             # 找到链接后替换 Host
             root, query = matchUrl[0].split("?")
             urlRoot = (
                 ROOT_OVERSEA_URL
                 if any(x in root for x in ["webstatic-sea", "hk4e-api-os"])
@@ -82,17 +83,18 @@
 
 
 async def configHelper(qq: str, data: Dict = {}) -> Dict:
     """
     配置缓存助手，既可根据 QQ 读取配置，也可根据数据写入/删除配置缓存
 
     * ``param qq: str`` 目标 QQ，为 ``"0"`` 时返回全部配置
-    * ``param data: Dict = {}`` 配置数据，根据是否传入决定更新或读取，只有配置中有链接、Cookie 或抽卡记录缓存 或 配置中包含 force/delete 参数时才写入
+    * ``param data: Dict = {}`` 配置数据，根据是否传入决定更新或读取。配置中有链接、Cookie 或抽卡记录缓存 或 配置中包含 force/delete 参数时才写入
     - ``return: Dict`` 目标 QQ 的配置数据，删除时返回 ``{}``，出错时返回 ``{"error": "错误信息"}``
-    """
+    """  # noqa: E501
+
     cfgFile = LOCAL_DIR / "config.json"
     # 尝试读取本地配置文件
     if not cfgFile.exists():
         cfgFile.write_text("{}", encoding="utf-8")
         cfg = {}
     else:
         cfg = json.loads(cfgFile.read_text(encoding="utf-8"))
@@ -136,14 +138,15 @@
     """
     抽卡记录缓存助手，既可根据 ``file`` 路径读取抽卡记录，也可根据 ``data`` 数据写入/删除抽卡记录缓存
 
     * ``param file: Union[Path, str]`` 抽卡记录缓存文件路径
     * ``param data: Dict = {}`` 抽卡记录数据，根据是否传入决定写入/删除或读取
     - ``return: Tuple[str, Dict]`` 抽卡记录所属 UID（出错时返回错误信息）、抽卡记录数据（写入/删除时固定返回 ``{}``）
     """
+
     uid = search(r"gachalogs-([0-9]{9}).json", str(file))
     if not uid:
         raise ValueError(f"记录所属 UID 不存在！{str(file)}")
     uid, logsFile = uid.group(1), Path(file)
     # 根据是否传入抽卡记录数据决定写入/删除或读取
     if data:
         delMode = bool(data.get("delete"))
@@ -168,21 +171,26 @@
         raise ValueError(f"UID{uid} 的本地抽卡记录不存在！")
 
 
 async def queryMihoyo(
     cookie: str, aType: Literal["获取令牌", "获取角色", "获取卡池", "生成密钥"], data: Dict = {}
 ) -> Dict:
     """
-    米哈游接口请求，支持获取 ``stoken`` 令牌、获取指定 ``cookie`` 名下原神游戏角色数据、查询最新祈愿活动 ``gacha_id`` 卡池数据、生成用于抽卡记录查询的 ``authkey`` 密钥
+    米哈游接口请求，支持以下功能：
+    - 获取 ``stoken`` 令牌
+    - 获取指定 ``cookie`` 名下原神游戏角色数据
+    - 查询最新祈愿活动 ``gacha_id`` 卡池数据
+    - 生成用于抽卡记录查询的 ``authkey`` 密钥
 
     * ``param cookie: str`` 米哈游通行证 Cookie，获取令牌和获取卡池时可传入空
     * ``param aType: Literal["获取令牌", "获取角色", "获取卡池", "生成密钥"]`` 请求类型
     * ``param data: Dict = {}`` 请求数据，根据需要被赋值为 ``params`` ``content`` 等
     - ``return: Dict`` 请求结果，出错时返回 ``{"error": "错误信息"}``
     """
+
     if aType == "获取卡池":
         # 可能不需要每次都向米游社发起请求，此处将返回固定为常驻祈愿活动数据
         return {"type": "200", "pool": "fecafa7b6560db5f3182222395d88aaa6aaac1bc"}
     t = str(int(time()))
     r = "".join(random.sample(string.ascii_lowercase + string.digits, 6))
     m = md5(f"salt={CLIENT_SALT}&t={t}&r={r}".encode()).hexdigest()
     headers = {
@@ -201,20 +209,17 @@
     }
     if aType == "获取令牌":
         headers.update(
             {
                 "origin": "https://webstatic.mihoyo.com",
                 "referer": "https://webstatic.mihoyo.com/",
                 "user-agent": (
-                    # "Mozilla/5.0 (Linux; Android 10; MIX 2 Build/QKQ1.190825.002; wv) "
-                    # "AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 "
-                    # f"Chrome/83.0.4103.101 Mobile Safari/537.36 miHoYoBBS/{CLIENT_VERSION}"
-                    "Mozilla/5.0 (Linux; Android 12; SM-G977N Build/SP1A.210812.016; wv) "
-                    "AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0"
-                    f"Chrome/104.0.5112.69 Mobile Safari/537.36 miHoYoBBS/{CLIENT_VERSION}"
+                    "Mozilla/5.0 (Linux; Android 12; SM-G977N Build/SP1A.210812.016"
+                    "; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome"
+                    f"/104.0.5112.69 Mobile Safari/537.36 miHoYoBBS/{CLIENT_VERSION}"
                 ),
                 "x-requested-with": "com.mihoyo.hyperion",
             }
         )
     elif aType == "生成密钥":
         headers["content-type"] = "application/json; charset=UTF-8"
     async with AsyncClient() as client:
@@ -258,14 +263,15 @@
     """
     抽卡记录链接验证，检查传入抽卡记录链接 `url` 是否有效（AuthKey 有效期 24h）
 
     * ``param url: str`` 抽卡记录链接
     * ``param skipFmt: bool = True`` 是否跳过格式检查，传入 ``False`` 将根据格式检查结果修正抽卡记录链接
     - ``return: str`` 抽卡记录链接，出错时返回错误信息
     """
+
     if not skipFmt:
         urlRes = formatInput(url, find="url")
         if not urlRes:
             return "未找到有效的抽卡记录链接！"
         else:
             url = urlRes["url"]
     logger.debug(f"验证抽卡记录链接 {url}")
@@ -283,30 +289,31 @@
             logger.opt(exception=e).error("抽卡记录链接验证出错")
             return f"[{e.__class__.__name__}] 链接验证出错！"
     if not resJson["data"]:
         if resJson.get("message", "") == "authkey timeout":
             return "链接 AuthKey 失效！"
         if resJson.get("message", "") == "authkey error":
             return "链接 AuthKey 错误！"
-        # ref: https://webstatic.mihoyo.com/admin/mi18n/hk4e_cn/20190926_5d8c80193de82/20190926_5d8c80193de82-zh-cn.json
+        # ref: https://webstatic.mihoyo.com/admin/mi18n/hk4e_cn/20190926_5d8c80193de82/20190926_5d8c80193de82-zh-cn.json  # noqa: E501
         logger.error(
             f"抽卡记录链接有问题 {resJson.get('retcode', 777)} {resJson.get('message', '')}"
         )
         return f"[{resJson.get('retcode', 777)}]链接有问题！"
     return url
 
 
 async def updateLogsUrl(url: str, cookie: str) -> Tuple[str, Dict]:
     """
     抽卡记录链接更新，可根据 `cookie` 初始化或更新抽卡记录链接
 
     * ``param url: str`` 抽卡记录链接
     * ``param cookie: str`` 含有 `stoken` 字段的米游社 Cookie
     - ``return: Tuple[str, Dict]`` 抽卡记录链接（出错时返回 ``"错误信息"``）、角色及 Cookie 字典数据（出错或旧链接未过期时返回 ``{}``）
-    """
+    """  # noqa: E501
+
     # 检查传入链接是否仍然有效
     url = await checkAuthKey(url)
     if url.startswith("https://"):
         return url, {}
     # 提取 cookie 中有效字段字典
     usefulCk = formatInput(cookie, find="cookie")
     # Cookie 验证及补全
@@ -338,16 +345,16 @@
     authkeyRes = await queryMihoyo(ckStr, "生成密钥", data=data)
     if not authkeyRes.get("authkey"):
         return "生成密钥失败！", {"cookie": ckStr}
     # 更新抽卡记录链接中的卡池 ID
     poolRes = await queryMihoyo("", "获取卡池")
     if not poolRes.get("pool"):
         poolRes = {
-            "type": "200",  # querys.get("init_type")
-            "pool": "fecafa7b6560db5f3182222395d88aaa6aaac1bc",  # querys.get("gacha_id")
+            "type": "200",  # init_type
+            "pool": "fecafa7b6560db5f3182222395d88aaa6aaac1bc",  # gacha_id
         }
     # 提取传入 url 中请求参数字典
     parsed = parse.urlparse(url)
     querys = dict(parse.parse_qsl(str(parsed.query)))
     # 更新抽卡记录链接
     if not querys:
         querys = {
@@ -355,16 +362,16 @@
             "sign_type": "2",
             "auth_appid": "webview_gacha",
             "init_type": poolRes["type"],
             "gacha_id": poolRes["pool"],
             "timestamp": str(int(time())),
             "lang": "zh-cn",
             "device_type": "mobile",
-            # "ext": {"loc":{"x":-672.817138671875,"y":122.54130554199219,"z":-87.4539794921875},"platform":"IOS"},  # "platform":"Android"
-            # "game_version": "CNRELiOS2.8.0_R9182063_S9401797_D9464149",  # CNRELAndroid2.8.0_R9182063_S9401797_D9464149
+            # "ext": {"loc":{"x":-672.817138671875,"y":122.54130554199219,"z":-87.4539794921875},"platform":"IOS"},  # noqa: E501
+            # "game_version": "CNRELiOS2.8.0_R9182063_S9401797_D9464149",
             "plat_type": "android",  # ios
             "region": role["region"],
             "authkey": authkeyRes["authkey"],
             "game_biz": role["game_biz"],
             "gacha_type": "301",
             "page": "1",
             "size": "6",
@@ -396,14 +403,15 @@
 
     * ``param logUrl: str`` 抽卡记录链接
     * ``param gachaType: str`` 祈愿类型（请求参数 ``gacha_type``）
     * ``param page: int`` 页码（请求参数 ``page``）
     * ``param endId: int`` 结束 ID（请求参数 ``end_id``）
     - ``return: str`` 指定类型抽卡记录接口
     """
+
     parsed = parse.urlparse(logUrl)
     querys = dict(parse.parse_qsl(str(parsed.query)))
     querys.update(
         {
             "lang": "zh-cn",
             "gacha_type": gachaType,
             "page": str(page),
@@ -418,14 +426,15 @@
     """
     指定类型抽卡记录获取
 
     * ``param logUrl: str`` 抽卡记录链接
     * ``param gachaType: str`` 祈愿类型，实际类型应为 ``Literal["100", "200", "301", "302"]``
     - ``return: List`` 指定类型抽卡记录
     """
+
     logsList, endId, page = [], 0, 1
     async with AsyncClient() as client:
         while True:
             logger.debug(f"正在获取 {GACHA_TYPE[gachaType]} 第 {page} 页")
             api = getGachaLogsApi(logUrl, gachaType, page, endId)
             res = await client.get(api)
             try:
@@ -452,14 +461,15 @@
 async def getAllTypeLogs(logUrl: str) -> Dict:
     """
     全部抽卡记录获取，可根据输入的抽卡记录链接获取 6 个月内全部抽卡记录
 
     * ``param logUrl: str`` 抽卡记录链接
     - ``return: Dict`` 全部抽卡记录，格式为``{"msg": "uid 或错误信息", "logs": {}]``
     """
+
     start, uidGot, newLogs = time(), "", {}
     # 获取最新抽卡记录
     for banner in GACHA_TYPE:
         remoteLogs = await getSingleTypeLogs(logUrl, banner)
         if remoteLogs:
             newLogs[banner] = remoteLogs
             if not uidGot:
@@ -480,27 +490,30 @@
 
     * ``param locLogs: Dict`` 本地记录数据
     * ``param newLogs: Dict`` 新增记录数据
     * ``param config: Dict`` 配置文件
     * ``param qq: str`` 目标 QQ
     - ``return: Dict`` 合并后的记录数据，格式为``{"uid": "123456789", "msg": "文字消息", "logs": {}]``
     """
+
     msgList, logs = [], {}  # 消息列表、待写入记录
     for banner in GACHA_TYPE:
         locItems, newItems = locLogs.get(banner, []), newLogs.get(banner, [])
         # 本地记录同步至待写入记录
         if locItems:
             logs[banner] = locItems
         # 本地记录与最新记录相同，跳过
         if locItems == newItems:
             continue
         # UID 不同，立即单独展示最新记录
         if len(locItems) and len(newItems) and locItems[0]["uid"] != newItems[0]["uid"]:
             logger.info(
-                f"{GACHA_TYPE[banner]}({banner}) 中发现 UID 不同（{locItems[0]['uid']}!={newItems[0]['uid']}），跳过合并"
+                "{}({}) 中发现 UID 不同（{}!={}），跳过合并".format(
+                    GACHA_TYPE[banner], banner, locItems[0]["uid"], newItems[0]["uid"]
+                )
             )
             return {
                 "uid": newItems[0]["uid"],
                 "msg": "新增与缓存数据 UID 不一致\n跳过合并，单独展示新增记录..",
                 "logs": newLogs,
             }
         # 本地记录与最新记录对比合并
@@ -546,14 +559,15 @@
     抽卡记录数据获取入口，可根据配置获取最新完整抽卡记录
 
     * ``param config: Dict`` 配置数据
     * ``param qq: str`` 目标 QQ
     * ``param force: bool`` 是否强制更新抽卡记录
     - ``return: Dict`` 抽卡记录数据，格式为``{"uid": "123456789", "msg": "文字消息", "logs": {}]``
     """
+
     # 读取抽卡记录缓存
     uid, locLogs = await logsHelper(config["logs"]) if config["logs"] else ("无记录", {})
     # msg = uid if not uid.isdigit() else ""
     if (not config["url"]) or (  # 缺少有效链接
         (not force) and (int(time()) - config["time"] < EXPIRE_SEC)  # 有缓存、未要求强制更新
     ):
         timeStr = strftime("%m-%d %H:%M", localtime(config["time"]))
```

### Comparing `nonebot_plugin_gachalogs-0.2.8/nonebot_plugin_gachalogs/gacha_achieve.py` & `nonebot_plugin_gachalogs-0.2.9/nonebot_plugin_gachalogs/gacha_achieve.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import asyncio
-from collections import Counter
 from datetime import datetime
+from collections import Counter
 from typing import Dict, List, Tuple
 
+from pytz import timezone
 from nonebot.log import logger
 from nonebot.utils import run_sync
-from pytz import timezone
 
-from .__meta__ import GACHA_TYPE, POOL_INFO
+from .__meta__ import POOL_INFO, GACHA_TYPE
 
 
 @run_sync
 def getLogsAnalysis(gachaLogs: Dict) -> Dict:
     """获取抽卡记录分析数据"""
 
     analysis = {
@@ -23,15 +23,15 @@
     renderOrder = sorted(GACHA_TYPE.keys(), key=lambda k: k[0], reverse=True)
     for banner in renderOrder:
         gachaList = gachaLogs.get(banner)
         if not gachaList:
             analysis["null"] += [banner]  # 未抽卡池统计
             continue
 
-        gachaList.reverse()  # 千万不可以 gachaList.sort(key=lambda item: item["time"], reverse=False)
+        gachaList.reverse()
         pityCounter = 0  # 保底计数
 
         # 遍历某个卡池全部记录
         for item in gachaList:
             rankType = int(item["rank_type"])
             itemName, itemType = item["name"], item["item_type"]
 
@@ -115,30 +115,38 @@
     )
     minPityItem, maxPityItem = _fiveData[0], _fiveData[-1]
     if minPityItem["pity"] <= 30:
         _results = [d["name"] for d in fiveData if d["pity"] == minPityItem["pity"]]
         achievements.append(
             {
                 "title": "「欧皇时刻」",
-                "info": f"只抽了 {minPityItem['pity']} 次就抽到了{mergeItemStr(_results)}{'，你的欧气无人能敌！' if minPityItem['pity'] <= 5 else ''}",
+                "info": "只抽了 {} 次就抽到了{}{}".format(
+                    minPityItem["pity"],
+                    mergeItemStr(_results),
+                    "，你的欧气无人能敌！" if minPityItem["pity"] <= 5 else "",
+                ),
                 "achievedTime": minPityItem["time"].replace("-", "/"),
                 "value": "达成" if len(_results) == 1 else f"总计 {len(_results)}",
             }
         )
     if maxPityItem["pity"] >= 30:
         _rarity = (
             ["百", "千", "万", "十万", "百万"][maxPityItem["pity"] - 84]
             if 83 < maxPityItem["pity"] < 89
             else "无穷"
         )
         _results = [d["name"] for d in fiveData if d["pity"] == maxPityItem["pity"]]
         achievements.append(
             {
                 "title": "「原来非酋竟是我自己」",
-                "info": f"抽了 {maxPityItem['pity']} 次才最终抽到了{mergeItemStr(_results)}{f'，你竟是{_rarity}里挑一的非酋！' if minPityItem['pity'] >= 84 else ''}",
+                "info": "抽了 {} 次才最终抽到了{}{}".format(
+                    maxPityItem["pity"],
+                    mergeItemStr(_results),
+                    f"，你竟是{_rarity}里挑一的非酋！" if minPityItem["pity"] >= 84 else "",
+                ),
                 "achievedTime": maxPityItem["time"].replace("-", "/"),
                 "value": "达成" if len(_results) == 1 else f"总计 {len(_results)}",
             }
         )
 
     return achievements
 
@@ -221,15 +229,17 @@
             }
         )
     else:
         _five = [i["name"] for i in days[dayIdx]["five"]]
         achievements.append(
             {
                 "title": "「豪掷千金」",
-                "info": f"在 {dayDisplay} 这一天，你共抽取了 {days[dayIdx]['count']} 次。在抽到{mergeItemStr(_five)}时，你有没有很开心呢？",
+                "info": "在 {} 这一天，你共抽取了 {} 次。在抽到{}时，你有没有很开心呢？".format(
+                    dayDisplay, days[dayIdx]["count"], mergeItemStr(_five)
+                ),
                 "achievedTime": dayDisplay,
                 "value": "达成",
             }
         )
 
     return achievements
 
@@ -315,15 +325,17 @@
 
     if miracle["single"] + miracle["ten"]:
         _str = "、".join(
             f"通过{'十连' if k == 'ten' else '单抽'}获取 {v} 次" for k, v in miracle.items() if v
         )
         _achievement = {
             "title": "「单抽出奇迹？」",
-            "info": f"在 {miracleLimit} 抽内获取五星共计 {miracle['single'] + miracle['ten']} 次，其中{_str}",
+            "info": "在 {} 抽内获取五星共计 {} 次，其中{}".format(
+                miracleLimit, miracle["single"] + miracle["ten"], _str
+            ),
         }
         if miracle["ten"] and miracle["single"] / miracle["ten"] < miraclePct:
             _achievement["title"] = "「十连出奇迹！」"
         if miracle["single"] and miracle["ten"] / miracle["single"] < miraclePct:
             _achievement["title"] = "「单抽出奇迹！」"
         achievements.append(_achievement)
 
@@ -343,15 +355,17 @@
 
     if manyGood:
         _map = ["四叶草", "福至五彩", "六六顺意", "七星高照", "八方鸿运", "九九同心", "十全十美"]
         achievements.extend(
             [
                 {
                     "title": f"「{_map[int(k) - 4]}」",
-                    "info": f"在一次十连中，你抽取到了 {k} 个四星或五星{'，这何尝不是另类的欧皇！' if int(k) > 4 else ''}",
+                    "info": "在一次十连中，你抽取到了 {} 个四星或五星{}".format(
+                        k, "，这何尝不是另类的欧皇！" if int(k) > 4 else ""
+                    ),
                     "achievedTime": v["first"].split()[0].replace("-", "/"),
                     "value": "达成" if v["count"] == 1 else f"总计 {v['count']}",
                 }
                 for k, v in manyGood.items()
             ]
         )
```

### Comparing `nonebot_plugin_gachalogs-0.2.8/pyproject.toml` & `nonebot_plugin_gachalogs-0.2.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,50 @@
 [tool.poetry]
 name = "nonebot-plugin-gachalogs"
-version = "0.2.8"
+version = "0.2.9"
 description = "Genshin gacha history analysis plugin for NoneBot2"
 authors = ["monsterxcn <monsterxcn@gmail.com>"]
 documentation = "https://github.com/monsterxcn/nonebot-plugin-gachalogs#readme"
 license = "MIT"
 homepage = "https://github.com/monsterxcn/nonebot-plugin-gachalogs"
 readme = "README.md"
 keywords = ["nonebot", "nonebot2", "genshin", "gacha"]
 
 [tool.poetry.dependencies]
-python = ">=3.7.3,<4.0"
+python = ">=3.8,<4.0"
 nonebot2 = ">=2.0.0a16"
 nonebot-adapter-onebot = ">=2.0.0b1"
 httpx = ">=0.20.0, <1.0.0"
 matplotlib = ">=3.5.1"
 xlsxwriter = ">=3.0.2"
 pytz = "*"
 
 [tool.poetry.dev-dependencies]
+pycln = "^2.1.2"
+pyupgrade = "^3.3.0"
+black = "^22.10.0"
+flake8 = "^5.0.4"
+isort = "^5.10.1"
+pre-commit = "^2.19.0"
+
+[tool.black]
+line-length = 88
+target-version = ["py38", "py39", "py310", "py311"]
+include = '\.pyi?$'
+extend-exclude = '''
+'''
+
+[tool.isort]
+profile = "black"
+line_length = 88
+length_sort = true
+skip_gitignore = true
+force_sort_within_sections = true
+extra_standard_library = ["typing_extensions"]
+
+[tool.pycln]
+path = "."
+all = false
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_gachalogs-0.2.8/setup.py` & `nonebot_plugin_gachalogs-0.2.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,23 +13,23 @@
  'nonebot-adapter-onebot>=2.0.0b1',
  'nonebot2>=2.0.0a16',
  'pytz',
  'xlsxwriter>=3.0.2']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-gachalogs',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'Genshin gacha history analysis plugin for NoneBot2',
-    'long_description': '<h1 align="center">NoneBot Plugin GachaLogs</h1></br>\n\n\n<p align="center">🤖 用于分析与管理原神祈愿记录的 NoneBot2 插件</p></br>\n\n\n<p align="center"><b>现已支持祈愿历史记录链接自动更新！</b></p></br>\n\n\n<p align="center">\n  <a href="https://github.com/monsterxcn/nonebot-plugin-gachalogs/actions">\n    <img src="https://img.shields.io/github/actions/workflow/status/monsterxcn/nonebot-plugin-gachalogs/publish.yml?branch=main&style=flat-square" alt="actions">\n  </a>\n  <a href="https://raw.githubusercontent.com/monsterxcn/nonebot-plugin-gachalogs/master/LICENSE">\n    <img src="https://img.shields.io/github/license/monsterxcn/nonebot-plugin-gachalogs?style=flat-square" alt="license">\n  </a>\n  <a href="https://pypi.python.org/pypi/nonebot-plugin-gachalogs">\n    <img src="https://img.shields.io/pypi/v/nonebot-plugin-gachalogs?style=flat-square" alt="pypi">\n  </a>\n  <img src="https://img.shields.io/badge/python-3.8+-blue?style=flat-square" alt="python"><br />\n</p></br>\n\n\n| ![祈愿统计图](https://user-images.githubusercontent.com/22407052/198547014-469865b5-a298-4b91-beb2-645e028a4721.PNG) | ![成就示意图](https://user-images.githubusercontent.com/22407052/210336667-ecb56bcb-42dc-4235-ab17-1e30bea04362.PNG) |\n|:--:|:--:|\n\n\n## 安装方法\n\n\n如果你正在使用 2.0.0.beta1 以上版本 NoneBot，推荐使用以下命令安装：\n\n\n```bash\n# 从 nb_cli 安装\npython -m nb_cli plugin install nonebot-plugin-gachalogs\n\n# 或从 PyPI 安装\npython -m pip install nonebot-plugin-gachalogs\n```\n\n\n## 使用须知\n\n\n - 初次使用 `抽卡记录` 命令时，要求输入祈愿历史记录链接或米哈游通行证 Cookie。如果初次使用输入链接（只要回复的内容中含有即可，不必手动截取准确的链接），在该链接的 AuthKey 过期（24 小时）后需要重新输入链接或 Cookie 才能刷新数据。如果初次使用输入 Cookie，只要 Cookie 有效，后续使用时祈愿历史记录链接将自动更新，无需再次输入。\n   \n - 插件使用米哈游通行证 Cookie 来自动更新祈愿历史记录链接，该 Cookie 可在 [米哈游通行证](https://user.mihoyo.com/#/login/) 登陆获取，并非一些教程中使用的 [米游社 BBS](https://bbs.mihoyo.com/) Cookie，其中需要包含 `stoken` `stuid` 或 `login_ticket`。\n   \n   你可以参考 [KimigaiiWuyi/GenshinUID#255](https://github.com/KimigaiiWuyi/GenshinUID/issues/255) 等教程获取米哈游通行证 Cookie。此处提供一种获取该 Cookie 的简便方法：\n   \n   1. 在桌面端浏览器新建 **隐身标签页**，后面均在此隐身标签页内操作\n   2. 进入 https://www.miyoushe.com/ys/ 并正常登录\n   3. 进入 http://user.mihoyo.com/ 并正常登录\n   4. 按下 F12 键，切换至「Console / 控制台」页面，在输入处（通常由蓝色「>」符号示意）输入 `document.cookie` 回车，控制台中出现的字符串即为插件需要的 Cookie\n   \n - 一般来说，插件安装完成后无需设置环境变量，只需重启 Bot 即可开始使用。你也可以在 NoneBot2 当前使用的 `.env` 文件中参考 [.env.example](.env.example) 添加下表给出的环境变量，对插件进行更多配置。环境变量修改后需要重启 Bot 才能生效。\n   \n   | 环境变量 | 必需 | 默认 | 说明 |\n   |:-------|:----:|:-----|:----|\n   | `gachalogs_safe_group` | 否 | `[]` | 安全群组，只有在安全群组内才允许输入链接、Cookie 等内容 |\n   | `gacha_expire_sec` | 否 | `3600` | 祈愿历史记录本地缓存过期秒数 |\n   | `resources_dir` | 否 | `/path/to/bot/data/` | 插件缓存目录的父文件夹，包含 `gachalogs` 文件夹的上级文件夹路径 |\n   | `gachalogs_font` | 否 | `/path/to/bot/data/gachalogs/LXGW-Bold.ttf` | 祈愿历史记录绘制字体 |\n   | `gachalogs_pie_font` | 否 | `/path/to/bot/data/gachalogs/LXGW-Bold-minipie.ttf` | 祈愿历史记录绘制饼图字体 |\n   | `gachalogs_achieve_font` | 否 | `/path/to/bot/data/gachalogs/HYWH-85W.ttf` | 祈愿历史记录绘制成就字体 |\n   \n - 在群组中发送米哈游通行证 Cookie 等内容存在安全隐患，因此即使某些命令在群组中触发，处理结果最终也会通过私聊发送。如果用户未添加 Bot 为好友，私聊消息将发送失败。添加安全群组环境变量，即可允许在这些群组中直接发送敏感消息，如果大家不在意的话。\n   \n - commit [`e2f38f3`](https://github.com/monsterxcn/nonebot-plugin-gachalogs/commit/e2f38f30379dac4f98f9314fa012a1272c2dcc95) 之后插件私聊文件发送功能不再依赖腾讯云 COS 转存，只需 go-cqhttp 支持 [上传私聊文件](https://docs.go-cqhttp.org/api/#%E4%B8%8A%E4%BC%A0%E7%A7%81%E8%81%8A%E6%96%87%E4%BB%B6) 接口。因此如果有私聊文件发送需求，务必保证 go-cqhttp 版本不低于 [v1.0.0-rc3](https://github.com/Mrs4s/go-cqhttp/releases/tag/v1.0.0-rc3)。\n   \n - 使用 `抽卡记录导出` 命令生成的表格与 JSON 文件均符合 [统一可交换祈愿记录标准](https://github.com/DGP-Studio/Snap.Genshin/wiki/StandardFormat)（UIGF）格式，你可以尝试在其他支持此标准的工具中导入。导出的祈愿历史记录链接、米哈游通行证 Cookie 在某些地方也许有用。\n   \n - 插件运行后，用户的基本配置信息会写入 `config.json` 文件，祈愿历史记录数据缓存于 `gachalogs-{uid}.json` 文件。\n\n\n## 命令说明\n\n\n - `抽卡记录` / `ckjl`\n   \n   返回一张祈愿历史记录统计图，样式与 https://genshin.voderl.cn/ 一致。\n   \n   | 可选附带参数 | 默认 | 说明 |\n   |:-----------|:-----|:----|\n   | `刷新` / `-f` / `--force` | 空 | 要求强制刷新最新祈愿历史记录，即使本地缓存未过期（结果默认缓存 1 小时） |\n   | 祈愿历史记录链接 | 空 | 指定祈愿历史记录链接（仅初次使用、无法自动更新祈愿历史记录链接时生效） |\n   | 米哈游通行证 Cookie | 空 | 指定米哈游通行证 Cookie（仅初次使用、无法自动更新祈愿历史记录链接时生效） |\n   \n - `抽卡成就` / `ckcj`\n   \n   返回一张祈愿历史记录成就图，样式与 https://genshin.voderl.cn/ 一致。\n   \n - 抽卡记录导入（在私聊或群聊中上传抽卡记录文件）\n   \n   返回导入结果及一张祈愿历史记录统计图。\n   \n   普通用户只允许导入与本地记录（如果有）归属 UID 相同的抽卡记录。超级用户在普通用户规则基础上，还允许为拥有本地记录的其他用户导入 UID 相同的抽卡记录。\n   \n   目前支持导入的文件格式有：\n   \n   + 程序内部缓存格式。导入后执行恢复，即将本地记录直接替换为该文件的记录\n   + UIGF v2.2 格式，并且每条记录必须拥有 `time` `rank_type` 等 UIGF v2.2 标准中定义为非必需的字段。导入后执行合并，即尝试将本地记录与该文件的记录合并\n   \n   如果导入前 *被导入者* 有本地记录，插件会创建一个本地记录备份文件用于意外恢复，并尝试通过私聊将此文件发送给 *被导入者*（如果发送成功则 Bot 在服务器上创建的备份文件会被删除）。一旦发现插件导入后记录异常，*被导入者* 可以直接发送此文件给 Bot 来触发记录恢复。\n   \n - `抽卡记录导出` / `logexp` / `ckjldc`\n   \n   导出祈愿历史记录表格，通过可选附带参数指定导出祈愿历史记录 JSON 文件、祈愿历史记录链接或米哈游通行证 Cookie。\n   \n   | 可选附带参数 | 默认 | 说明 |\n   |:-----------|:-----|:----|\n   | @某人 | **@自己** | 指定导出记录用户，仅 **Bot 管理员** 可导出其他用户的记录 |\n   | `统一` / `标准` / `uigf` / `json` | 空 | 指定导出祈愿历史记录为 JSON 文件 |\n   | `链接` / `地址` / `url` | 空 | 指定导出祈愿历史记录链接 |\n   | `饼干` / `ck` / `cookie` | 空 | 指定导出米哈游通行证 Cookie |\n   \n   ![导出示意图](https://user-images.githubusercontent.com/22407052/187933780-64fa0be4-a43f-40f1-9fa9-88e033e9d372.png)\n   \n - `抽卡记录删除` / `logdel` / `ckjldc`\n   \n   默认只删除本地祈愿历史记录缓存（不会影响 Cookie 等配置数据），即只删除 `gachalogs-{uid}.json` 文件。\n   \n   如果需要连同指定用户在 `config.json` 文件中的配置一起删除，请使用附带参数 `全部` 等。\n   \n   记录、配置一旦删除将无法恢复，所以只有输入中附带了 `确认` 等附带参数时，命令才会真正对本地文件执行删除动作。\n   \n   | 可选附带参数 | 默认 | 说明 |\n   |:-----------|:-----|:----|\n   | @某人 | **@自己** | 指定删除记录或配置的用户，仅 **Bot 管理员** 可删除其他用户的记录或配置 |\n   | `强制` / `确认` / `force` / `-f` / `-y` | 空 | 删除操作确认 |\n   | `全部` / `所有` / `配置` / `all` / `-a` / `config` / `-c` | 空 | 指定删除用户的 **配置和记录** 全部数据 |\n\n\n## 特别鸣谢\n\n\n[@nonebot/nonebot2](https://github.com/nonebot/nonebot2/) | [@Mrs4s/go-cqhttp](https://github.com/Mrs4s/go-cqhttp) | **[@sunfkny/genshin-gacha-export](https://github.com/sunfkny/genshin-gacha-export)** | **[@voderl/genshin-gacha-analyzer](https://github.com/voderl/genshin-gacha-analyzer)** | [@vikiboss/genshin-helper](https://github.com/vikiboss/genshin-helper) | [@DGP-Studio/Snap.Metadata](https://github.com/DGP-Studio/Snap.Metadata)\n',
+    'long_description': '<h1 align="center">NoneBot Plugin GachaLogs</h1></br>\n\n\n<p align="center">🤖 用于分析与管理原神祈愿记录的 NoneBot2 插件</p></br>\n\n\n<p align="center">\n  <a href="https://github.com/monsterxcn/nonebot-plugin-gachalogs/actions">\n    <img src="https://img.shields.io/github/actions/workflow/status/monsterxcn/nonebot-plugin-gachalogs/publish.yml?branch=main" alt="actions">\n  </a>\n  <a href="https://raw.githubusercontent.com/monsterxcn/nonebot-plugin-gachalogs/master/LICENSE">\n    <img src="https://img.shields.io/github/license/monsterxcn/nonebot-plugin-gachalogs" alt="license">\n  </a>\n  <a href="https://pypi.python.org/pypi/nonebot-plugin-gachalogs">\n    <img src="https://img.shields.io/pypi/v/nonebot-plugin-gachalogs" alt="pypi">\n  </a>\n  <a href="https://www.python.org/">\n    <img src="https://img.shields.io/badge/python-3.8+-blue" alt="python" />\n  </a><br />\n  <a href="https://github.com/psf/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black" />\n  </a>\n  <a href="https://pycqa.github.io/isort">\n    <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?&labelColor=ef8336" alt="Imports: isort" />\n  </a>\n  <a href="https://results.pre-commit.ci/latest/github/monsterxcn/nonebot-plugin-gachalogs/main">\n    <img src="https://results.pre-commit.ci/badge/github/monsterxcn/nonebot-plugin-gachalogs/main.svg" alt="pre-commit" />\n  </a>\n</p></br>\n\n\n| ![祈愿统计图](https://user-images.githubusercontent.com/22407052/198547014-469865b5-a298-4b91-beb2-645e028a4721.PNG) | ![成就示意图](https://user-images.githubusercontent.com/22407052/210336667-ecb56bcb-42dc-4235-ab17-1e30bea04362.PNG) |\n|:--:|:--:|\n\n\n## 安装方法\n\n\n如果你正在使用 2.0.0.beta1 以上版本 NoneBot2，推荐使用以下命令安装：\n\n\n```bash\n# 从 nb_cli 安装\npython -m nb_cli plugin install nonebot-plugin-gachalogs\n\n# 或从 PyPI 安装\npython -m pip install nonebot-plugin-gachalogs\n```\n\n\n## 使用须知\n\n\n - 初次使用 `抽卡记录` 命令时，要求输入祈愿历史记录链接或米哈游通行证 Cookie。如果初次使用输入链接（只要回复的内容中含有即可，不必手动截取准确的链接），在该链接的 AuthKey 过期（24 小时）后需要重新输入链接或 Cookie 才能刷新数据。如果初次使用输入 Cookie，只要 Cookie 有效，后续使用时祈愿历史记录链接将自动更新，无需再次输入。\n   \n - 插件使用米哈游通行证 Cookie 来自动更新祈愿历史记录链接，该 Cookie 可在 [米哈游通行证](https://user.mihoyo.com/#/login/) 登陆获取，并非一些教程中使用的 [米游社 BBS](https://bbs.mihoyo.com/) Cookie，其中需要包含 `stoken` `stuid` 或 `login_ticket`。\n   \n   你可以参考 [KimigaiiWuyi/GenshinUID#255](https://github.com/KimigaiiWuyi/GenshinUID/issues/255) 等教程获取米哈游通行证 Cookie。此处提供一种获取该 Cookie 的简便方法：\n   \n   1. 在桌面端浏览器新建 **隐身标签页**，后面均在此隐身标签页内操作\n   2. 进入 https://www.miyoushe.com/ys/ 并正常登录\n   3. 进入 http://user.mihoyo.com/ 并正常登录\n   4. 按下 F12 键，切换至「Console / 控制台」页面，在输入处（通常由蓝色「>」符号示意）输入 `document.cookie` 回车，控制台中出现的字符串即为插件需要的 Cookie\n   \n - 一般来说，插件安装完成后无需设置环境变量，只需重启 Bot 即可开始使用。你也可以在 NoneBot2 当前使用的 `.env` 文件中参考 [.env.example](.env.example) 添加下表给出的环境变量，对插件进行更多配置。环境变量修改后需要重启 Bot 才能生效。\n   \n   | 环境变量 | 必需 | 默认 | 说明 |\n   |:-------|:----:|:-----|:----|\n   | `gachalogs_safe_group` | 否 | `[]` | 安全群组，只有在安全群组内才允许输入链接、Cookie 等内容 |\n   | `gacha_expire_sec` | 否 | `3600` | 祈愿历史记录本地缓存过期秒数 |\n   | `resources_dir` | 否 | `/path/to/bot/data/` | 插件缓存目录的父文件夹，包含 `gachalogs` 文件夹的上级文件夹路径 |\n   | `gachalogs_font` | 否 | `/path/to/bot/data/gachalogs/LXGW-Bold.ttf` | 祈愿历史记录绘制字体 |\n   | `gachalogs_pie_font` | 否 | `/path/to/bot/data/gachalogs/LXGW-Bold-minipie.ttf` | 祈愿历史记录绘制饼图字体 |\n   | `gachalogs_achieve_font` | 否 | `/path/to/bot/data/gachalogs/HYWH-85W.ttf` | 祈愿历史记录绘制成就字体 |\n   \n - 在群组中发送米哈游通行证 Cookie 等内容存在安全隐患，因此即使某些命令在群组中触发，处理结果最终也会通过私聊发送。如果用户未添加 Bot 为好友，私聊消息将发送失败。添加安全群组环境变量，即可允许在这些群组中直接发送敏感消息，如果大家不在意的话。\n   \n - commit [`e2f38f3`](https://github.com/monsterxcn/nonebot-plugin-gachalogs/commit/e2f38f30379dac4f98f9314fa012a1272c2dcc95) 之后插件私聊文件发送功能不再依赖腾讯云 COS 转存，只需 go-cqhttp 支持 [上传私聊文件](https://docs.go-cqhttp.org/api/#%E4%B8%8A%E4%BC%A0%E7%A7%81%E8%81%8A%E6%96%87%E4%BB%B6) 接口。因此如果有私聊文件发送需求，务必保证 go-cqhttp 版本不低于 [v1.0.0-rc3](https://github.com/Mrs4s/go-cqhttp/releases/tag/v1.0.0-rc3)。\n   \n - 使用 `抽卡记录导出` 命令生成的表格与 JSON 文件均符合 [统一可交换祈愿记录标准](https://github.com/DGP-Studio/Snap.Genshin/wiki/StandardFormat)（UIGF）格式，你可以尝试在其他支持此标准的工具中导入。导出的祈愿历史记录链接、米哈游通行证 Cookie 在某些地方也许有用。\n   \n - 插件运行后，用户的基本配置信息会写入 `config.json` 文件，祈愿历史记录数据缓存于 `gachalogs-{uid}.json` 文件。\n\n\n## 命令说明\n\n\n - `抽卡记录` / `ckjl`\n   \n   返回一张祈愿历史记录统计图，样式与 https://genshin.voderl.cn/ 一致。\n   \n   | 可选附带参数 | 默认 | 说明 |\n   |:-----------|:-----|:----|\n   | `刷新` / `-f` / `--force` | 空 | 要求强制刷新最新祈愿历史记录，即使本地缓存未过期（结果默认缓存 1 小时） |\n   | 祈愿历史记录链接 | 空 | 指定祈愿历史记录链接（仅初次使用、无法自动更新祈愿历史记录链接时生效） |\n   | 米哈游通行证 Cookie | 空 | 指定米哈游通行证 Cookie（仅初次使用、无法自动更新祈愿历史记录链接时生效） |\n   \n - `抽卡成就` / `ckcj`\n   \n   返回一张祈愿历史记录成就图，样式与 https://genshin.voderl.cn/ 一致。\n   \n - 抽卡记录导入（在私聊或群聊中上传抽卡记录文件）\n   \n   返回导入结果及一张祈愿历史记录统计图。\n   \n   普通用户只允许导入与本地记录（如果有）归属 UID 相同的抽卡记录。超级用户在普通用户规则基础上，还允许为拥有本地记录的其他用户导入 UID 相同的抽卡记录。\n   \n   目前支持导入的文件格式有：\n   \n   + 程序内部缓存格式。导入后执行恢复，即将本地记录直接替换为该文件的记录\n   + UIGF v2.2 格式，并且每条记录必须拥有 `time` `rank_type` 等 UIGF v2.2 标准中定义为非必需的字段。导入后执行合并，即尝试将本地记录与该文件的记录合并\n   \n   如果导入前 *被导入者* 有本地记录，插件会创建一个本地记录备份文件用于意外恢复，并尝试通过私聊将此文件发送给 *被导入者*（如果发送成功则 Bot 在服务器上创建的备份文件会被删除）。一旦发现插件导入后记录异常，*被导入者* 可以直接发送此文件给 Bot 来触发记录恢复。\n   \n - `抽卡记录导出` / `logexp` / `ckjldc`\n   \n   导出祈愿历史记录表格，通过可选附带参数指定导出祈愿历史记录 JSON 文件、祈愿历史记录链接或米哈游通行证 Cookie。\n   \n   | 可选附带参数 | 默认 | 说明 |\n   |:-----------|:-----|:----|\n   | @某人 | **@自己** | 指定导出记录用户，仅 **Bot 管理员** 可导出其他用户的记录 |\n   | `统一` / `标准` / `uigf` / `json` | 空 | 指定导出祈愿历史记录为 JSON 文件 |\n   | `链接` / `地址` / `url` | 空 | 指定导出祈愿历史记录链接 |\n   | `饼干` / `ck` / `cookie` | 空 | 指定导出米哈游通行证 Cookie |\n   \n   ![导出示意图](https://user-images.githubusercontent.com/22407052/187933780-64fa0be4-a43f-40f1-9fa9-88e033e9d372.png)\n   \n - `抽卡记录删除` / `logdel` / `ckjldc`\n   \n   默认只删除本地祈愿历史记录缓存（不会影响 Cookie 等配置数据），即只删除 `gachalogs-{uid}.json` 文件。\n   \n   如果需要连同指定用户在 `config.json` 文件中的配置一起删除，请使用附带参数 `全部` 等。\n   \n   记录、配置一旦删除将无法恢复，所以只有输入中附带了 `确认` 等附带参数时，命令才会真正对本地文件执行删除动作。\n   \n   | 可选附带参数 | 默认 | 说明 |\n   |:-----------|:-----|:----|\n   | @某人 | **@自己** | 指定删除记录或配置的用户，仅 **Bot 管理员** 可删除其他用户的记录或配置 |\n   | `强制` / `确认` / `force` / `-f` / `-y` | 空 | 删除操作确认 |\n   | `全部` / `所有` / `配置` / `all` / `-a` / `config` / `-c` | 空 | 指定删除用户的 **配置和记录** 全部数据 |\n\n\n## 特别鸣谢\n\n\n[@nonebot/nonebot2](https://github.com/nonebot/nonebot2/) | [@Mrs4s/go-cqhttp](https://github.com/Mrs4s/go-cqhttp) | **[@sunfkny/genshin-gacha-export](https://github.com/sunfkny/genshin-gacha-export)** | **[@voderl/genshin-gacha-analyzer](https://github.com/voderl/genshin-gacha-analyzer)** | [@vikiboss/genshin-helper](https://github.com/vikiboss/genshin-helper) | [@DGP-Studio/Snap.Metadata](https://github.com/DGP-Studio/Snap.Metadata)\n',
     'author': 'monsterxcn',
     'author_email': 'monsterxcn@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/monsterxcn/nonebot-plugin-gachalogs',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7.3,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,28 +1,26 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_gachalogs'] package_data = \ {'': ['*']} install_requires = \
 ['httpx>=0.20.0,<1.0.0', 'matplotlib>=3.5.1', 'nonebot-adapter-
 onebot>=2.0.0b1', 'nonebot2>=2.0.0a16', 'pytz', 'xlsxwriter>=3.0.2']
-setup_kwargs = { 'name': 'nonebot-plugin-gachalogs', 'version': '0.2.8',
+setup_kwargs = { 'name': 'nonebot-plugin-gachalogs', 'version': '0.2.9',
 'description': 'Genshin gacha history analysis plugin for NoneBot2',
 'long_description': '
                     ****** NoneBot Plugin GachaLogs ******
 \n\n\n
         ð¤ ç¨äºåæä¸ç®¡çåç¥ç¥æ¿è®°å½ç NoneBot2 æä»¶
 \n\n\n
-              ç°å·²æ¯æç¥æ¿åå²è®°å½é¾æ¥èªå¨æ´æ°ï¼
-\n\n\n
-          \n \n_[actions]\n\n \n_[license]\n\n \n_[pypi]\n\n [python]
-                                      \n
+       \n \n_[actions]\n\n \n_[license]\n\n \n_[pypi]\n\n \n_[python]\n
+   \n \n_[Code_style:_black]\n\n \n_[Imports:_isort]\n\n \n_[pre-commit]\n\n
 \n\n\n| ![ç¥æ¿ç»è®¡å¾](https://user-images.githubusercontent.com/22407052/
 198547014-469865b5-a298-4b91-beb2-645e028a4721.PNG) | ![æå°±ç¤ºæå¾](https:
 //user-images.githubusercontent.com/22407052/210336667-ecb56bcb-42dc-4235-ab17-
 1e30bea04362.PNG) |\n|:--:|:--:|\n\n\n##
 å®è£æ¹æ³\n\n\nå¦æä½ æ­£å¨ä½¿ç¨ 2.0.0.beta1 ä»¥ä¸çæ¬
-NoneBotï¼æ¨èä½¿ç¨ä»¥ä¸å½ä»¤å®è£ï¼\n\n\n```bash\n# ä» nb_cli
+NoneBot2ï¼æ¨èä½¿ç¨ä»¥ä¸å½ä»¤å®è£ï¼\n\n\n```bash\n# ä» nb_cli
 å®è£\npython -m nb_cli plugin install nonebot-plugin-gachalogs\n\n# æä»
 PyPI å®è£\npython -m pip install nonebot-plugin-gachalogs\n```\n\n\n##
 ä½¿ç¨é¡»ç¥\n\n\n - åæ¬¡ä½¿ç¨ `æ½å¡è®°å½`
 å½ä»¤æ¶ï¼è¦æ±è¾å¥ç¥æ¿åå²è®°å½é¾æ¥æç±³åæ¸¸éè¡è¯
 Cookieãå¦æåæ¬¡ä½¿ç¨è¾å¥é¾æ¥ï¼åªè¦åå¤çåå®¹ä¸­å«æå³å¯ï¼ä¸å¿æå¨æªååç¡®çé¾æ¥ï¼ï¼å¨è¯¥é¾æ¥ç
 AuthKey è¿æï¼24 å°æ¶ï¼åéè¦éæ°è¾å¥é¾æ¥æ Cookie
 æè½å·æ°æ°æ®ãå¦æåæ¬¡ä½¿ç¨è¾å¥ Cookieï¼åªè¦ Cookie
@@ -133,9 +131,9 @@
 github.com/sunfkny/genshin-gacha-export)** | **[@voderl/genshin-gacha-analyzer]
 (https://github.com/voderl/genshin-gacha-analyzer)** | [@vikiboss/genshin-
 helper](https://github.com/vikiboss/genshin-helper) | [@DGP-Studio/
 Snap.Metadata](https://github.com/DGP-Studio/Snap.Metadata)\n', 'author':
 'monsterxcn', 'author_email': 'monsterxcn@gmail.com', 'maintainer': 'None',
 'maintainer_email': 'None', 'url': 'https://github.com/monsterxcn/nonebot-
 plugin-gachalogs', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.7.3,<4.0', }
-setup(**setup_kwargs)
+'install_requires': install_requires, 'python_requires': '>=3.8,<4.0', } setup
+(**setup_kwargs)
```

### Comparing `nonebot_plugin_gachalogs-0.2.8/PKG-INFO` & `nonebot_plugin_gachalogs-0.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-gachalogs
-Version: 0.2.8
+Version: 0.2.9
 Summary: Genshin gacha history analysis plugin for NoneBot2
 Home-page: https://github.com/monsterxcn/nonebot-plugin-gachalogs
 License: MIT
 Keywords: nonebot,nonebot2,genshin,gacha
 Author: monsterxcn
 Author-email: monsterxcn@gmail.com
-Requires-Python: >=3.7.3,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.20.0,<1.0.0)
@@ -25,39 +25,47 @@
 
 <h1 align="center">NoneBot Plugin GachaLogs</h1></br>
 
 
 <p align="center">🤖 用于分析与管理原神祈愿记录的 NoneBot2 插件</p></br>
 
 
-<p align="center"><b>现已支持祈愿历史记录链接自动更新！</b></p></br>
-
-
 <p align="center">
   <a href="https://github.com/monsterxcn/nonebot-plugin-gachalogs/actions">
-    <img src="https://img.shields.io/github/actions/workflow/status/monsterxcn/nonebot-plugin-gachalogs/publish.yml?branch=main&style=flat-square" alt="actions">
+    <img src="https://img.shields.io/github/actions/workflow/status/monsterxcn/nonebot-plugin-gachalogs/publish.yml?branch=main" alt="actions">
   </a>
   <a href="https://raw.githubusercontent.com/monsterxcn/nonebot-plugin-gachalogs/master/LICENSE">
-    <img src="https://img.shields.io/github/license/monsterxcn/nonebot-plugin-gachalogs?style=flat-square" alt="license">
+    <img src="https://img.shields.io/github/license/monsterxcn/nonebot-plugin-gachalogs" alt="license">
   </a>
   <a href="https://pypi.python.org/pypi/nonebot-plugin-gachalogs">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-gachalogs?style=flat-square" alt="pypi">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-gachalogs" alt="pypi">
+  </a>
+  <a href="https://www.python.org/">
+    <img src="https://img.shields.io/badge/python-3.8+-blue" alt="python" />
+  </a><br />
+  <a href="https://github.com/psf/black">
+    <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black" />
+  </a>
+  <a href="https://pycqa.github.io/isort">
+    <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?&labelColor=ef8336" alt="Imports: isort" />
+  </a>
+  <a href="https://results.pre-commit.ci/latest/github/monsterxcn/nonebot-plugin-gachalogs/main">
+    <img src="https://results.pre-commit.ci/badge/github/monsterxcn/nonebot-plugin-gachalogs/main.svg" alt="pre-commit" />
   </a>
-  <img src="https://img.shields.io/badge/python-3.8+-blue?style=flat-square" alt="python"><br />
 </p></br>
 
 
 | ![祈愿统计图](https://user-images.githubusercontent.com/22407052/198547014-469865b5-a298-4b91-beb2-645e028a4721.PNG) | ![成就示意图](https://user-images.githubusercontent.com/22407052/210336667-ecb56bcb-42dc-4235-ab17-1e30bea04362.PNG) |
 |:--:|:--:|
 
 
 ## 安装方法
 
 
-如果你正在使用 2.0.0.beta1 以上版本 NoneBot，推荐使用以下命令安装：
+如果你正在使用 2.0.0.beta1 以上版本 NoneBot2，推荐使用以下命令安装：
 
 
 ```bash
 # 从 nb_cli 安装
 python -m nb_cli plugin install nonebot-plugin-gachalogs
 
 # 或从 PyPI 安装
```

#### html2text {}

```diff
@@ -1,30 +1,30 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-gachalogs Version: 0.2.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-gachalogs Version: 0.2.9 Summary:
 Genshin gacha history analysis plugin for NoneBot2 Home-page: https://
 github.com/monsterxcn/nonebot-plugin-gachalogs License: MIT Keywords:
 nonebot,nonebot2,genshin,gacha Author: monsterxcn Author-email:
-monsterxcn@gmail.com Requires-Python: >=3.7.3,<4.0 Classifier: License :: OSI
+monsterxcn@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: httpx
 (>=0.20.0,<1.0.0) Requires-Dist: matplotlib (>=3.5.1) Requires-Dist: nonebot-
 adapter-onebot (>=2.0.0b1) Requires-Dist: nonebot2 (>=2.0.0a16) Requires-Dist:
 pytz Requires-Dist: xlsxwriter (>=3.0.2) Project-URL: Documentation, https://
 github.com/monsterxcn/nonebot-plugin-gachalogs#readme Description-Content-Type:
 text/markdown
                     ****** NoneBot Plugin GachaLogs ******
         ð¤ ç¨äºåæä¸ç®¡çåç¥ç¥æ¿è®°å½ç NoneBot2 æä»¶
-              ç°å·²æ¯æç¥æ¿åå²è®°å½é¾æ¥èªå¨æ´æ°ï¼
                       [actions] [license] [pypi] [python]
+               [Code_style:_black] [Imports:_isort] [pre-commit]
 | ![ç¥æ¿ç»è®¡å¾](https://user-images.githubusercontent.com/22407052/
 198547014-469865b5-a298-4b91-beb2-645e028a4721.PNG) | ![æå°±ç¤ºæå¾](https:
 //user-images.githubusercontent.com/22407052/210336667-ecb56bcb-42dc-4235-ab17-
 1e30bea04362.PNG) | |:--:|:--:| ## å®è£æ¹æ³ å¦æä½ æ­£å¨ä½¿ç¨
-2.0.0.beta1 ä»¥ä¸çæ¬ NoneBotï¼æ¨èä½¿ç¨ä»¥ä¸å½ä»¤å®è£ï¼ ```bash #
+2.0.0.beta1 ä»¥ä¸çæ¬ NoneBot2ï¼æ¨èä½¿ç¨ä»¥ä¸å½ä»¤å®è£ï¼ ```bash #
 ä» nb_cli å®è£ python -m nb_cli plugin install nonebot-plugin-gachalogs #
 æä» PyPI å®è£ python -m pip install nonebot-plugin-gachalogs ``` ##
 ä½¿ç¨é¡»ç¥ - åæ¬¡ä½¿ç¨ `æ½å¡è®°å½`
 å½ä»¤æ¶ï¼è¦æ±è¾å¥ç¥æ¿åå²è®°å½é¾æ¥æç±³åæ¸¸éè¡è¯
 Cookieãå¦æåæ¬¡ä½¿ç¨è¾å¥é¾æ¥ï¼åªè¦åå¤çåå®¹ä¸­å«æå³å¯ï¼ä¸å¿æå¨æªååç¡®çé¾æ¥ï¼ï¼å¨è¯¥é¾æ¥ç
 AuthKey è¿æï¼24 å°æ¶ï¼åéè¦éæ°è¾å¥é¾æ¥æ Cookie
 æè½å·æ°æ°æ®ãå¦æåæ¬¡ä½¿ç¨è¾å¥ Cookieï¼åªè¦ Cookie
```

