# Comparing `tmp/telebot_components-0.8.4.tar.gz` & `tmp/telebot_components-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telebot_components-0.8.4.tar", max compression
+gzip compressed data, was "telebot_components-0.8.5.tar", max compression
```

## Comparing `telebot_components-0.8.4.tar` & `telebot_components-0.8.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    35148 2023-06-27 09:35:12.676991 telebot_components-0.8.4/LICENSE
--rw-r--r--   0        0        0     2258 2023-06-27 09:35:12.676991 telebot_components-0.8.4/README.md
--rw-r--r--   0        0        0     1619 2023-06-27 09:35:28.941136 telebot_components-0.8.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/__init__.py
--rw-r--r--   0        0        0    13083 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/broadcast/__init__.py
--rw-r--r--   0        0        0     2835 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/broadcast/message_senders.py
--rw-r--r--   0        0        0      159 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/broadcast/subscriber.py
--rw-r--r--   0        0        0        0 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/constants/__init__.py
--rw-r--r--   0        0        0    15212 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/constants/emoji.py
--rw-r--r--   0        0        0      168 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/constants/times.py
--rw-r--r--   0        0        0    50254 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/feedback/__init__.py
--rw-r--r--   0        0        0     2075 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/feedback/anti_spam.py
--rw-r--r--   0        0        0        0 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/feedback/integration/__init__.py
--rw-r--r--   0        0        0     8255 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/feedback/integration/aux_feedback_handler.py
--rw-r--r--   0        0        0     3983 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/feedback/integration/interface.py
--rw-r--r--   0        0        0    34435 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/feedback/integration/trello.py
--rw-r--r--   0        0        0      237 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/feedback/trello_integration.py
--rw-r--r--   0        0        0      493 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/feedback/types.py
--rw-r--r--   0        0        0        0 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/form/__init__.py
--rw-r--r--   0        0        0    31714 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/form/field.py
--rw-r--r--   0        0        0    18987 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/form/form.py
--rw-r--r--   0        0        0    20318 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/form/handler.py
--rw-r--r--   0        0        0        0 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/form/helpers/__init__.py
--rw-r--r--   0        0        0     7572 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/form/helpers/calendar_keyboard.py
--rw-r--r--   0        0        0        0 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/menu/__init__.py
--rw-r--r--   0        0        0    11976 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/menu/menu.py
--rw-r--r--   0        0        0        0 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/py.typed
--rw-r--r--   0        0        0        0 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/redis_utils/__init__.py
--rw-r--r--   0        0        0    10640 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/redis_utils/emulation.py
--rw-r--r--   0        0        0     6078 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/redis_utils/interface.py
--rw-r--r--   0        0        0        0 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/stores/__init__.py
--rw-r--r--   0        0        0     1825 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/stores/banned_users.py
--rw-r--r--   0        0        0     8229 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/stores/category.py
--rw-r--r--   0        0        0     9342 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/stores/forum_topics.py
--rw-r--r--   0        0        0     9845 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/stores/generic.py
--rw-r--r--   0        0        0     8298 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/stores/language.py
--rw-r--r--   0        0        0      397 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/stores/types.py
--rw-r--r--   0        0        0     3914 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/stores/user_group.py
--rw-r--r--   0        0        0      614 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/stores/utils.py
--rw-r--r--   0        0        0     8134 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/utils/__init__.py
--rw-r--r--   0        0        0     5136 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/utils/airtable.py
--rw-r--r--   0        0        0     2564 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/utils/alerts.py
--rw-r--r--   0        0        0     1257 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/utils/strings.py
--rw-r--r--   0        0        0     3411 1970-01-01 00:00:00.000000 telebot_components-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-07-10 15:12:36.186927 telebot_components-0.8.5/LICENSE
+-rw-r--r--   0        0        0     2242 2023-07-10 15:12:36.186927 telebot_components-0.8.5/README.md
+-rw-r--r--   0        0        0     1619 2023-07-10 15:12:57.572719 telebot_components-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 15:12:36.186927 telebot_components-0.8.5/telebot_components/__init__.py
+-rw-r--r--   0        0        0    13083 2023-07-10 15:12:36.186927 telebot_components-0.8.5/telebot_components/broadcast/__init__.py
+-rw-r--r--   0        0        0     2835 2023-07-10 15:12:36.186927 telebot_components-0.8.5/telebot_components/broadcast/message_senders.py
+-rw-r--r--   0        0        0      159 2023-07-10 15:12:36.186927 telebot_components-0.8.5/telebot_components/broadcast/subscriber.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:12:36.186927 telebot_components-0.8.5/telebot_components/constants/__init__.py
+-rw-r--r--   0        0        0    15212 2023-07-10 15:12:36.186927 telebot_components-0.8.5/telebot_components/constants/emoji.py
+-rw-r--r--   0        0        0      168 2023-07-10 15:12:36.186927 telebot_components-0.8.5/telebot_components/constants/times.py
+-rw-r--r--   0        0        0    50254 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/feedback/__init__.py
+-rw-r--r--   0        0        0     2075 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/feedback/anti_spam.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/feedback/integration/__init__.py
+-rw-r--r--   0        0        0     8255 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/feedback/integration/aux_feedback_handler.py
+-rw-r--r--   0        0        0     3983 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/feedback/integration/interface.py
+-rw-r--r--   0        0        0    34435 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/feedback/integration/trello.py
+-rw-r--r--   0        0        0      237 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/feedback/trello_integration.py
+-rw-r--r--   0        0        0      493 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/feedback/types.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/form/__init__.py
+-rw-r--r--   0        0        0    31714 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/form/field.py
+-rw-r--r--   0        0        0    18987 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/form/form.py
+-rw-r--r--   0        0        0    20318 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/form/handler.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/form/helpers/__init__.py
+-rw-r--r--   0        0        0     7572 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/form/helpers/calendar_keyboard.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/menu/__init__.py
+-rw-r--r--   0        0        0    13686 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/menu/menu.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/py.typed
+-rw-r--r--   0        0        0        0 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/redis_utils/__init__.py
+-rw-r--r--   0        0        0    10640 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/redis_utils/emulation.py
+-rw-r--r--   0        0        0     6078 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/redis_utils/interface.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/stores/__init__.py
+-rw-r--r--   0        0        0     1825 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/stores/banned_users.py
+-rw-r--r--   0        0        0     8229 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/stores/category.py
+-rw-r--r--   0        0        0     9342 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/stores/forum_topics.py
+-rw-r--r--   0        0        0     9845 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/stores/generic.py
+-rw-r--r--   0        0        0     8298 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/stores/language.py
+-rw-r--r--   0        0        0      397 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/stores/types.py
+-rw-r--r--   0        0        0     3914 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/stores/user_group.py
+-rw-r--r--   0        0        0      614 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/stores/utils.py
+-rw-r--r--   0        0        0     8134 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/utils/__init__.py
+-rw-r--r--   0        0        0     5185 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/utils/airtable.py
+-rw-r--r--   0        0        0     2564 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/utils/alerts.py
+-rw-r--r--   0        0        0     1257 2023-07-10 15:12:36.190927 telebot_components-0.8.5/telebot_components/utils/strings.py
+-rw-r--r--   0        0        0     3395 1970-01-01 00:00:00.000000 telebot_components-0.8.5/PKG-INFO
```

### Comparing `telebot_components-0.8.4/LICENSE` & `telebot_components-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/README.md` & `telebot_components-0.8.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 ### Setup
 1. Clone repository
    ```bash
    git clone git@github.com:bots-against-war/telebot-components.git baw
    cd ./baw
    ```
 
-2. The project requires Poerty 1.2.x or higher (see [installation instruction](https://python-poetry.org/docs/master#installing-with-the-official-installer))).
-   For example, to install `1.2.0b2` on Unix, run
+2. The project requires Poerty 1.5.1 (see [installation instruction](https://python-poetry.org/docs/master#installing-with-the-official-installer))).
+   For example, to install `1.5.1` on Unix, run
    ```bash
-   curl -sSL https://install.python-poetry.org | python3 - --version 1.2.0b2
+   curl -sSL https://install.python-poetry.org | python3 - --version 1.5.1
    ```
 
 3. Then, to install the library with all dependencies, run from project root
    ```bash
    poetry install
    ```
    - You might need to manually install dynamic versioning plugin (without it local build will
      always have version `0.0.0`):
      ```bash
-     poetry plugin add poetry-dynamic-versioning-plugin
+     poetry self add poetry-dynamic-versioning-plugin
      ```
    - To create virtualenv inside the project’s root directory, use command
      ```bash
      poetry config virtualenvs.in-project false --local
      ```
 4. Run `pre-commit` to set up git hook scripts
    ```bash
```

### Comparing `telebot_components-0.8.4/pyproject.toml` & `telebot_components-0.8.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "telebot-components"
-version = "0.8.4"
+version = "0.8.5"
 description = "Framework/toolkit for building Telegram bots with telebot and redis"
 authors = ["Igor Vaiman <gosha.vaiman@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/bots-against-war/telebot-components"
 packages = [{include = "telebot_components"}]
 
@@ -22,15 +22,15 @@
 python = "^3.10"
 telebot-against-war = "^0.6.3"
 redis = "^4.3.1"
 py-trello = "^0.18.0"
 markdownify = "^0.11.2"
 pytest-mock = "^3.7.0"
 "ruamel.yaml" = "^0.17.21"
-pyairtable = "^1.3.0"
+pyairtable = "^1.5.0"
 Pillow = "^9.2.0"
 markdown = "^3.4.1"
 beautifulsoup4 = "^4.11.1"
 tenacity = "^8.1.0"
 async-lru = "^2.0.2"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `telebot_components-0.8.4/telebot_components/broadcast/__init__.py` & `telebot_components-0.8.5/telebot_components/broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/broadcast/message_senders.py` & `telebot_components-0.8.5/telebot_components/broadcast/message_senders.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/constants/emoji.py` & `telebot_components-0.8.5/telebot_components/constants/emoji.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/feedback/__init__.py` & `telebot_components-0.8.5/telebot_components/feedback/__init__.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/feedback/anti_spam.py` & `telebot_components-0.8.5/telebot_components/feedback/anti_spam.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/feedback/integration/aux_feedback_handler.py` & `telebot_components-0.8.5/telebot_components/feedback/integration/aux_feedback_handler.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/feedback/integration/interface.py` & `telebot_components-0.8.5/telebot_components/feedback/integration/interface.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/feedback/integration/trello.py` & `telebot_components-0.8.5/telebot_components/feedback/integration/trello.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/form/field.py` & `telebot_components-0.8.5/telebot_components/form/field.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/form/form.py` & `telebot_components-0.8.5/telebot_components/form/form.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/form/handler.py` & `telebot_components-0.8.5/telebot_components/form/handler.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/form/helpers/calendar_keyboard.py` & `telebot_components-0.8.5/telebot_components/form/helpers/calendar_keyboard.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/menu/menu.py` & `telebot_components-0.8.5/telebot_components/menu/menu.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,31 @@
 
 from telebot import AsyncTeleBot
 from telebot import types as tg
 from telebot.api import ApiHTTPException
 from telebot.callback_data import CallbackData
 
 from telebot_components.stores.category import Category, CategoryStore
+from telebot_components.stores.language import (
+    AnyText,
+    LanguageStore,
+    MaybeLanguage,
+    any_text_to_str,
+    vaildate_singlelang_text,
+)
 
 ROUTE_MENU_CALLBACK_DATA = CallbackData("route_to", prefix="menu")
 TERMINATE_MENU_CALLBACK_DATA = CallbackData("id", prefix="terminator")
 INACTIVE_BUTTON_CALLBACK_DATA = CallbackData(prefix="inactive_button")
 
 
 class MenuItem:
     def __init__(
         self,
-        label: str,
+        label: AnyText,
         submenu: Optional["Menu"] = None,
         terminator: Optional[str] = None,
         link_url: Optional[str] = None,
         bound_category: Optional[Category] = None,
     ):
         self.label = label
         self.bound_category = bound_category
@@ -74,51 +81,51 @@
             raise RuntimeError("MenuItem object was not properly initialized.")
         return self._parent_menu
 
     @parent_menu.setter
     def parent_menu(self, parent_menu: "Menu"):
         self._parent_menu = parent_menu
 
-    def get_inline_button(self):
+    def get_inline_button(self, language: MaybeLanguage):
         if self.submenu is not None:
             return tg.InlineKeyboardButton(
-                text=self.label,
+                text=any_text_to_str(self.label, language),
                 callback_data=ROUTE_MENU_CALLBACK_DATA.new(self.submenu.id),
             )
         elif self.link_url is not None:
             return tg.InlineKeyboardButton(
-                text=self.label,
+                text=any_text_to_str(self.label, language),
                 url=self.link_url,
             )
         else:
             return tg.InlineKeyboardButton(
-                text=self.label,
+                text=any_text_to_str(self.label, language),
                 callback_data=TERMINATE_MENU_CALLBACK_DATA.new(self.id),
             )
 
-    def get_inactive_inline_button(self, selected_item_id: str):
-        button_text = self.label
+    def get_inactive_inline_button(self, selected_item_id: str, language: MaybeLanguage):
+        button_text = any_text_to_str(self.label, language)
         if self.id == selected_item_id:
             button_text = "✅ " + button_text
         return tg.InlineKeyboardButton(
             text=button_text,
             callback_data=INACTIVE_BUTTON_CALLBACK_DATA.new(),
         )
 
 
 @dataclass(frozen=True)
 class MenuConfig:
-    back_label: str
+    back_label: AnyText
     lock_after_termination: bool
 
 
 class Menu:
     def __init__(
         self,
-        text: str,
+        text: AnyText,
         menu_items: list[MenuItem],
         config: Optional[MenuConfig] = None,
     ):
         self._id: Optional[str] = None
         self.parent_menu: Optional["Menu"] = None
         self.text = text
         self.menu_items = menu_items
@@ -149,49 +156,61 @@
     def descendants(self) -> list["Menu"]:
         children = [mi.submenu for mi in self.menu_items if mi.submenu is not None]
         grandchildren: list[Menu] = []
         for menu in children:
             grandchildren.extend(menu.descendants())
         return children + grandchildren
 
-    def get_keyboard_markup(self):
-        keyboard = [[menu_item.get_inline_button()] for menu_item in self.menu_items]
+    def get_keyboard_markup(self, language: MaybeLanguage):
+        keyboard = [[menu_item.get_inline_button(language)] for menu_item in self.menu_items]
         if self.parent_menu is not None:
-            keyboard.append([MenuItem(label=self.config.back_label, submenu=self.parent_menu).get_inline_button()])
+            if isinstance(self.config.back_label, str):
+                keyboard.append(
+                    [MenuItem(label=self.config.back_label, submenu=self.parent_menu).get_inline_button(None)]
+                )
+            else:
+                keyboard.append(
+                    [MenuItem(label=self.config.back_label, submenu=self.parent_menu).get_inline_button(language)]
+                )
         return tg.InlineKeyboardMarkup(keyboard=keyboard)
 
-    def get_inactive_keyboard_markup(self, selected_item_id: str):
+    def get_inactive_keyboard_markup(self, selected_item_id: str, language: MaybeLanguage):
         return tg.InlineKeyboardMarkup(
-            keyboard=[[menu_item.get_inactive_inline_button(selected_item_id)] for menu_item in self.menu_items]
+            keyboard=[
+                [menu_item.get_inactive_inline_button(selected_item_id, language)] for menu_item in self.menu_items
+            ]
         )
 
 
 @dataclass
 class TerminatorContext:
     bot: AsyncTeleBot
     user: tg.User
     menu_message: tg.Message
     terminator: str
 
 
 @dataclass
 class TerminatorResult:
-    menu_message_text_update: str
+    menu_message_text_update: AnyText
     parse_mode: Optional[str] = None
     lock_menu: Optional[bool] = None  # if set, overrides the default lock_after_termination value in Menu config
 
 
 class MenuHandler:
     def __init__(
         self,
         bot_prefix: str,
         menu_tree: Menu,
         category_store: Optional[CategoryStore] = None,
+        language_store: Optional[LanguageStore] = None,
     ):
         self.category_store = category_store
+        self.language_store = language_store
+
         self.menus_list: list[Menu] = [menu_tree]
         self.menus_list.extend(menu_tree.descendants())
 
         self.init_menu_ids()
         self.init_parent_menu()
 
         self.menu_by_id: dict[str, Menu] = {m.id: m for m in self.menus_list}
@@ -213,16 +232,32 @@
                 raise ValueError(
                     "Some categories bound to menu items are not storable "
                     + f"with the passed category store: {menu_items_with_non_storable_categories}"
                 )
 
         self.menu_item_by_id: dict[str, MenuItem] = {mi.id: mi for mi in self.menu_items_list}
 
+        menu_texts = [menu.text for menu in self.menus_list]
+        menu_item_labels = [menu_item.label for menu_item in self.menu_items_list]
+        menu_back_labels = [menu.config.back_label for menu in self.menus_list]
+
+        for any_text in menu_texts + menu_item_labels + menu_back_labels:
+            if self.language_store is not None:
+                self.language_store.validate_multilang(any_text)
+            else:
+                vaildate_singlelang_text(any_text)
+
         self.logger = logging.getLogger(f"{__name__}[{bot_prefix}]")
 
+    async def get_maybe_language(self, user: tg.User) -> MaybeLanguage:
+        if self.language_store is None:
+            return None
+        else:
+            return await self.language_store.get_user_language(user)
+
     def init_item_ids_and_get_item_list(self) -> list[MenuItem]:
         item_list: list[MenuItem] = []
         for menu in self.menus_list:
             for menu_item in menu.menu_items:
                 item_list.append(menu_item)
         for i, menu_item in enumerate(item_list):
             menu_item.id = str(i)
@@ -246,34 +281,36 @@
         self,
         bot: AsyncTeleBot,
         on_terminal_menu_option_selected: Callable[[TerminatorContext], Awaitable[Optional[TerminatorResult]]],
     ):
         @bot.callback_query_handler(callback_data=ROUTE_MENU_CALLBACK_DATA, auto_answer=True)
         async def handle_menu(call: tg.CallbackQuery):
             user = call.from_user
+            language = await self.get_maybe_language(user)
             data = ROUTE_MENU_CALLBACK_DATA.parse(call.data)
             route_to = data["route_to"]
             menu = self.menu_by_id[route_to]
             try:
                 await bot.edit_message_text(
-                    text=menu.text,
+                    text=any_text_to_str(menu.text, language),
                     chat_id=user.id,
                     message_id=call.message.id,
-                    reply_markup=menu.get_keyboard_markup(),
+                    reply_markup=menu.get_keyboard_markup(language),
                 )
             except ApiHTTPException as e:
                 self.logger.info(f"Error editing message text and reply markup: {e!r}")
 
         @bot.callback_query_handler(callback_data=INACTIVE_BUTTON_CALLBACK_DATA, auto_answer=True)
         async def handle_inactive_menu(call: tg.CallbackQuery):
             pass
 
         @bot.callback_query_handler(callback_data=TERMINATE_MENU_CALLBACK_DATA, auto_answer=True)
         async def handle_terminator(call: tg.CallbackQuery):
             user = call.from_user
+            language = await self.get_maybe_language(user)
             data = TERMINATE_MENU_CALLBACK_DATA.parse(call.data)
             selected_menu_item_id = data["id"]
 
             selected_menu_item = self.menu_item_by_id[selected_menu_item_id]
             terminator = selected_menu_item.terminator
             if terminator is None:
                 self.logger.error(f"handle_terminator got non-terminating menu item: {selected_menu_item}")
@@ -289,15 +326,15 @@
             except Exception:
                 self.logger.exception("Unexpected error in on_terminal_menu_option_selected callback, ignoring")
                 terminator_callback_result = None
 
             if terminator_callback_result is not None:
                 try:
                     await bot.edit_message_text(
-                        terminator_callback_result.menu_message_text_update,
+                        text=any_text_to_str(terminator_callback_result.menu_message_text_update, language),
                         chat_id=call.message.chat.id,
                         message_id=call.message.id,
                         parse_mode=terminator_callback_result.parse_mode,
                     )
                 except Exception:
                     self.logger.info(
                         f"Eror editing menu message with callback returned value {terminator_callback_result!r}",
@@ -311,11 +348,11 @@
                 else current_menu.config.lock_after_termination
             )
             if lock_menu:
                 try:
                     await bot.edit_message_reply_markup(
                         chat_id=user.id,
                         message_id=call.message.id,
-                        reply_markup=current_menu.get_inactive_keyboard_markup(selected_menu_item_id),
+                        reply_markup=current_menu.get_inactive_keyboard_markup(selected_menu_item_id, language),
                     )
                 except ApiHTTPException:
                     self.logger.info("Error editing message reply markup", exc_info=True)
```

### Comparing `telebot_components-0.8.4/telebot_components/redis_utils/emulation.py` & `telebot_components-0.8.5/telebot_components/redis_utils/emulation.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/redis_utils/interface.py` & `telebot_components-0.8.5/telebot_components/redis_utils/interface.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/stores/banned_users.py` & `telebot_components-0.8.5/telebot_components/stores/banned_users.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/stores/category.py` & `telebot_components-0.8.5/telebot_components/stores/category.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/stores/forum_topics.py` & `telebot_components-0.8.5/telebot_components/stores/forum_topics.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/stores/generic.py` & `telebot_components-0.8.5/telebot_components/stores/generic.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/stores/language.py` & `telebot_components-0.8.5/telebot_components/stores/language.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/stores/user_group.py` & `telebot_components-0.8.5/telebot_components/stores/user_group.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/stores/utils.py` & `telebot_components-0.8.5/telebot_components/stores/utils.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/utils/__init__.py` & `telebot_components-0.8.5/telebot_components/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/utils/airtable.py` & `telebot_components-0.8.5/telebot_components/utils/airtable.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 from functools import partial
 from typing import Any, Generic, Type, TypedDict, TypeVar, Union
 
-from pyairtable import Table
+from pyairtable import Table, retry_strategy
 
 logger = logging.getLogger(__name__)
 
 
 AirtableColumnEnumT = TypeVar("AirtableColumnEnumT", bound=Enum)
 AirtableValueT = Union[str, int, float, bool, list[str], dict]
 
@@ -68,15 +68,15 @@
             if col not in column_id_by_enum_item:
                 raise ValueError(f"column_id_by_name mapping misses id for column {col.name!r}")
         self.field_id_by_column_enum_item = column_id_by_enum_item
         self.column_enum_item_by_field_id = {v: k for k, v in self.field_id_by_column_enum_item.items()}
         self.config = config
         self.ColumnsEnumClass = ColumnsEnumClass
         self.thread_pool = ThreadPoolExecutor(max_workers=16)
-        self._table = Table(api_key, config["base_id"], config["table_name"])
+        self._table = Table(api_key, config["base_id"], config["table_name"], retry_strategy=retry_strategy())
 
     def _dump_entry(self, data: dict[AirtableColumnEnumT, Any]) -> dict[str, Any]:
         return {self.field_id_by_column_enum_item[k]: v for k, v in data.items()}
 
     async def create(self, entry: dict[AirtableColumnEnumT, Any]) -> str:
         """Returning record id as a string"""
         loop = asyncio.get_running_loop()
```

### Comparing `telebot_components-0.8.4/telebot_components/utils/alerts.py` & `telebot_components-0.8.5/telebot_components/utils/alerts.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/telebot_components/utils/strings.py` & `telebot_components-0.8.5/telebot_components/utils/strings.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.4/PKG-INFO` & `telebot_components-0.8.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telebot-components
-Version: 0.8.4
+Version: 0.8.5
 Summary: Framework/toolkit for building Telegram bots with telebot and redis
 Home-page: https://github.com/bots-against-war/telebot-components
 License: GPLv3
 Author: Igor Vaiman
 Author-email: gosha.vaiman@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.2.0,<10.0.0)
 Requires-Dist: async-lru (>=2.0.2,<3.0.0)
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: markdown (>=3.4.1,<4.0.0)
 Requires-Dist: markdownify (>=0.11.2,<0.12.0)
 Requires-Dist: py-trello (>=0.18.0,<0.19.0)
-Requires-Dist: pyairtable (>=1.3.0,<2.0.0)
+Requires-Dist: pyairtable (>=1.5.0,<2.0.0)
 Requires-Dist: pytest-mock (>=3.7.0,<4.0.0)
 Requires-Dist: redis (>=4.3.1,<5.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: telebot-against-war (>=0.6.3,<0.7.0)
 Requires-Dist: tenacity (>=8.1.0,<9.0.0)
 Project-URL: Repository, https://github.com/bots-against-war/telebot-components
 Description-Content-Type: text/markdown
@@ -36,28 +36,28 @@
 ### Setup
 1. Clone repository
    ```bash
    git clone git@github.com:bots-against-war/telebot-components.git baw
    cd ./baw
    ```
 
-2. The project requires Poerty 1.2.x or higher (see [installation instruction](https://python-poetry.org/docs/master#installing-with-the-official-installer))).
-   For example, to install `1.2.0b2` on Unix, run
+2. The project requires Poerty 1.5.1 (see [installation instruction](https://python-poetry.org/docs/master#installing-with-the-official-installer))).
+   For example, to install `1.5.1` on Unix, run
    ```bash
-   curl -sSL https://install.python-poetry.org | python3 - --version 1.2.0b2
+   curl -sSL https://install.python-poetry.org | python3 - --version 1.5.1
    ```
 
 3. Then, to install the library with all dependencies, run from project root
    ```bash
    poetry install
    ```
    - You might need to manually install dynamic versioning plugin (without it local build will
      always have version `0.0.0`):
      ```bash
-     poetry plugin add poetry-dynamic-versioning-plugin
+     poetry self add poetry-dynamic-versioning-plugin
      ```
    - To create virtualenv inside the project’s root directory, use command
      ```bash
      poetry config virtualenvs.in-project false --local
      ```
 4. Run `pre-commit` to set up git hook scripts
    ```bash
```

