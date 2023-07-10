# Comparing `tmp/nonebot-plugin-nobahpictrue-1.0.2.tar.gz` & `tmp/nonebot-plugin-nobahpictrue-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-nobahpictrue-1.0.2.tar", last modified: Mon Jul 10 03:16:56 2023, max compression
+gzip compressed data, was "nonebot-plugin-nobahpictrue-1.0.3.tar", last modified: Mon Jul 10 05:05:26 2023, max compression
```

## Comparing `nonebot-plugin-nobahpictrue-1.0.2.tar` & `nonebot-plugin-nobahpictrue-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 03:16:56.556317 nonebot-plugin-nobahpictrue-1.0.2/
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     1065 2023-07-10 02:38:31.000000 nonebot-plugin-nobahpictrue-1.0.2/LICENSE
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      942 2023-07-10 03:16:56.556317 nonebot-plugin-nobahpictrue-1.0.2/PKG-INFO
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      516 2023-07-10 03:13:06.000000 nonebot-plugin-nobahpictrue-1.0.2/README.md
-drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 03:16:56.552317 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpictrue.egg-info/
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      942 2023-07-10 03:16:56.000000 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpictrue.egg-info/PKG-INFO
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      448 2023-07-10 03:16:56.000000 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpictrue.egg-info/SOURCES.txt
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-10 03:16:56.000000 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpictrue.egg-info/dependency_links.txt
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       17 2023-07-10 03:16:56.000000 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpictrue.egg-info/requires.txt
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       28 2023-07-10 03:16:56.000000 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpictrue.egg-info/top_level.txt
-drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 03:16:56.556317 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpicture/
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     2710 2023-07-10 02:36:37.000000 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpicture/__init__.py
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      382 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpicture/config.py
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     1857 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpicture/get_picture.py
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      347 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpicture/rules.py
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       78 2023-07-10 03:16:56.560317 nonebot-plugin-nobahpictrue-1.0.2/setup.cfg
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      656 2023-07-10 03:16:54.000000 nonebot-plugin-nobahpictrue-1.0.2/setup.py
+drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 05:05:26.712224 nonebot-plugin-nobahpictrue-1.0.3/
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     1065 2023-07-10 02:38:31.000000 nonebot-plugin-nobahpictrue-1.0.3/LICENSE
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      942 2023-07-10 05:05:26.712224 nonebot-plugin-nobahpictrue-1.0.3/PKG-INFO
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      516 2023-07-10 03:13:06.000000 nonebot-plugin-nobahpictrue-1.0.3/README.md
+drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 05:05:26.708223 nonebot-plugin-nobahpictrue-1.0.3/nonebot_plugin_nobahpictrue.egg-info/
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      942 2023-07-10 05:05:26.000000 nonebot-plugin-nobahpictrue-1.0.3/nonebot_plugin_nobahpictrue.egg-info/PKG-INFO
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      448 2023-07-10 05:05:26.000000 nonebot-plugin-nobahpictrue-1.0.3/nonebot_plugin_nobahpictrue.egg-info/SOURCES.txt
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-10 05:05:26.000000 nonebot-plugin-nobahpictrue-1.0.3/nonebot_plugin_nobahpictrue.egg-info/dependency_links.txt
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       17 2023-07-10 05:05:26.000000 nonebot-plugin-nobahpictrue-1.0.3/nonebot_plugin_nobahpictrue.egg-info/requires.txt
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       28 2023-07-10 05:05:26.000000 nonebot-plugin-nobahpictrue-1.0.3/nonebot_plugin_nobahpictrue.egg-info/top_level.txt
+drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 05:05:26.712224 nonebot-plugin-nobahpictrue-1.0.3/nonebot_plugin_nobahpicture/
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     3195 2023-07-10 05:04:43.000000 nonebot-plugin-nobahpictrue-1.0.3/nonebot_plugin_nobahpicture/__init__.py
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      382 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpictrue-1.0.3/nonebot_plugin_nobahpicture/config.py
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     1857 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpictrue-1.0.3/nonebot_plugin_nobahpicture/get_picture.py
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      347 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpictrue-1.0.3/nonebot_plugin_nobahpicture/rules.py
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       78 2023-07-10 05:05:26.716224 nonebot-plugin-nobahpictrue-1.0.3/setup.cfg
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      656 2023-07-10 05:04:25.000000 nonebot-plugin-nobahpictrue-1.0.3/setup.py
```

### Comparing `nonebot-plugin-nobahpictrue-1.0.2/LICENSE` & `nonebot-plugin-nobahpictrue-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-nobahpictrue-1.0.2/PKG-INFO` & `nonebot-plugin-nobahpictrue-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nobahpictrue
-Version: 1.0.2
+Version: 1.0.3
 Summary: 获取碧蓝档案涩图
 Home-page: https://github.com/Lptr-byte/nonebot-plugin-nobahpicture
 Author: Hansa
 Author-email: hanasakayui2022@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot-plugin-nobahpictrue-1.0.2/README.md` & `nonebot-plugin-nobahpictrue-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpictrue.egg-info/PKG-INFO` & `nonebot-plugin-nobahpictrue-1.0.3/nonebot_plugin_nobahpictrue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nobahpictrue
-Version: 1.0.2
+Version: 1.0.3
 Summary: 获取碧蓝档案涩图
 Home-page: https://github.com/Lptr-byte/nonebot-plugin-nobahpicture
 Author: Hansa
 Author-email: hanasakayui2022@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpicture/__init__.py` & `nonebot-plugin-nobahpictrue-1.0.3/nonebot_plugin_nobahpicture/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,44 @@
 from re import I, sub
 from typing import Any, Tuple, Union, Annotated
 
 from nonebot import on_regex, get_driver, on_command
 from nonebot.log import logger
 from nonebot.rule import to_me
 from nonebot.params import Command, RegexGroup
+from nonebot.plugin import PluginMetadata  # type: ignore
 from nonebot.permission import SUPERUSER
 from nonebot.adapters.onebot.v11 import (GROUP, PRIVATE_FRIEND, Bot, Event,
                                          Message, MessageSegment,
                                          GroupMessageEvent,
                                          PrivateMessageEvent)
 
 from .rules import rule, plugin_rule
 from .config import Config
 from .get_picture import GetPicture
 
 global_config = get_driver().config
 config = Config.parse_obj(global_config)
 
 
+__plugin_meta__ = PluginMetadata(
+    name='nonebot-plugin-nobahpicture',
+    description='获取碧蓝档案涩图',
+    usage='https://github.com/Lptr-byte/nonebot-plugin-nobahpicture',
+    homepage='https://github.com/Lptr-byte/nonebot-plugin-nobahpicture',
+    type='application',
+    supported_adapters=('~onebot.v11'),
+    extra={
+        'author': 'Hanasa',
+        'version': '1.0.3',
+        'priority': 1,
+    },
+)
+
+
 change_plugin_state = on_command(('Ba涩图', '开启'), rule=to_me(), aliases={('Ba涩图', '禁用')},
                                  permission=SUPERUSER)
 save_picture_state = on_command(('Ba涩图保存功能', '开启'), rule=to_me(), aliases={('Ba涩图保存功能', '关闭')},
                                 permission=SUPERUSER)
 give_me_picture = on_regex(r'^(来点Ba涩图)\s?([x|X|*]?\d+[张|个|份]?)?\s?(.*)?',
                            rule=plugin_rule, flags=I,
                            permission=PRIVATE_FRIEND | GROUP)
```

### Comparing `nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpicture/get_picture.py` & `nonebot-plugin-nobahpictrue-1.0.3/nonebot_plugin_nobahpicture/get_picture.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-nobahpictrue-1.0.2/setup.py` & `nonebot-plugin-nobahpictrue-1.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='nonebot-plugin-nobahpictrue',
-    version='1.0.2',
+    version='1.0.3',
     author='Hansa',
     author_email='hanasakayui2022@gmail.com',
     description='获取碧蓝档案涩图',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Lptr-byte/nonebot-plugin-nobahpicture',
     packages=setuptools.find_packages(),
```

