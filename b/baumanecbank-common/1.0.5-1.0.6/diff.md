# Comparing `tmp/baumanecbank_common-1.0.5.tar.gz` & `tmp/baumanecbank_common-1.0.6.tar.gz`

## Comparing `baumanecbank_common-1.0.5.tar` & `baumanecbank_common-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/Makefile
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/src/baumanecbank_common/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/src/baumanecbank_common/abstract.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/src/baumanecbank_common/application.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/src/baumanecbank_common/application_create.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/src/baumanecbank_common/filter.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/src/baumanecbank_common/handlers.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/src/baumanecbank_common/i18n.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/src/baumanecbank_common/log.py
--rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/src/baumanecbank_common/postgres.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/src/baumanecbank_common/qr.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/.gitignore
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/README.md
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/Makefile
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/src/baumanecbank_common/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/src/baumanecbank_common/abstract.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/src/baumanecbank_common/application.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/src/baumanecbank_common/application_create.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/src/baumanecbank_common/filter.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/src/baumanecbank_common/handlers.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/src/baumanecbank_common/i18n.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/src/baumanecbank_common/log.py
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/src/baumanecbank_common/postgres.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/src/baumanecbank_common/qr.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/.gitignore
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/README.md
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.6/PKG-INFO
```

### Comparing `baumanecbank_common-1.0.5/src/baumanecbank_common/__init__.py` & `baumanecbank_common-1.0.6/src/baumanecbank_common/__init__.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.5/src/baumanecbank_common/application.py` & `baumanecbank_common-1.0.6/src/baumanecbank_common/application.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.5/src/baumanecbank_common/application_create.py` & `baumanecbank_common-1.0.6/src/baumanecbank_common/application_create.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.5/src/baumanecbank_common/filter.py` & `baumanecbank_common-1.0.6/src/baumanecbank_common/filter.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.5/src/baumanecbank_common/handlers.py` & `baumanecbank_common-1.0.6/src/baumanecbank_common/handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from telegram import Bot, Update, Chat
 from telegram.constants import ParseMode
 from telegram.ext import ContextTypes
 
 from baumanecbank_common.log import Log
 from baumanecbank_common.application import ApplicationBb
 
+from psycopg2 import OperationalError
+
 async def ErrorHandlerFun(update: Update|dict, context: ContextTypes.DEFAULT_TYPE) -> None:
     Log.error(msg="Exception while handling an update:", exc_info=context.error)
     app: ApplicationBb = context.application
     bot: Bot = app.bot
 
     tb_list = traceback.format_exception(None, context.error, context.error.__traceback__)
     tb_string = "".join(tb_list)
@@ -22,18 +24,21 @@
         f"An exception was raised while handling an update\n"
         f"<pre>update = {html.escape(json.dumps(update_str, indent=2, ensure_ascii=False))}"
         "</pre>\n\n"
         f"<pre>context.chat_data = {html.escape(str(context.chat_data))}</pre>\n\n"
         f"<pre>context.user_data = {html.escape(str(context.user_data))}</pre>\n\n"
         f"<pre>{html.escape(tb_string)}</pre>"
     )
-    app.pgcon.write_event(message)
     for group_id in app.pgcon.get_admin_groups():
         await bot.send_message(group_id, message, parse_mode=ParseMode.HTML)
 
+    if context.error.__class__ == OperationalError.__class__:
+        exit(127)
+    app.pgcon.write_event(message)
+
 async def ChatMemberHandlerFun(update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
     Log.debug(f"Chat member event \n{update.my_chat_member}\n")
     app: ApplicationBb = context.application
     chat_id = update.effective_chat.id
     if update.effective_chat.type in [Chat.GROUP, Chat.SUPERGROUP, Chat.CHANNEL]:
         message = (
             f"{update.my_chat_member.new_chat_member['status'].title()} event "
```

### Comparing `baumanecbank_common-1.0.5/src/baumanecbank_common/i18n.py` & `baumanecbank_common-1.0.6/src/baumanecbank_common/i18n.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.5/src/baumanecbank_common/log.py` & `baumanecbank_common-1.0.6/src/baumanecbank_common/log.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.5/src/baumanecbank_common/postgres.py` & `baumanecbank_common-1.0.6/src/baumanecbank_common/postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,8 +242,17 @@
         with self.connection.cursor() as cursor:
             cursor.execute((
                 "INSERT INTO transactions"
                 " (source_card_code_id, amount, type)"
                 " VALUES"
                 f" ({card_code_id}, {amount}, '{PURCHASE}')"
             ))
-            Log.info(f"INSERT transaction {PURCHASE} {card_code_id=} {amount=}")
+            Log.info(f"INSERT transaction {PURCHASE} {card_code_id=} {amount=}")
+    
+    def get_frim_operations_by_account_chat_id(self, chat_id: int|str) -> list[Any]:
+        with self.connection.cursor(cursor_factory=psycopg2.extras.NamedTupleCursor) as cursor:
+            cursor.execute((
+                "SELECT * "
+                "FROM firm_operations_balance_account "
+                f"WHERE client_chat_id = '{chat_id}'"
+            ))
+            return cursor.fetchall()
```

### Comparing `baumanecbank_common-1.0.5/src/baumanecbank_common/qr.py` & `baumanecbank_common-1.0.6/src/baumanecbank_common/qr.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.5/README.md` & `baumanecbank_common-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.5/pyproject.toml` & `baumanecbank_common-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "baumanecbank_common"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Egor Dubrovin", email="dubrovin.en@ya.ru" },
 ]
 description = "Common funcions package for Baumanec Bank bots"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `baumanecbank_common-1.0.5/PKG-INFO` & `baumanecbank_common-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baumanecbank_common
-Version: 1.0.5
+Version: 1.0.6
 Summary: Common funcions package for Baumanec Bank bots
 Project-URL: Homepage, https://github.com/twobrowin-study/baumanec-bank
 Project-URL: Bug Tracker, https://github.com/twobrowin-study/baumanec-bank/issues
 Author-email: Egor Dubrovin <dubrovin.en@ya.ru>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

