# Comparing `tmp/telegramweb-5.8.tar.gz` & `tmp/telegramweb-5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegramweb-5.8.tar", last modified: Mon Jul 10 12:52:32 2023, max compression
+gzip compressed data, was "telegramweb-5.9.tar", last modified: Mon Jul 10 14:02:41 2023, max compression
```

## Comparing `telegramweb-5.8.tar` & `telegramweb-5.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:52:32.167474 telegramweb-5.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-10 12:52:11.000000 telegramweb-5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 12:52:11.000000 telegramweb-5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-07-10 12:52:32.167474 telegramweb-5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-10 12:52:11.000000 telegramweb-5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 12:52:32.167474 telegramweb-5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-10 12:52:11.000000 telegramweb-5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:52:32.163474 telegramweb-5.8/telegram_news/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-10 12:52:11.000000 telegramweb-5.8/telegram_news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-10 12:52:11.000000 telegramweb-5.8/telegram_news/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-10 12:52:11.000000 telegramweb-5.8/telegram_news/displaypolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-10 12:52:11.000000 telegramweb-5.8/telegram_news/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 12:52:11.000000 telegramweb-5.8/telegram_news/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:52:32.167474 telegramweb-5.8/telegram_news/template/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-10 12:52:11.000000 telegramweb-5.8/telegram_news/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44443 2023-07-10 12:52:11.000000 telegramweb-5.8/telegram_news/template/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-07-10 12:52:11.000000 telegramweb-5.8/telegram_news/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:52:32.167474 telegramweb-5.8/telegramweb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-07-10 12:52:32.000000 telegramweb-5.8/telegramweb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-10 12:52:32.000000 telegramweb-5.8/telegramweb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:52:32.000000 telegramweb-5.8/telegramweb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 12:52:32.000000 telegramweb-5.8/telegramweb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 12:52:32.000000 telegramweb-5.8/telegramweb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:02:41.058008 telegramweb-5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-10 14:02:20.000000 telegramweb-5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 14:02:20.000000 telegramweb-5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-07-10 14:02:41.058008 telegramweb-5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-10 14:02:20.000000 telegramweb-5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 14:02:41.058008 telegramweb-5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-10 14:02:20.000000 telegramweb-5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:02:41.054008 telegramweb-5.9/telegram_news/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-10 14:02:20.000000 telegramweb-5.9/telegram_news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-10 14:02:20.000000 telegramweb-5.9/telegram_news/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-10 14:02:20.000000 telegramweb-5.9/telegram_news/displaypolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-10 14:02:20.000000 telegramweb-5.9/telegram_news/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 14:02:20.000000 telegramweb-5.9/telegram_news/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:02:41.054008 telegramweb-5.9/telegram_news/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-10 14:02:20.000000 telegramweb-5.9/telegram_news/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44444 2023-07-10 14:02:20.000000 telegramweb-5.9/telegram_news/template/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-07-10 14:02:20.000000 telegramweb-5.9/telegram_news/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:02:41.054008 telegramweb-5.9/telegramweb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-07-10 14:02:41.000000 telegramweb-5.9/telegramweb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-10 14:02:41.000000 telegramweb-5.9/telegramweb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:02:41.000000 telegramweb-5.9/telegramweb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 14:02:41.000000 telegramweb-5.9/telegramweb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 14:02:41.000000 telegramweb-5.9/telegramweb.egg-info/top_level.txt
```

### Comparing `telegramweb-5.8/LICENSE` & `telegramweb-5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `telegramweb-5.8/PKG-INFO` & `telegramweb-5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegramweb
-Version: 5.8
+Version: 5.9
 Summary: Python package for automatically fetching and pushing news by Telegram.
 Home-page: https://github.com/craziks-creator/telegram-web
 Author: craziks
 Author-email: chandrashekharpanday07@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `telegramweb-5.8/README.md` & `telegramweb-5.9/README.md`

 * *Files identical despite different names*

### Comparing `telegramweb-5.8/setup.py` & `telegramweb-5.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ]
 
 DESCRIPTION = 'Python package for automatically fetching and pushing news by Telegram.'
 LONG_DESCRIPTION = open("README.md").read()
 
 setup(
     name='telegramweb',
-    version='5.8',
+    version='5.9',
     author='craziks',
     author_email='chandrashekharpanday07@gmail.com',
     url='https://github.com/craziks-creator/telegram-web',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

### Comparing `telegramweb-5.8/telegram_news/__init__.py` & `telegramweb-5.9/telegram_news/__init__.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.8/telegram_news/constant.py` & `telegramweb-5.9/telegram_news/constant.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.8/telegram_news/displaypolicy.py` & `telegramweb-5.9/telegram_news/displaypolicy.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 Display policies and id policies for different situation.
 
 Add new ones when possible.
 """
 
 import re
-
+from telegram import InlineKeyboardButton, InlineKeyboardMarkup
 
 MAXLEN = 4096
 
 
 def default_policy(item, max_len=1000, max_par_num=40):
     """
     Generate formatted message from item, the default way.
@@ -63,15 +63,16 @@
 
     if len(po) > MAXLEN:
         return "Too long message!\n" + item['id'], parse_mode, disable_web_page_preview
 
     return {
         'text': po,
         'parse_mode': parse_mode,
-        'disable_web_page_preview': disable_web_page_preview
+        'disable_web_page_preview': disable_web_page_preview,
+        'reply_markup': InlineKeyboardMarkup([[InlineKeyboardButton(text=item['id'], url=item['link'])]])
     }
 
 
 def best_effort_display_policy(item, max_len=1000, max_par_num=40, suffix='...'):
     """
     Display as more paragraphs as possible.
     If over max_len, end with suffix.
@@ -131,15 +132,16 @@
 
     if len(po) > 4096:
         return "Too long message!\n" + item['id'], parse_mode, disable_web_page_preview
 
     return {
         'text': po,
         'parse_mode': parse_mode,
-        'disable_web_page_preview': disable_web_page_preview
+        'disable_web_page_preview': disable_web_page_preview,
+        'reply_markup': InlineKeyboardMarkup([[InlineKeyboardButton(text=item['id'], url=item['link'])]])
     }
 
 
 def default_id_policy(self, link):
     """
     Generate id from link, the default way.
```

### Comparing `telegramweb-5.8/telegram_news/ratelimit.py` & `telegramweb-5.9/telegram_news/ratelimit.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.8/telegram_news/template/common.py` & `telegramweb-5.9/telegram_news/template/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -990,15 +990,15 @@
         if self._DEBUG:
             print(data)
         return data, method
 
     @sleep_and_retry
     @limits(calls=1, period=1)
     def _real_post(self, token, method, data):
-        data['reply_markup'] = InlineKeyboardMarkup([[InlineKeyboardButton(text="TEST_BUTTON", url="www.python.org")]])
+        #data['reply_markup'] = InlineKeyboardMarkup([[InlineKeyboardButton(text="TEST_BUTTON", url="www.python.org")]])
         # https://core.telegram.org/bots/api#sendmessage
         res = requests.post('https://api.telegram.org/bot' + token + '/' + method, data, files=data['files'], proxies=self._proxies)
         return res
 
     def _post(self, item, news_id):
 
         res = None
```

### Comparing `telegramweb-5.8/telegram_news/utils.py` & `telegramweb-5.9/telegram_news/utils.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.8/telegramweb.egg-info/PKG-INFO` & `telegramweb-5.9/telegramweb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegramweb
-Version: 5.8
+Version: 5.9
 Summary: Python package for automatically fetching and pushing news by Telegram.
 Home-page: https://github.com/craziks-creator/telegram-web
 Author: craziks
 Author-email: chandrashekharpanday07@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

