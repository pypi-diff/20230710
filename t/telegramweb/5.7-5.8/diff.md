# Comparing `tmp/telegramweb-5.7.tar.gz` & `tmp/telegramweb-5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegramweb-5.7.tar", last modified: Mon Jul 10 12:44:33 2023, max compression
+gzip compressed data, was "telegramweb-5.8.tar", last modified: Mon Jul 10 12:52:32 2023, max compression
```

## Comparing `telegramweb-5.7.tar` & `telegramweb-5.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:44:33.149514 telegramweb-5.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-10 12:44:05.000000 telegramweb-5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 12:44:05.000000 telegramweb-5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-07-10 12:44:33.149514 telegramweb-5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-10 12:44:05.000000 telegramweb-5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 12:44:33.149514 telegramweb-5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-10 12:44:05.000000 telegramweb-5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:44:33.149514 telegramweb-5.7/telegram_news/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-10 12:44:05.000000 telegramweb-5.7/telegram_news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-10 12:44:05.000000 telegramweb-5.7/telegram_news/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-10 12:44:05.000000 telegramweb-5.7/telegram_news/displaypolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-10 12:44:05.000000 telegramweb-5.7/telegram_news/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 12:44:05.000000 telegramweb-5.7/telegram_news/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:44:33.149514 telegramweb-5.7/telegram_news/template/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-10 12:44:05.000000 telegramweb-5.7/telegram_news/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44449 2023-07-10 12:44:05.000000 telegramweb-5.7/telegram_news/template/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-07-10 12:44:05.000000 telegramweb-5.7/telegram_news/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:44:33.149514 telegramweb-5.7/telegramweb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-07-10 12:44:33.000000 telegramweb-5.7/telegramweb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-10 12:44:33.000000 telegramweb-5.7/telegramweb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:44:33.000000 telegramweb-5.7/telegramweb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 12:44:33.000000 telegramweb-5.7/telegramweb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 12:44:33.000000 telegramweb-5.7/telegramweb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:52:32.167474 telegramweb-5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-10 12:52:11.000000 telegramweb-5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 12:52:11.000000 telegramweb-5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-07-10 12:52:32.167474 telegramweb-5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-10 12:52:11.000000 telegramweb-5.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 12:52:32.167474 telegramweb-5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-10 12:52:11.000000 telegramweb-5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:52:32.163474 telegramweb-5.8/telegram_news/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-10 12:52:11.000000 telegramweb-5.8/telegram_news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-10 12:52:11.000000 telegramweb-5.8/telegram_news/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-10 12:52:11.000000 telegramweb-5.8/telegram_news/displaypolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-10 12:52:11.000000 telegramweb-5.8/telegram_news/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 12:52:11.000000 telegramweb-5.8/telegram_news/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:52:32.167474 telegramweb-5.8/telegram_news/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-10 12:52:11.000000 telegramweb-5.8/telegram_news/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44443 2023-07-10 12:52:11.000000 telegramweb-5.8/telegram_news/template/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-07-10 12:52:11.000000 telegramweb-5.8/telegram_news/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:52:32.167474 telegramweb-5.8/telegramweb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-07-10 12:52:32.000000 telegramweb-5.8/telegramweb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-10 12:52:32.000000 telegramweb-5.8/telegramweb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:52:32.000000 telegramweb-5.8/telegramweb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 12:52:32.000000 telegramweb-5.8/telegramweb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 12:52:32.000000 telegramweb-5.8/telegramweb.egg-info/top_level.txt
```

### Comparing `telegramweb-5.7/LICENSE` & `telegramweb-5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `telegramweb-5.7/PKG-INFO` & `telegramweb-5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegramweb
-Version: 5.7
+Version: 5.8
 Summary: Python package for automatically fetching and pushing news by Telegram.
 Home-page: https://github.com/craziks-creator/telegram-web
 Author: craziks
 Author-email: chandrashekharpanday07@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `telegramweb-5.7/README.md` & `telegramweb-5.8/README.md`

 * *Files identical despite different names*

### Comparing `telegramweb-5.7/setup.py` & `telegramweb-5.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ]
 
 DESCRIPTION = 'Python package for automatically fetching and pushing news by Telegram.'
 LONG_DESCRIPTION = open("README.md").read()
 
 setup(
     name='telegramweb',
-    version='5.7',
+    version='5.8',
     author='craziks',
     author_email='chandrashekharpanday07@gmail.com',
     url='https://github.com/craziks-creator/telegram-web',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

### Comparing `telegramweb-5.7/telegram_news/__init__.py` & `telegramweb-5.8/telegram_news/__init__.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.7/telegram_news/constant.py` & `telegramweb-5.8/telegram_news/constant.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.7/telegram_news/displaypolicy.py` & `telegramweb-5.8/telegram_news/displaypolicy.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.7/telegram_news/ratelimit.py` & `telegramweb-5.8/telegram_news/ratelimit.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.7/telegram_news/template/common.py` & `telegramweb-5.8/telegram_news/template/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import math
 import os
 import random
 import threading
 import traceback
 import warnings
 from time import sleep
-from pyrogram.types import InlineKeyboardButton, InlineKeyboardMarkup
+from telegram import InlineKeyboardButton, InlineKeyboardMarkup
 import requests
 import sqlalchemy
 from bs4 import BeautifulSoup
 
 from ..displaypolicy import (
     best_effort_display_policy,
     default_id_policy,
```

### Comparing `telegramweb-5.7/telegram_news/utils.py` & `telegramweb-5.8/telegram_news/utils.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.7/telegramweb.egg-info/PKG-INFO` & `telegramweb-5.8/telegramweb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegramweb
-Version: 5.7
+Version: 5.8
 Summary: Python package for automatically fetching and pushing news by Telegram.
 Home-page: https://github.com/craziks-creator/telegram-web
 Author: craziks
 Author-email: chandrashekharpanday07@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

