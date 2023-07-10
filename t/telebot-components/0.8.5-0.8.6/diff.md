# Comparing `tmp/telebot_components-0.8.5.tar.gz` & `tmp/telebot_components-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telebot_components-0.8.5.tar", max compression
+gzip compressed data, was "telebot_components-0.8.6.tar", max compression
```

## Comparing `telebot_components-0.8.5.tar` & `telebot_components-0.8.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    35148 2023-07-10 15:12:36.186927 telebot_components-0.8.5/LICENSE
--rw-r--r--   0        0        0     2242 2023-07-10 15:12:36.186927 telebot_components-0.8.5/README.md
--rw-r--r--   0        0        0     1619 2023-07-10 15:12:57.572719 telebot_components-0.8.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 15:12:36.186927 telebot_components-0.8.5/telebot_components/__init__.py
--rw-r--r--   0        0        0    13083 2023-07-10 15:12:36.186927 telebot_components-0.8.5/telebot_components/broadcast/__init__.py
--rw-r--r--   0        0        0     2835 2023-07-10 15:12:36.186927 telebot_components-0.8.5/telebot_components/broadcast/message_senders.py
--rw-r--r--   0        0        0      159 2023-07-10 15:12:36.186927 telebot_components-0.8.5/telebot_components/broadcast/subscriber.py
--rw-r--r--   0        0        0        0 2023-07-10 15:12:36.186927 telebot_components-0.8.5/telebot_components/constants/__init__.py
--rw-r--r--   0        0        0    15212 2023-07-10 15:12:36.186927 telebot_components-0.8.5/telebot_components/constants/emoji.py
--rw-r--r--   0        0        0      168 2023-07-10 15:12:36.186927 telebot_components-0.8.5/telebot_components/constants/times.py
--rw-r--r--   0        0        0    50254 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/feedback/__init__.py
--rw-r--r--   0        0        0     2075 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/feedback/anti_spam.py
--rw-r--r--   0        0        0        0 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/feedback/integration/__init__.py
--rw-r--r--   0        0        0     8255 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/feedback/integration/aux_feedback_handler.py
--rw-r--r--   0        0        0     3983 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/feedback/integration/interface.py
--rw-r--r--   0        0        0    34435 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/feedback/integration/trello.py
--rw-r--r--   0        0        0      237 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/feedback/trello_integration.py
--rw-r--r--   0        0        0      493 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/feedback/types.py
--rw-r--r--   0        0        0        0 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/form/__init__.py
--rw-r--r--   0        0        0    31714 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/form/field.py
--rw-r--r--   0        0        0    18987 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/form/form.py
--rw-r--r--   0        0        0    20318 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/form/handler.py
--rw-r--r--   0        0        0        0 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/form/helpers/__init__.py
--rw-r--r--   0        0        0     7572 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/form/helpers/calendar_keyboard.py
--rw-r--r--   0        0        0        0 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/menu/__init__.py
--rw-r--r--   0        0        0    13686 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/menu/menu.py
--rw-r--r--   0        0        0        0 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/py.typed
--rw-r--r--   0        0        0        0 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/redis_utils/__init__.py
--rw-r--r--   0        0        0    10640 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/redis_utils/emulation.py
--rw-r--r--   0        0        0     6078 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/redis_utils/interface.py
--rw-r--r--   0        0        0        0 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/stores/__init__.py
--rw-r--r--   0        0        0     1825 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/stores/banned_users.py
--rw-r--r--   0        0        0     8229 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/stores/category.py
--rw-r--r--   0        0        0     9342 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/stores/forum_topics.py
--rw-r--r--   0        0        0     9845 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/stores/generic.py
--rw-r--r--   0        0        0     8298 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/stores/language.py
--rw-r--r--   0        0        0      397 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/stores/types.py
--rw-r--r--   0        0        0     3914 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/stores/user_group.py
--rw-r--r--   0        0        0      614 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/stores/utils.py
--rw-r--r--   0        0        0     8134 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/utils/__init__.py
--rw-r--r--   0        0        0     5185 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/utils/airtable.py
--rw-r--r--   0        0        0     2564 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/utils/alerts.py
--rw-r--r--   0        0        0     1257 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/utils/strings.py
--rw-r--r--   0        0        0     3395 1970-01-01 00:00:00.000000 telebot_components-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-07-10 18:27:29.737302 telebot_components-0.8.6/LICENSE
+-rw-r--r--   0        0        0     2242 2023-07-10 18:27:29.737302 telebot_components-0.8.6/README.md
+-rw-r--r--   0        0        0     1619 2023-07-10 18:27:46.901545 telebot_components-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/__init__.py
+-rw-r--r--   0        0        0    13083 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/broadcast/__init__.py
+-rw-r--r--   0        0        0     2835 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/broadcast/message_senders.py
+-rw-r--r--   0        0        0      159 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/broadcast/subscriber.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/constants/__init__.py
+-rw-r--r--   0        0        0    15212 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/constants/emoji.py
+-rw-r--r--   0        0        0      168 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/constants/times.py
+-rw-r--r--   0        0        0    54382 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/feedback/__init__.py
+-rw-r--r--   0        0        0     2075 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/feedback/anti_spam.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/feedback/integration/__init__.py
+-rw-r--r--   0        0        0     8321 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/feedback/integration/aux_feedback_handler.py
+-rw-r--r--   0        0        0     3983 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/feedback/integration/interface.py
+-rw-r--r--   0        0        0    34435 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/feedback/integration/trello.py
+-rw-r--r--   0        0        0      237 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/feedback/trello_integration.py
+-rw-r--r--   0        0        0      493 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/feedback/types.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/form/__init__.py
+-rw-r--r--   0        0        0    31714 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/form/field.py
+-rw-r--r--   0        0        0    18987 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/form/form.py
+-rw-r--r--   0        0        0    20318 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/form/handler.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/form/helpers/__init__.py
+-rw-r--r--   0        0        0     7572 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/form/helpers/calendar_keyboard.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/menu/__init__.py
+-rw-r--r--   0        0        0    13686 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/menu/menu.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/py.typed
+-rw-r--r--   0        0        0        0 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/redis_utils/__init__.py
+-rw-r--r--   0        0        0    10640 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/redis_utils/emulation.py
+-rw-r--r--   0        0        0     6078 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/redis_utils/interface.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/stores/__init__.py
+-rw-r--r--   0        0        0     1825 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/stores/banned_users.py
+-rw-r--r--   0        0        0     8229 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/stores/category.py
+-rw-r--r--   0        0        0     9342 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/stores/forum_topics.py
+-rw-r--r--   0        0        0     9845 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/stores/generic.py
+-rw-r--r--   0        0        0     8298 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/stores/language.py
+-rw-r--r--   0        0        0      397 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/stores/types.py
+-rw-r--r--   0        0        0     3914 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/stores/user_group.py
+-rw-r--r--   0        0        0      614 2023-07-10 18:27:29.741302 telebot_components-0.8.6/telebot_components/stores/utils.py
+-rw-r--r--   0        0        0     8172 2023-07-10 18:27:29.745303 telebot_components-0.8.6/telebot_components/utils/__init__.py
+-rw-r--r--   0        0        0     5185 2023-07-10 18:27:29.745303 telebot_components-0.8.6/telebot_components/utils/airtable.py
+-rw-r--r--   0        0        0     2564 2023-07-10 18:27:29.745303 telebot_components-0.8.6/telebot_components/utils/alerts.py
+-rw-r--r--   0        0        0     1257 2023-07-10 18:27:29.745303 telebot_components-0.8.6/telebot_components/utils/strings.py
+-rw-r--r--   0        0        0     3395 1970-01-01 00:00:00.000000 telebot_components-0.8.6/PKG-INFO
```

### Comparing `telebot_components-0.8.5/LICENSE` & `telebot_components-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/README.md` & `telebot_components-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/pyproject.toml` & `telebot_components-0.8.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "telebot-components"
-version = "0.8.5"
+version = "0.8.6"
 description = "Framework/toolkit for building Telegram bots with telebot and redis"
 authors = ["Igor Vaiman <gosha.vaiman@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/bots-against-war/telebot-components"
 packages = [{include = "telebot_components"}]
 
@@ -16,15 +16,15 @@
 enable = false
 vcs = "git"
 dirty = true
 style="semver"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-telebot-against-war = "^0.6.3"
+telebot-against-war = "^0.6.7"
 redis = "^4.3.1"
 py-trello = "^0.18.0"
 markdownify = "^0.11.2"
 pytest-mock = "^3.7.0"
 "ruamel.yaml" = "^0.17.21"
 pyairtable = "^1.5.0"
 Pillow = "^9.2.0"
```

### Comparing `telebot_components-0.8.5/telebot_components/broadcast/__init__.py` & `telebot_components-0.8.6/telebot_components/broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/broadcast/message_senders.py` & `telebot_components-0.8.6/telebot_components/broadcast/message_senders.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/constants/emoji.py` & `telebot_components-0.8.6/telebot_components/constants/emoji.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/feedback/__init__.py` & `telebot_components-0.8.6/telebot_components/feedback/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import asyncio
 import copy
 import dataclasses
+import enum
 import logging
 import math
 import random
+import warnings
 from collections.abc import Awaitable
 from dataclasses import dataclass
 from datetime import timedelta
 from typing import Any, Callable, Coroutine, Optional, Protocol, TypedDict, cast
 
 from telebot import AsyncTeleBot
 from telebot import types as tg
@@ -109,14 +111,27 @@
 @dataclass
 class AdminChatAction:
     command: str
     callback: AdminChatActionCallback
     delete_everything_related_to_user_after: bool = False
 
 
+class UserAnonymization(enum.Enum):
+    # name, username and user id are shown to admins
+    NONE = enum.auto()
+
+    # legacy option
+    # nothing is shown intentionally, but message forwarding mechanism is used,
+    # which gives a link to user profile unless they opted in to anonymize it
+    LEGACY = enum.auto()
+
+    # admins only see anonymized identifier for the user
+    FULL = enum.auto()
+
+
 @dataclass
 class FeedbackConfig:
     # if False, message log is sent to PM with the admin that has invoked the '/log' cmd
     message_log_to_admin_chat: bool
 
     # if True, user's messages are not forwarded until they select a category
     force_category_selection: bool
@@ -138,29 +153,42 @@
     custom_user_message_filter: Optional[Callable[[tg.Message], Coroutine[None, None, bool]]] = None
     before_forwarding: Optional[Callable[[tg.User], Coroutine[None, None, Optional[tg.Message]]]] = None
     after_forwarding: Optional[Callable[[tg.User], Coroutine[None, None, Optional[tg.Message]]]] = None
 
     # appended to admin chat help under "Other" section; Supports HTML markup
     admin_chat_help_extra: Optional[str] = None
 
+    # LEGACY OPTION
     # if True, user messages are not forwarded but copied to admin chat without any back
     # link to the user account; before the message, user id hash is sent for identification
     full_user_anonymization: bool = False
 
+    user_anonymization: UserAnonymization = UserAnonymization.LEGACY
+
     # (user id, bot prefix) -> unique string identifying the user
     # used to generate user id hash for a particular bot;
     user_id_hash_func: Callable[[int, str], str] = emoji_hash
 
     # how many messages to forward in one go on /log command
     message_log_page_size: int = 30
 
     # [⚠️ experimental] create new forum topic per new user
     forum_topic_per_user: bool = False
 
-    user_forum_topic_lifetime: timedelta = timedelta(days=7)
+    # if set, admins can reply to users by just writing to their topic, no need to use Telegram message reply
+    any_message_in_user_topic_is_reply: bool = True
+
+    user_forum_topic_lifetime: timedelta = timedelta(days=30)
+
+    def __post_init__(self):
+        if self.full_user_anonymization:
+            warnings.warn(
+                "full_user_anonymization argument is deprecated, use user_anonymization=UserAnonymization.FULL"
+            )
+            self.user_anonymization = UserAnonymization.FULL
 
 
 @dataclasses.dataclass
 class MessageForwarderResult:
     admin_chat_msg: tg.Message
     user_msg: Optional[tg.Message]
 
@@ -299,32 +327,40 @@
             name="copied-to-user-ok",
             prefix=bot_prefix,
             redis=redis,
             expiration_time=times.FIVE_MINUTES,
         )
 
         # const key -> last sent user id hash to avoid repeating it on multiple consequtive messages
-        self.last_sent_user_id_hash_store = KeyValueStore[str](
+        self.last_sent_user_identifier_store = KeyValueStore[str](
             name="last-sent-user-id-hash",
             prefix=bot_prefix,
             redis=redis,
             expiration_time=timedelta(hours=12),
             loader=str,
             dumper=str,
         )
 
-        # message
+        # if forum_topic_per_user option is used
         self.message_thread_id_by_user_id_store = KeyValueStore[int](
             name="message-thread-id-by-user",
             prefix=bot_prefix,
             redis=redis,
             expiration_time=self.config.user_forum_topic_lifetime,
             loader=int,
             dumper=str,
         )
+        self.last_forwarded_message_id_by_message_thread_id = KeyValueStore[int](
+            name="last-fwd-msg-id-in-thread",
+            prefix=bot_prefix,
+            redis=redis,
+            expiration_time=self.config.user_forum_topic_lifetime,
+            loader=int,
+            dumper=str,
+        )
 
     @property
     def bot(self) -> AsyncTeleBot:
         if self._bot is None:
             raise RuntimeError("Bot was not initialized")
         return self._bot
 
@@ -347,37 +383,45 @@
 
     async def _ban_admin_chat_action(
         self, admin_message: tg.Message, forwarded_message: tg.Message, origin_chat_id: int
     ):
         if self.banned_users_store is not None:
             await self.banned_users_store.ban_user(origin_chat_id)
 
-    async def save_message_from_user(self, author: tg.User, forwarded_message_id: int):
+    async def save_message_from_user(
+        self, author: tg.User, forwarded_message_id: int, message_thread_id: Optional[int]
+    ):
         origin_chat_id = author.id
         await self.origin_chat_id_store.save(forwarded_message_id, origin_chat_id)
         await self.user_related_messages_store.add(origin_chat_id, forwarded_message_id, reset_ttl=True)
         await self.message_log_store.push(origin_chat_id, forwarded_message_id, reset_ttl=True)
+        if message_thread_id is not None:
+            await self.last_forwarded_message_id_by_message_thread_id.save(message_thread_id, forwarded_message_id)
 
     def _admin_help_message(self) -> str:
         paragraphs = [
             "<b>Справка-памятка для админского чата</b>",
             "<i>Сообщение сгенерировано автоматически по команде /help</i>",
         ]
-        copies_or_forwards = "пересылает" if not self.config.full_user_anonymization else "копирует"
+        copies_or_forwards = "пересылает" if self.config.user_anonymization is UserAnonymization.LEGACY else "копирует"
         paragraphs.append(
             "💬 <i>Основное</i>\n"
             + f"· В этот чат бот {copies_or_forwards} все сообщения (кроме специальных случаев вроде /команд), "
             + "которые ему пишут в личку.\n"
             + (
                 (
                     "· Перед скопированным сообщением бот указывает анонимизированный идентификатор пользователь_ницы, "
                     + f"например такой: «{self.config.user_id_hash_func(random.randint(1, 1000), self.bot_prefix)}»\n"
                 )
-                if self.config.full_user_anonymization
-                else ""
+                if self.config.user_anonymization is UserAnonymization.FULL
+                else (
+                    "· Перед скопированным сообщением бот указывает имя и юзернейм пользователь_ницы"
+                    if self.config.user_anonymization is UserAnonymization.NONE
+                    else ""
+                )
             )
             + "· Если в этом чате ответить на сообщение, бот скопирует ответ в чат с пользователь_ницей.\n"
             + "· Чтобы отменить отправку сообщения пользователь_нице - отправьте реплай с командой /undo на ваше "
             + "сообщение или на подтверждение отправки бота (доступно в течение 5 минут)"
         )
         if self.category_store is not None:
             categories_help = (
@@ -441,21 +485,36 @@
 
     async def _user_message_filter(self, message: tg.Message) -> bool:
         if self.config.custom_user_message_filter is not None:
             return await self.config.custom_user_message_filter(message)
         else:
             return True
 
+    def user_identifier(self, user: tg.User, support_html: bool) -> str:
+        """Human readable identifier for the user (not to be confused with user id)"""
+        if self.config.user_anonymization is UserAnonymization.FULL:
+            return self.config.user_id_hash_func(user.id, self.bot_prefix)
+        elif self.config.user_anonymization is UserAnonymization.NONE:
+            user_identifier = user.full_name
+            if user.username:
+                user_identifier += " @" + user.username
+            if not support_html:
+                return user_identifier
+            else:
+                return html_link(href=f"tg://user?id={user.id}", text=user_identifier)
+        elif self.config.user_anonymization is UserAnonymization.LEGACY:
+            return user.full_name  # it's shown on message forward anyway
+
     async def _handle_user_message(
         self,
         bot: AsyncTeleBot,
         user: tg.User,
         message_forwarder: Callable[[Optional[int]], Awaitable[MessageForwarderResult]],
         user_replier: Callable[[str, Optional[tg.ReplyMarkup]], Coroutine[None, None, Any]],
-        send_user_id_hash: bool,
+        send_user_identifier: bool,
         export_to_integrations: bool = True,
     ) -> Optional[int]:
         if self.banned_users_store is not None and await self.banned_users_store.is_banned(user.id):
             return None
         anti_spam_status = await self.anti_spam.status(user)
         if anti_spam_status is AntiSpamStatus.SOFT_BAN:
             return None
@@ -474,20 +533,16 @@
             message_thread_id: Optional[int] = await self.forum_topic_store.get_message_thread_id(category)
         elif self.config.forum_topic_per_user:
             message_thread_id = await self.message_thread_id_by_user_id_store.load(user.id)
             if message_thread_id is None:
                 try:
                     new_topic = await bot.create_forum_topic(
                         chat_id=self.admin_chat_id,
-                        name=self.config.user_id_hash_func(
-                            user.id,
-                            self.bot_prefix,
-                        ),
+                        name=self.user_identifier(user, support_html=False),
                     )
-                    # TODO: sent the topic to redis-backed queue for cleanup...
                     message_thread_id = new_topic.message_thread_id
                     await self.message_thread_id_by_user_id_store.save(user.id, message_thread_id)
                 except Exception:
                     self.logger.exception(
                         f"Error creating forum topic for user {user}, will send without message thread id"
                     )
         else:
@@ -528,41 +583,44 @@
                         _join_hashtags(hashtags),
                         message_thread_id=message_thread_id,
                     )
                     await self.user_related_messages_store.add(user.id, hashtag_msg.id, reset_ttl=False)
                     hashtag_msg_data = HashtagMessageData(message_id=hashtag_msg.id, hashtags=hashtags)
                     await self.recent_hashtag_message_for_user_store.save(user.id, hashtag_msg_data)
 
-        if send_user_id_hash and not self.config.forum_topic_per_user:
-            user_id_hash = self.config.user_id_hash_func(user.id, self.bot_prefix)
-            last_sent_user_id_hash = await self.last_sent_user_id_hash_store.load(self.CONST_KEY)
-            if last_sent_user_id_hash is None or last_sent_user_id_hash != user_id_hash:
-                user_id_hash_msg = await bot.send_message(
+        if send_user_identifier and not self.config.forum_topic_per_user:
+            user_identifier = self.user_identifier(user, support_html=True)
+            last_sent_user_identifier = await self.last_sent_user_identifier_store.load(self.CONST_KEY)
+            if last_sent_user_identifier is None or last_sent_user_identifier != user_identifier:
+                user_identifier_msg = await bot.send_message(
                     self.admin_chat_id,
-                    user_id_hash,
+                    user_identifier,
                     message_thread_id=message_thread_id,
+                    parse_mode="HTML",
                 )
-                await self.last_sent_user_id_hash_store.save(self.CONST_KEY, user_id_hash)
-                await self.save_message_from_user(user, user_id_hash_msg.id)
+                await self.last_sent_user_identifier_store.save(self.CONST_KEY, user_identifier)
+                await self.save_message_from_user(user, user_identifier_msg.id, message_thread_id=message_thread_id)
 
         preforwarded_msg = None
         if self.config.before_forwarding is not None:
             preforwarded_msg = await self.config.before_forwarding(user)
             if isinstance(preforwarded_msg, tg.Message):
-                await self.save_message_from_user(user, preforwarded_msg.id)
+                await self.save_message_from_user(user, preforwarded_msg.id, message_thread_id=message_thread_id)
 
         # admin_chat_forwarded_msg_id, user_content_message = await message_forwarder()
         message_forwarder_result = await message_forwarder(message_thread_id)
-        await self.save_message_from_user(user, message_forwarder_result.admin_chat_msg.id)
+        await self.save_message_from_user(
+            user, message_forwarder_result.admin_chat_msg.id, message_thread_id=message_thread_id
+        )
 
         postforwarded_msg = None
         if self.config.after_forwarding is not None:
             postforwarded_msg = await self.config.after_forwarding(user)
             if isinstance(postforwarded_msg, tg.Message):
-                await self.save_message_from_user(user, postforwarded_msg.id)
+                await self.save_message_from_user(user, postforwarded_msg.id, message_thread_id=message_thread_id)
 
         if self.config.hashtags_in_admin_chat and hashtag_msg_data is not None:
             await self.hashtag_message_for_forwarded_message_store.save(
                 message_forwarder_result.admin_chat_msg.id, hashtag_msg_data
             )
 
         if self.service_messages.forwarded_to_admin_ok is not None and (
@@ -605,37 +663,29 @@
                         bot=bot,
                     )
                     for integration in self.integrations
                 ]
             )
         return message_forwarder_result.admin_chat_msg.id
 
-    async def _send_user_id_hash_message(self, bot: AsyncTeleBot, user_id: int) -> Optional[int]:
-        user_id_hash = self.config.user_id_hash_func(user_id, self.bot_prefix)
-        last_sent_user_id_hash = await self.last_sent_user_id_hash_store.load(self.CONST_KEY)
-        if last_sent_user_id_hash is None or last_sent_user_id_hash != user_id_hash:
-            user_id_hash_msg = await bot.send_message(self.admin_chat_id, user_id_hash)
-            await self.last_sent_user_id_hash_store.save(self.CONST_KEY, user_id_hash)
-            return user_id_hash_msg.id
-        else:
-            return None
-
     async def emulate_user_message(
         self,
         bot: AsyncTeleBot,
         user: tg.User,
         text: str,
         attachment: Optional[TelegramAttachment] = None,
         no_response: bool = False,
         export_to_trello: bool = True,
         remove_exif_data: bool = True,
-        send_user_id_hash_message: bool = False,
+        send_user_id_hash_message: bool = False,  # DEPRECATED, USE send_user_identifier_message
+        send_user_identifier_message: bool = False,
         **send_message_kwargs,
     ) -> Optional[int]:
-        """Sometimes we want FeedbackHandler to act like the user has sent us a message, but without actually
+        """
+        Sometimes we want FeedbackHandler to act like the user has sent us a message, but without actually
         a message there (they might have pressed a button or interacted with the bot in some other way). This
         method can be used in such cases.
 
         If the message has been successfully sent to the admin chat, this method returns its id.
         """
 
         async def message_forwarder(message_thread_id: Optional[int]) -> MessageForwarderResult:
@@ -668,49 +718,49 @@
                 return await bot.send_message(user.id, text=text, reply_markup=reply_markup)
 
         return await self._handle_user_message(
             bot=bot,
             user=user,
             message_forwarder=message_forwarder,
             user_replier=user_replier,
-            send_user_id_hash=send_user_id_hash_message,
+            send_user_identifier=send_user_identifier_message or send_user_id_hash_message,
             export_to_integrations=export_to_trello,
         )
 
     async def handle_user_message(self, message: tg.Message, bot: AsyncTeleBot, reply_to_user: bool) -> Optional[int]:
         async def message_forwarder(message_thread_id: Optional[int]) -> MessageForwarderResult:
-            if self.config.full_user_anonymization:
+            if self.config.user_anonymization is UserAnonymization.LEGACY:
+                forwarded_message = await bot.forward_message(
+                    self.admin_chat_id,
+                    from_chat_id=message.chat.id,
+                    message_id=message.id,
+                    message_thread_id=message_thread_id,
+                )
+                return MessageForwarderResult(admin_chat_msg=forwarded_message, user_msg=message)
+            else:
                 copied_message_id = await bot.copy_message(
                     chat_id=self.admin_chat_id,
                     from_chat_id=message.chat.id,
                     message_id=message.id,
                     message_thread_id=message_thread_id,
                 )
                 fake_admin_chat_message = copy.deepcopy(message)
                 fake_admin_chat_message.chat = await self.admin_chat()
                 fake_admin_chat_message.id = copied_message_id.message_id
                 return MessageForwarderResult(admin_chat_msg=fake_admin_chat_message, user_msg=message)
-            else:
-                forwarded_message = await bot.forward_message(
-                    self.admin_chat_id,
-                    from_chat_id=message.chat.id,
-                    message_id=message.id,
-                    message_thread_id=message_thread_id,
-                )
-                return MessageForwarderResult(admin_chat_msg=forwarded_message, user_msg=message)
 
         async def user_replier(text: str, reply_markup: Optional[tg.ReplyMarkup]):
             if reply_to_user:
                 return await bot.reply_to(message, text, reply_markup=reply_markup)
 
         return await self._handle_user_message(
             bot=bot,
             user=message.from_user,
             message_forwarder=message_forwarder,
-            send_user_id_hash=self.config.full_user_anonymization,
+            send_user_identifier=self.config.user_anonymization is not UserAnonymization.LEGACY,
             user_replier=user_replier,
         )
 
     async def setup(self, bot: AsyncTeleBot) -> None:
         # user messages handler
         @bot.message_handler(
             func=cast(FilterFunc, self._user_message_filter),
@@ -858,29 +908,59 @@
             except Exception as e:
                 self.logger.exception("error deleting message")
                 if self.service_messages.can_not_delete_message is not None:
                     await bot.reply_to(message, self.service_messages.can_not_delete_message)
 
         @bot.message_handler(
             chat_id=[self.admin_chat_id],
-            is_reply=True,
             content_types=list(tg_constants.MediaContentType),
         )
         async def admin_to_bot(message: tg.Message):
             try:
-                forwarded_msg = message.reply_to_message
-                if forwarded_msg is None:
+                replied_to_msg = message.reply_to_message
+                if replied_to_msg is not None and replied_to_msg.forum_topic_created is None:
+                    self.logger.debug("Message in admin chat is a non-trivial reply")
+                    forwarded_msg_id = replied_to_msg.id
+                    forwarded_msg: Optional[tg.Message] = replied_to_msg
+                elif not self.config.forum_topic_per_user:
+                    self.logger.debug(
+                        "Ignoring message in admin chat: not a reply and forum topic per user not enabled"
+                    )
+                    return
+                elif not self.config.any_message_in_user_topic_is_reply:
+                    self.logger.debug(
+                        "Ignoring message in admin chat: not a reply and "
+                        + f"{self.config.any_message_in_user_topic_is_reply = }"
+                    )
                     return
-                origin_chat_id = await self.origin_chat_id_store.load(forwarded_msg.id)
+                else:
+                    forwarded_msg = None
+                    if message.message_thread_id is None:
+                        self.logger.debug("Message in admin chat is not a reply and not in topic")
+                        return
+                    maybe_forwarded_msg_id = await self.last_forwarded_message_id_by_message_thread_id.load(
+                        message.message_thread_id
+                    )
+                    if maybe_forwarded_msg_id is None:
+                        self.logger.debug("Message in admin chat is not a reply and not in user's topic")
+                        return
+                    forwarded_msg_id = maybe_forwarded_msg_id
+
+                origin_chat_id = await self.origin_chat_id_store.load(forwarded_msg_id)
                 if origin_chat_id is None:
                     return
 
                 if message.text is not None and message.text.startswith("/"):
                     # admin chat commands
                     if message.text in self.admin_chat_response_action_by_command:
+                        if forwarded_msg is None:
+                            raise RuntimeError(
+                                "Admin chat response actions are not supported in per-user forum topics, "
+                                "please try replying to a user's message directly."
+                            )
                         admin_chat_action = self.admin_chat_response_action_by_command[message.text]
                         await admin_chat_action.callback(message, forwarded_msg, origin_chat_id)
                         if admin_chat_action.delete_everything_related_to_user_after:
                             user_related_message_ids = await self.user_related_messages_store.all(origin_chat_id)
                             user_related_message_ids.add(message.id)
                             for message_id in user_related_message_ids:
                                 try:
@@ -988,29 +1068,29 @@
                             copied_to_user_ok_message.id,
                             CopiedMessageToUserData(
                                 origin_chat_id=origin_chat_id, sent_message_id=int(copied_message_id.message_id)
                             ),
                         )
 
                     if self.config.hashtags_in_admin_chat:
-                        await self._remove_unanswered_hashtag(bot, forwarded_msg.id)
+                        await self._remove_unanswered_hashtag(bot, forwarded_msg_id)
                     has_attachments = message.content_type != "text"
                     await asyncio.gather(
                         *[
                             integration.handle_user_message_replied_elsewhere(
                                 UserMessageRepliedEvent(
                                     bot=bot,
                                     origin_chat_id=origin_chat_id,
                                     reply_text=(
                                         (message.html_text if not has_attachments else message.html_caption) or ""
                                     ),
                                     reply_has_attachments=has_attachments,
                                     reply_author=message.from_user.first_name,
                                     reply_link=telegram_message_url(self.admin_chat_id, message.id),
-                                    main_admin_chat_message_id=forwarded_msg.id,
+                                    main_admin_chat_message_id=forwarded_msg_id,
                                 )
                             )
                             for integration in self.integrations
                         ]
                     )
             except Exception as e:
                 await bot.reply_to(message, f"Something went wrong! {e}")
```

### Comparing `telebot_components-0.8.5/telebot_components/feedback/anti_spam.py` & `telebot_components-0.8.6/telebot_components/feedback/anti_spam.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/feedback/integration/aux_feedback_handler.py` & `telebot_components-0.8.6/telebot_components/feedback/integration/aux_feedback_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import copy
 import logging
 from typing import Optional
 
 from telebot import AsyncTeleBot
 from telebot import types as tg
 
-from telebot_components.feedback import FeedbackHandler, MessageForwarderResult
+from telebot_components.feedback import (
+    FeedbackHandler,
+    MessageForwarderResult,
+    UserAnonymization,
+)
 from telebot_components.feedback.integration.interface import (
     FeedbackHandlerIntegration,
     UserMessageRepliedFromIntegrationEvent,
 )
 from telebot_components.feedback.types import UserMessageRepliedEvent
 from telebot_components.redis_utils.interface import RedisInterface
 from telebot_components.stores.category import Category
@@ -138,15 +142,15 @@
             async def noop(*args, **kwargs) -> None:
                 pass
 
             await self.feedback_handler._handle_user_message(
                 bot=bot,
                 user=user,
                 message_forwarder=message_forwarder,
-                send_user_id_hash=self.feedback_handler.config.full_user_anonymization,
+                send_user_identifier=self.feedback_handler.config.user_anonymization is not UserAnonymization.LEGACY,
                 user_replier=noop,
                 export_to_integrations=True,
             )
 
     async def handle_user_message_replied_elsewhere(self, event: UserMessageRepliedEvent) -> None:
         aux_admin_chat_message_id = await self.aux_by_main_admin_chat_message_id_store.load(
             event.main_admin_chat_message_id
```

### Comparing `telebot_components-0.8.5/telebot_components/feedback/integration/interface.py` & `telebot_components-0.8.6/telebot_components/feedback/integration/interface.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/feedback/integration/trello.py` & `telebot_components-0.8.6/telebot_components/feedback/integration/trello.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/form/field.py` & `telebot_components-0.8.6/telebot_components/form/field.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/form/form.py` & `telebot_components-0.8.6/telebot_components/form/form.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/form/handler.py` & `telebot_components-0.8.6/telebot_components/form/handler.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/form/helpers/calendar_keyboard.py` & `telebot_components-0.8.6/telebot_components/form/helpers/calendar_keyboard.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/menu/menu.py` & `telebot_components-0.8.6/telebot_components/menu/menu.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/redis_utils/emulation.py` & `telebot_components-0.8.6/telebot_components/redis_utils/emulation.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/redis_utils/interface.py` & `telebot_components-0.8.6/telebot_components/redis_utils/interface.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/stores/banned_users.py` & `telebot_components-0.8.6/telebot_components/stores/banned_users.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/stores/category.py` & `telebot_components-0.8.6/telebot_components/stores/category.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/stores/forum_topics.py` & `telebot_components-0.8.6/telebot_components/stores/forum_topics.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/stores/generic.py` & `telebot_components-0.8.6/telebot_components/stores/generic.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/stores/language.py` & `telebot_components-0.8.6/telebot_components/stores/language.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/stores/user_group.py` & `telebot_components-0.8.6/telebot_components/stores/user_group.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/stores/utils.py` & `telebot_components-0.8.6/telebot_components/stores/utils.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/utils/__init__.py` & `telebot_components-0.8.6/telebot_components/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,15 @@
 
 def telegram_html_escape(string: str) -> str:
     """See https://core.telegram.org/bots/api#html-style"""
     return string.replace("<", "&lt;").replace(">", "&gt;").replace("&", "&amp;")
 
 
 def html_link(href: str, text: str) -> str:
+    text = telegram_html_escape(text)
     return f'<a href="{href}">{text}</a>'
 
 
 def markdown_link(href: str, text: str) -> str:
     return f"[{text}]({href})"
```

### Comparing `telebot_components-0.8.5/telebot_components/utils/airtable.py` & `telebot_components-0.8.6/telebot_components/utils/airtable.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/utils/alerts.py` & `telebot_components-0.8.6/telebot_components/utils/alerts.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/telebot_components/utils/strings.py` & `telebot_components-0.8.6/telebot_components/utils/strings.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.5/PKG-INFO` & `telebot_components-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telebot-components
-Version: 0.8.5
+Version: 0.8.6
 Summary: Framework/toolkit for building Telegram bots with telebot and redis
 Home-page: https://github.com/bots-against-war/telebot-components
 License: GPLv3
 Author: Igor Vaiman
 Author-email: gosha.vaiman@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
@@ -17,15 +17,15 @@
 Requires-Dist: markdown (>=3.4.1,<4.0.0)
 Requires-Dist: markdownify (>=0.11.2,<0.12.0)
 Requires-Dist: py-trello (>=0.18.0,<0.19.0)
 Requires-Dist: pyairtable (>=1.5.0,<2.0.0)
 Requires-Dist: pytest-mock (>=3.7.0,<4.0.0)
 Requires-Dist: redis (>=4.3.1,<5.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
-Requires-Dist: telebot-against-war (>=0.6.3,<0.7.0)
+Requires-Dist: telebot-against-war (>=0.6.7,<0.7.0)
 Requires-Dist: tenacity (>=8.1.0,<9.0.0)
 Project-URL: Repository, https://github.com/bots-against-war/telebot-components
 Description-Content-Type: text/markdown
 
 # telebot-components
 
 Framework / toolkit for building bots with [telebot](https://github.com/bots-against-war/telebot).
```

