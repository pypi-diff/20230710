# Comparing `tmp/nonebot_plugin_friends-0.1.0.tar.gz` & `tmp/nonebot_plugin_friends-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_friends-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_friends-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_friends-0.1.0.tar` & `nonebot_plugin_friends-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1089 2023-07-01 09:08:41.165535 nonebot_plugin_friends-0.1.0/LICENSE
--rw-r--r--   0        0        0     5347 2023-07-09 13:56:11.538687 nonebot_plugin_friends-0.1.0/nonebot_plugin_friends/__init__.py
--rw-r--r--   0        0        0     1256 2023-07-09 12:50:10.684895 nonebot_plugin_friends-0.1.0/nonebot_plugin_friends/config.py
--rw-r--r--   0        0        0     6580 2023-07-09 13:51:45.559350 nonebot_plugin_friends-0.1.0/nonebot_plugin_friends/event.py
--rw-r--r--   0        0        0      919 2023-07-09 13:02:12.031759 nonebot_plugin_friends-0.1.0/nonebot_plugin_friends/utils.py
--rw-r--r--   0        0        0      994 2023-07-09 13:52:36.832855 nonebot_plugin_friends-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2175 2023-07-09 13:58:11.810945 nonebot_plugin_friends-0.1.0/README.md
--rw-r--r--   0        0        0     3018 1970-01-01 00:00:00.000000 nonebot_plugin_friends-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-10 08:45:27.610574 nonebot_plugin_friends-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2116 2023-07-10 08:45:27.614575 nonebot_plugin_friends-0.1.1/README.md
+-rw-r--r--   0        0        0     5181 2023-07-10 08:45:27.614575 nonebot_plugin_friends-0.1.1/nonebot_plugin_friends/__init__.py
+-rw-r--r--   0        0        0     1591 2023-07-10 08:45:27.614575 nonebot_plugin_friends-0.1.1/nonebot_plugin_friends/config.py
+-rw-r--r--   0        0        0     7476 2023-07-10 08:45:27.614575 nonebot_plugin_friends-0.1.1/nonebot_plugin_friends/event.py
+-rw-r--r--   0        0        0      882 2023-07-10 08:45:27.614575 nonebot_plugin_friends-0.1.1/nonebot_plugin_friends/utils.py
+-rw-r--r--   0        0        0      960 2023-07-10 08:45:27.614575 nonebot_plugin_friends-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3018 1970-01-01 00:00:00.000000 nonebot_plugin_friends-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_friends-0.1.0/LICENSE` & `nonebot_plugin_friends-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 PadorFelice
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 PadorFelice
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `nonebot_plugin_friends-0.1.0/pyproject.toml` & `nonebot_plugin_friends-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-[tool.poetry]
-name = "nonebot_plugin_friends"
-version = "0.1.0"
-description = "Nonebot2插件处理好友申请"
-authors = ["Agnes_Digital <Z735803792@163.com>"]
-license = "MIT"
-readme = "README.md"
-homepage = "https://github.com/Agnes4m/nonebot_plugin_friends"
-repository = "https://github.com/Agnes4m/nonebot_plugin_friends"
-keywords = ["maimai", "nonebot2", "plugin"]
-classifiers = [
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Operating System :: OS Independent",
-
-]
-include = [
-    "LICENSE","README.md"
-]
- 
-[tool.poetry.dependencies]
-python = "^3.8"
-nonebot2 = "^2.0.0"
-nonebot-adapter-onebot = "^2.1.3"
-
-[tool.poetry.dev-dependencies]
- 
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "nonebot_plugin_friends"
+version = "0.1.1"
+description = "Nonebot2插件处理好友申请"
+authors = ["Agnes_Digital <Z735803792@163.com>"]
+license = "MIT"
+readme = "README.md"
+homepage = "https://github.com/Agnes4m/nonebot_plugin_friends"
+repository = "https://github.com/Agnes4m/nonebot_plugin_friends"
+keywords = ["maimai", "nonebot2", "plugin"]
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Operating System :: OS Independent",
+
+]
+include = [
+    "LICENSE","README.md"
+]
+ 
+[tool.poetry.dependencies]
+python = "^3.8"
+nonebot2 = "^2.0.0"
+nonebot-adapter-onebot = "^2.1.3"
+
+[tool.poetry.dev-dependencies]
+ 
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_friends-0.1.0/README.md` & `nonebot_plugin_friends-0.1.1/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-<div align="center">
-  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
-  <br>
-  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
-</div>
-
-<div align="center">
-
-# nonebot_plugin_friends
-
-__✨Nonebot同意好友✨__
-
-<a href="https://github.com/Agnes4m/nonebot_plugin_friends/stargazers">
-        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_friends" alt="stars">
-</a>
-<a href="https://github.com/Agnes4m/nonebot_plugin_friends/issues">
-        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_friends" alt="issues">
-</a>
-<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">
-        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">
-</a>
-<a href="https://pypi.python.org/pypi/nonebot_plugin_friends">
-        <img src="https://img.shields.io/pypi/v/nonebot_plugin_friends.svg" alt="pypi">
-</a>
-    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
-    <img src="https://img.shields.io/badge/nonebot-2.0.0-red.svg" alt="NoneBot">
-</div>
-
-## 指令
-
-### 好友申请（权限为master_id|SUPERUSER）
-
-- (被动) —— 接受好友请求
-- 同意 —— 同意最近一次好友请求
-- 同意[number] —— 同意指定qq号添加好友
-- (回复消息)同意 —— 同意改申请的对象
-
-### 群聊申请(权限为群主|管理|master_id|SUPERUSER)
-
-- (被动) —— 接受群聊申请
-- 同意[number] —— 同意指定qq号添加好友
-- (回复消息)同意 —— 同意改申请的对象
-
-## env配置
-
-不知道可以不写
-知道就按下面参数改添加到env中
-
-    bot_nickname = '宁宁'
-    master_nickname = '主人'
-    master_id = ['114514']
-    group_request = True      # 开启群聊申请处理
-
-
-## 🙈 其他
-
-- 本项目仅供学习使用，请勿用于商业用途，喜欢该项目可以Star或者提供PR
-- [爱发电](https://afdian.net/a/agnes_digital)
-
+<div align="center">
+  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
+  <br>
+  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
+</div>
+
+<div align="center">
+
+# nonebot_plugin_friends
+
+__✨Nonebot同意好友✨__
+
+<a href="https://github.com/Agnes4m/nonebot_plugin_friends/stargazers">
+        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_friends" alt="stars">
+</a>
+<a href="https://github.com/Agnes4m/nonebot_plugin_friends/issues">
+        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_friends" alt="issues">
+</a>
+<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">
+        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot_plugin_friends">
+        <img src="https://img.shields.io/pypi/v/nonebot_plugin_friends.svg" alt="pypi">
+</a>
+    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+    <img src="https://img.shields.io/badge/nonebot-2.0.0-red.svg" alt="NoneBot">
+</div>
+
+## 指令
+
+### 好友申请（权限为master_id|SUPERUSER）
+
+- (被动) —— 接受好友请求
+- 同意 —— 同意最近一次好友请求
+- 同意[number] —— 同意指定qq号添加好友
+- (回复消息)同意 —— 同意改申请的对象
+
+### 群聊申请(权限为群主|管理|master_id|SUPERUSER)
+
+- (被动) —— 接受群聊申请
+- 同意[number] —— 同意指定qq号添加好友
+- (回复消息)同意 —— 同意改申请的对象
+
+## env配置
+
+不知道可以不写
+知道就按下面参数改添加到env中
+
+    bot_nickname = '宁宁'
+    master_nickname = '主人'
+    master_id = ['114514']
+    group_request = True      # 开启群聊申请处理
+
+
+## 🙈 其他
+
+- 本项目仅供学习使用，请勿用于商业用途，喜欢该项目可以Star或者提供PR
+- [爱发电](https://afdian.net/a/agnes_digital)
+
```

### Comparing `nonebot_plugin_friends-0.1.0/PKG-INFO` & `nonebot_plugin_friends-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-friends
-Version: 0.1.0
+Version: 0.1.1
 Summary: Nonebot2插件处理好友申请
 Home-page: https://github.com/Agnes4m/nonebot_plugin_friends
 License: MIT
 Keywords: maimai,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-friends Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-friends Version: 0.1.1 Summary:
 Nonebot2æä»¶å¤çå¥½åç³è¯· Home-page: https://github.com/Agnes4m/
 nonebot_plugin_friends License: MIT Keywords: maimai,nonebot2,plugin Author:
 Agnes_Digital Author-email: Z735803792@163.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

