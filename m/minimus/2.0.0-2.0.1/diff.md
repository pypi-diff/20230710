# Comparing `tmp/minimus-2.0.0.tar.gz` & `tmp/minimus-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minimus-2.0.0.tar", last modified: Mon Jul 10 09:18:13 2023, max compression
+gzip compressed data, was "minimus-2.0.1.tar", last modified: Mon Jul 10 09:36:15 2023, max compression
```

## Comparing `minimus-2.0.0.tar` & `minimus-2.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 09:18:13.345615 minimus-2.0.0/
--rw-rw-rw-   0        0        0     1089 2023-07-10 09:16:41.000000 minimus-2.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     4926 2023-07-10 09:18:13.341616 minimus-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4473 2023-07-10 09:12:02.000000 minimus-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 09:18:13.260585 minimus-2.0.0/minimus/
--rw-rw-rw-   0        0        0        0 2022-12-26 10:28:49.000000 minimus-2.0.0/minimus/__init__.py
--rw-rw-rw-   0        0        0     2625 2023-07-10 09:07:22.000000 minimus-2.0.0/minimus/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:18:13.335453 minimus-2.0.0/minimus/src/
--rw-rw-rw-   0        0        0        0 2023-07-10 09:07:22.000000 minimus-2.0.0/minimus/src/__init__.py
--rw-rw-rw-   0        0        0     4062 2023-07-10 09:07:22.000000 minimus-2.0.0/minimus/src/constants.py
--rw-rw-rw-   0        0        0     4727 2023-07-10 09:07:22.000000 minimus-2.0.0/minimus/src/markup.py
--rw-rw-rw-   0        0        0     5218 2023-07-10 09:07:22.000000 minimus-2.0.0/minimus/src/objects.py
--rw-rw-rw-   0        0        0     1007 2023-07-10 09:07:22.000000 minimus-2.0.0/minimus/src/output.py
--rw-rw-rw-   0        0        0     2893 2023-07-10 09:07:22.000000 minimus-2.0.0/minimus/src/storage.py
--rw-rw-rw-   0        0        0     1347 2023-07-10 09:07:22.000000 minimus-2.0.0/minimus/src/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:18:13.291674 minimus-2.0.0/minimus.egg-info/
--rw-rw-rw-   0        0        0     4926 2023-07-10 09:18:13.000000 minimus-2.0.0/minimus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-07-10 09:18:13.000000 minimus-2.0.0/minimus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 09:18:13.000000 minimus-2.0.0/minimus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-07-10 09:18:13.000000 minimus-2.0.0/minimus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-07-10 09:18:13.000000 minimus-2.0.0/minimus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      626 2023-07-10 09:07:22.000000 minimus-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-10 09:18:13.345735 minimus-2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-10 09:36:15.958152 minimus-2.0.1/
+-rw-rw-rw-   0        0        0     1089 2023-07-10 09:16:41.000000 minimus-2.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     4830 2023-07-10 09:36:15.954013 minimus-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4377 2023-07-10 09:35:04.000000 minimus-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 09:36:15.875387 minimus-2.0.1/minimus/
+-rw-rw-rw-   0        0        0        0 2022-12-26 10:28:49.000000 minimus-2.0.1/minimus/__init__.py
+-rw-rw-rw-   0        0        0     2625 2023-07-10 09:07:22.000000 minimus-2.0.1/minimus/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:36:15.947031 minimus-2.0.1/minimus/src/
+-rw-rw-rw-   0        0        0        0 2023-07-10 09:07:22.000000 minimus-2.0.1/minimus/src/__init__.py
+-rw-rw-rw-   0        0        0     3984 2023-07-10 09:33:38.000000 minimus-2.0.1/minimus/src/constants.py
+-rw-rw-rw-   0        0        0     4727 2023-07-10 09:07:22.000000 minimus-2.0.1/minimus/src/markup.py
+-rw-rw-rw-   0        0        0     5218 2023-07-10 09:07:22.000000 minimus-2.0.1/minimus/src/objects.py
+-rw-rw-rw-   0        0        0     1007 2023-07-10 09:07:22.000000 minimus-2.0.1/minimus/src/output.py
+-rw-rw-rw-   0        0        0     2893 2023-07-10 09:07:22.000000 minimus-2.0.1/minimus/src/storage.py
+-rw-rw-rw-   0        0        0     1347 2023-07-10 09:07:22.000000 minimus-2.0.1/minimus/src/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:36:15.905883 minimus-2.0.1/minimus.egg-info/
+-rw-rw-rw-   0        0        0     4830 2023-07-10 09:36:15.000000 minimus-2.0.1/minimus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-07-10 09:36:15.000000 minimus-2.0.1/minimus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 09:36:15.000000 minimus-2.0.1/minimus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-07-10 09:36:15.000000 minimus-2.0.1/minimus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-07-10 09:36:15.000000 minimus-2.0.1/minimus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      626 2023-07-10 09:33:38.000000 minimus-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-10 09:36:15.959087 minimus-2.0.1/setup.cfg
```

### Comparing `minimus-2.0.0/LICENSE.txt` & `minimus-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `minimus-2.0.0/PKG-INFO` & `minimus-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minimus
-Version: 2.0.0
+Version: 2.0.1
 Summary: Personal knowledge storage formatter
 Author-email: Igor Zyktin <nicord@yandex.ru>
 Project-URL: Homepage, https://github.com/IgorZyktin/minimus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -98,32 +98,32 @@
 
 Живёт почти везде.
 ```
 
 Нормальный вывод программы выглядит примерно вот так:
 
 ```
--------------------------------------------------------------------------------------
-███╗   ███╗██╗███╗   ██╗██╗   ██╗███╗   ███╗██╗   ██╗███████╗    ██████╗     ██████╗
-████╗ ████║██║████╗  ██║██║   ██║████╗ ████║██║   ██║██╔════╝    ╚════██╗   ██╔═████╗
-██╔████╔██║██║██╔██╗ ██║██║   ██║██╔████╔██║██║   ██║███████╗     █████╔╝   ██║██╔██║
-██║╚██╔╝██║██║██║╚██╗██║██║   ██║██║╚██╔╝██║██║   ██║╚════██║    ██╔═══╝    ████╔╝██║
-██║ ╚═╝ ██║██║██║ ╚████║╚██████╔╝██║ ╚═╝ ██║╚██████╔╝███████║    ███████╗██╗╚██████╔╝
-╚═╝     ╚═╝╚═╝╚═╝  ╚═══╝ ╚═════╝ ╚═╝     ╚═╝ ╚═════╝ ╚══════╝    ╚══════╝╚═╝ ╚═════╝
--------------------------------------------------------------------------------------
+-------------------------------------------------------------------------------
+███╗   ███╗██╗███╗   ██╗██╗███╗   ███╗██╗   ██╗███████╗    ██████╗     ██████╗ 
+████╗ ████║██║████╗  ██║██║████╗ ████║██║   ██║██╔════╝    ╚════██╗   ██╔═████╗
+██╔████╔██║██║██╔██╗ ██║██║██╔████╔██║██║   ██║███████╗     █████╔╝   ██║██╔██║
+██║╚██╔╝██║██║██║╚██╗██║██║██║╚██╔╝██║██║   ██║╚════██║    ██╔═══╝    ████╔╝██║
+██║ ╚═╝ ██║██║██║ ╚████║██║██║ ╚═╝ ██║╚██████╔╝███████║    ███████╗██╗╚██████╔╝
+╚═╝     ╚═╝╚═╝╚═╝  ╚═══╝╚═╝╚═╝     ╚═╝ ╚═════╝ ╚══════╝    ╚══════╝╚═╝ ╚═════╝ 
+-------------------------------------------------------------------------------
 Исходный каталог: /home/test-minimus
 
 Сохранение заметок
         +++ Сохранён: 2020-07-06_recursion.md
         +++ Сохранён: 2020-07-06_vacuum.md
         +++ Сохранён: Животные/2020-07-06_elephant.md
         +++ Сохранён: Животные/2020-07-06_mouse.md
 
 Сохранение тегов
         Сохранено тегов: 5 шт. 
 
 Генерация вспомогательных файлов
         Сохранён: /home/test-minimus/README.md
         Сохранён: /home/test-minimus/.minimus_cache.json
--------------------------------------------------------------------------------------
+-------------------------------------------------------------------------------
 Обработка заняла 0.02 сек.
 ```
```

### Comparing `minimus-2.0.0/README.md` & `minimus-2.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -85,32 +85,32 @@
 
 Живёт почти везде.
 ```
 
 Нормальный вывод программы выглядит примерно вот так:
 
 ```
--------------------------------------------------------------------------------------
-███╗   ███╗██╗███╗   ██╗██╗   ██╗███╗   ███╗██╗   ██╗███████╗    ██████╗     ██████╗
-████╗ ████║██║████╗  ██║██║   ██║████╗ ████║██║   ██║██╔════╝    ╚════██╗   ██╔═████╗
-██╔████╔██║██║██╔██╗ ██║██║   ██║██╔████╔██║██║   ██║███████╗     █████╔╝   ██║██╔██║
-██║╚██╔╝██║██║██║╚██╗██║██║   ██║██║╚██╔╝██║██║   ██║╚════██║    ██╔═══╝    ████╔╝██║
-██║ ╚═╝ ██║██║██║ ╚████║╚██████╔╝██║ ╚═╝ ██║╚██████╔╝███████║    ███████╗██╗╚██████╔╝
-╚═╝     ╚═╝╚═╝╚═╝  ╚═══╝ ╚═════╝ ╚═╝     ╚═╝ ╚═════╝ ╚══════╝    ╚══════╝╚═╝ ╚═════╝
--------------------------------------------------------------------------------------
+-------------------------------------------------------------------------------
+███╗   ███╗██╗███╗   ██╗██╗███╗   ███╗██╗   ██╗███████╗    ██████╗     ██████╗ 
+████╗ ████║██║████╗  ██║██║████╗ ████║██║   ██║██╔════╝    ╚════██╗   ██╔═████╗
+██╔████╔██║██║██╔██╗ ██║██║██╔████╔██║██║   ██║███████╗     █████╔╝   ██║██╔██║
+██║╚██╔╝██║██║██║╚██╗██║██║██║╚██╔╝██║██║   ██║╚════██║    ██╔═══╝    ████╔╝██║
+██║ ╚═╝ ██║██║██║ ╚████║██║██║ ╚═╝ ██║╚██████╔╝███████║    ███████╗██╗╚██████╔╝
+╚═╝     ╚═╝╚═╝╚═╝  ╚═══╝╚═╝╚═╝     ╚═╝ ╚═════╝ ╚══════╝    ╚══════╝╚═╝ ╚═════╝ 
+-------------------------------------------------------------------------------
 Исходный каталог: /home/test-minimus
 
 Сохранение заметок
         +++ Сохранён: 2020-07-06_recursion.md
         +++ Сохранён: 2020-07-06_vacuum.md
         +++ Сохранён: Животные/2020-07-06_elephant.md
         +++ Сохранён: Животные/2020-07-06_mouse.md
 
 Сохранение тегов
         Сохранено тегов: 5 шт. 
 
 Генерация вспомогательных файлов
         Сохранён: /home/test-minimus/README.md
         Сохранён: /home/test-minimus/.minimus_cache.json
--------------------------------------------------------------------------------------
+-------------------------------------------------------------------------------
 Обработка заняла 0.02 сек.
 ```
```

### Comparing `minimus-2.0.0/minimus/__main__.py` & `minimus-2.0.1/minimus/__main__.py`

 * *Files identical despite different names*

### Comparing `minimus-2.0.0/minimus/src/constants.py` & `minimus-2.0.1/minimus/src/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Постоянные значения.
 """
 import re
 
 LOGO = """
-███╗   ███╗██╗███╗   ██╗██╗   ██╗███╗   ███╗██╗   ██╗███████╗    ██████╗     ██████╗
-████╗ ████║██║████╗  ██║██║   ██║████╗ ████║██║   ██║██╔════╝    ╚════██╗   ██╔═████╗
-██╔████╔██║██║██╔██╗ ██║██║   ██║██╔████╔██║██║   ██║███████╗     █████╔╝   ██║██╔██║
-██║╚██╔╝██║██║██║╚██╗██║██║   ██║██║╚██╔╝██║██║   ██║╚════██║    ██╔═══╝    ████╔╝██║
-██║ ╚═╝ ██║██║██║ ╚████║╚██████╔╝██║ ╚═╝ ██║╚██████╔╝███████║    ███████╗██╗╚██████╔╝
-╚═╝     ╚═╝╚═╝╚═╝  ╚═══╝ ╚═════╝ ╚═╝     ╚═╝ ╚═════╝ ╚══════╝    ╚══════╝╚═╝ ╚═════╝
+███╗   ███╗██╗███╗   ██╗██╗███╗   ███╗██╗   ██╗███████╗    ██████╗     ██████╗ 
+████╗ ████║██║████╗  ██║██║████╗ ████║██║   ██║██╔════╝    ╚════██╗   ██╔═████╗
+██╔████╔██║██║██╔██╗ ██║██║██╔████╔██║██║   ██║███████╗     █████╔╝   ██║██╔██║
+██║╚██╔╝██║██║██║╚██╗██║██║██║╚██╔╝██║██║   ██║╚════██║    ██╔═══╝    ████╔╝██║
+██║ ╚═╝ ██║██║██║ ╚████║██║██║ ╚═╝ ██║╚██████╔╝███████║    ███████╗██╗╚██████╔╝
+╚═╝     ╚═╝╚═╝╚═╝  ╚═══╝╚═╝╚═╝     ╚═╝ ╚═════╝ ╚══════╝    ╚══════╝╚═╝ ╚═════╝ 
 """.strip()  # noqa
 
 LINE = '-' * (max(len(x) for x in LOGO.split('\n')))
 
 UNKNOWN = '???'
 README_FILENAME = 'README.md'
 CACHE_FILENAME = '.minimus_cache.json'
```

### Comparing `minimus-2.0.0/minimus/src/markup.py` & `minimus-2.0.1/minimus/src/markup.py`

 * *Files identical despite different names*

### Comparing `minimus-2.0.0/minimus/src/objects.py` & `minimus-2.0.1/minimus/src/objects.py`

 * *Files identical despite different names*

### Comparing `minimus-2.0.0/minimus/src/output.py` & `minimus-2.0.1/minimus/src/output.py`

 * *Files identical despite different names*

### Comparing `minimus-2.0.0/minimus/src/storage.py` & `minimus-2.0.1/minimus/src/storage.py`

 * *Files identical despite different names*

### Comparing `minimus-2.0.0/minimus/src/utils.py` & `minimus-2.0.1/minimus/src/utils.py`

 * *Files identical despite different names*

### Comparing `minimus-2.0.0/minimus.egg-info/PKG-INFO` & `minimus-2.0.1/minimus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minimus
-Version: 2.0.0
+Version: 2.0.1
 Summary: Personal knowledge storage formatter
 Author-email: Igor Zyktin <nicord@yandex.ru>
 Project-URL: Homepage, https://github.com/IgorZyktin/minimus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -98,32 +98,32 @@
 
 Живёт почти везде.
 ```
 
 Нормальный вывод программы выглядит примерно вот так:
 
 ```
--------------------------------------------------------------------------------------
-███╗   ███╗██╗███╗   ██╗██╗   ██╗███╗   ███╗██╗   ██╗███████╗    ██████╗     ██████╗
-████╗ ████║██║████╗  ██║██║   ██║████╗ ████║██║   ██║██╔════╝    ╚════██╗   ██╔═████╗
-██╔████╔██║██║██╔██╗ ██║██║   ██║██╔████╔██║██║   ██║███████╗     █████╔╝   ██║██╔██║
-██║╚██╔╝██║██║██║╚██╗██║██║   ██║██║╚██╔╝██║██║   ██║╚════██║    ██╔═══╝    ████╔╝██║
-██║ ╚═╝ ██║██║██║ ╚████║╚██████╔╝██║ ╚═╝ ██║╚██████╔╝███████║    ███████╗██╗╚██████╔╝
-╚═╝     ╚═╝╚═╝╚═╝  ╚═══╝ ╚═════╝ ╚═╝     ╚═╝ ╚═════╝ ╚══════╝    ╚══════╝╚═╝ ╚═════╝
--------------------------------------------------------------------------------------
+-------------------------------------------------------------------------------
+███╗   ███╗██╗███╗   ██╗██╗███╗   ███╗██╗   ██╗███████╗    ██████╗     ██████╗ 
+████╗ ████║██║████╗  ██║██║████╗ ████║██║   ██║██╔════╝    ╚════██╗   ██╔═████╗
+██╔████╔██║██║██╔██╗ ██║██║██╔████╔██║██║   ██║███████╗     █████╔╝   ██║██╔██║
+██║╚██╔╝██║██║██║╚██╗██║██║██║╚██╔╝██║██║   ██║╚════██║    ██╔═══╝    ████╔╝██║
+██║ ╚═╝ ██║██║██║ ╚████║██║██║ ╚═╝ ██║╚██████╔╝███████║    ███████╗██╗╚██████╔╝
+╚═╝     ╚═╝╚═╝╚═╝  ╚═══╝╚═╝╚═╝     ╚═╝ ╚═════╝ ╚══════╝    ╚══════╝╚═╝ ╚═════╝ 
+-------------------------------------------------------------------------------
 Исходный каталог: /home/test-minimus
 
 Сохранение заметок
         +++ Сохранён: 2020-07-06_recursion.md
         +++ Сохранён: 2020-07-06_vacuum.md
         +++ Сохранён: Животные/2020-07-06_elephant.md
         +++ Сохранён: Животные/2020-07-06_mouse.md
 
 Сохранение тегов
         Сохранено тегов: 5 шт. 
 
 Генерация вспомогательных файлов
         Сохранён: /home/test-minimus/README.md
         Сохранён: /home/test-minimus/.minimus_cache.json
--------------------------------------------------------------------------------------
+-------------------------------------------------------------------------------
 Обработка заняла 0.02 сек.
 ```
```

### Comparing `minimus-2.0.0/pyproject.toml` & `minimus-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "minimus"
-version = "2.0.0"
+version = "2.0.1"
 authors = [
     { name = "Igor Zyktin", email = "nicord@yandex.ru" },
 ]
 description = "Personal knowledge storage formatter"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

