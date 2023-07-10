# Comparing `tmp/nonebot-plugin-nobahpictrue-1.0.0.tar.gz` & `tmp/nonebot-plugin-nobahpictrue-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-nobahpictrue-1.0.0.tar", last modified: Mon Jul 10 03:00:04 2023, max compression
+gzip compressed data, was "nonebot-plugin-nobahpictrue-1.0.2.tar", last modified: Mon Jul 10 03:16:56 2023, max compression
```

## Comparing `nonebot-plugin-nobahpictrue-1.0.0.tar` & `nonebot-plugin-nobahpictrue-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 03:00:04.030092 nonebot-plugin-nobahpictrue-1.0.0/
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     1065 2023-07-10 02:38:31.000000 nonebot-plugin-nobahpictrue-1.0.0/LICENSE
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      788 2023-07-10 03:00:04.030092 nonebot-plugin-nobahpictrue-1.0.0/PKG-INFO
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      362 2023-07-10 02:58:54.000000 nonebot-plugin-nobahpictrue-1.0.0/README.md
-drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 03:00:04.030092 nonebot-plugin-nobahpictrue-1.0.0/nonebot_plugin_nobahpictrue.egg-info/
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      788 2023-07-10 03:00:03.000000 nonebot-plugin-nobahpictrue-1.0.0/nonebot_plugin_nobahpictrue.egg-info/PKG-INFO
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      448 2023-07-10 03:00:03.000000 nonebot-plugin-nobahpictrue-1.0.0/nonebot_plugin_nobahpictrue.egg-info/SOURCES.txt
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-10 03:00:03.000000 nonebot-plugin-nobahpictrue-1.0.0/nonebot_plugin_nobahpictrue.egg-info/dependency_links.txt
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       17 2023-07-10 03:00:03.000000 nonebot-plugin-nobahpictrue-1.0.0/nonebot_plugin_nobahpictrue.egg-info/requires.txt
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       28 2023-07-10 03:00:03.000000 nonebot-plugin-nobahpictrue-1.0.0/nonebot_plugin_nobahpictrue.egg-info/top_level.txt
-drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 03:00:04.030092 nonebot-plugin-nobahpictrue-1.0.0/nonebot_plugin_nobahpicture/
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     2710 2023-07-10 02:36:37.000000 nonebot-plugin-nobahpictrue-1.0.0/nonebot_plugin_nobahpicture/__init__.py
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      382 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpictrue-1.0.0/nonebot_plugin_nobahpicture/config.py
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     1857 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpictrue-1.0.0/nonebot_plugin_nobahpicture/get_picture.py
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      347 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpictrue-1.0.0/nonebot_plugin_nobahpicture/rules.py
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       78 2023-07-10 03:00:04.030092 nonebot-plugin-nobahpictrue-1.0.0/setup.cfg
--rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      656 2023-07-09 13:15:33.000000 nonebot-plugin-nobahpictrue-1.0.0/setup.py
+drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 03:16:56.556317 nonebot-plugin-nobahpictrue-1.0.2/
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     1065 2023-07-10 02:38:31.000000 nonebot-plugin-nobahpictrue-1.0.2/LICENSE
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      942 2023-07-10 03:16:56.556317 nonebot-plugin-nobahpictrue-1.0.2/PKG-INFO
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      516 2023-07-10 03:13:06.000000 nonebot-plugin-nobahpictrue-1.0.2/README.md
+drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 03:16:56.552317 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpictrue.egg-info/
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      942 2023-07-10 03:16:56.000000 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpictrue.egg-info/PKG-INFO
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      448 2023-07-10 03:16:56.000000 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpictrue.egg-info/SOURCES.txt
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-10 03:16:56.000000 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpictrue.egg-info/dependency_links.txt
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       17 2023-07-10 03:16:56.000000 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpictrue.egg-info/requires.txt
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       28 2023-07-10 03:16:56.000000 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpictrue.egg-info/top_level.txt
+drwxr-x---   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 03:16:56.556317 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpicture/
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     2710 2023-07-10 02:36:37.000000 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpicture/__init__.py
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      382 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpicture/config.py
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)     1857 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpicture/get_picture.py
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      347 2023-07-09 12:35:49.000000 nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpicture/rules.py
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)       78 2023-07-10 03:16:56.560317 nonebot-plugin-nobahpictrue-1.0.2/setup.cfg
+-rw-r-----   0 ubuntu    (1000) ubuntu    (1000)      656 2023-07-10 03:16:54.000000 nonebot-plugin-nobahpictrue-1.0.2/setup.py
```

### Comparing `nonebot-plugin-nobahpictrue-1.0.0/LICENSE` & `nonebot-plugin-nobahpictrue-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-nobahpictrue-1.0.0/PKG-INFO` & `nonebot-plugin-nobahpictrue-1.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nobahpictrue
-Version: 1.0.0
+Version: 1.0.2
 Summary: 获取碧蓝档案涩图
 Home-page: https://github.com/Lptr-byte/nonebot-plugin-nobahpicture
 Author: Hansa
 Author-email: hanasakayui2022@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nonebot-plugin-nobahpicture
-## 指令
+## 安装
+### 使用```nb-cli```安装：
+nb plugin install nonebot-plugin-nobahpicture
+### 使用```pip```安装
+pip install nonebot-plugin-nobahpicture
+## 使用
 * ```来点Ba涩图 [num] [tag]```
 * 上述指令```[num]```为所需图片张数，为可选参数，默认为1,以8张为例 ~虽然目前最大张数限制为2张~ 可以为```8``` ```x8``` ```x8张/个/份``` ```8张/个/份```
 * ```[tag]``` 为可选参数，可输入想要学生的名字，如 ```美游```
 ## TODO:
```

### Comparing `nonebot-plugin-nobahpictrue-1.0.0/nonebot_plugin_nobahpictrue.egg-info/PKG-INFO` & `nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpictrue.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nobahpictrue
-Version: 1.0.0
+Version: 1.0.2
 Summary: 获取碧蓝档案涩图
 Home-page: https://github.com/Lptr-byte/nonebot-plugin-nobahpicture
 Author: Hansa
 Author-email: hanasakayui2022@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nonebot-plugin-nobahpicture
-## 指令
+## 安装
+### 使用```nb-cli```安装：
+nb plugin install nonebot-plugin-nobahpicture
+### 使用```pip```安装
+pip install nonebot-plugin-nobahpicture
+## 使用
 * ```来点Ba涩图 [num] [tag]```
 * 上述指令```[num]```为所需图片张数，为可选参数，默认为1,以8张为例 ~虽然目前最大张数限制为2张~ 可以为```8``` ```x8``` ```x8张/个/份``` ```8张/个/份```
 * ```[tag]``` 为可选参数，可输入想要学生的名字，如 ```美游```
 ## TODO:
```

### Comparing `nonebot-plugin-nobahpictrue-1.0.0/nonebot_plugin_nobahpicture/__init__.py` & `nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpicture/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-nobahpictrue-1.0.0/nonebot_plugin_nobahpicture/get_picture.py` & `nonebot-plugin-nobahpictrue-1.0.2/nonebot_plugin_nobahpicture/get_picture.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-nobahpictrue-1.0.0/setup.py` & `nonebot-plugin-nobahpictrue-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='nonebot-plugin-nobahpictrue',
-    version='1.0.0',
+    version='1.0.2',
     author='Hansa',
     author_email='hanasakayui2022@gmail.com',
     description='获取碧蓝档案涩图',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Lptr-byte/nonebot-plugin-nobahpicture',
     packages=setuptools.find_packages(),
```

