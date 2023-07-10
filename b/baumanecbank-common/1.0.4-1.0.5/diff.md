# Comparing `tmp/baumanecbank_common-1.0.4.tar.gz` & `tmp/baumanecbank_common-1.0.5.tar.gz`

## Comparing `baumanecbank_common-1.0.4.tar` & `baumanecbank_common-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/Makefile
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/src/baumanecbank_common/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/src/baumanecbank_common/abstract.py
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/src/baumanecbank_common/application.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/src/baumanecbank_common/application_create.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/src/baumanecbank_common/filter.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/src/baumanecbank_common/handlers.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/src/baumanecbank_common/i18n.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/src/baumanecbank_common/log.py
--rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/src/baumanecbank_common/postgres.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/src/baumanecbank_common/qr.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/.gitignore
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/README.md
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/Makefile
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/src/baumanecbank_common/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/src/baumanecbank_common/abstract.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/src/baumanecbank_common/application.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/src/baumanecbank_common/application_create.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/src/baumanecbank_common/filter.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/src/baumanecbank_common/handlers.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/src/baumanecbank_common/i18n.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/src/baumanecbank_common/log.py
+-rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/src/baumanecbank_common/postgres.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/src/baumanecbank_common/qr.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/.gitignore
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/README.md
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 baumanecbank_common-1.0.5/PKG-INFO
```

### Comparing `baumanecbank_common-1.0.4/src/baumanecbank_common/__init__.py` & `baumanecbank_common-1.0.5/src/baumanecbank_common/__init__.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.4/src/baumanecbank_common/application.py` & `baumanecbank_common-1.0.5/src/baumanecbank_common/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 from baumanecbank_common.postgres import PgCon
 from baumanecbank_common.i18n import I18n
 
 from telegram import ReplyKeyboardMarkup, ReplyKeyboardRemove
 
 class ApplicationBb(Application):
-    def __init__(self, *, bot: Any, update_queue: asyncio.Queue, updater: Updater | None, job_queue: Any, update_processor: BaseUpdateProcessor, concurrent_updates: bool | int, persistence: BasePersistence | None, context_types: ContextTypes, post_init: Callable[[Application], Coroutine[Any, Any, None]] | None, post_shutdown: Callable[[Application], Coroutine[Any, Any, None]] | None, post_stop: Callable[[Application], Coroutine[Any, Any, None]] | None):
-        super().__init__(bot=bot, update_queue=update_queue, updater=updater, job_queue=job_queue, update_processor=update_processor, concurrent_updates=concurrent_updates, persistence=persistence, context_types=context_types, post_init=post_init, post_shutdown=post_shutdown, post_stop=post_stop)
+    def __init__(self, *, bot: Any, update_queue: asyncio.Queue, updater: Updater | None, job_queue: Any, update_processor: BaseUpdateProcessor, persistence: BasePersistence | None, context_types: ContextTypes, post_init: Callable[[Application], Coroutine[Any, Any, None]] | None, post_shutdown: Callable[[Application], Coroutine[Any, Any, None]] | None, post_stop: Callable[[Application], Coroutine[Any, Any, None]] | None):
+        super().__init__(bot=bot, update_queue=update_queue, updater=updater, job_queue=job_queue, update_processor=update_processor, persistence=persistence, context_types=context_types, post_init=post_init, post_shutdown=post_shutdown, post_stop=post_stop)
         self.appname: str   = None
         self.pgcon:   PgCon = None
         self.i18n:    I18n  = None
 
         self.reply_keyboard_keys = []
         self.reply_keyboard      = ReplyKeyboardRemove()
```

### Comparing `baumanecbank_common-1.0.4/src/baumanecbank_common/application_create.py` & `baumanecbank_common-1.0.5/src/baumanecbank_common/application_create.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.4/src/baumanecbank_common/filter.py` & `baumanecbank_common-1.0.5/src/baumanecbank_common/filter.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.4/src/baumanecbank_common/handlers.py` & `baumanecbank_common-1.0.5/src/baumanecbank_common/handlers.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.4/src/baumanecbank_common/i18n.py` & `baumanecbank_common-1.0.5/src/baumanecbank_common/i18n.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.4/src/baumanecbank_common/log.py` & `baumanecbank_common-1.0.5/src/baumanecbank_common/log.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.4/src/baumanecbank_common/postgres.py` & `baumanecbank_common-1.0.5/src/baumanecbank_common/postgres.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.4/src/baumanecbank_common/qr.py` & `baumanecbank_common-1.0.5/src/baumanecbank_common/qr.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.4/README.md` & `baumanecbank_common-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.0.4/pyproject.toml` & `baumanecbank_common-1.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "baumanecbank_common"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Egor Dubrovin", email="dubrovin.en@ya.ru" },
 ]
 description = "Common funcions package for Baumanec Bank bots"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `baumanecbank_common-1.0.4/PKG-INFO` & `baumanecbank_common-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baumanecbank_common
-Version: 1.0.4
+Version: 1.0.5
 Summary: Common funcions package for Baumanec Bank bots
 Project-URL: Homepage, https://github.com/twobrowin-study/baumanec-bank
 Project-URL: Bug Tracker, https://github.com/twobrowin-study/baumanec-bank/issues
 Author-email: Egor Dubrovin <dubrovin.en@ya.ru>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

