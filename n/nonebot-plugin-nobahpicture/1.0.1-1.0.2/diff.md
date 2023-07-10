# Comparing `tmp/nonebot-plugin-nobahpicture-1.0.1.tar.gz` & `tmp/nonebot-plugin-nobahpicture-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-nobahpicture-1.0.1.tar", last modified: Mon Jul 10 06:44:43 2023, max compression
+gzip compressed data, was "nonebot-plugin-nobahpicture-1.0.2.tar", last modified: Mon Jul 10 06:52:17 2023, max compression
```

## Comparing `nonebot-plugin-nobahpicture-1.0.1.tar` & `nonebot-plugin-nobahpicture-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:44:43.136536 nonebot-plugin-nobahpicture-1.0.1/
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     1065 2023-07-10 02:38:31.000000 nonebot-plugin-nobahpicture-1.0.1/LICENSE
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      942 2023-07-10 06:44:43.136536 nonebot-plugin-nobahpicture-1.0.1/PKG-INFO
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      516 2023-07-10 03:13:06.000000 nonebot-plugin-nobahpicture-1.0.1/README.md
-drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:44:43.132536 nonebot-plugin-nobahpicture-1.0.1/nonebot_plugin_nobahpicture/
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     3239 2023-07-10 06:44:26.000000 nonebot-plugin-nobahpicture-1.0.1/nonebot_plugin_nobahpicture/__init__.py
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      382 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpicture-1.0.1/nonebot_plugin_nobahpicture/config.py
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     2004 2023-07-10 05:50:58.000000 nonebot-plugin-nobahpicture-1.0.1/nonebot_plugin_nobahpicture/get_picture.py
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      347 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpicture-1.0.1/nonebot_plugin_nobahpicture/rules.py
-drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:44:43.136536 nonebot-plugin-nobahpicture-1.0.1/nonebot_plugin_nobahpicture.egg-info/
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      942 2023-07-10 06:44:43.000000 nonebot-plugin-nobahpicture-1.0.1/nonebot_plugin_nobahpicture.egg-info/PKG-INFO
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      448 2023-07-10 06:44:43.000000 nonebot-plugin-nobahpicture-1.0.1/nonebot_plugin_nobahpicture.egg-info/SOURCES.txt
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-10 06:44:43.000000 nonebot-plugin-nobahpicture-1.0.1/nonebot_plugin_nobahpicture.egg-info/dependency_links.txt
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       30 2023-07-10 06:44:43.000000 nonebot-plugin-nobahpicture-1.0.1/nonebot_plugin_nobahpicture.egg-info/requires.txt
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       28 2023-07-10 06:44:43.000000 nonebot-plugin-nobahpicture-1.0.1/nonebot_plugin_nobahpicture.egg-info/top_level.txt
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       78 2023-07-10 06:44:43.140536 nonebot-plugin-nobahpicture-1.0.1/setup.cfg
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      672 2023-07-10 06:44:37.000000 nonebot-plugin-nobahpicture-1.0.1/setup.py
+drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:52:17.147344 nonebot-plugin-nobahpicture-1.0.2/
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     1065 2023-07-10 02:38:31.000000 nonebot-plugin-nobahpicture-1.0.2/LICENSE
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      942 2023-07-10 06:52:17.147344 nonebot-plugin-nobahpicture-1.0.2/PKG-INFO
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      516 2023-07-10 03:13:06.000000 nonebot-plugin-nobahpicture-1.0.2/README.md
+drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:52:17.147344 nonebot-plugin-nobahpicture-1.0.2/nonebot_plugin_nobahpicture/
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     3239 2023-07-10 06:52:11.000000 nonebot-plugin-nobahpicture-1.0.2/nonebot_plugin_nobahpicture/__init__.py
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      382 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpicture-1.0.2/nonebot_plugin_nobahpicture/config.py
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     2004 2023-07-10 05:50:58.000000 nonebot-plugin-nobahpicture-1.0.2/nonebot_plugin_nobahpicture/get_picture.py
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      347 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpicture-1.0.2/nonebot_plugin_nobahpicture/rules.py
+drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 06:52:17.147344 nonebot-plugin-nobahpicture-1.0.2/nonebot_plugin_nobahpicture.egg-info/
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      942 2023-07-10 06:52:17.000000 nonebot-plugin-nobahpicture-1.0.2/nonebot_plugin_nobahpicture.egg-info/PKG-INFO
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      448 2023-07-10 06:52:17.000000 nonebot-plugin-nobahpicture-1.0.2/nonebot_plugin_nobahpicture.egg-info/SOURCES.txt
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-10 06:52:17.000000 nonebot-plugin-nobahpicture-1.0.2/nonebot_plugin_nobahpicture.egg-info/dependency_links.txt
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       53 2023-07-10 06:52:17.000000 nonebot-plugin-nobahpicture-1.0.2/nonebot_plugin_nobahpicture.egg-info/requires.txt
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       28 2023-07-10 06:52:17.000000 nonebot-plugin-nobahpicture-1.0.2/nonebot_plugin_nobahpicture.egg-info/top_level.txt
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       78 2023-07-10 06:52:17.151344 nonebot-plugin-nobahpicture-1.0.2/setup.cfg
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      698 2023-07-10 06:51:59.000000 nonebot-plugin-nobahpicture-1.0.2/setup.py
```

### Comparing `nonebot-plugin-nobahpicture-1.0.1/LICENSE` & `nonebot-plugin-nobahpicture-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-nobahpicture-1.0.1/PKG-INFO` & `nonebot-plugin-nobahpicture-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nobahpicture
-Version: 1.0.1
+Version: 1.0.2
 Summary: 获取碧蓝档案涩图
 Home-page: https://github.com/Lptr-byte/nonebot-plugin-nobahpicture
 Author: Hansa
 Author-email: hanasakayui2022@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot-plugin-nobahpicture-1.0.1/README.md` & `nonebot-plugin-nobahpicture-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-nobahpicture-1.0.1/nonebot_plugin_nobahpicture/__init__.py` & `nonebot-plugin-nobahpicture-1.0.2/nonebot_plugin_nobahpicture/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     description='获取碧蓝档案涩图',
     usage='https://github.com/Lptr-byte/nonebot-plugin-nobahpicture',
     homepage='https://github.com/Lptr-byte/nonebot-plugin-nobahpicture',
     type='application',
     supported_adapters={'nonebot.adapters.onebot.v11'},
     extra={
         'author': 'Hanasa',
-        'version': '1.0.1',
+        'version': '1.0.2',
         'priority': 1,
     },
 )
 
 
 change_plugin_state = on_command(('Ba涩图', '开启'), rule=to_me(), aliases={('Ba涩图', '禁用')},
                                  permission=SUPERUSER)
```

### Comparing `nonebot-plugin-nobahpicture-1.0.1/nonebot_plugin_nobahpicture/get_picture.py` & `nonebot-plugin-nobahpicture-1.0.2/nonebot_plugin_nobahpicture/get_picture.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-nobahpicture-1.0.1/nonebot_plugin_nobahpicture.egg-info/PKG-INFO` & `nonebot-plugin-nobahpicture-1.0.2/nonebot_plugin_nobahpicture.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nobahpicture
-Version: 1.0.1
+Version: 1.0.2
 Summary: 获取碧蓝档案涩图
 Home-page: https://github.com/Lptr-byte/nonebot-plugin-nobahpicture
 Author: Hansa
 Author-email: hanasakayui2022@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot-plugin-nobahpicture-1.0.1/setup.py` & `nonebot-plugin-nobahpicture-1.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='nonebot-plugin-nobahpicture',
-    version='1.0.1',
+    version='1.0.2',
     author='Hansa',
     author_email='hanasakayui2022@gmail.com',
     description='获取碧蓝档案涩图',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Lptr-byte/nonebot-plugin-nobahpicture',
     packages=setuptools.find_packages(),
-    install_requires=['httpx==0.24.1', 'nonebot2==2.0.0'],
+    install_requires=['httpx==0.24.1', 'nonebot2==2.0.0', 'nonebot-adapter-onebot'],
     classifiers=(
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License'
     )  # type: ignore
 )
```

