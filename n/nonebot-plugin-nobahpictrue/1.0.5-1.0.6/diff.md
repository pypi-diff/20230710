# Comparing `tmp/nonebot-plugin-nobahpictrue-1.0.5.tar.gz` & `tmp/nonebot-plugin-nobahpictrue-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-nobahpictrue-1.0.5.tar", last modified: Mon Jul 10 06:10:55 2023, max compression
+gzip compressed data, was "nonebot-plugin-nobahpictrue-1.0.6.tar", last modified: Mon Jul 10 06:14:19 2023, max compression
```

## Comparing `nonebot-plugin-nobahpictrue-1.0.5.tar` & `nonebot-plugin-nobahpictrue-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:10:55.072095 nonebot-plugin-nobahpictrue-1.0.5/
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     1065 2023-07-10 02:38:31.000000 nonebot-plugin-nobahpictrue-1.0.5/LICENSE
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      942 2023-07-10 06:10:55.072095 nonebot-plugin-nobahpictrue-1.0.5/PKG-INFO
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      516 2023-07-10 03:13:06.000000 nonebot-plugin-nobahpictrue-1.0.5/README.md
-drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:10:55.072095 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpictrue.egg-info/
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      942 2023-07-10 06:10:54.000000 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpictrue.egg-info/PKG-INFO
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      448 2023-07-10 06:10:55.000000 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpictrue.egg-info/SOURCES.txt
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-10 06:10:54.000000 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpictrue.egg-info/dependency_links.txt
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       33 2023-07-10 06:10:55.000000 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpictrue.egg-info/requires.txt
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       28 2023-07-10 06:10:55.000000 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpictrue.egg-info/top_level.txt
-drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:10:55.072095 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpicture/
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     3223 2023-07-10 06:10:14.000000 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpicture/__init__.py
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      382 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpicture/config.py
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     2004 2023-07-10 05:50:58.000000 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpicture/get_picture.py
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      347 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpicture/rules.py
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       78 2023-07-10 06:10:55.076094 nonebot-plugin-nobahpictrue-1.0.5/setup.cfg
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      675 2023-07-10 06:10:48.000000 nonebot-plugin-nobahpictrue-1.0.5/setup.py
+drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:14:19.173336 nonebot-plugin-nobahpictrue-1.0.6/
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     1065 2023-07-10 02:38:31.000000 nonebot-plugin-nobahpictrue-1.0.6/LICENSE
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      942 2023-07-10 06:14:19.173336 nonebot-plugin-nobahpictrue-1.0.6/PKG-INFO
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      516 2023-07-10 03:13:06.000000 nonebot-plugin-nobahpictrue-1.0.6/README.md
+drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:14:19.173336 nonebot-plugin-nobahpictrue-1.0.6/nonebot_plugin_nobahpictrue.egg-info/
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      942 2023-07-10 06:14:19.000000 nonebot-plugin-nobahpictrue-1.0.6/nonebot_plugin_nobahpictrue.egg-info/PKG-INFO
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      448 2023-07-10 06:14:19.000000 nonebot-plugin-nobahpictrue-1.0.6/nonebot_plugin_nobahpictrue.egg-info/SOURCES.txt
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-10 06:14:19.000000 nonebot-plugin-nobahpictrue-1.0.6/nonebot_plugin_nobahpictrue.egg-info/dependency_links.txt
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       30 2023-07-10 06:14:19.000000 nonebot-plugin-nobahpictrue-1.0.6/nonebot_plugin_nobahpictrue.egg-info/requires.txt
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       28 2023-07-10 06:14:19.000000 nonebot-plugin-nobahpictrue-1.0.6/nonebot_plugin_nobahpictrue.egg-info/top_level.txt
+drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:14:19.173336 nonebot-plugin-nobahpictrue-1.0.6/nonebot_plugin_nobahpicture/
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     3223 2023-07-10 06:14:12.000000 nonebot-plugin-nobahpictrue-1.0.6/nonebot_plugin_nobahpicture/__init__.py
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      382 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpictrue-1.0.6/nonebot_plugin_nobahpicture/config.py
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     2004 2023-07-10 05:50:58.000000 nonebot-plugin-nobahpictrue-1.0.6/nonebot_plugin_nobahpicture/get_picture.py
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      347 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpictrue-1.0.6/nonebot_plugin_nobahpicture/rules.py
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       78 2023-07-10 06:14:19.173336 nonebot-plugin-nobahpictrue-1.0.6/setup.cfg
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      672 2023-07-10 06:14:02.000000 nonebot-plugin-nobahpictrue-1.0.6/setup.py
```

### Comparing `nonebot-plugin-nobahpictrue-1.0.5/LICENSE` & `nonebot-plugin-nobahpictrue-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-nobahpictrue-1.0.5/PKG-INFO` & `nonebot-plugin-nobahpictrue-1.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nobahpictrue
-Version: 1.0.5
+Version: 1.0.6
 Summary: 获取碧蓝档案涩图
 Home-page: https://github.com/Lptr-byte/nonebot-plugin-nobahpicture
 Author: Hansa
 Author-email: hanasakayui2022@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot-plugin-nobahpictrue-1.0.5/README.md` & `nonebot-plugin-nobahpictrue-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpictrue.egg-info/PKG-INFO` & `nonebot-plugin-nobahpictrue-1.0.6/nonebot_plugin_nobahpictrue.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nobahpictrue
-Version: 1.0.5
+Version: 1.0.6
 Summary: 获取碧蓝档案涩图
 Home-page: https://github.com/Lptr-byte/nonebot-plugin-nobahpicture
 Author: Hansa
 Author-email: hanasakayui2022@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpicture/__init__.py` & `nonebot-plugin-nobahpictrue-1.0.6/nonebot_plugin_nobahpicture/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     description='获取碧蓝档案涩图',
     usage='https://github.com/Lptr-byte/nonebot-plugin-nobahpicture',
     homepage='https://github.com/Lptr-byte/nonebot-plugin-nobahpicture',
     type='application',
     supported_adapters={'~onebot.v11'},
     extra={
         'author': 'Hanasa',
-        'version': '1.0.5',
+        'version': '1.0.6',
         'priority': 1,
     },
 )
 
 
 change_plugin_state = on_command(('Ba涩图', '开启'), rule=to_me(), aliases={('Ba涩图', '禁用')},
                                  permission=SUPERUSER)
```

### Comparing `nonebot-plugin-nobahpictrue-1.0.5/nonebot_plugin_nobahpicture/get_picture.py` & `nonebot-plugin-nobahpictrue-1.0.6/nonebot_plugin_nobahpicture/get_picture.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-nobahpictrue-1.0.5/setup.py` & `nonebot-plugin-nobahpictrue-1.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='nonebot-plugin-nobahpictrue',
-    version='1.0.5',
+    version='1.0.6',
     author='Hansa',
     author_email='hanasakayui2022@gmail.com',
     description='获取碧蓝档案涩图',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Lptr-byte/nonebot-plugin-nobahpicture',
     packages=setuptools.find_packages(),
-    install_requires=['requests==2.25.1', 'nonebot2==2.0.0'],
+    install_requires=['httpx==0.24.1', 'nonebot2==2.0.0'],
     classifiers=(
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License'
     )  # type: ignore
 )
```

