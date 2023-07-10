# Comparing `tmp/telegramweb-6.6.tar.gz` & `tmp/telegramweb-6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegramweb-6.6.tar", last modified: Mon Jul 10 17:55:18 2023, max compression
+gzip compressed data, was "telegramweb-6.7.tar", last modified: Mon Jul 10 18:01:58 2023, max compression
```

## Comparing `telegramweb-6.6.tar` & `telegramweb-6.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:55:18.134537 telegramweb-6.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-10 17:54:56.000000 telegramweb-6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 17:54:56.000000 telegramweb-6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-07-10 17:55:18.134537 telegramweb-6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-10 17:54:56.000000 telegramweb-6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 17:55:18.134537 telegramweb-6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-10 17:54:56.000000 telegramweb-6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:55:18.134537 telegramweb-6.6/telegram_news/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-10 17:54:56.000000 telegramweb-6.6/telegram_news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-10 17:54:56.000000 telegramweb-6.6/telegram_news/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-10 17:54:56.000000 telegramweb-6.6/telegram_news/displaypolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-10 17:54:56.000000 telegramweb-6.6/telegram_news/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 17:54:56.000000 telegramweb-6.6/telegram_news/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:55:18.134537 telegramweb-6.6/telegram_news/template/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-10 17:54:56.000000 telegramweb-6.6/telegram_news/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44443 2023-07-10 17:54:56.000000 telegramweb-6.6/telegram_news/template/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-07-10 17:54:56.000000 telegramweb-6.6/telegram_news/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:55:18.134537 telegramweb-6.6/telegramweb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-07-10 17:55:18.000000 telegramweb-6.6/telegramweb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-10 17:55:18.000000 telegramweb-6.6/telegramweb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 17:55:18.000000 telegramweb-6.6/telegramweb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 17:55:18.000000 telegramweb-6.6/telegramweb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 17:55:18.000000 telegramweb-6.6/telegramweb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:01:58.476196 telegramweb-6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-10 18:01:36.000000 telegramweb-6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 18:01:36.000000 telegramweb-6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-07-10 18:01:58.476196 telegramweb-6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-10 18:01:36.000000 telegramweb-6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:01:58.476196 telegramweb-6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-10 18:01:36.000000 telegramweb-6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:01:58.472196 telegramweb-6.7/telegram_news/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-10 18:01:36.000000 telegramweb-6.7/telegram_news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-10 18:01:36.000000 telegramweb-6.7/telegram_news/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-10 18:01:36.000000 telegramweb-6.7/telegram_news/displaypolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-10 18:01:36.000000 telegramweb-6.7/telegram_news/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 18:01:36.000000 telegramweb-6.7/telegram_news/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:01:58.472196 telegramweb-6.7/telegram_news/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-10 18:01:36.000000 telegramweb-6.7/telegram_news/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44563 2023-07-10 18:01:36.000000 telegramweb-6.7/telegram_news/template/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-07-10 18:01:36.000000 telegramweb-6.7/telegram_news/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:01:58.476196 telegramweb-6.7/telegramweb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-07-10 18:01:58.000000 telegramweb-6.7/telegramweb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-10 18:01:58.000000 telegramweb-6.7/telegramweb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:01:58.000000 telegramweb-6.7/telegramweb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 18:01:58.000000 telegramweb-6.7/telegramweb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 18:01:58.000000 telegramweb-6.7/telegramweb.egg-info/top_level.txt
```

### Comparing `telegramweb-6.6/LICENSE` & `telegramweb-6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `telegramweb-6.6/PKG-INFO` & `telegramweb-6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegramweb
-Version: 6.6
+Version: 6.7
 Summary: Python package for automatically fetching and pushing news by Telegram.
 Home-page: https://github.com/craziks-creator/telegram-web
 Author: craziks
 Author-email: chandrashekharpanday07@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `telegramweb-6.6/README.md` & `telegramweb-6.7/README.md`

 * *Files identical despite different names*

### Comparing `telegramweb-6.6/setup.py` & `telegramweb-6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ]
 
 DESCRIPTION = 'Python package for automatically fetching and pushing news by Telegram.'
 LONG_DESCRIPTION = open("README.md").read()
 
 setup(
     name='telegramweb',
-    version='6.6',
+    version='6.7',
     author='craziks',
     author_email='chandrashekharpanday07@gmail.com',
     url='https://github.com/craziks-creator/telegram-web',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

### Comparing `telegramweb-6.6/telegram_news/__init__.py` & `telegramweb-6.7/telegram_news/__init__.py`

 * *Files identical despite different names*

### Comparing `telegramweb-6.6/telegram_news/constant.py` & `telegramweb-6.7/telegram_news/constant.py`

 * *Files identical despite different names*

### Comparing `telegramweb-6.6/telegram_news/displaypolicy.py` & `telegramweb-6.7/telegram_news/displaypolicy.py`

 * *Files identical despite different names*

### Comparing `telegramweb-6.6/telegram_news/ratelimit.py` & `telegramweb-6.7/telegram_news/ratelimit.py`

 * *Files identical despite different names*

### Comparing `telegramweb-6.6/telegram_news/template/common.py` & `telegramweb-6.7/telegram_news/template/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -991,14 +991,15 @@
             print(data)
         return data, method
 
     @sleep_and_retry
     @limits(calls=1, period=1)
     def _real_post(self, token, method, data):
         #data['reply_markup'] = InlineKeyboardMarkup([[InlineKeyboardButton(text="CLICK HERE", url="www.google.com")]])
+        data['reply_markup'] = InlineKeyboardMarkup([[InlineKeyboardButton(text="TEST_BUTTON", url="www.ssc.nic.in")]])
         # https://core.telegram.org/bots/api#sendmessage
         res = requests.post('https://api.telegram.org/bot' + token + '/' + method, data, files=data['files'], proxies=self._proxies)
         return res
 
     def _post(self, item, news_id):
 
         res = None
```

### Comparing `telegramweb-6.6/telegram_news/utils.py` & `telegramweb-6.7/telegram_news/utils.py`

 * *Files identical despite different names*

### Comparing `telegramweb-6.6/telegramweb.egg-info/PKG-INFO` & `telegramweb-6.7/telegramweb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegramweb
-Version: 6.6
+Version: 6.7
 Summary: Python package for automatically fetching and pushing news by Telegram.
 Home-page: https://github.com/craziks-creator/telegram-web
 Author: craziks
 Author-email: chandrashekharpanday07@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

