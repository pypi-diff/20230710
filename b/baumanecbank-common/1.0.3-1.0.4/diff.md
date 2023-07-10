# Comparing `tmp/baumanecbank_common-1.0.3.tar.gz` & `tmp/baumanecbank_common-1.0.4.tar.gz`

## Comparing `baumanecbank_common-1.0.3.tar` & `baumanecbank_common-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.3/=20.4
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.3/Makefile
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.3/src/baumanecbank_common/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.3/src/baumanecbank_common/abstract.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.3/src/baumanecbank_common/application.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.3/src/baumanecbank_common/application_create.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.3/src/baumanecbank_common/filter.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.3/src/baumanecbank_common/handlers.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.3/src/baumanecbank_common/i18n.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.3/src/baumanecbank_common/log.py
--rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.3/src/baumanecbank_common/postgres.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.3/src/baumanecbank_common/qr.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.3/.gitignore
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.3/README.md
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/Makefile
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/src/baumanecbank_common/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/src/baumanecbank_common/abstract.py
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/src/baumanecbank_common/application.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/src/baumanecbank_common/application_create.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/src/baumanecbank_common/filter.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/src/baumanecbank_common/handlers.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/src/baumanecbank_common/i18n.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/src/baumanecbank_common/log.py
+-rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/src/baumanecbank_common/postgres.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/src/baumanecbank_common/qr.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/.gitignore
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/README.md
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/PKG-INFO
```

### Comparing `baumanecbank_common-1.0.3/src/baumanecbank_common/__init__.py` & `baumanecbank_common-1.0.4/src/baumanecbank_common/__init__.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.3/src/baumanecbank_common/application.py` & `baumanecbank_common-1.0.4/src/baumanecbank_common/application.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 from baumanecbank_common.postgres import PgCon
 from baumanecbank_common.i18n import I18n
 
 from telegram import ReplyKeyboardMarkup, ReplyKeyboardRemove
 
 class ApplicationBb(Application):
-    def __init__(self, *, bot: Any, update_queue: asyncio.Queue, updater: Updater | None, job_queue: Any, update_processor: BaseUpdateProcessor, concurrent_updates: bool | int, persistence: BasePersistence | None, context_types: ContextTypes, post_init: Callable[[Application], Coroutine[Any, Any, None]] | None, post_shutdown: Callable[[Application], Coroutine[Any, Any, None]] | None):
-        super().__init__(bot=bot, update_queue=update_queue, updater=updater, job_queue=job_queue, update_processor=update_processor, concurrent_updates=concurrent_updates, persistence=persistence, context_types=context_types, post_init=post_init, post_shutdown=post_shutdown)
+    def __init__(self, *, bot: Any, update_queue: asyncio.Queue, updater: Updater | None, job_queue: Any, update_processor: BaseUpdateProcessor, concurrent_updates: bool | int, persistence: BasePersistence | None, context_types: ContextTypes, post_init: Callable[[Application], Coroutine[Any, Any, None]] | None, post_shutdown: Callable[[Application], Coroutine[Any, Any, None]] | None, post_stop: Callable[[Application], Coroutine[Any, Any, None]] | None):
+        super().__init__(bot=bot, update_queue=update_queue, updater=updater, job_queue=job_queue, update_processor=update_processor, concurrent_updates=concurrent_updates, persistence=persistence, context_types=context_types, post_init=post_init, post_shutdown=post_shutdown, post_stop=post_stop)
         self.appname: str   = None
         self.pgcon:   PgCon = None
         self.i18n:    I18n  = None
 
         self.reply_keyboard_keys = []
         self.reply_keyboard      = ReplyKeyboardRemove()
```

### Comparing `baumanecbank_common-1.0.3/src/baumanecbank_common/application_create.py` & `baumanecbank_common-1.0.4/src/baumanecbank_common/application_create.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.3/src/baumanecbank_common/filter.py` & `baumanecbank_common-1.0.4/src/baumanecbank_common/filter.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.3/src/baumanecbank_common/handlers.py` & `baumanecbank_common-1.0.4/src/baumanecbank_common/handlers.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.3/src/baumanecbank_common/i18n.py` & `baumanecbank_common-1.0.4/src/baumanecbank_common/i18n.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.3/src/baumanecbank_common/log.py` & `baumanecbank_common-1.0.4/src/baumanecbank_common/log.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.3/src/baumanecbank_common/postgres.py` & `baumanecbank_common-1.0.4/src/baumanecbank_common/postgres.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.3/src/baumanecbank_common/qr.py` & `baumanecbank_common-1.0.4/src/baumanecbank_common/qr.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.3/README.md` & `baumanecbank_common-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.3/pyproject.toml` & `baumanecbank_common-1.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "baumanecbank_common"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Egor Dubrovin", email="dubrovin.en@ya.ru" },
 ]
 description = "Common funcions package for Baumanec Bank bots"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  'python-telegram-bot>=20.4',
+  'python-telegram-bot==20.4',
   'psycopg2-binary',
   'python-dotenv',
   'pyzbar',
   'Pillow',
   'pyyaml'
 ]
```

### Comparing `baumanecbank_common-1.0.3/PKG-INFO` & `baumanecbank_common-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: baumanecbank_common
-Version: 1.0.3
+Version: 1.0.4
 Summary: Common funcions package for Baumanec Bank bots
 Project-URL: Homepage, https://github.com/twobrowin-study/baumanec-bank
 Project-URL: Bug Tracker, https://github.com/twobrowin-study/baumanec-bank/issues
 Author-email: Egor Dubrovin <dubrovin.en@ya.ru>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Requires-Dist: pillow
 Requires-Dist: psycopg2-binary
 Requires-Dist: python-dotenv
-Requires-Dist: python-telegram-bot>=20.4
+Requires-Dist: python-telegram-bot==20.4
 Requires-Dist: pyyaml
 Requires-Dist: pyzbar
 Description-Content-Type: text/markdown
 
 # Пакет основных функций для ботов БауБанка
 
 Для работы требуются пременные окружения:
```

