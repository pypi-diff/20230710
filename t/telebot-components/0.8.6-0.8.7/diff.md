# Comparing `tmp/telebot_components-0.8.6.tar.gz` & `tmp/telebot_components-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telebot_components-0.8.6.tar", max compression
+gzip compressed data, was "telebot_components-0.8.7.tar", max compression
```

## Comparing `telebot_components-0.8.6.tar` & `telebot_components-0.8.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    35148 2023-07-10 18:27:29.737302 telebot_components-0.8.6/LICENSE
--rw-r--r--   0        0        0     2242 2023-07-10 18:27:29.737302 telebot_components-0.8.6/README.md
--rw-r--r--   0        0        0     1619 2023-07-10 18:27:46.901545 telebot_components-0.8.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/__init__.py
--rw-r--r--   0        0        0    13083 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/broadcast/__init__.py
--rw-r--r--   0        0        0     2835 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/broadcast/message_senders.py
--rw-r--r--   0        0        0      159 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/broadcast/subscriber.py
--rw-r--r--   0        0        0        0 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/constants/__init__.py
--rw-r--r--   0        0        0    15212 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/constants/emoji.py
--rw-r--r--   0        0        0      168 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/constants/times.py
--rw-r--r--   0        0        0    54382 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/feedback/__init__.py
--rw-r--r--   0        0        0     2075 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/feedback/anti_spam.py
--rw-r--r--   0        0        0        0 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/feedback/integration/__init__.py
--rw-r--r--   0        0        0     8321 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/feedback/integration/aux_feedback_handler.py
--rw-r--r--   0        0        0     3983 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/feedback/integration/interface.py
--rw-r--r--   0        0        0    34435 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/feedback/integration/trello.py
--rw-r--r--   0        0        0      237 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/feedback/trello_integration.py
--rw-r--r--   0        0        0      493 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/feedback/types.py
--rw-r--r--   0        0        0        0 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/form/__init__.py
--rw-r--r--   0        0        0    31714 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/form/field.py
--rw-r--r--   0        0        0    18987 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/form/form.py
--rw-r--r--   0        0        0    20318 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/form/handler.py
--rw-r--r--   0        0        0        0 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/form/helpers/__init__.py
--rw-r--r--   0        0        0     7572 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/form/helpers/calendar_keyboard.py
--rw-r--r--   0        0        0        0 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/menu/__init__.py
--rw-r--r--   0        0        0    13686 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/menu/menu.py
--rw-r--r--   0        0        0        0 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/py.typed
--rw-r--r--   0        0        0        0 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/redis_utils/__init__.py
--rw-r--r--   0        0        0    10640 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/redis_utils/emulation.py
--rw-r--r--   0        0        0     6078 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/redis_utils/interface.py
--rw-r--r--   0        0        0        0 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/stores/__init__.py
--rw-r--r--   0        0        0     1825 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/stores/banned_users.py
--rw-r--r--   0        0        0     8229 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/stores/category.py
--rw-r--r--   0        0        0     9342 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/stores/forum_topics.py
--rw-r--r--   0        0        0     9845 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/stores/generic.py
--rw-r--r--   0        0        0     8298 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/stores/language.py
--rw-r--r--   0        0        0      397 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/stores/types.py
--rw-r--r--   0        0        0     3914 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/stores/user_group.py
--rw-r--r--   0        0        0      614 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/stores/utils.py
--rw-r--r--   0        0        0     8172 2023-07-10 18:27:29.745303 telebot_components-0.8.6/telebot_components/utils/__init__.py
--rw-r--r--   0        0        0     5185 2023-07-10 18:27:29.745303 telebot_components-0.8.6/telebot_components/utils/airtable.py
--rw-r--r--   0        0        0     2564 2023-07-10 18:27:29.745303 telebot_components-0.8.6/telebot_components/utils/alerts.py
--rw-r--r--   0        0        0     1257 2023-07-10 18:27:29.745303 telebot_components-0.8.6/telebot_components/utils/strings.py
--rw-r--r--   0        0        0     3395 1970-01-01 00:00:00.000000 telebot_components-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-07-10 18:44:53.743598 telebot_components-0.8.7/LICENSE
+-rw-r--r--   0        0        0     2242 2023-07-10 18:44:53.743598 telebot_components-0.8.7/README.md
+-rw-r--r--   0        0        0     1619 2023-07-10 18:45:11.043600 telebot_components-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 18:44:53.747598 telebot_components-0.8.7/telebot_components/__init__.py
+-rw-r--r--   0        0        0    13083 2023-07-10 18:44:53.747598 telebot_components-0.8.7/telebot_components/broadcast/__init__.py
+-rw-r--r--   0        0        0     2835 2023-07-10 18:44:53.747598 telebot_components-0.8.7/telebot_components/broadcast/message_senders.py
+-rw-r--r--   0        0        0      159 2023-07-10 18:44:53.747598 telebot_components-0.8.7/telebot_components/broadcast/subscriber.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:44:53.747598 telebot_components-0.8.7/telebot_components/constants/__init__.py
+-rw-r--r--   0        0        0    15212 2023-07-10 18:44:53.747598 telebot_components-0.8.7/telebot_components/constants/emoji.py
+-rw-r--r--   0        0        0      168 2023-07-10 18:44:53.747598 telebot_components-0.8.7/telebot_components/constants/times.py
+-rw-r--r--   0        0        0    54431 2023-07-10 18:44:53.747598 telebot_components-0.8.7/telebot_components/feedback/__init__.py
+-rw-r--r--   0        0        0     2075 2023-07-10 18:44:53.747598 telebot_components-0.8.7/telebot_components/feedback/anti_spam.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:44:53.747598 telebot_components-0.8.7/telebot_components/feedback/integration/__init__.py
+-rw-r--r--   0        0        0     8321 2023-07-10 18:44:53.747598 telebot_components-0.8.7/telebot_components/feedback/integration/aux_feedback_handler.py
+-rw-r--r--   0        0        0     3983 2023-07-10 18:44:53.747598 telebot_components-0.8.7/telebot_components/feedback/integration/interface.py
+-rw-r--r--   0        0        0    34435 2023-07-10 18:44:53.747598 telebot_components-0.8.7/telebot_components/feedback/integration/trello.py
+-rw-r--r--   0        0        0      237 2023-07-10 18:44:53.747598 telebot_components-0.8.7/telebot_components/feedback/trello_integration.py
+-rw-r--r--   0        0        0      493 2023-07-10 18:44:53.747598 telebot_components-0.8.7/telebot_components/feedback/types.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:44:53.747598 telebot_components-0.8.7/telebot_components/form/__init__.py
+-rw-r--r--   0        0        0    31714 2023-07-10 18:44:53.747598 telebot_components-0.8.7/telebot_components/form/field.py
+-rw-r--r--   0        0        0    18987 2023-07-10 18:44:53.747598 telebot_components-0.8.7/telebot_components/form/form.py
+-rw-r--r--   0        0        0    20318 2023-07-10 18:44:53.747598 telebot_components-0.8.7/telebot_components/form/handler.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:44:53.747598 telebot_components-0.8.7/telebot_components/form/helpers/__init__.py
+-rw-r--r--   0        0        0     7572 2023-07-10 18:44:53.747598 telebot_components-0.8.7/telebot_components/form/helpers/calendar_keyboard.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:44:53.751598 telebot_components-0.8.7/telebot_components/menu/__init__.py
+-rw-r--r--   0        0        0    13686 2023-07-10 18:44:53.751598 telebot_components-0.8.7/telebot_components/menu/menu.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:44:53.751598 telebot_components-0.8.7/telebot_components/py.typed
+-rw-r--r--   0        0        0        0 2023-07-10 18:44:53.751598 telebot_components-0.8.7/telebot_components/redis_utils/__init__.py
+-rw-r--r--   0        0        0    10640 2023-07-10 18:44:53.751598 telebot_components-0.8.7/telebot_components/redis_utils/emulation.py
+-rw-r--r--   0        0        0     6078 2023-07-10 18:44:53.751598 telebot_components-0.8.7/telebot_components/redis_utils/interface.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:44:53.751598 telebot_components-0.8.7/telebot_components/stores/__init__.py
+-rw-r--r--   0        0        0     1825 2023-07-10 18:44:53.751598 telebot_components-0.8.7/telebot_components/stores/banned_users.py
+-rw-r--r--   0        0        0     8229 2023-07-10 18:44:53.751598 telebot_components-0.8.7/telebot_components/stores/category.py
+-rw-r--r--   0        0        0     9342 2023-07-10 18:44:53.751598 telebot_components-0.8.7/telebot_components/stores/forum_topics.py
+-rw-r--r--   0        0        0     9845 2023-07-10 18:44:53.751598 telebot_components-0.8.7/telebot_components/stores/generic.py
+-rw-r--r--   0        0        0     8298 2023-07-10 18:44:53.751598 telebot_components-0.8.7/telebot_components/stores/language.py
+-rw-r--r--   0        0        0      397 2023-07-10 18:44:53.751598 telebot_components-0.8.7/telebot_components/stores/types.py
+-rw-r--r--   0        0        0     3914 2023-07-10 18:44:53.751598 telebot_components-0.8.7/telebot_components/stores/user_group.py
+-rw-r--r--   0        0        0      614 2023-07-10 18:44:53.751598 telebot_components-0.8.7/telebot_components/stores/utils.py
+-rw-r--r--   0        0        0     8172 2023-07-10 18:44:53.751598 telebot_components-0.8.7/telebot_components/utils/__init__.py
+-rw-r--r--   0        0        0     5185 2023-07-10 18:44:53.751598 telebot_components-0.8.7/telebot_components/utils/airtable.py
+-rw-r--r--   0        0        0     2564 2023-07-10 18:44:53.751598 telebot_components-0.8.7/telebot_components/utils/alerts.py
+-rw-r--r--   0        0        0     1257 2023-07-10 18:44:53.751598 telebot_components-0.8.7/telebot_components/utils/strings.py
+-rw-r--r--   0        0        0     3395 1970-01-01 00:00:00.000000 telebot_components-0.8.7/PKG-INFO
```

### Comparing `telebot_components-0.8.6/LICENSE` & `telebot_components-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/README.md` & `telebot_components-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/pyproject.toml` & `telebot_components-0.8.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "telebot-components"
-version = "0.8.6"
+version = "0.8.7"
 description = "Framework/toolkit for building Telegram bots with telebot and redis"
 authors = ["Igor Vaiman <gosha.vaiman@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/bots-against-war/telebot-components"
 packages = [{include = "telebot_components"}]
```

### Comparing `telebot_components-0.8.6/telebot_components/broadcast/__init__.py` & `telebot_components-0.8.7/telebot_components/broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/broadcast/message_senders.py` & `telebot_components-0.8.7/telebot_components/broadcast/message_senders.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/constants/emoji.py` & `telebot_components-0.8.7/telebot_components/constants/emoji.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/feedback/__init__.py` & `telebot_components-0.8.7/telebot_components/feedback/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -493,14 +493,16 @@
         """Human readable identifier for the user (not to be confused with user id)"""
         if self.config.user_anonymization is UserAnonymization.FULL:
             return self.config.user_id_hash_func(user.id, self.bot_prefix)
         elif self.config.user_anonymization is UserAnonymization.NONE:
             user_identifier = user.full_name
             if user.username:
                 user_identifier += " @" + user.username
+            user_identifier += f" (#{user.id})"
+
             if not support_html:
                 return user_identifier
             else:
                 return html_link(href=f"tg://user?id={user.id}", text=user_identifier)
         elif self.config.user_anonymization is UserAnonymization.LEGACY:
             return user.full_name  # it's shown on message forward anyway
```

### Comparing `telebot_components-0.8.6/telebot_components/feedback/anti_spam.py` & `telebot_components-0.8.7/telebot_components/feedback/anti_spam.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/feedback/integration/aux_feedback_handler.py` & `telebot_components-0.8.7/telebot_components/feedback/integration/aux_feedback_handler.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/feedback/integration/interface.py` & `telebot_components-0.8.7/telebot_components/feedback/integration/interface.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/feedback/integration/trello.py` & `telebot_components-0.8.7/telebot_components/feedback/integration/trello.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/form/field.py` & `telebot_components-0.8.7/telebot_components/form/field.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/form/form.py` & `telebot_components-0.8.7/telebot_components/form/form.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/form/handler.py` & `telebot_components-0.8.7/telebot_components/form/handler.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/form/helpers/calendar_keyboard.py` & `telebot_components-0.8.7/telebot_components/form/helpers/calendar_keyboard.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/menu/menu.py` & `telebot_components-0.8.7/telebot_components/menu/menu.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/redis_utils/emulation.py` & `telebot_components-0.8.7/telebot_components/redis_utils/emulation.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/redis_utils/interface.py` & `telebot_components-0.8.7/telebot_components/redis_utils/interface.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/stores/banned_users.py` & `telebot_components-0.8.7/telebot_components/stores/banned_users.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/stores/category.py` & `telebot_components-0.8.7/telebot_components/stores/category.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/stores/forum_topics.py` & `telebot_components-0.8.7/telebot_components/stores/forum_topics.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/stores/generic.py` & `telebot_components-0.8.7/telebot_components/stores/generic.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/stores/language.py` & `telebot_components-0.8.7/telebot_components/stores/language.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/stores/user_group.py` & `telebot_components-0.8.7/telebot_components/stores/user_group.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/stores/utils.py` & `telebot_components-0.8.7/telebot_components/stores/utils.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/utils/__init__.py` & `telebot_components-0.8.7/telebot_components/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/utils/airtable.py` & `telebot_components-0.8.7/telebot_components/utils/airtable.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/utils/alerts.py` & `telebot_components-0.8.7/telebot_components/utils/alerts.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/telebot_components/utils/strings.py` & `telebot_components-0.8.7/telebot_components/utils/strings.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.6/PKG-INFO` & `telebot_components-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telebot-components
-Version: 0.8.6
+Version: 0.8.7
 Summary: Framework/toolkit for building Telegram bots with telebot and redis
 Home-page: https://github.com/bots-against-war/telebot-components
 License: GPLv3
 Author: Igor Vaiman
 Author-email: gosha.vaiman@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

