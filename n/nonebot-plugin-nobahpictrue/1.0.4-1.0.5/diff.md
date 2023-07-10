# Comparing `tmp/nonebot-plugin-nobahpictrue-1.0.4.tar.gz` & `tmp/nonebot-plugin-nobahpictrue-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-nobahpictrue-1.0.4.tar", last modified: Mon Jul 10 05:24:59 2023, max compression
+gzip compressed data, was "nonebot-plugin-nobahpictrue-1.0.5.tar", last modified: Mon Jul 10 06:10:55 2023, max compression
```

## Comparing `nonebot-plugin-nobahpictrue-1.0.4.tar` & `nonebot-plugin-nobahpictrue-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 05:24:59.415346 nonebot-plugin-nobahpictrue-1.0.4/
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     1065 2023-07-10 02:38:31.000000 nonebot-plugin-nobahpictrue-1.0.4/LICENSE
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      942 2023-07-10 05:24:59.415346 nonebot-plugin-nobahpictrue-1.0.4/PKG-INFO
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      516 2023-07-10 03:13:06.000000 nonebot-plugin-nobahpictrue-1.0.4/README.md
-drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 05:24:59.415346 nonebot-plugin-nobahpictrue-1.0.4/nonebot_plugin_nobahpictrue.egg-info/
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      942 2023-07-10 05:24:59.000000 nonebot-plugin-nobahpictrue-1.0.4/nonebot_plugin_nobahpictrue.egg-info/PKG-INFO
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      448 2023-07-10 05:24:59.000000 nonebot-plugin-nobahpictrue-1.0.4/nonebot_plugin_nobahpictrue.egg-info/SOURCES.txt
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-10 05:24:59.000000 nonebot-plugin-nobahpictrue-1.0.4/nonebot_plugin_nobahpictrue.egg-info/dependency_links.txt
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       17 2023-07-10 05:24:59.000000 nonebot-plugin-nobahpictrue-1.0.4/nonebot_plugin_nobahpictrue.egg-info/requires.txt
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       28 2023-07-10 05:24:59.000000 nonebot-plugin-nobahpictrue-1.0.4/nonebot_plugin_nobahpictrue.egg-info/top_level.txt
-drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 05:24:59.415346 nonebot-plugin-nobahpictrue-1.0.4/nonebot_plugin_nobahpicture/
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     3179 2023-07-10 05:24:24.000000 nonebot-plugin-nobahpictrue-1.0.4/nonebot_plugin_nobahpicture/__init__.py
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      382 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpictrue-1.0.4/nonebot_plugin_nobahpicture/config.py
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     1857 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpictrue-1.0.4/nonebot_plugin_nobahpicture/get_picture.py
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      347 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpictrue-1.0.4/nonebot_plugin_nobahpicture/rules.py
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       78 2023-07-10 05:24:59.423347 nonebot-plugin-nobahpictrue-1.0.4/setup.cfg
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      656 2023-07-10 05:24:30.000000 nonebot-plugin-nobahpictrue-1.0.4/setup.py
+drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:10:55.072095 nonebot-plugin-nobahpictrue-1.0.5/
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     1065 2023-07-10 02:38:31.000000 nonebot-plugin-nobahpictrue-1.0.5/LICENSE
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      942 2023-07-10 06:10:55.072095 nonebot-plugin-nobahpictrue-1.0.5/PKG-INFO
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      516 2023-07-10 03:13:06.000000 nonebot-plugin-nobahpictrue-1.0.5/README.md
+drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:10:55.072095 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpictrue.egg-info/
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      942 2023-07-10 06:10:54.000000 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpictrue.egg-info/PKG-INFO
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      448 2023-07-10 06:10:55.000000 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpictrue.egg-info/SOURCES.txt
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-10 06:10:54.000000 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpictrue.egg-info/dependency_links.txt
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       33 2023-07-10 06:10:55.000000 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpictrue.egg-info/requires.txt
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       28 2023-07-10 06:10:55.000000 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpictrue.egg-info/top_level.txt
+drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:10:55.072095 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpicture/
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     3223 2023-07-10 06:10:14.000000 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpicture/__init__.py
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      382 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpicture/config.py
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     2004 2023-07-10 05:50:58.000000 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpicture/get_picture.py
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      347 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpicture/rules.py
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       78 2023-07-10 06:10:55.076094 nonebot-plugin-nobahpictrue-1.0.5/setup.cfg
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      675 2023-07-10 06:10:48.000000 nonebot-plugin-nobahpictrue-1.0.5/setup.py
```

### Comparing `nonebot-plugin-nobahpictrue-1.0.4/LICENSE` & `nonebot-plugin-nobahpictrue-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-nobahpictrue-1.0.4/PKG-INFO` & `nonebot-plugin-nobahpictrue-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nobahpictrue
-Version: 1.0.4
+Version: 1.0.5
 Summary: 获取碧蓝档案涩图
 Home-page: https://github.com/Lptr-byte/nonebot-plugin-nobahpicture
 Author: Hansa
 Author-email: hanasakayui2022@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot-plugin-nobahpictrue-1.0.4/README.md` & `nonebot-plugin-nobahpictrue-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-nobahpictrue-1.0.4/nonebot_plugin_nobahpictrue.egg-info/PKG-INFO` & `nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpictrue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nobahpictrue
-Version: 1.0.4
+Version: 1.0.5
 Summary: 获取碧蓝档案涩图
 Home-page: https://github.com/Lptr-byte/nonebot-plugin-nobahpicture
 Author: Hansa
 Author-email: hanasakayui2022@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot-plugin-nobahpictrue-1.0.4/nonebot_plugin_nobahpicture/__init__.py` & `nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpicture/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 from re import I, sub
 from typing import Any, Tuple, Union, Annotated
 
 from nonebot import on_regex, get_driver, on_command
 from nonebot.log import logger
 from nonebot.rule import to_me
 from nonebot.params import Command, RegexGroup
@@ -25,15 +26,15 @@
     description='获取碧蓝档案涩图',
     usage='https://github.com/Lptr-byte/nonebot-plugin-nobahpicture',
     homepage='https://github.com/Lptr-byte/nonebot-plugin-nobahpicture',
     type='application',
     supported_adapters={'~onebot.v11'},
     extra={
         'author': 'Hanasa',
-        'version': '1.0.4',
+        'version': '1.0.5',
         'priority': 1,
     },
 )
 
 
 change_plugin_state = on_command(('Ba涩图', '开启'), rule=to_me(), aliases={('Ba涩图', '禁用')},
                                  permission=SUPERUSER)
@@ -72,16 +73,17 @@
     num = args[1]
     tag = args[2]
     #处理数据
     num = int(sub(r'\D', '', num)) if num else 1
     num = min(num, config.max_picture)
     tag = tag if tag else ''
     get_pic = GetPicture(pic_num=num, user_tag=tag, save=config.save_enabled)
+    await get_pic.get_picture()
     image_urls = []
-    image_urls = get_pic.get_picture()
+    image_urls = get_pic.get_urls()
     del get_pic
     for url in image_urls:
         try:
             await bot.send(event, MessageSegment.image(url))
         except:
             await bot.send(event, MessageSegment.text('发送图片失败……'))
             logger.error('发送图片失败……')
```

### Comparing `nonebot-plugin-nobahpictrue-1.0.4/nonebot_plugin_nobahpicture/get_picture.py` & `nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpicture/get_picture.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 import os
 
-import requests
+import httpx
 
 
 class GetPicture():
     def __init__(self, pic_num: int = 1, user_tag: str = '', size: str = 'original', save: bool = False):
         self.pic_num = pic_num  #需要获取的图片数量
         #Ba Tag
         self.tag = [
             ['BlueArchive', '碧蓝档案', '蔚蓝档案']     #等有日语输入法再加tag
         ]
         self.user_tag = user_tag
         self.size = size
         self.save = save
+        self.res_url = []
 
-    def get_picture(self):
+    async def get_picture(self):
         #请求头
         headers = {
             'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/96.0.4664.45 Safari/537.36',
             'Referer': 'www.pixiv.net',
             'Content-Type': 'application/json'
         }
         #使用POST请求获取网页返回的json数据
         url = 'https://api.lolicon.app/setu/v2'
         #如果用户有指定tag，则添加tag
         if len(self.user_tag):
             self.tag.append([self.user_tag])
         payload = {'r18': 0, 'num': self.pic_num, 'tag': self.tag, 'size': self.size, 'exCludeAI': False}
-        r = requests.post(url, json=payload, headers=headers).json()
+        async with httpx.AsyncClient() as client:
+            r = await client.post(url=url, json=payload, headers=headers)
+            r = r.json()
         #将图片url保存至列表
-        res_url = []
+        self.res_url = []
         for i in range(1, self.pic_num + 1):
-            res_url.append(r['data'][i - 1]['urls'][self.size])
+            self.res_url.append(r['data'][i - 1]['urls'][self.size])
 
         #下载图片并保存到本地
         if self.save:
             if not os.path.isdir('./pics'):
                 os.mkdir('./pics')
             for i in range(1, self.pic_num + 1):
                 with open('./pics/{name}.{ext}'.format(name=r['data'][i - 1]['title'],
-                                                    ext=r['data'][i - 1]['ext']), mode='wb') as f:
-                    res = requests.get(r['data'][i - 1]['urls'][self.size], headers=headers)
+                                                       ext=r['data'][i - 1]['ext']), mode='wb') as f:
+                    res = httpx.get(r['data'][i - 1]['urls'][self.size], headers=headers)
                     f.write(res.content)
 
-        return res_url
+    def get_urls(self):
+        return self.res_url
```

### Comparing `nonebot-plugin-nobahpictrue-1.0.4/setup.py` & `nonebot-plugin-nobahpictrue-1.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='nonebot-plugin-nobahpictrue',
-    version='1.0.4',
+    version='1.0.5',
     author='Hansa',
     author_email='hanasakayui2022@gmail.com',
     description='获取碧蓝档案涩图',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Lptr-byte/nonebot-plugin-nobahpicture',
     packages=setuptools.find_packages(),
-    install_requires=['requests==2.25.1'],
+    install_requires=['requests==2.25.1', 'nonebot2==2.0.0'],
     classifiers=(
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License'
     )  # type: ignore
 )
```

