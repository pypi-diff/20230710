# Comparing `tmp/telegramweb-5.5.tar.gz` & `tmp/telegramweb-5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegramweb-5.5.tar", last modified: Sat Jul  8 09:55:36 2023, max compression
+gzip compressed data, was "dist/telegramweb-5.6.tar", last modified: Mon Jul 10 12:12:04 2023, max compression
```

## Comparing `telegramweb-5.5.tar` & `telegramweb-5.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:55:36.914713 telegramweb-5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-08 09:55:21.000000 telegramweb-5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-08 09:55:21.000000 telegramweb-5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-07-08 09:55:36.914713 telegramweb-5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-08 09:55:21.000000 telegramweb-5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 09:55:36.914713 telegramweb-5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-08 09:55:21.000000 telegramweb-5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:55:36.914713 telegramweb-5.5/telegram_news/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-08 09:55:21.000000 telegramweb-5.5/telegram_news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-08 09:55:21.000000 telegramweb-5.5/telegram_news/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-08 09:55:21.000000 telegramweb-5.5/telegram_news/displaypolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-08 09:55:21.000000 telegramweb-5.5/telegram_news/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-08 09:55:21.000000 telegramweb-5.5/telegram_news/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:55:36.914713 telegramweb-5.5/telegram_news/template/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-08 09:55:21.000000 telegramweb-5.5/telegram_news/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44260 2023-07-08 09:55:21.000000 telegramweb-5.5/telegram_news/template/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-07-08 09:55:21.000000 telegramweb-5.5/telegram_news/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:55:36.914713 telegramweb-5.5/telegramweb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-07-08 09:55:36.000000 telegramweb-5.5/telegramweb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-08 09:55:36.000000 telegramweb-5.5/telegramweb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 09:55:36.000000 telegramweb-5.5/telegramweb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-08 09:55:36.000000 telegramweb-5.5/telegramweb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-08 09:55:36.000000 telegramweb-5.5/telegramweb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:12:04.000000 telegramweb-5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-10 12:11:43.000000 telegramweb-5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 12:11:43.000000 telegramweb-5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-07-10 12:12:04.000000 telegramweb-5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-10 12:11:43.000000 telegramweb-5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 12:12:04.000000 telegramweb-5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-10 12:11:43.000000 telegramweb-5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:12:04.000000 telegramweb-5.6/telegram_news/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-10 12:11:43.000000 telegramweb-5.6/telegram_news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-10 12:11:43.000000 telegramweb-5.6/telegram_news/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-10 12:11:43.000000 telegramweb-5.6/telegram_news/displaypolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-10 12:11:43.000000 telegramweb-5.6/telegram_news/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 12:11:43.000000 telegramweb-5.6/telegram_news/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:12:04.000000 telegramweb-5.6/telegram_news/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-10 12:11:43.000000 telegramweb-5.6/telegram_news/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44443 2023-07-10 12:11:43.000000 telegramweb-5.6/telegram_news/template/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-07-10 12:11:43.000000 telegramweb-5.6/telegram_news/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:12:04.000000 telegramweb-5.6/telegramweb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-07-10 12:12:04.000000 telegramweb-5.6/telegramweb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-10 12:12:04.000000 telegramweb-5.6/telegramweb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:12:04.000000 telegramweb-5.6/telegramweb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 12:12:04.000000 telegramweb-5.6/telegramweb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 12:12:04.000000 telegramweb-5.6/telegramweb.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `telegramweb-5.5/LICENSE` & `telegramweb-5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `telegramweb-5.5/PKG-INFO` & `telegramweb-5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegramweb
-Version: 5.5
+Version: 5.6
 Summary: Python package for automatically fetching and pushing news by Telegram.
 Home-page: https://github.com/craziks-creator/telegram-web
 Author: craziks
 Author-email: chandrashekharpanday07@gmail.com
 License: MIT
 Description: <h1 align="center">
           <img src="https://raw.githubusercontent.com/ESWZY/telegram-news/master/docs/images/banner.png" alt="Telegram-news">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: telegramweb Version: 5.5 Summary: Python package
+Metadata-Version: 2.1 Name: telegramweb Version: 5.6 Summary: Python package
 for automatically fetching and pushing news by Telegram. Home-page: https://
 github.com/craziks-creator/telegram-web Author: craziks Author-email:
 chandrashekharpanday07@gmail.com License: MIT Description:
                             ****** [Telegram-news]
                                  Telegram-news
                                      ******
   Python package for automatically fetching and pushing news by Telegram. [!
```

### Comparing `telegramweb-5.5/README.md` & `telegramweb-5.6/README.md`

 * *Files identical despite different names*

### Comparing `telegramweb-5.5/setup.py` & `telegramweb-5.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ]
 
 DESCRIPTION = 'Python package for automatically fetching and pushing news by Telegram.'
 LONG_DESCRIPTION = open("README.md").read()
 
 setup(
     name='telegramweb',
-    version='5.5',
+    version='5.6',
     author='craziks',
     author_email='chandrashekharpanday07@gmail.com',
     url='https://github.com/craziks-creator/telegram-web',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

### Comparing `telegramweb-5.5/telegram_news/__init__.py` & `telegramweb-5.6/telegram_news/__init__.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.5/telegram_news/constant.py` & `telegramweb-5.6/telegram_news/constant.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.5/telegram_news/displaypolicy.py` & `telegramweb-5.6/telegram_news/displaypolicy.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.5/telegram_news/ratelimit.py` & `telegramweb-5.6/telegram_news/ratelimit.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.5/telegram_news/template/common.py` & `telegramweb-5.6/telegram_news/template/common.py`

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
-
+from telegram import InlineKeyboardButton, InlineKeyboardMarkup
 import requests
 import sqlalchemy
 from bs4 import BeautifulSoup
 
 from ..displaypolicy import (
     best_effort_display_policy,
     default_id_policy,
@@ -990,14 +990,15 @@
         if self._DEBUG:
             print(data)
         return data, method
 
     @sleep_and_retry
     @limits(calls=1, period=1)
     def _real_post(self, token, method, data):
+        data['reply_markup'] = InlineKeyboardMarkup([[InlineKeyboardButton(text="TEST_BUTTON", url="www.python.org")]])
         # https://core.telegram.org/bots/api#sendmessage
         res = requests.post('https://api.telegram.org/bot' + token + '/' + method, data, files=data['files'], proxies=self._proxies)
         return res
 
     def _post(self, item, news_id):
 
         res = None
```

### Comparing `telegramweb-5.5/telegram_news/utils.py` & `telegramweb-5.6/telegram_news/utils.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.5/telegramweb.egg-info/PKG-INFO` & `telegramweb-5.6/telegramweb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegramweb
-Version: 5.5
+Version: 5.6
 Summary: Python package for automatically fetching and pushing news by Telegram.
 Home-page: https://github.com/craziks-creator/telegram-web
 Author: craziks
 Author-email: chandrashekharpanday07@gmail.com
 License: MIT
 Description: <h1 align="center">
           <img src="https://raw.githubusercontent.com/ESWZY/telegram-news/master/docs/images/banner.png" alt="Telegram-news">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: telegramweb Version: 5.5 Summary: Python package
+Metadata-Version: 2.1 Name: telegramweb Version: 5.6 Summary: Python package
 for automatically fetching and pushing news by Telegram. Home-page: https://
 github.com/craziks-creator/telegram-web Author: craziks Author-email:
 chandrashekharpanday07@gmail.com License: MIT Description:
                             ****** [Telegram-news]
                                  Telegram-news
                                      ******
   Python package for automatically fetching and pushing news by Telegram. [!
```

