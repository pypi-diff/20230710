# Comparing `tmp/NekoGram-2.1.0.tar.gz` & `tmp/NekoGram-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NekoGram-2.1.0.tar", last modified: Sat Mar  4 12:26:54 2023, max compression
+gzip compressed data, was "NekoGram-2.2.0.tar", last modified: Mon Jul 10 09:47:25 2023, max compression
```

## Comparing `NekoGram-2.1.0.tar` & `NekoGram-2.2.0.tar`

### file list

```diff
@@ -1,76 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-03-04 12:26:54.884647 NekoGram-2.1.0/
--rw-rw-rw-   0        0        0     1086 2021-07-29 12:59:10.000000 NekoGram-2.1.0/LICENSE
--rw-rw-rw-   0        0        0    17999 2023-03-04 12:26:54.884647 NekoGram-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    16128 2022-11-11 15:21:46.000000 NekoGram-2.1.0/README.md
--rw-rw-rw-   0        0        0      966 2023-03-04 12:25:51.000000 NekoGram-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-04 12:26:54.884647 NekoGram-2.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-04 12:26:54.784577 NekoGram-2.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-04 12:26:54.809889 NekoGram-2.1.0/src/NekoGram/
--rw-rw-rw-   0        0        0       78 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/__init__.py
--rw-rw-rw-   0        0        0     6702 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/base_neko.py
--rw-rw-rw-   0        0        0     8273 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/filters.py
-drwxrwxrwx   0        0        0        0 2023-03-04 12:26:54.815639 NekoGram-2.1.0/src/NekoGram/handlers/
--rw-rw-rw-   0        0        0       92 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/handlers/__init__.py
--rw-rw-rw-   0        0        0     1877 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/handlers/callback.py
--rw-rw-rw-   0        0        0     5281 2023-03-03 12:13:23.000000 NekoGram-2.1.0/src/NekoGram/handlers/message.py
--rw-rw-rw-   0        0        0       71 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/logger.py
--rw-rw-rw-   0        0        0    11212 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/menus.py
--rw-rw-rw-   0        0        0    16487 2023-03-03 11:35:14.000000 NekoGram-2.1.0/src/NekoGram/neko.py
--rw-rw-rw-   0        0        0     4372 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/router.py
-drwxrwxrwx   0        0        0        0 2023-03-04 12:26:54.825680 NekoGram-2.1.0/src/NekoGram/storages/
--rw-rw-rw-   0        0        0       80 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/storages/__init__.py
--rw-rw-rw-   0        0        0     2893 2023-03-03 12:21:07.000000 NekoGram-2.1.0/src/NekoGram/storages/base_storage.py
--rw-rw-rw-   0        0        0     3847 2023-03-04 12:11:32.000000 NekoGram-2.1.0/src/NekoGram/storages/memory_storage.py
-drwxrwxrwx   0        0        0        0 2023-03-04 12:26:54.834700 NekoGram-2.1.0/src/NekoGram/storages/mysql/
--rw-rw-rw-   0        0        0       51 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/storages/mysql/__init__.py
--rw-rw-rw-   0        0        0    13819 2023-03-03 12:13:23.000000 NekoGram-2.1.0/src/NekoGram/storages/mysql/mysql.py
--rw-rw-rw-   0        0        0     1114 2023-03-03 10:27:47.000000 NekoGram-2.1.0/src/NekoGram/storages/mysql/tables.json
-drwxrwxrwx   0        0        0        0 2023-03-04 12:26:54.835782 NekoGram-2.1.0/src/NekoGram/storages/pg/
--rw-rw-rw-   0        0        0       26 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/storages/pg/__init__.py
--rw-rw-rw-   0        0        0     7366 2023-03-04 12:11:32.000000 NekoGram-2.1.0/src/NekoGram/storages/pg/pg.py
-drwxrwxrwx   0        0        0        0 2023-03-04 12:26:54.844314 NekoGram-2.1.0/src/NekoGram/text_processors/
--rw-rw-rw-   0        0        0       84 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/text_processors/__init__.py
--rw-rw-rw-   0        0        0      437 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/text_processors/base_processor.py
--rw-rw-rw-   0        0        0     3182 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/text_processors/json_processor.py
--rw-rw-rw-   0        0        0     2704 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/utils.py
--rw-rw-rw-   0        0        0     1310 2023-03-04 12:17:51.000000 NekoGram-2.1.0/src/NekoGram/webhook.py
-drwxrwxrwx   0        0        0        0 2023-03-04 12:26:54.844314 NekoGram-2.1.0/src/NekoGram/widgets/
--rw-rw-rw-   0        0        0       42 2023-03-03 11:35:14.000000 NekoGram-2.1.0/src/NekoGram/widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-04 12:26:54.857769 NekoGram-2.1.0/src/NekoGram/widgets/broadcast/
--rw-rw-rw-   0        0        0      128 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/widgets/broadcast/__init__.py
--rw-rw-rw-   0        0        0     1898 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/widgets/broadcast/formatters.py
--rw-rw-rw-   0        0        0     5287 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/widgets/broadcast/functions.py
-drwxrwxrwx   0        0        0        0 2023-03-04 12:26:54.857769 NekoGram-2.1.0/src/NekoGram/widgets/broadcast/translations/
--rw-rw-rw-   0        0        0     2058 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/widgets/broadcast/translations/en.json
--rw-rw-rw-   0        0        0     2134 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/widgets/broadcast/translations/pl.json
--rw-rw-rw-   0        0        0     2390 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/widgets/broadcast/translations/ru.json
--rw-rw-rw-   0        0        0     2380 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/widgets/broadcast/translations/uk.json
--rw-rw-rw-   0        0        0       77 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/widgets/broadcast/util.py
--rw-rw-rw-   0        0        0     1803 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/widgets/broadcast/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-04 12:26:54.864289 NekoGram-2.1.0/src/NekoGram/widgets/languages/
--rw-rw-rw-   0        0        0      128 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/widgets/languages/__init__.py
--rw-rw-rw-   0        0        0      646 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/widgets/languages/formatters.py
--rw-rw-rw-   0        0        0      447 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/widgets/languages/functions.py
--rw-rw-rw-   0        0        0       44 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/widgets/languages/replacements.json
-drwxrwxrwx   0        0        0        0 2023-03-04 12:26:54.875619 NekoGram-2.1.0/src/NekoGram/widgets/languages/translations/
--rw-rw-rw-   0        0        0      262 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/widgets/languages/translations/en.json
--rw-rw-rw-   0        0        0      272 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/widgets/languages/translations/he.json
--rw-rw-rw-   0        0        0      260 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/widgets/languages/translations/pl.json
--rw-rw-rw-   0        0        0      284 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/widgets/languages/translations/ru.json
--rw-rw-rw-   0        0        0      280 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/widgets/languages/translations/uk.json
--rw-rw-rw-   0        0        0      371 2023-03-03 10:18:38.000000 NekoGram-2.1.0/src/NekoGram/widgets/languages/util.py
-drwxrwxrwx   0        0        0        0 2023-03-04 12:26:54.883635 NekoGram-2.1.0/src/NekoGram/widgets/stats/
--rw-rw-rw-   0        0        0      128 2023-03-03 11:35:14.000000 NekoGram-2.1.0/src/NekoGram/widgets/stats/__init__.py
--rw-rw-rw-   0        0        0      902 2023-03-03 12:17:25.000000 NekoGram-2.1.0/src/NekoGram/widgets/stats/formatters.py
--rw-rw-rw-   0        0        0       79 2023-03-04 12:11:32.000000 NekoGram-2.1.0/src/NekoGram/widgets/stats/functions.py
-drwxrwxrwx   0        0        0        0 2023-03-04 12:26:54.884647 NekoGram-2.1.0/src/NekoGram/widgets/stats/sql/
--rw-rw-rw-   0        0        0     1003 2023-03-03 15:20:54.000000 NekoGram-2.1.0/src/NekoGram/widgets/stats/sql/tables.json
-drwxrwxrwx   0        0        0        0 2023-03-04 12:26:54.884647 NekoGram-2.1.0/src/NekoGram/widgets/stats/translations/
--rw-rw-rw-   0        0        0      223 2023-03-03 12:18:33.000000 NekoGram-2.1.0/src/NekoGram/widgets/stats/translations/en.json
--rw-rw-rw-   0        0        0     2538 2023-03-03 15:30:24.000000 NekoGram-2.1.0/src/NekoGram/widgets/stats/util.py
-drwxrwxrwx   0        0        0        0 2023-03-04 12:26:54.815639 NekoGram-2.1.0/src/NekoGram.egg-info/
--rw-rw-rw-   0        0        0    17999 2023-03-04 12:26:54.000000 NekoGram-2.1.0/src/NekoGram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2132 2023-03-04 12:26:54.000000 NekoGram-2.1.0/src/NekoGram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-04 12:26:54.000000 NekoGram-2.1.0/src/NekoGram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-03-04 12:26:54.000000 NekoGram-2.1.0/src/NekoGram.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-04 12:26:54.000000 NekoGram-2.1.0/src/NekoGram.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.148330 NekoGram-2.2.0/
+-rw-rw-rw-   0        0        0     1086 2021-07-29 12:59:10.000000 NekoGram-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0    17999 2023-07-10 09:47:25.147329 NekoGram-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    16128 2022-11-11 15:21:46.000000 NekoGram-2.2.0/README.md
+-rw-rw-rw-   0        0        0      966 2023-07-10 09:47:18.000000 NekoGram-2.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-10 09:47:25.148330 NekoGram-2.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.082633 NekoGram-2.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.099134 NekoGram-2.2.0/src/NekoGram/
+-rw-rw-rw-   0        0        0       78 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/__init__.py
+-rw-rw-rw-   0        0        0     6752 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/base_neko.py
+-rw-rw-rw-   0        0        0     8274 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/filters.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.114417 NekoGram-2.2.0/src/NekoGram/handlers/
+-rw-rw-rw-   0        0        0       92 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/handlers/__init__.py
+-rw-rw-rw-   0        0        0     1919 2023-06-18 11:48:30.000000 NekoGram-2.2.0/src/NekoGram/handlers/callback.py
+-rw-rw-rw-   0        0        0     5421 2023-06-18 11:48:30.000000 NekoGram-2.2.0/src/NekoGram/handlers/message.py
+-rw-rw-rw-   0        0        0       72 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/logger.py
+-rw-rw-rw-   0        0        0    11418 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/menus.py
+-rw-rw-rw-   0        0        0    16959 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/neko.py
+-rw-rw-rw-   0        0        0     4373 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/router.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.115924 NekoGram-2.2.0/src/NekoGram/storages/
+-rw-rw-rw-   0        0        0       39 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/storages/__init__.py
+-rw-rw-rw-   0        0        0     3460 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/storages/base_storage.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.118475 NekoGram-2.2.0/src/NekoGram/storages/mysql/
+-rw-rw-rw-   0        0        0       51 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/storages/mysql/__init__.py
+-rw-rw-rw-   0        0        0    16032 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/storages/mysql/mysql.py
+-rw-rw-rw-   0        0        0     1114 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/storages/mysql/tables.json
+drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.119978 NekoGram-2.2.0/src/NekoGram/storages/pg/
+-rw-rw-rw-   0        0        0       43 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/storages/pg/__init__.py
+-rw-rw-rw-   0        0        0    11705 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/storages/pg/pg.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.121986 NekoGram-2.2.0/src/NekoGram/storages/sqlite/
+-rw-rw-rw-   0        0        0       55 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/storages/sqlite/__init__.py
+-rw-rw-rw-   0        0        0    11324 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/storages/sqlite/sqlite.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.123491 NekoGram-2.2.0/src/NekoGram/text_processors/
+-rw-rw-rw-   0        0        0       84 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/text_processors/__init__.py
+-rw-rw-rw-   0        0        0      437 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/text_processors/base_processor.py
+-rw-rw-rw-   0        0        0     3183 2023-06-18 11:48:30.000000 NekoGram-2.2.0/src/NekoGram/text_processors/json_processor.py
+-rw-rw-rw-   0        0        0     2710 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/utils.py
+-rw-rw-rw-   0        0        0     1311 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/webhook.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.124498 NekoGram-2.2.0/src/NekoGram/widgets/
+-rw-rw-rw-   0        0        0       42 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.128873 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/
+-rw-rw-rw-   0        0        0      128 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/__init__.py
+-rw-rw-rw-   0        0        0     1923 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/formatters.py
+-rw-rw-rw-   0        0        0     5410 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/functions.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.131986 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/translations/
+-rw-rw-rw-   0        0        0     2058 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/translations/en.json
+-rw-rw-rw-   0        0        0     2134 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/translations/pl.json
+-rw-rw-rw-   0        0        0     2390 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/translations/ru.json
+-rw-rw-rw-   0        0        0     2380 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/translations/uk.json
+-rw-rw-rw-   0        0        0       77 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/util.py
+-rw-rw-rw-   0        0        0     1804 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.136942 NekoGram-2.2.0/src/NekoGram/widgets/languages/
+-rw-rw-rw-   0        0        0      128 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/languages/__init__.py
+-rw-rw-rw-   0        0        0      648 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/widgets/languages/formatters.py
+-rw-rw-rw-   0        0        0      449 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/widgets/languages/functions.py
+-rw-rw-rw-   0        0        0       44 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/languages/replacements.json
+drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.140500 NekoGram-2.2.0/src/NekoGram/widgets/languages/translations/
+-rw-rw-rw-   0        0        0      262 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/languages/translations/en.json
+-rw-rw-rw-   0        0        0      272 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/languages/translations/he.json
+-rw-rw-rw-   0        0        0      260 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/languages/translations/pl.json
+-rw-rw-rw-   0        0        0      284 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/languages/translations/ru.json
+-rw-rw-rw-   0        0        0      280 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/languages/translations/uk.json
+-rw-rw-rw-   0        0        0      373 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/widgets/languages/util.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.144308 NekoGram-2.2.0/src/NekoGram/widgets/stats/
+-rw-rw-rw-   0        0        0      128 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/stats/__init__.py
+-rw-rw-rw-   0        0        0      905 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/widgets/stats/formatters.py
+-rw-rw-rw-   0        0        0       80 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/widgets/stats/functions.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.145819 NekoGram-2.2.0/src/NekoGram/widgets/stats/sql/
+-rw-rw-rw-   0        0        0     1003 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/stats/sql/tables.json
+drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.146323 NekoGram-2.2.0/src/NekoGram/widgets/stats/translations/
+-rw-rw-rw-   0        0        0      223 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/stats/translations/en.json
+-rw-rw-rw-   0        0        0     2540 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/widgets/stats/util.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.110903 NekoGram-2.2.0/src/NekoGram.egg-info/
+-rw-rw-rw-   0        0        0    17999 2023-07-10 09:47:25.000000 NekoGram-2.2.0/src/NekoGram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2023-07-10 09:47:25.000000 NekoGram-2.2.0/src/NekoGram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 09:47:25.000000 NekoGram-2.2.0/src/NekoGram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-10 09:47:25.000000 NekoGram-2.2.0/src/NekoGram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-10 09:47:25.000000 NekoGram-2.2.0/src/NekoGram.egg-info/top_level.txt
```

### Comparing `NekoGram-2.1.0/LICENSE` & `NekoGram-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `NekoGram-2.1.0/PKG-INFO` & `NekoGram-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NekoGram
-Version: 2.1.0
+Version: 2.2.0
 Summary: Creating bots has never been simpler.
 Author-email: lyteloli <me@lyteloli.space>
 License: MIT License
         
         Copyright (c) 2020 lyteloli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `NekoGram-2.1.0/README.md` & `NekoGram-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `NekoGram-2.1.0/pyproject.toml` & `NekoGram-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NekoGram"
-version = "2.1.0"
+version = "2.2.0"
 authors = [
   { name="lyteloli", email="me@lyteloli.space" },
 ]
 description = "Creating bots has never been simpler."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `NekoGram-2.1.0/src/NekoGram/base_neko.py` & `NekoGram-2.2.0/src/NekoGram/base_neko.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,161 +1,159 @@
-from typing import Optional, Dict, List, Union, Any, Callable, Awaitable
-from aiogram.dispatcher.filters.builtin import ChatTypeFilter
-from .text_processors import BaseProcessor, JSONProcessor
-from .filters import StartsWith, HasMenu, BuiltInFilters
-from aiogram import Bot, Dispatcher, executor, types
-from .storages import BaseStorage, MemoryStorage
-from aiogram.dispatcher.filters import Filter
-from abc import ABC, abstractmethod
-from .logger import LOGGER
-from . import handlers
-
-
-class BaseNeko(ABC):
-    def __init__(self, storage: Optional[BaseStorage] = None, token: Optional[str] = None, bot: Optional[Bot] = None,
-                 dp: Optional[Dispatcher] = None, text_processor: Optional[BaseProcessor] = None,
-                 entrypoint: str = 'start', menu_prefixes: Union[List[str]] = 'menu_',
-                 callback_parameters_delimiter: str = '#'):
-        """
-        Initialize a Neko
-        :param storage: A class that inherits from BaseDatabase class
-        :param token: Telegram bot token
-        :param bot: Aiogram Bot object
-        :param dp: Aiogram Dispatcher object
-        :param text_processor: A text processor to use (a class inherited from text_processors.BaseProcessor),
-        JSONProcessor by default
-        :param entrypoint: App entrypoint menu name (defaults to start)
-        :param menu_prefixes: Common prefixes for menus defined in translation files
-        :param callback_parameters_delimiter: A delimiter for callback data arguments
-        """
-        self.bot: Bot
-        self.dp: Dispatcher
-        if dp:
-            self.bot, self.dp = (dp.bot, dp)
-        elif bot:
-            self.bot, self.dp = (bot, Dispatcher(bot=bot))
-        elif token:
-            self.bot = Bot(token=token)
-            self.dp = Dispatcher(bot=self.bot)
-        else:
-            raise ValueError('No Dispatcher, Bot or token provided during Neko initialization')
-
-        if storage is None:
-            storage = MemoryStorage()
-        self.storage: BaseStorage = storage
-
-        if text_processor is None:
-            text_processor = JSONProcessor()
-        self.text_processor: BaseProcessor = text_processor
-
-        if type(storage) == MemoryStorage:  # Check if MemoryStorage is used
-            LOGGER.warning('You are using MemoryStorage which does not store data permanently! *sigh of condemnation*')
-
-        if isinstance(menu_prefixes, str):
-            menu_prefixes = [menu_prefixes]
-        self._entrypoint: str = entrypoint
-        self.menu_prefixes: List[str] = menu_prefixes
-        self.filters: Dict[str, callable] = dict()
-        self.callback_parameters_delimiter: str = callback_parameters_delimiter
-        self.register_handlers()
-
-        builtin_filters = BuiltInFilters()
-        for f in builtin_filters.to_list:
-            self.filters[f] = getattr(builtin_filters, f'is_{f}')
-
-        self.functions: Dict[str, Callable[[Any, Union[types.Message, types.CallbackQuery, types.InlineQuery],
-                                            BaseNeko], Awaitable[Any]]] = dict()
-        self.format_functions: Dict[str, Callable[[Any, types.User, BaseNeko], Awaitable[Any]]] = dict()
-        self.prev_menu_handlers: Dict[str, Callable[[Any], Awaitable[str]]] = dict()
-        self.next_menu_handlers: Dict[str, Callable[[Any], Awaitable[str]]] = dict()
-        self._markup_overriders: Dict[str, Dict[str, Callable[[Any], Awaitable[List[List[Dict[str, str]]]]]]] = dict()
-
-        print(r'''
-   _  __    __        _____             
-  / |/ /__ / /_____  / ___/______ ___ _ 
- /    / -_)  '_/ _ \/ (_ / __/ _ `/  ' \
-/_/|_/\__/_/\_\\___/\___/_/  \_,_/_/_/_/''')
-
-    def register_handlers(self):
-        """
-        Registers default handlers
-        """
-        self.dp.register_message_handler(handlers.menu_message_handler, ChatTypeFilter(types.ChatType.PRIVATE),
-                                         commands=['start'])
-        for menu_prefix in self.menu_prefixes:
-            self.dp.register_callback_query_handler(handlers.menu_callback_query_handler, StartsWith(menu_prefix))
-        if 'widget_' not in self.menu_prefixes:
-            self.dp.register_callback_query_handler(handlers.menu_callback_query_handler, StartsWith('widget_'))
-        self.dp.register_message_handler(handlers.menu_message_handler, ChatTypeFilter(types.ChatType.PRIVATE),
-                                         HasMenu(self.storage), content_types=types.ContentType.ANY)
-
-    def add_filter(self, name: str, callback: Union[callable, Filter]):
-        if self.filters.get(name):
-            LOGGER.warning(f'Filter named {name} was overridden. *eyes filling with tears*')
-
-        if isinstance(callback, Filter):
-            callback = callback.check
-        self.filters[name] = callback
-
-    def remove_filter(self, name: str):
-        self.filters.pop(name)
-
-    @abstractmethod
-    def get_widget_data(self, key: str) -> Optional[Any]:
-        pass
-
-    @abstractmethod
-    def get_full_widget_data(self) -> Dict[str, Any]:
-        pass
-
-    @abstractmethod
-    async def check_text_exists(self, text: str, lang: Optional[str] = None) -> bool:
-        pass
-
-    def start_polling(self, on_startup: Optional[callable] = None, on_shutdown: Optional[callable] = None):
-        executor.start_polling(self.dp, on_startup=on_startup, on_shutdown=on_shutdown)
-
-    @abstractmethod
-    def register_formatter(self, callback: callable, name: Optional[str] = None):
-        pass
-
-    @abstractmethod
-    def formatter(self, name: Optional[str] = None):
-        pass
-
-    @abstractmethod
-    def register_function(self, callback: callable, name: Optional[str] = None):
-        pass
-
-    @abstractmethod
-    def function(self, name: Optional[str] = None):
-        pass
-
-    @abstractmethod
-    def register_prev_menu_handler(self, callback: callable, name: Optional[str] = None):
-        pass
-
-    @abstractmethod
-    def prev_menu_handler(self, name: Optional[str] = None):
-        pass
-
-    @abstractmethod
-    def register_next_menu_handler(self, callback: callable, name: Optional[str] = None):
-        pass
-
-    @abstractmethod
-    def next_menu_handler(self, name: Optional[str] = None):
-        pass
-
-    @abstractmethod
-    def register_markup_overrider(self, callback: callable, lang: str, name: Optional[str] = None):
-        pass
-
-    @abstractmethod
-    def markup_overrider(self, lang: str, name: Optional[str] = None):
-        pass
-
-    @abstractmethod
-    async def build_menu(self, name: str, obj: Union[types.Message, types.CallbackQuery, types.InlineQuery],
-                         user_id: Optional[int] = None, callback_data: Optional[Union[str, int]] = None,
-                         auto_build: bool = True):
-        pass
+from typing import Optional, Dict, List, Union, Any, Callable, Awaitable
+from aiogram.dispatcher.filters.builtin import ChatTypeFilter
+from aiogram import Bot, Dispatcher, executor, types
+from aiogram.dispatcher.filters import Filter
+from abc import ABC, abstractmethod
+
+from .text_processors import BaseProcessor, JSONProcessor
+from .filters import StartsWith, HasMenu, BuiltInFilters
+from .storages import BaseStorage
+from .logger import LOGGER
+from . import handlers
+
+
+class BaseNeko(ABC):
+    def __init__(self, storage: Optional[BaseStorage], token: Optional[str] = None, bot: Optional[Bot] = None,
+                 dp: Optional[Dispatcher] = None, text_processor: Optional[BaseProcessor] = None,
+                 entrypoint: str = 'start', menu_prefixes: Union[List[str]] = 'menu_',
+                 callback_parameters_delimiter: str = '#', delete_messages: bool = True):
+        """
+        Initialize a Neko
+        :param storage: A class that inherits from BaseDatabase class
+        :param token: Telegram bot token
+        :param bot: Aiogram Bot object
+        :param dp: Aiogram Dispatcher object
+        :param text_processor: A text processor to use (a class inherited from text_processors.BaseProcessor),
+        JSONProcessor by default
+        :param entrypoint: App entrypoint menu name (defaults to start)
+        :param menu_prefixes: Common prefixes for menus defined in translation files
+        :param callback_parameters_delimiter: A delimiter for callback data arguments
+        :param delete_messages: Whether to delete old messages in conversation automatically
+        """
+        self.bot: Bot
+        self.dp: Dispatcher
+        if dp:
+            self.bot, self.dp = (dp.bot, dp)
+        elif bot:
+            self.bot, self.dp = (bot, Dispatcher(bot=bot))
+        elif token:
+            self.bot = Bot(token=token)
+            self.dp = Dispatcher(bot=self.bot)
+        else:
+            raise ValueError('No Dispatcher, Bot or token provided during Neko initialization')
+
+        self.storage: BaseStorage = storage
+
+        if text_processor is None:
+            text_processor = JSONProcessor()
+        self.text_processor: BaseProcessor = text_processor
+
+        if isinstance(menu_prefixes, str):
+            menu_prefixes = [menu_prefixes]
+        self._entrypoint: str = entrypoint
+        self.menu_prefixes: List[str] = menu_prefixes
+        self.filters: Dict[str, callable] = dict()
+        self.callback_parameters_delimiter: str = callback_parameters_delimiter
+        self.register_handlers()
+
+        builtin_filters = BuiltInFilters()
+        for f in builtin_filters.to_list:
+            self.filters[f] = getattr(builtin_filters, f'is_{f}')
+
+        self.functions: Dict[str, Callable[[Any, Union[types.Message, types.CallbackQuery, types.InlineQuery],
+                                            BaseNeko], Awaitable[Any]]] = dict()
+        self.format_functions: Dict[str, Callable[[Any, types.User, BaseNeko], Awaitable[Any]]] = dict()
+        self.prev_menu_handlers: Dict[str, Callable[[Any], Awaitable[str]]] = dict()
+        self.next_menu_handlers: Dict[str, Callable[[Any], Awaitable[str]]] = dict()
+        self._markup_overriders: Dict[str, Dict[str, Callable[[Any], Awaitable[List[List[Dict[str, str]]]]]]] = dict()
+        self.delete_messages: bool = delete_messages
+
+        print(r'''
+   _  __    __        _____             
+  / |/ /__ / /_____  / ___/______ ___ _ 
+ /    / -_)  '_/ _ \/ (_ / __/ _ `/  ' \
+/_/|_/\__/_/\_\\___/\___/_/  \_,_/_/_/_/''')
+
+    def register_handlers(self):
+        """
+        Registers default handlers
+        """
+        self.dp.register_message_handler(handlers.menu_message_handler, ChatTypeFilter(types.ChatType.PRIVATE),
+                                         commands=['start'])
+        for menu_prefix in self.menu_prefixes:
+            self.dp.register_callback_query_handler(handlers.menu_callback_query_handler, StartsWith(menu_prefix))
+        if 'widget_' not in self.menu_prefixes:
+            self.dp.register_callback_query_handler(handlers.menu_callback_query_handler, StartsWith('widget_'))
+        self.dp.register_message_handler(handlers.menu_message_handler, ChatTypeFilter(types.ChatType.PRIVATE),
+                                         HasMenu(self.storage), content_types=types.ContentType.ANY)
+
+    def add_filter(self, name: str, callback: Union[callable, Filter]):
+        if self.filters.get(name):
+            LOGGER.warning(f'Filter named {name} was overridden. *eyes filling with tears*')
+
+        if isinstance(callback, Filter):
+            callback = callback.check
+        self.filters[name] = callback
+
+    def remove_filter(self, name: str):
+        self.filters.pop(name)
+
+    @abstractmethod
+    def get_widget_data(self, key: str) -> Optional[Any]:
+        pass
+
+    @abstractmethod
+    def get_full_widget_data(self) -> Dict[str, Any]:
+        pass
+
+    @abstractmethod
+    async def check_text_exists(self, text: str, lang: Optional[str] = None) -> bool:
+        pass
+
+    def start_polling(self, on_startup: Optional[callable] = None, on_shutdown: Optional[callable] = None):
+        executor.start_polling(self.dp, on_startup=on_startup, on_shutdown=on_shutdown)
+
+    @abstractmethod
+    def register_formatter(self, callback: callable, name: Optional[str] = None):
+        pass
+
+    @abstractmethod
+    def formatter(self, name: Optional[str] = None):
+        pass
+
+    @abstractmethod
+    def register_function(self, callback: callable, name: Optional[str] = None):
+        pass
+
+    @abstractmethod
+    def function(self, name: Optional[str] = None):
+        pass
+
+    @abstractmethod
+    def register_prev_menu_handler(self, callback: callable, name: Optional[str] = None):
+        pass
+
+    @abstractmethod
+    def prev_menu_handler(self, name: Optional[str] = None):
+        pass
+
+    @abstractmethod
+    def register_next_menu_handler(self, callback: callable, name: Optional[str] = None):
+        pass
+
+    @abstractmethod
+    def next_menu_handler(self, name: Optional[str] = None):
+        pass
+
+    @abstractmethod
+    def register_markup_overrider(self, callback: callable, lang: str, name: Optional[str] = None):
+        pass
+
+    @abstractmethod
+    def markup_overrider(self, lang: str, name: Optional[str] = None):
+        pass
+
+    @abstractmethod
+    async def build_menu(self, name: str, obj: Union[types.Message, types.CallbackQuery, types.InlineQuery],
+                         user_id: Optional[int] = None, callback_data: Optional[Union[str, int]] = None,
+                         auto_build: bool = True):
+        pass
```

### Comparing `NekoGram-2.1.0/src/NekoGram/filters.py` & `NekoGram-2.2.0/src/NekoGram/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from aiogram.dispatcher.filters import Filter
 from aiogram.types import Message, CallbackQuery
 from typing import Dict, List, Any, Union, Optional
-from .storages.base_storage import BaseStorage
 import re
 
+from .storages.base_storage import BaseStorage
+
 
 class HasMenu(Filter):
     def __init__(self, database: BaseStorage):
         self.database: BaseStorage = database
 
     @classmethod
     def validate(cls, _: Dict[str, Any]):
```

### Comparing `NekoGram-2.1.0/src/NekoGram/handlers/callback.py` & `NekoGram-2.2.0/src/NekoGram/handlers/callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from aiogram import exceptions as aiogram_exceptions, types
 from typing import List, Optional, Union
 from contextlib import suppress
+
 import NekoGram
 
 
 def _convert_call_data(call_data: List[str]) -> Optional[Union[str, int]]:
     if len(call_data) == 1:
         return None
 
@@ -31,12 +32,13 @@
             await intermediate_menu.edit_text()
         await neko.functions[current_menu.name](current_menu, call, neko)
         return
 
     try:
         await current_menu.edit_text()
     except aiogram_exceptions.InlineKeyboardExpected:
-        with suppress(Exception):
-            await call.message.delete()
+        if neko.delete_messages:
+            with suppress(Exception):
+                await call.message.delete()
         await current_menu.send_message()
     except (aiogram_exceptions.MessageCantBeEdited, aiogram_exceptions.MessageToEditNotFound):
         await current_menu.send_message()
```

### Comparing `NekoGram-2.1.0/src/NekoGram/handlers/message.py` & `NekoGram-2.2.0/src/NekoGram/handlers/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from aiogram import types, exceptions as aiogram_exc
 from typing import Union, Dict, Any, Optional
 from contextlib import suppress
+
 from ..logger import LOGGER
 import NekoGram
 
 
 async def default_start_handler(message: types.Message):
     neko: NekoGram.Neko = message.conf['neko']
 
@@ -22,16 +23,17 @@
         raise RuntimeError(f'Start menu formatter should not break execution')
 
     if neko.functions.get('start'):
         await neko.functions['start'](current_menu, message, neko)
         return
     else:
         await current_menu.send_message()
-        with suppress(Exception):
-            await message.delete()
+        if neko.delete_messages:
+            with suppress(Exception):
+                await message.delete()
 
 
 async def menu_message_handler(message: types.Message):
     neko: NekoGram.Neko = message.conf['neko']
     if message.text and message.text.startswith('/start'):  # Start case
         await default_start_handler(message)
         return
@@ -42,30 +44,32 @@
     current_menu = await neko.build_menu(name=user_data['menu'], obj=message)  # Prebuild current menu
     if current_menu is None:
         return
 
     if message.text and message.text.startswith('⬅️'):  # Back button clicked
         await neko.storage.set_user_menu(menu=current_menu.prev_menu or None, user_id=message.from_user.id,
                                          bot_token=bot_token)
-        last_message_id = await neko.storage.get_last_message_id(user_id=message.from_user.id)
-        try:
-            await neko.bot.delete_message(chat_id=message.from_user.id, message_id=last_message_id)
-        except (aiogram_exc.MessageCantBeDeleted, aiogram_exc.MessageToDeleteNotFound):
-            with suppress(Exception):
-                await neko.bot.edit_message_reply_markup(chat_id=message.from_user.id, message_id=last_message_id)
+        if neko.delete_messages:
+            last_message_id = await neko.storage.get_last_message_id(user_id=message.from_user.id)
+            try:
+                await neko.bot.delete_message(chat_id=message.from_user.id, message_id=last_message_id)
+            except (aiogram_exc.MessageCantBeDeleted, aiogram_exc.MessageToDeleteNotFound):
+                with suppress(Exception):
+                    await neko.bot.edit_message_reply_markup(chat_id=message.from_user.id, message_id=last_message_id)
 
         if neko.prev_menu_handlers.get(current_menu.name):
             current_menu.prev_menu = await neko.prev_menu_handlers[current_menu.name](current_menu)
         menu = await neko.build_menu(name=current_menu.prev_menu or 'start', obj=message)
         if menu is None:
             return
         await menu.send_message()
 
-        with suppress(Exception):
-            await message.delete()
+        if neko.delete_messages:
+            with suppress(Exception):
+                await message.delete()
         return
 
     if current_menu.filters:  # Check filters
         filters_passed: bool = False
         for f in current_menu.filters:
             if await neko.filters[f](message):
                 filters_passed = True
```

### Comparing `NekoGram-2.1.0/src/NekoGram/menus.py` & `NekoGram-2.2.0/src/NekoGram/menus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Optional, Union, Dict, List, Any, Type
 from contextlib import suppress
-from .base_neko import BaseNeko
 from aiogram import types
+
+from .base_neko import BaseNeko
 from .logger import LOGGER
 
 
 class Menu:
     __default_keyboard_values: Dict[str, str] = {'callback_data': 'call_data', 'switch_inline_query': 'query',
                                                  'switch_inline_query_current_chat': 'cc_query',
-                                                 'text': 'text', 'url': 'url'}
+                                                 'text': 'text', 'url': 'url', 'menu': 'call_data'}
     __inline_markup_identifiers: List[str] = ['call_data', 'callback_data', 'query', 'switch_inline_query', 'cc_query',
                                               'switch_inline_query_current_chat', 'url']
 
     def __init__(self, name: str, obj: Union[types.Message, types.CallbackQuery, types.InlineQuery],
                  markup: Optional[List[List[Dict[str, str]]]] = None, markup_row_width: Optional[int] = None,
                  text: Optional[str] = None, no_preview: Optional[bool] = None, parse_mode: Optional[str] = None,
                  silent: Optional[bool] = None, validation_error: Optional[str] = None,
@@ -36,17 +37,21 @@
         self.keyboard_values_to_format = keyboard_values_to_format or list(self.__default_keyboard_values.keys())
         self.markup_type: Optional[str] = markup_type
         self.prev_menu: Optional[str] = prev_menu
         self.next_menu: Optional[str] = next_menu
         self.filters: Optional[List[str]] = filters
         self._call_data: Optional[Union[str, int]] = callback_data
         self.bot_token: Optional[str] = bot_token
+        self.bot_id: Optional[int] = None
         self.intermediate_menu: Optional[str] = intermediate_menu
         self._break_execution: bool = False
 
+        if self.bot_token:
+            self.bot_id = int(self.bot_token.split(':')[0])
+
     def break_execution(self):
         self._break_execution = True
 
     @property
     def is_broken(self) -> bool:
         return self._break_execution
 
@@ -75,18 +80,19 @@
         :return: Sent message
         """
         if user_id is None:
             user_id = self.obj.from_user.id
         msg = await self.obj.bot.send_message(chat_id=user_id, text=self.text,
                                               parse_mode=self.parse_mode, disable_web_page_preview=self.no_preview,
                                               disable_notification=self.silent, reply_markup=self.markup)
-        last_message_id = await self.neko.storage.get_last_message_id(user_id=user_id)
-        await self.neko.storage.set_last_message_id(user_id=user_id, message_id=msg.message_id)
-        with suppress(Exception):
-            await self.obj.bot.delete_message(chat_id=user_id, message_id=last_message_id)
+        if self.neko.delete_messages:
+            last_message_id = await self.neko.storage.get_last_message_id(user_id=user_id)
+            await self.neko.storage.set_last_message_id(user_id=user_id, message_id=msg.message_id)
+            with suppress(Exception):
+                await self.obj.bot.delete_message(chat_id=user_id, message_id=last_message_id)
         return msg
 
     async def edit_text(self) -> types.Message:
         """
         Edits message text with menu properties
         :return: Edited message
         """
```

### Comparing `NekoGram-2.1.0/src/NekoGram/neko.py` & `NekoGram-2.2.0/src/NekoGram/neko.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,349 +1,352 @@
-from typing import Dict, List, Union, Optional, Any, Callable, Awaitable
-from .webhook import KittyWebhook, KittyExecutor
-from .text_processors import BaseProcessor
-from aiogram import Dispatcher, Bot, types
-from .storages.mysql import MySQLStorage
-from .utils import HandlerInjector
-from .storages import BaseStorage
-from .base_neko import BaseNeko
-from .router import NekoRouter
-from datetime import datetime
-from .logger import LOGGER
-from copy import deepcopy
-from .menus import Menu
-import inspect
-import os
-
-try:
-    import ujson as json
-except ImportError:
-    import json
-
-
-class Neko(BaseNeko):
-    _registration_warned: bool = False
-    _builtin_widgets: List[str] = ['broadcast', 'languages', 'stats']
-    _widgets_warned: bool = False
-    __MENU_ARGS: List[str] = list(inspect.signature(Menu.__init__).parameters.keys())
-
-    def __init__(self, storage: Optional[BaseStorage] = None, token: Optional[str] = None, bot: Optional[Bot] = None,
-                 dp: Optional[Dispatcher] = None, text_processor: Optional[BaseProcessor] = None,
-                 menu_prefixes: Union[List[str]] = 'menu_', load_texts: bool = True,
-                 callback_parameters_delimiter: str = '#', attach_required_middleware: bool = True,
-                 webhook_host: str = 'localhost', webhook_port: Optional[int] = None,
-                 webhook_path: Optional[str] = None, webhook_url: Optional[str] = None):
-        super().__init__(storage=storage, token=token, bot=bot, dp=dp, text_processor=text_processor,
-                         menu_prefixes=menu_prefixes, callback_parameters_delimiter=callback_parameters_delimiter)
-        if attach_required_middleware:
-            self.dp.middleware.setup(HandlerInjector(self))  # Set up the handler injector middleware
-        else:
-            LOGGER.warning('You canceled embedded middleware attachment, this is a dangerous thing to do, make sure '
-                           'you perform same actions in your middleware, otherwise the app will crash or stay idle.')
-
-        self._cached_user_languages: Dict[str, Dict[str, Union[str, datetime]]] = dict()
-        if load_texts:
-            self.text_processor.add_texts()
-        self.widgets: List[str] = list()
-        self.__widget_data: Dict[str, Any] = dict()
-        self.executor: KittyExecutor = KittyExecutor(neko=self)
-        self.__webhook_host: str = webhook_host
-        self.__webhook_port: Optional[int] = webhook_port
-        self.__webhook_path: Optional[str] = webhook_path
-        self.__webhook_url: Optional[str] = webhook_url
-        if webhook_path and '{token}' not in webhook_path:
-            raise ValueError('{token} placeholder has to be present in webhook_path.')
-
-    def get_widget_data(self, key: str) -> Optional[Any]:
-        return self.__widget_data.get(key)
-
-    def get_full_widget_data(self) -> Dict[str, Any]:
-        return self.__widget_data.copy()
-
-    async def check_text_exists(self, text: str, lang: Optional[str] = None) -> bool:
-        if lang is None:
-            lang = list(self.text_processor.texts.keys())[0]
-        return text in self.text_processor.texts[lang].keys()
-
-    def register_formatter(self, callback: Callable[[Menu, types.User, BaseNeko], Awaitable[Any]],
-                           name: Optional[str] = None):
-        """
-        Register a formatter
-        :param callback: A formatter to call
-        :param name: Menu name
-        """
-        if not self._registration_warned:
-            LOGGER.warning('It is not recommended to register formatters and functions within a Neko class, '
-                           'consider using a NekoRouter.')
-            self._registration_warned = True
-        self.format_functions[name or callback.__name__] = callback
-
-    def formatter(self, name: Optional[str] = None):
-        """
-        Register a formatter
-        :param name: Menu name
-        """
-
-        def decorator(callback: Callable[[Menu, types.User, BaseNeko], Awaitable[Any]]):
-            self.register_formatter(callback=callback, name=name)
-            return callback
-
-        return decorator
-
-    def register_function(self, callback: Callable[[Menu, Union[types.Message, types.CallbackQuery], BaseNeko],
-                                                   Awaitable[Any]], name: Optional[str] = None):
-        """
-        Register a function
-        :param callback: A function to call
-        :param name: Menu name
-        """
-        if not self._registration_warned:
-            LOGGER.warning('It is not recommended to register formatters and functions within a Neko class, '
-                           'consider using a NekoRouter.')
-            self._registration_warned = True
-        self.functions[name or callback.__name__] = callback
-
-    def function(self, name: Optional[str] = None):
-        """
-        Register a function
-        :param name: Menu name
-        """
-
-        def decorator(callback: Callable[[Menu, Union[types.Message, types.CallbackQuery], BaseNeko], Awaitable[Any]]):
-            self.register_function(callback=callback, name=name)
-            return callback
-
-        return decorator
-
-    def register_prev_menu_handler(self, callback: Callable[[Menu], Awaitable[str]], name: Optional[str] = None):
-        """
-        Register a prev menu handler
-        :param callback: A prev menu handler to call
-        :param name: Menu name
-        """
-        self.prev_menu_handlers[name or callback.__name__] = callback
-
-    def prev_menu_handler(self, name: Optional[str] = None):
-        """
-        Register a prev menu handler
-        :param name: Menu name
-        """
-
-        def decorator(callback: Callable[[Menu], Awaitable[str]]):
-            self.register_prev_menu_handler(callback=callback, name=name)
-            return callback
-
-        return decorator
-
-    def register_next_menu_handler(self, callback: Callable[[Menu], Awaitable[str]], name: Optional[str] = None):
-        """
-        Register a next menu handler
-        :param callback: A next menu handler to call
-        :param name: Menu name
-        """
-        self.prev_menu_handlers[name or callback.__name__] = callback
-
-    def next_menu_handler(self, name: Optional[str] = None):
-        """
-        Register a next menu handler
-        :param name: Menu name
-        """
-
-        def decorator(callback: Callable[[Menu], Awaitable[str]]):
-            self.register_next_menu_handler(callback=callback, name=name)
-            return callback
-
-        return decorator
-
-    def register_markup_overrider(self, callback: Callable[[Menu], Awaitable[List[List[Dict[str, str]]]]], lang: str,
-                                  name: Optional[str] = None):
-        """
-        Register a markup overrider
-        :param callback: A markup overrider to call
-        :param lang: Language to override markup for
-        :param name: Menu name
-        """
-        if name is None:
-            name = callback.__name__
-        if name not in self._markup_overriders:
-            self._markup_overriders[name] = dict()
-        self._markup_overriders[name][lang] = callback
-
-    def markup_overrider(self, lang: str, name: Optional[str] = None):
-        """
-        Register a markup overrider
-        :param lang: Language to override markup for
-        :param name: Menu name
-        """
-
-        def decorator(callback: Callable[[Menu], Awaitable[List[List[Dict[str, str]]]]]):
-            self.register_markup_overrider(callback=callback, name=name, lang=lang)
-            return callback
-
-        return decorator
-
-    async def build_menu(self, name: str, obj: Union[types.Message, types.CallbackQuery, types.InlineQuery],
-                         user_id: Optional[int] = None,
-                         callback_data: Optional[Union[str, int]] = None,
-                         auto_build: bool = True) -> Optional[Menu]:
-        """
-        Build a menu by its name
-        :param name: Menu name, same as in translation file
-        :param obj: An Aiogram Message or CallbackQuery object
-        :param user_id: An ID of a user to build menu for
-        :param callback_data: Callback data to assign to a menu
-        :param auto_build: Whether to build the Menu if no formatter is defined
-        :return: A Menu object
-        """
-        if name == 'menu_start':  # Start patch
-            name = 'start'
-
-        lang = await self.storage.get_user_language(user_id=user_id or obj.from_user.id)
-        text: Dict[str, Any] = deepcopy(self.text_processor.texts[lang].get(name))
-        if not obj:
-            raise RuntimeError(f'Neither Message nor CallbackQuery was provided during menu building for {name}! '
-                               f'*brain explosion sounds accompanied by intense meowing*')
-        if text is None:  # Try to fetch the menu in another language
-            if 'en' in self.text_processor.texts.keys():
-                text = self.text_processor.texts['en'].get(name)
-            if text is None:
-                for language in self.text_processor.texts.keys():
-                    text = self.text_processor.texts[language].get(name)
-                    if text:
-                        LOGGER.warning(f'{name} menu does not have {lang} translation, using {language}.')
-                        break
-            else:
-                LOGGER.warning(f'{name} menu does not have {lang} translation, using en.')
-            if text is None:
-                raise RuntimeError(f'There is no menu called {name}! *facePAWm*')
-        if text.get('text') is None and text:
-            LOGGER.warning(f'No text provided for {name}. *suspicious stare*')
-
-        text.update(dict(name=name, obj=obj, callback_data=callback_data, bot_token=obj.conf.get('request_token')))
-        args_to_pass: Dict[str, Any] = dict()
-        for key, value in text.items():
-            if key in self.__MENU_ARGS:
-                args_to_pass[key] = value
-            else:
-                LOGGER.warning(f'Field {key} in {name} is extra, it was ignored during Menu initialization.')
-        menu = Menu(**args_to_pass)
-
-        if self._markup_overriders.get(name, dict()).get(lang):
-            menu.raw_markup = await self._markup_overriders[name][lang](menu)
-
-        format_func = self.format_functions.get(name)
-        if format_func:
-            r = await format_func(menu, obj.from_user, self)
-            if isinstance(r, Menu):  # Replace the menu if required
-                menu = r
-            if menu.markup is None and menu.raw_markup:
-                await menu.build()
-        elif auto_build:
-            await menu.build()
-
-        return menu if not menu.is_broken else None
-
-    def attach_router(self, router: NekoRouter):
-        """
-        Attach a NekoRouter to Neko
-        :param router: A NekoRouter to attach
-        """
-        if not router.mark_attached():
-            return
-        self.functions.update(router.functions)
-        self.format_functions.update(router.format_functions)
-        self.prev_menu_handlers.update(router.prev_menu_handlers)
-        self.next_menu_handlers.update(router.next_menu_handlers)
-
-    async def attach_widget(self, formatters_router: NekoRouter, functions_router: NekoRouter,
-                            startup: Callable[[BaseNeko], Awaitable[Optional[Dict[str, Any]]]],
-                            texts_path: Optional[str] = None,
-                            db_table_structure_path: Optional[str] = None,
-                            formatters_to_ignore: Optional[List[str]] = None,
-                            functions_to_ignore: Optional[List[str]] = None):
-        """
-        Attach a widget to Neko
-        :param formatters_router: A NekoRouter object responsible for formatters
-        :param functions_router: A NekoRouter object responsible for functions
-        :param startup: A startup function that returns data required for a widget to work to call
-        :param texts_path: A path to translation files
-        :param db_table_structure_path: A path to table structure file
-        :param formatters_to_ignore: A list of formatter names to ignore
-        :param functions_to_ignore: A list of function names to ignore
-        """
-        if not isinstance(self.storage, MySQLStorage) and not self._widgets_warned:
-            LOGGER.warning(f'Your storage is not MySQLStorage, widgets may function improperly.')
-            self._widgets_warned = True
-        if formatters_router.name is None or formatters_router.name != functions_router.name \
-                or functions_router.name is None:
-            raise RuntimeError('Widget router names must be present and must be same for formatter and function router')
-
-        if formatters_router.name in self.widgets:
-            LOGGER.warning(f'Widget {formatters_router.name} is being attached again, ignored. *ultrasonic meowing*')
-            return
-
-        raw_widget_data = await startup(self)
-        if raw_widget_data:
-            widget_data: Dict[str, Any] = dict()
-            for key, value in raw_widget_data.items():
-                if not key.startswith(f'{formatters_router.name}_'):
-                    LOGGER.warning(f'Widget {formatters_router.name} is not allowed to access `{key}` in widget data, '
-                                   f'all keys for this widget have to start with `{formatters_router.name}_`. '
-                                   'This key was ignored. *visible disappointment*')
-                else:
-                    widget_data[key] = value
-            self.__widget_data.update(widget_data)
-        self.widgets.append(formatters_router.name)
-
-        if formatters_to_ignore:  # Ignore formatters
-            for name, func in formatters_router.format_functions.copy().items():
-                if name in formatters_to_ignore:
-                    formatters_router.format_functions.pop(name)
-
-        if functions_to_ignore:  # Ignore functions
-            for name, func in functions_router.functions.copy().items():
-                if name in functions_to_ignore:
-                    functions_router.functions.pop(name)
-
-        self.attach_router(formatters_router)
-        self.attach_router(functions_router)
-
-        if db_table_structure_path and isinstance(self.storage, MySQLStorage):
-            with open(db_table_structure_path, 'r') as f:
-                table_structure = json.load(f)
-            await self.storage.add_tables(table_structure, required_by=formatters_router.name)
-
-        if texts_path is None:
-            if formatters_router.name in self._builtin_widgets:
-                path = os.path.abspath(__file__).rstrip('neko.py')
-                delim = path[-1]
-                self.text_processor.add_texts(f'{path}widgets{delim}{formatters_router.name}{delim}translations',
-                                              is_widget=True)
-            else:
-                raise RuntimeError(f'Widget {formatters_router.name} is not builtin, '
-                                   'therefore texts_path has to be provided')
-        LOGGER.info(f'{formatters_router.name.capitalize()} widget attached successfully')
-
-    def start_webhook(self, loop=None):
-        """
-        Start webhook
-        :param loop: Abstract asyncio loop
-        """
-        if self.__webhook_path is None or self.__webhook_port is None:
-            raise RuntimeError('You must set webhook_host, webhook_host and webhook_port parameters for a Neko class '
-                               'during initialization to run a webhook')
-        self.executor.start_webhook(webhook_path=self.__webhook_path, host=self.__webhook_host,
-                                    port=self.__webhook_port, request_handler=KittyWebhook, loop=loop)
-
-    async def set_webhook(self, bot_token: str, validate_token: bool = True,
-                          drop_pending_updates: Optional[bool] = None):
-        """
-        Set a webhook for a child bot
-        :param bot_token: Child bot token
-        :param validate_token: Whether to validate a token
-        :param drop_pending_updates: Whether to skip unprocessed updates for a child bot
-        """
-        if self.__webhook_url is None or '{token}' not in self.__webhook_url:
-            raise RuntimeError('webhook_url must be specified and contain {token} placeholder to set a webhook.')
-        with self.bot.with_token(bot_token=bot_token, validate_token=validate_token):
-            await self.bot.set_webhook(url=self.__webhook_url.format(token=bot_token),
-                                       drop_pending_updates=drop_pending_updates)
+from typing import Dict, List, Union, Optional, Any, Callable, Awaitable
+from aiogram import Dispatcher, Bot, types
+from datetime import datetime
+from copy import deepcopy
+import inspect
+import os
+
+try:
+    import ujson as json
+except ImportError:
+    import json
+
+from .webhook import KittyWebhook, KittyExecutor
+from .text_processors import BaseProcessor
+from .utils import HandlerInjector
+from .storages import BaseStorage
+from .base_neko import BaseNeko
+from .router import NekoRouter
+from .logger import LOGGER
+from .menus import Menu
+
+
+class Neko(BaseNeko):
+    _registration_warned: bool = False
+    _builtin_widgets: List[str] = ['broadcast', 'languages', 'stats']
+    _widgets_warned: bool = False
+    __MENU_ARGS: List[str] = list(inspect.signature(Menu.__init__).parameters.keys())
+
+    def __init__(self, storage: Optional[BaseStorage], token: Optional[str] = None, bot: Optional[Bot] = None,
+                 dp: Optional[Dispatcher] = None, text_processor: Optional[BaseProcessor] = None,
+                 menu_prefixes: Union[List[str]] = 'menu_', load_texts: bool = True,
+                 callback_parameters_delimiter: str = '#', attach_required_middleware: bool = True,
+                 webhook_host: str = 'localhost', webhook_port: Optional[int] = None,
+                 webhook_path: Optional[str] = None, webhook_url: Optional[str] = None):
+        super().__init__(storage=storage, token=token, bot=bot, dp=dp, text_processor=text_processor,
+                         menu_prefixes=menu_prefixes, callback_parameters_delimiter=callback_parameters_delimiter)
+        if attach_required_middleware:
+            self.dp.middleware.setup(HandlerInjector(self))  # Set up the handler injector middleware
+        else:
+            LOGGER.warning('You canceled embedded middleware attachment, this is a dangerous thing to do, make sure '
+                           'you perform same actions in your middleware, otherwise the app will crash or stay idle.')
+
+        self._cached_user_languages: Dict[str, Dict[str, Union[str, datetime]]] = dict()
+        if load_texts:
+            self.text_processor.add_texts()
+        self.widgets: List[str] = list()
+        self.__widget_data: Dict[str, Any] = dict()
+        self.executor: KittyExecutor = KittyExecutor(neko=self)
+        self.__webhook_host: str = webhook_host
+        self.__webhook_port: Optional[int] = webhook_port
+        self.__webhook_path: Optional[str] = webhook_path
+        self.__webhook_url: Optional[str] = webhook_url
+        if webhook_path and '{token}' not in webhook_path:
+            raise ValueError('{token} placeholder has to be present in webhook_path.')
+
+    def get_widget_data(self, key: str) -> Optional[Any]:
+        return self.__widget_data.get(key)
+
+    def get_full_widget_data(self) -> Dict[str, Any]:
+        return self.__widget_data.copy()
+
+    async def check_text_exists(self, text: str, lang: Optional[str] = None) -> bool:
+        if lang is None:
+            lang = list(self.text_processor.texts.keys())[0]
+        return text in self.text_processor.texts[lang].keys()
+
+    def register_formatter(self, callback: Callable[[Menu, types.User, BaseNeko], Awaitable[Any]],
+                           name: Optional[str] = None):
+        """
+        Register a formatter
+        :param callback: A formatter to call
+        :param name: Menu name
+        """
+        if not self._registration_warned:
+            LOGGER.warning('It is not recommended to register formatters and functions within a Neko class, '
+                           'consider using a NekoRouter.')
+            self._registration_warned = True
+        self.format_functions[name or callback.__name__] = callback
+
+    def formatter(self, name: Optional[str] = None):
+        """
+        Register a formatter
+        :param name: Menu name
+        """
+
+        def decorator(callback: Callable[[Menu, types.User, BaseNeko], Awaitable[Any]]):
+            self.register_formatter(callback=callback, name=name)
+            return callback
+
+        return decorator
+
+    def register_function(self, callback: Callable[[Menu, Union[types.Message, types.CallbackQuery], BaseNeko],
+                                                   Awaitable[Any]], name: Optional[str] = None):
+        """
+        Register a function
+        :param callback: A function to call
+        :param name: Menu name
+        """
+        if not self._registration_warned:
+            LOGGER.warning('It is not recommended to register formatters and functions within a Neko class, '
+                           'consider using a NekoRouter.')
+            self._registration_warned = True
+        self.functions[name or callback.__name__] = callback
+
+    def function(self, name: Optional[str] = None):
+        """
+        Register a function
+        :param name: Menu name
+        """
+
+        def decorator(callback: Callable[[Menu, Union[types.Message, types.CallbackQuery], BaseNeko], Awaitable[Any]]):
+            self.register_function(callback=callback, name=name)
+            return callback
+
+        return decorator
+
+    def register_prev_menu_handler(self, callback: Callable[[Menu], Awaitable[str]], name: Optional[str] = None):
+        """
+        Register a prev menu handler
+        :param callback: A prev menu handler to call
+        :param name: Menu name
+        """
+        self.prev_menu_handlers[name or callback.__name__] = callback
+
+    def prev_menu_handler(self, name: Optional[str] = None):
+        """
+        Register a prev menu handler
+        :param name: Menu name
+        """
+
+        def decorator(callback: Callable[[Menu], Awaitable[str]]):
+            self.register_prev_menu_handler(callback=callback, name=name)
+            return callback
+
+        return decorator
+
+    def register_next_menu_handler(self, callback: Callable[[Menu], Awaitable[str]], name: Optional[str] = None):
+        """
+        Register a next menu handler
+        :param callback: A next menu handler to call
+        :param name: Menu name
+        """
+        self.prev_menu_handlers[name or callback.__name__] = callback
+
+    def next_menu_handler(self, name: Optional[str] = None):
+        """
+        Register a next menu handler
+        :param name: Menu name
+        """
+
+        def decorator(callback: Callable[[Menu], Awaitable[str]]):
+            self.register_next_menu_handler(callback=callback, name=name)
+            return callback
+
+        return decorator
+
+    def register_markup_overrider(self, callback: Callable[[Menu], Awaitable[List[List[Dict[str, str]]]]], lang: str,
+                                  name: Optional[str] = None):
+        """
+        Register a markup overrider
+        :param callback: A markup overrider to call
+        :param lang: Language to override markup for
+        :param name: Menu name
+        """
+        if name is None:
+            name = callback.__name__
+        if name not in self._markup_overriders:
+            self._markup_overriders[name] = dict()
+        self._markup_overriders[name][lang] = callback
+
+    def markup_overrider(self, lang: str, name: Optional[str] = None):
+        """
+        Register a markup overrider
+        :param lang: Language to override markup for
+        :param name: Menu name
+        """
+
+        def decorator(callback: Callable[[Menu], Awaitable[List[List[Dict[str, str]]]]]):
+            self.register_markup_overrider(callback=callback, name=name, lang=lang)
+            return callback
+
+        return decorator
+
+    async def build_menu(self, name: str, obj: Union[types.Message, types.CallbackQuery, types.InlineQuery],
+                         user_id: Optional[int] = None,
+                         callback_data: Optional[Union[str, int]] = None,
+                         auto_build: bool = True, lang: Optional[str] = None) -> Optional[Menu]:
+        """
+        Build a menu by its name
+        :param name: Menu name, same as in translation file
+        :param obj: An Aiogram Message or CallbackQuery object
+        :param user_id: An ID of a user to build menu for
+        :param callback_data: Callback data to assign to a menu
+        :param auto_build: Whether to build the Menu if no formatter is defined
+        :param lang: User language
+        :return: A Menu object
+        """
+        if name == 'menu_start':  # Start patch
+            name = 'start'
+
+        if lang is None:
+            lang = await self.storage.get_user_language(user_id=user_id or obj.from_user.id)
+        text: Dict[str, Any] = deepcopy(self.text_processor.texts[lang].get(name))
+        if not obj:
+            raise RuntimeError(f'Neither Message nor CallbackQuery was provided during menu building for {name}! '
+                               f'*brain explosion sounds accompanied by intense meowing*')
+        if text is None:  # Try to fetch the menu in another language
+            if 'en' in self.text_processor.texts.keys():
+                text = self.text_processor.texts['en'].get(name)
+            if text is None:
+                for language in self.text_processor.texts.keys():
+                    text = self.text_processor.texts[language].get(name)
+                    if text:
+                        LOGGER.warning(f'{name} menu does not have {lang} translation, using {language}.')
+                        break
+            else:
+                LOGGER.warning(f'{name} menu does not have {lang} translation, using en.')
+            if text is None:
+                raise RuntimeError(f'There is no menu called {name}! *facePAWm*')
+        if text.get('text') is None and text:
+            LOGGER.warning(f'No text provided for {name}. *suspicious stare*')
+
+        text.update(dict(name=name, obj=obj, callback_data=callback_data, bot_token=obj.conf.get('request_token')))
+        args_to_pass: Dict[str, Any] = dict()
+        for key, value in text.items():
+            if key in self.__MENU_ARGS:
+                args_to_pass[key] = value
+            else:
+                LOGGER.warning(f'Field {key} in {name} is extra, it was ignored during Menu initialization.')
+        menu = Menu(**args_to_pass)
+
+        if self._markup_overriders.get(name, dict()).get(lang):
+            menu.raw_markup = await self._markup_overriders[name][lang](menu)
+
+        format_func = self.format_functions.get(name)
+        if format_func:
+            r = await format_func(menu, obj.from_user, self)
+            if isinstance(r, Menu):  # Replace the menu if required
+                menu = r
+            if menu.markup is None and menu.raw_markup:
+                await menu.build()
+        elif auto_build:
+            await menu.build()
+
+        return menu if not menu.is_broken else None
+
+    def attach_router(self, router: NekoRouter):
+        """
+        Attach a NekoRouter to Neko
+        :param router: A NekoRouter to attach
+        """
+        if not router.mark_attached():
+            return
+        self.functions.update(router.functions)
+        self.format_functions.update(router.format_functions)
+        self.prev_menu_handlers.update(router.prev_menu_handlers)
+        self.next_menu_handlers.update(router.next_menu_handlers)
+
+    async def attach_widget(self, formatters_router: NekoRouter, functions_router: NekoRouter,
+                            startup: Callable[[BaseNeko], Awaitable[Optional[Dict[str, Any]]]],
+                            texts_path: Optional[str] = None,
+                            db_table_structure_path: Optional[str] = None,
+                            formatters_to_ignore: Optional[List[str]] = None,
+                            functions_to_ignore: Optional[List[str]] = None):
+        """
+        Attach a widget to Neko
+        :param formatters_router: A NekoRouter object responsible for formatters
+        :param functions_router: A NekoRouter object responsible for functions
+        :param startup: A startup function that returns data required for a widget to work to call
+        :param texts_path: A path to translation files
+        :param db_table_structure_path: A path to table structure file
+        :param formatters_to_ignore: A list of formatter names to ignore
+        :param functions_to_ignore: A list of function names to ignore
+        """
+        if self.storage.__class__.__name__ != 'MySQLStorage' and not self._widgets_warned:
+            LOGGER.warning(f'Your storage is not MySQLStorage, widgets may function improperly.')
+            self._widgets_warned = True
+        if formatters_router.name is None or formatters_router.name != functions_router.name \
+                or functions_router.name is None:
+            raise RuntimeError('Widget router names must be present and must be same for formatter and function router')
+
+        if formatters_router.name in self.widgets:
+            LOGGER.warning(f'Widget {formatters_router.name} is being attached again, ignored. *ultrasonic meowing*')
+            return
+
+        raw_widget_data = await startup(self)
+        if raw_widget_data:
+            widget_data: Dict[str, Any] = dict()
+            for key, value in raw_widget_data.items():
+                if not key.startswith(f'{formatters_router.name}_'):
+                    LOGGER.warning(f'Widget {formatters_router.name} is not allowed to access `{key}` in widget data, '
+                                   f'all keys for this widget have to start with `{formatters_router.name}_`. '
+                                   'This key was ignored. *visible disappointment*')
+                else:
+                    widget_data[key] = value
+            self.__widget_data.update(widget_data)
+        self.widgets.append(formatters_router.name)
+
+        if formatters_to_ignore:  # Ignore formatters
+            for name, func in formatters_router.format_functions.copy().items():
+                if name in formatters_to_ignore:
+                    formatters_router.format_functions.pop(name)
+
+        if functions_to_ignore:  # Ignore functions
+            for name, func in functions_router.functions.copy().items():
+                if name in functions_to_ignore:
+                    functions_router.functions.pop(name)
+
+        self.attach_router(formatters_router)
+        self.attach_router(functions_router)
+
+        if db_table_structure_path and self.storage.__class__.__name__ == 'MySQLStorage':
+            with open(db_table_structure_path, 'r') as f:
+                table_structure = json.load(f)
+            await self.storage.add_tables(table_structure, required_by=formatters_router.name)
+
+        if texts_path is None:
+            if formatters_router.name in self._builtin_widgets:
+                path = os.path.abspath(__file__).rstrip('neko.py')
+                delim = path[-1]
+                self.text_processor.add_texts(f'{path}widgets{delim}{formatters_router.name}{delim}translations',
+                                              is_widget=True)
+            else:
+                raise RuntimeError(f'Widget {formatters_router.name} is not builtin, '
+                                   'therefore texts_path has to be provided')
+        LOGGER.info(f'{formatters_router.name.capitalize()} widget attached successfully')
+
+    def start_webhook(self, loop=None):
+        """
+        Start webhook
+        :param loop: Abstract asyncio loop
+        """
+        if self.__webhook_path is None or self.__webhook_port is None:
+            raise RuntimeError('You must set webhook_host, webhook_host and webhook_port parameters for a Neko class '
+                               'during initialization to run a webhook')
+        self.executor.start_webhook(webhook_path=self.__webhook_path, host=self.__webhook_host,
+                                    port=self.__webhook_port, request_handler=KittyWebhook, loop=loop)
+
+    async def set_webhook(self, bot_token: str, validate_token: bool = True,
+                          drop_pending_updates: Optional[bool] = None) -> types.User:
+        """
+        Set a webhook for a child bot
+        :param bot_token: Child bot token
+        :param validate_token: Whether to validate a token
+        :param drop_pending_updates: Whether to skip unprocessed updates for a child bot
+        """
+        if self.__webhook_url is None or '{token}' not in self.__webhook_url:
+            raise RuntimeError('webhook_url must be specified and contain {token} placeholder to set a webhook.')
+        with self.bot.with_token(bot_token=bot_token, validate_token=validate_token):
+            await self.bot.set_webhook(url=self.__webhook_url.format(token=bot_token),
+                                       drop_pending_updates=drop_pending_updates)
+            return await self.bot.get_me()
```

### Comparing `NekoGram-2.1.0/src/NekoGram/router.py` & `NekoGram-2.2.0/src/NekoGram/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Callable, Optional, Union, Dict, Any, Awaitable
+from aiogram import types
+
 from .base_neko import BaseNeko
 from .logger import LOGGER
-from aiogram import types
 from .menus import Menu
 
 
 class NekoRouter:
     def __init__(self, name: Optional[str] = None):
         self.functions: Dict[str, Callable[[Menu, Union[types.Message, types.CallbackQuery], BaseNeko],
                                            Awaitable[Any]]] = dict()
```

### Comparing `NekoGram-2.1.0/src/NekoGram/storages/mysql/mysql.py` & `NekoGram-2.2.0/src/NekoGram/storages/mysql/mysql.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,307 +1,362 @@
-from typing import Optional, Union, Any, AsyncGenerator, List, Dict, Tuple
-from pymysql import err as mysql_errors
-from ..base_storage import BaseStorage
-from pymysql.constants import CLIENT
-from contextlib import suppress
-from ...logger import LOGGER
-import aiomysql
-import os
-
-try:
-    from aiomysql.cursors import DictCursor
-except ImportError:
-    raise ImportError('Install aiomysql to use MySQLStorage!')
-
-try:
-    import ujson as json
-except ImportError:
-    import json
-
-
-class MySQLStorage(BaseStorage):
-    def __init__(self, database: str, host: str = 'localhost', port: int = 3306, user: str = 'root',
-                 password: Optional[str] = None, default_language: str = 'en'):
-        """
-        Initialize database
-        :param database: Database name
-        :param host: Database host
-        :param port: Database port
-        :param user: Database user
-        :param password: Database password
-        """
-
-        self.pool: Optional[aiomysql.Pool] = None
-        self.host: str = host
-        self.port: int = port
-        self.user: str = user
-        self.password: str = password
-        self.database = database
-
-        with open(os.path.abspath(__file__).replace('mysql.py', 'tables.json'), 'r', encoding='utf-8') as file:
-            self._table_structs: Dict[str, Dict[str, Dict[str, Optional[str]]]] = json.load(file)
-        super().__init__(default_language=default_language)
-
-    def __del__(self):
-        self.pool.close()
-
-    async def verify_table(self, table: str, required_by: str):
-        r = await self.get(f'DESCRIBE {table}', fetch_all=True)
-        structure = self._table_structs[table]
-        if isinstance(r, list):  # Table exists
-            r: Dict[str, Dict[str, Optional[str]]] = {x['Field']: x for x in r}
-            table_struct: Dict[str, Dict[str, Optional[str]]] = {x['Field']: x for x in structure.values()
-                                                                 if not isinstance(x, list)}
-            for key, value in table_struct.items():
-                sql_code = value['struct']
-                value.pop('struct')
-                if not r.get(key):  # Field does not exist
-                    await self.apply(f'ALTER TABLE {table} ADD {sql_code}')
-                    LOGGER.warning(f'Added {key} to {table} required by {required_by}.')
-                elif r[key] != value:  # Field is defined in a wrong way
-                    await self.apply(f'ALTER TABLE {table} MODIFY {sql_code}')
-                    LOGGER.warning(f'Altered {key} in {table} required by {required_by}.')
-
-        else:  # Table does not exist
-            LOGGER.warning(f'Table {table} required by {required_by} does not exist, creating..')
-            fields = ','.join([f['struct'] for f in structure.values() if not isinstance(f, list)])
-            await self.apply(f'CREATE TABLE {table} ({fields}) '
-                             f'ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_unicode_ci;')
-
-        if structure.get('_extras'):
-            for i in structure['_extras']:
-                await self.apply(i, ignore_errors=True)
-
-    async def add_tables(self, structure: Dict[str, Dict[str, Dict[str, Optional[str]]]], required_by: str):
-        self._table_structs.update(structure)
-        for table in structure.keys():
-            await self.verify_table(table=table, required_by=required_by)
-
-    async def _verify(self):
-        connection = await aiomysql.connect(host=self.host, user=self.user, password=self.password, port=self.port,
-                                            client_flag=CLIENT.MULTI_STATEMENTS)
-        async with connection.cursor(DictCursor) as cursor:
-            await cursor.execute('SHOW DATABASES LIKE %s', self.database)
-            if not await cursor.fetchone():
-                LOGGER.warning(f'MySQL database {self.database} does not exist, creating..')
-                await cursor.execute(f'CREATE DATABASE IF NOT EXISTS {self.database} DEFAULT CHARACTER SET '
-                                     f'utf8mb4 COLLATE utf8mb4_unicode_ci')
-                await connection.commit()
-        connection.close()
-
-    async def acquire_pool(self):
-        """
-        Creates a new MySQL pool
-        """
-        LOGGER.info('Verifying database existence..')
-        await self._verify()
-        if isinstance(self.pool, aiomysql.Pool):
-            with suppress(Exception):
-                self.pool.close()
-
-        self.pool = await aiomysql.create_pool(host=self.host, port=self.port, user=self.user,
-                                               password=self.password, db=self.database)
-        LOGGER.info('Verifying table structures, hold tight..')
-        await self.verify_table(table='nekogram_users', required_by='NekoGram')
-        LOGGER.info('MySQLStorage initialized successfully. ~nya')
-
-    @staticmethod
-    def _verify_args(args: Optional[Union[Tuple[Union[Any, Dict[str, Any]], ...], Any]]):
-        if args is None:
-            args = tuple()
-        if not isinstance(args, (tuple, dict)):
-            args = (args,)
-        return args
-
-    async def apply(self, query: str, args: Optional[Union[Tuple[Any, ...], Dict[str, Any], Any]] = None,
-                    ignore_errors: bool = False) -> int:
-        """
-        Executes SQL query and returns the number of affected rows
-        :param query: SQL query to execute
-        :param args: Arguments passed to the SQL query
-        :param ignore_errors: Whether to ignore errors (recommended for internal usage only)
-        :return: Number of affected rows
-        """
-        args = self._verify_args(args)
-        async with self.pool.acquire() as conn:
-            async with conn.cursor(DictCursor) as cursor:
-                try:
-                    await cursor.execute(query, args)
-                    await conn.commit()
-                except mysql_errors.Error as e:
-                    if not ignore_errors:
-                        LOGGER.exception(e)
-                    await conn.rollback()
-
-                if 'insert into' in query.lower():
-                    return cursor.lastrowid
-                else:
-                    return cursor.rowcount
-
-    async def select(self, query: str, args: Optional[Union[Tuple[Any, ...], Dict[str, Any], Any]] = None) -> \
-            AsyncGenerator[Dict[str, Any], None]:
-        """
-        Generator that yields rows
-        :param query: SQL query to execute
-        :param args: Arguments passed to the SQL query
-        :return: Yields rows one by one
-        """
-        args = self._verify_args(args)
-        async with self.pool.acquire() as conn:
-            async with conn.cursor(DictCursor) as cursor:
-                try:
-                    await cursor.execute(query, args)
-                    await conn.commit()
-                    while True:
-                        item = await cursor.fetchone()
-                        if item:
-                            yield item
-                        else:
-                            break
-                except mysql_errors.Error:
-                    pass
-
-    async def get(self, query: str, args: Optional[Union[Tuple[Any, ...], Dict[str, Any], Any]] = None,
-                  fetch_all: bool = False) -> Union[bool, List[Dict[str, Any]], Dict[str, Any]]:
-        """
-        Get a single row or a list of rows from the database
-        :param query: SQL query to execute
-        :param args: Arguments passed to the SQL query
-        :param fetch_all: Set True if you need a list of rows instead of just a single row
-        :return: A row or a list or rows
-        """
-        args = self._verify_args(args)
-        async with self.pool.acquire() as conn:
-            async with conn.cursor(DictCursor) as cursor:
-                try:
-                    await cursor.execute(query, args)
-                    await conn.commit()
-
-                    if fetch_all:
-                        return await cursor.fetchall()
-                    else:
-                        result = await cursor.fetchone()
-                        return result if result else dict()
-                except mysql_errors.Error:
-                    return False
-
-    async def check(self, query: str, args: Optional[Union[Tuple[Any, ...], Dict[str, Any], Any]] = None) -> int:
-        args = self._verify_args(args)
-        async with self.pool.acquire() as conn:
-            async with conn.cursor(DictCursor) as cursor:
-                try:
-                    await cursor.execute(query, args)
-                    await conn.commit()
-
-                    return cursor.rowcount
-                except mysql_errors.Error:
-                    return 0
-
-    async def set_user_language(self, user_id: int, language: str):
-        await super().set_user_language(user_id=user_id, language=language)
-        await self.apply('UPDATE nekogram_users SET lang = %s WHERE id = %s', (language, user_id))
-
-    async def get_user_language(self, user_id: int) -> str:
-        """
-        Get user's language
-        :param user_id: Telegram ID of the user
-        :return: User's language
-        """
-        lang = await self.get_cached_user_language(user_id=user_id)
-        if lang is None:
-            lang = (await self.get('SELECT lang FROM nekogram_users WHERE id = %s',
-                                   user_id)).get('lang', self.default_language)
-        await super().set_user_language(user_id=user_id, language=lang)
-        return lang
-
-    async def get_user_data(self, user_id: int, **kwargs) -> Union[Dict[str, Any], bool]:
-        """
-        Get user data
-        :param user_id: Telegram ID of the user
-        :return: Decoded JSON user data
-        """
-        try:
-            return json.loads((await self.get('SELECT data FROM nekogram_users WHERE id = %s',
-                                              user_id))['data'])
-        except TypeError:
-            return False
-
-    async def set_user_data(self, user_id: int, data: Optional[Dict[str, Any]] = None,
-                            replace: bool = False, **kwargs) -> Dict[str, Any]:
-        if data is None:
-            data = dict()
-            replace = True
-
-        if replace:
-            user_data = data
-        else:
-            user_data = await self.get_user_data(user_id=user_id)
-            user_data.update(data)
-
-        await self.apply('UPDATE nekogram_users SET data = %s WHERE id = %s', (json.dumps(user_data), user_id))
-        return user_data
-
-    async def set_user_menu(self, user_id: int, menu: Optional[str] = None, **kwargs):
-        await self.set_user_data(user_id=user_id, data={'menu': menu})
-        return menu
-
-    async def get_user_menu(self, user_id: int, **kwargs) -> Optional[str]:
-        return (await self.get_user_data(user_id=user_id)).get('menu')
-
-    async def check_user_exists(self, user_id: int) -> bool:
-        return bool(await self.check('SELECT id FROM nekogram_users WHERE id = %s', user_id))
-
-    async def set_last_message_id(self, user_id: int, message_id: int):
-        await self.apply('UPDATE nekogram_users SET last_message_id = %s WHERE id = %s', (message_id, user_id))
-
-    async def get_last_message_id(self, user_id: int) -> Optional[int]:
-        return (await self.get('SELECT last_message_id FROM nekogram_users WHERE id = %s',
-                               user_id)).get('last_message_id')
-
-    async def create_user(self, user_id: int, name: str, username: Optional[str] = None,
-                          language: Optional[str] = None):
-        if language is None:
-            language = self.default_language
-
-        await self.apply('INSERT INTO nekogram_users (id, lang, full_name, username) VALUES (%s, %s, %s, %s)',
-                         (user_id, language, name, username))
-
-
-class KittyMySQLStorage(MySQLStorage):
-    def __init__(self, database: str, host: str = 'localhost', port: int = 3306, user: str = 'root',
-                 password: Optional[str] = None, default_language: str = 'en'):
-        MySQLStorage.__init__(self, database=database, host=host, port=port, user=user, password=password,
-                              default_language=default_language)
-
-    async def get_user_data(self, user_id: int, bot_token: Optional[str] = None) -> Union[Dict[str, Any], bool]:
-        """
-        Get user data
-        :param user_id: Telegram ID of the user
-        :param bot_token: Token of the current bot
-        :return: Decoded JSON user data
-        """
-        try:
-            return json.loads((await self.get('SELECT data FROM nekogram_users WHERE id = %s',
-                                              user_id))['data']).get(bot_token, dict())
-        except TypeError:
-            return False
-
-    async def set_user_data(self, user_id: int, data: Optional[Dict[str, Any]] = None,
-                            replace: bool = False, bot_token: Optional[str] = None) -> Dict[str, Any]:
-        raw_user_data = json.loads((await self.get('SELECT data FROM nekogram_users WHERE id = %s', user_id))['data'])
-        if data is None:
-            raw_user_data.pop(bot_token, None)
-        else:
-            if bot_token not in raw_user_data.keys():
-                raw_user_data[bot_token] = data
-            else:
-                raw_user_data[bot_token].update(data)
-
-        await self.apply('UPDATE nekogram_users SET data = %s WHERE id = %s', (json.dumps(raw_user_data), user_id))
-        return raw_user_data.get(bot_token, dict())
-
-    async def set_user_menu(self, user_id: int, menu: Optional[str] = None, bot_token: Optional[str] = None):
-        await self.set_user_data(user_id=user_id, data={'menu': menu}, bot_token=bot_token)
-        return menu
-
-    async def get_user_menu(self, user_id: int, bot_token: Optional[str] = None) -> Optional[str]:
-        return (await self.get_user_data(user_id=user_id, bot_token=bot_token)).get('menu')
+from typing import Optional, Union, Any, AsyncGenerator, List, Dict, Tuple
+from pymysql import err as mysql_errors
+from pymysql.constants import CLIENT
+from contextlib import suppress
+import aiomysql
+import os
+
+try:
+    from aiomysql.cursors import DictCursor
+except ImportError:
+    raise ImportError('Install aiomysql to use MySQLStorage!')
+
+try:
+    import ujson as json
+except ImportError:
+    import json
+
+from ..base_storage import BaseStorage
+from ...logger import LOGGER
+
+
+class MySQLStorage(BaseStorage):
+    def __init__(self, database: str, host: str = 'localhost', port: int = 3306, user: str = 'root',
+                 password: Optional[str] = None, default_language: str = 'en'):
+        """
+        Initialize database
+        :param database: Database name
+        :param host: Database host
+        :param port: Database port
+        :param user: Database user
+        :param password: Database password
+        """
+
+        self.pool: Optional[aiomysql.Pool] = None
+        self.host: str = host
+        self.port: int = port
+        self.user: str = user
+        self.password: str = password
+        self.database = database
+
+        with open(os.path.abspath(__file__).replace('mysql.py', 'tables.json'), 'r', encoding='utf-8') as file:
+            self._table_structs: Dict[str, Dict[str, Dict[str, Optional[str]]]] = json.load(file)
+        super().__init__(default_language=default_language)
+
+    def __del__(self):
+        self.pool.close()
+
+    async def verify_table(self, table: str, required_by: str) -> None:
+        r = await self.get(f'DESCRIBE {table}', fetch_all=True)
+        structure = self._table_structs[table]
+        if isinstance(r, list):  # Table exists
+            r: Dict[str, Dict[str, Optional[str]]] = {x['Field']: x for x in r}
+            table_struct: Dict[str, Dict[str, Optional[str]]] = {x['Field']: x for x in structure.values()
+                                                                 if not isinstance(x, list)}
+            for key, value in table_struct.items():
+                sql_code = value['struct']
+                value.pop('struct')
+                if not r.get(key):  # Field does not exist
+                    await self.apply(f'ALTER TABLE {table} ADD {sql_code}')
+                    LOGGER.warning(f'Added {key} to {table} required by {required_by}.')
+                elif r[key] != value:  # Field is defined in a wrong way
+                    await self.apply(f'ALTER TABLE {table} MODIFY {sql_code}')
+                    LOGGER.warning(f'Altered {key} in {table} required by {required_by}.')
+
+        else:  # Table does not exist
+            LOGGER.warning(f'Table {table} required by {required_by} does not exist, creating..')
+            fields = ','.join([f['struct'] for f in structure.values() if not isinstance(f, list)])
+            await self.apply(f'CREATE TABLE {table} ({fields}) '
+                             f'ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_unicode_ci;')
+
+        if structure.get('_extras'):
+            for i in structure['_extras']:
+                await self.apply(i, ignore_errors=True)
+
+    async def add_tables(self, structure: Dict[str, Dict[str, Dict[str, Optional[str]]]], required_by: str) -> None:
+        self._table_structs.update(structure)
+        for table in structure.keys():
+            await self.verify_table(table=table, required_by=required_by)
+
+    async def _verify(self) -> None:
+        connection = await aiomysql.connect(host=self.host, user=self.user, password=self.password, port=self.port,
+                                            client_flag=CLIENT.MULTI_STATEMENTS)
+        async with connection.cursor(DictCursor) as cursor:
+            await cursor.execute('SHOW DATABASES LIKE %s', self.database)
+            if not await cursor.fetchone():
+                LOGGER.warning(f'MySQL database {self.database} does not exist, creating..')
+                await cursor.execute(f'CREATE DATABASE IF NOT EXISTS {self.database} DEFAULT CHARACTER SET '
+                                     f'utf8mb4 COLLATE utf8mb4_unicode_ci')
+                await connection.commit()
+        connection.close()
+
+    async def acquire_pool(self) -> bool:
+        """
+        Creates a new MySQL pool
+        """
+        LOGGER.info('Verifying database existence..')
+        await self._verify()
+        if isinstance(self.pool, aiomysql.Pool):
+            with suppress(Exception):
+                self.pool.close()
+
+        self.pool = await aiomysql.create_pool(host=self.host, port=self.port, user=self.user,
+                                               password=self.password, db=self.database)
+        LOGGER.info('Verifying table structures, hold tight..')
+        await self.verify_table(table='nekogram_users', required_by='NekoGram')
+        LOGGER.info('MySQLStorage initialized successfully. ~nya')
+        return True
+
+    async def close_pool(self) -> bool:
+        """
+        Closes existing MySQL pool.
+        :return: True if the pool was successfully closed, otherwise False.
+        """
+        try:
+            self.pool.close()
+        except Exception:
+            return False
+        return True
+
+    async def apply(self, query: str, args: Union[Tuple[Any, ...], Dict[str, Any], Any] = (),
+                    ignore_errors: bool = False) -> int:
+        """
+        Executes SQL query and returns the number of affected rows
+        :param query: SQL query to execute
+        :param args: Arguments passed to the SQL query
+        :param ignore_errors: Whether to ignore errors (recommended for internal usage only)
+        :return: Number of affected rows
+        """
+        args = self._verify_args(args)
+        async with self.pool.acquire() as conn:
+            async with conn.cursor(DictCursor) as cursor:
+                try:
+                    await cursor.execute(query, args)
+                    await conn.commit()
+                except mysql_errors.Error as e:
+                    if not ignore_errors:
+                        LOGGER.exception(e)
+                    await conn.rollback()
+
+                if 'insert into' in query.lower():
+                    return cursor.lastrowid
+                else:
+                    return cursor.rowcount
+
+    async def select(self, query: str, args: Union[Tuple[Any, ...], Dict[str, Any], Any] = ()) -> \
+            AsyncGenerator[Dict[str, Any], None]:
+        """
+        Generator that yields rows
+        :param query: SQL query to execute
+        :param args: Arguments passed to the SQL query
+        :return: Yields rows one by one
+        """
+        args = self._verify_args(args)
+        async with self.pool.acquire() as conn:
+            async with conn.cursor(DictCursor) as cursor:
+                try:
+                    await cursor.execute(query, args)
+                    await conn.commit()
+                    while True:
+                        item = await cursor.fetchone()
+                        if item:
+                            yield item
+                        else:
+                            break
+                except mysql_errors.Error:
+                    pass
+
+    async def get(self, query: str, args: Union[Tuple[Any, ...], Dict[str, Any], Any] = (),
+                  fetch_all: bool = False) -> Union[bool, List[Dict[str, Any]], Dict[str, Any]]:
+        """
+        Get a single row or a list of rows from the database
+        :param query: SQL query to execute
+        :param args: Arguments passed to the SQL query
+        :param fetch_all: Set True if you need a list of rows instead of just a single row
+        :return: A row or a list or rows
+        """
+        args = self._verify_args(args)
+        async with self.pool.acquire() as conn:
+            async with conn.cursor(DictCursor) as cursor:
+                try:
+                    await cursor.execute(query, args)
+                    await conn.commit()
+
+                    if fetch_all:
+                        return await cursor.fetchall()
+                    else:
+                        result = await cursor.fetchone()
+                        return result if result else dict()
+                except mysql_errors.Error:
+                    return False
+
+    async def check(self, query: str, args: Union[Tuple[Any, ...], Dict[str, Any], Any] = ()) -> int:
+        """
+        Executes SQL query and returns the number of affected rows.
+        :param query: SQL query to execute.
+        :param args: Arguments passed to the SQL query.
+        :return: Number of affected rows.
+        """
+        args = self._verify_args(args)
+        async with self.pool.acquire() as conn:
+            async with conn.cursor(DictCursor) as cursor:
+                try:
+                    await cursor.execute(query, args)
+                    await conn.commit()
+
+                    return cursor.rowcount
+                except mysql_errors.Error:
+                    return 0
+
+    async def set_user_language(self, user_id: int, language: str) -> None:
+        """
+        Get user's language
+        :param user_id: Telegram ID of the user
+        :param language: User's language to be set
+        :return: None
+        """
+        await super().set_user_language(user_id=user_id, language=language)
+        await self.apply('UPDATE nekogram_users SET lang = %s WHERE id = %s', (language, user_id))
+
+    async def get_user_language(self, user_id: int) -> str:
+        """
+        Get user's language
+        :param user_id: Telegram ID of the user
+        :return: User's language
+        """
+        lang = await self.get_cached_user_language(user_id=user_id)
+        if lang is None:
+            lang = (await self.get('SELECT lang FROM nekogram_users WHERE id = %s',
+                                   user_id)).get('lang', self.default_language)
+        await super().set_user_language(user_id=user_id, language=lang)
+        return lang
+
+    async def get_user_data(self, user_id: int, **kwargs) -> Union[Dict[str, Any], bool]:
+        """
+        Get user data
+        :param user_id: Telegram ID of the user
+        :return: Decoded JSON user data
+        """
+        return json.loads((await self.get('SELECT data FROM nekogram_users WHERE id = %s', user_id))['data'])
+
+    async def set_user_data(self, user_id: int, data: Optional[Dict[str, Any]] = None,
+                            replace: bool = False, **kwargs) -> Dict[str, Any]:
+        """
+        Set user data
+        :param user_id: Telegram ID of the user
+        :param data: User data
+        :param replace: Replace user data with `data` if replace=True, otherwise merge existing with `data`
+        :return: Decoded JSON user data
+        """
+        if data is None:
+            data = dict()
+            replace = True
+
+        if replace:
+            user_data = data
+        else:
+            user_data = await self.get_user_data(user_id=user_id)
+            user_data.update(data)
+
+        await self.apply('UPDATE nekogram_users SET data = %s WHERE id = %s', (json.dumps(user_data), user_id))
+        return user_data
+
+    async def check_user_exists(self, user_id: int) -> bool:
+        """
+        Check that user exists in the database.
+        :param user_id: Telegram ID of the user.
+        :return: boolean value.
+        """
+        return bool(await self.check('SELECT id FROM nekogram_users WHERE id = %s', user_id))
+
+    async def set_last_message_id(self, user_id: int, message_id: int) -> None:
+        """
+        Set last message ID.
+        :param user_id: Telegram ID of the user.
+        :param message_id: Telegram ID of the message.
+        :return: None.
+        """
+        await self.apply('UPDATE nekogram_users SET last_message_id = %s WHERE id = %s', (message_id, user_id))
+
+    async def get_last_message_id(self, user_id: int) -> Optional[int]:
+        """
+        Set last message ID.
+        :param user_id: Telegram ID of the user.
+        :return: Telegram ID of the message if was set, otherwise None.
+        """
+        return (await self.get('SELECT last_message_id FROM nekogram_users WHERE id = %s',
+                               user_id)).get('last_message_id')
+
+    async def create_user(self, user_id: int, name: str, username: Optional[str] = None,
+                          language: Optional[str] = None) -> None:
+        """
+        Create user.
+        :param user_id: Telegram ID of the user.
+        :param name: Telegram first and last name of the user.
+        :param username: Telegram username of the user.
+        :param language: User's language.
+        :return: None.
+        """
+        if language is None:
+            language = self.default_language
+
+        await self.apply('INSERT INTO nekogram_users (id, lang, full_name, username) VALUES (%s, %s, %s, %s)',
+                         (user_id, language, name, username))
+
+
+class KittyMySQLStorage(MySQLStorage):
+    def __init__(self, database: str, host: str = 'localhost', port: int = 3306, user: str = 'root',
+                 password: Optional[str] = None, default_language: str = 'en'):
+        MySQLStorage.__init__(self, database=database, host=host, port=port, user=user, password=password,
+                              default_language=default_language)
+
+    async def get_user_data(self, user_id: int, bot_token: Optional[str] = None) -> Union[Dict[str, Any], bool]:
+        """
+        Get user data
+        :param user_id: Telegram ID of the user
+        :param bot_token: Token of the current bot
+        :return: Decoded JSON user data
+        """
+        return json.loads((await self.get('SELECT data FROM nekogram_users WHERE id = %s',
+                                          user_id))['data']).get(bot_token, dict())
+
+    async def set_user_data(self, user_id: int, data: Optional[Dict[str, Any]] = None,
+                            replace: bool = False, bot_token: Optional[str] = None) -> Dict[str, Any]:
+        """
+        Set user data.
+        :param user_id: Telegram ID of the user.
+        :param data: User data.
+        :param replace: Replace user data with `data` if replace=True, otherwise merge existing with `data`.
+        :param bot_token: Token of the Telegram bot obtained through @BotFather.
+        :return: Decoded JSON user data.
+        """
+        raw_user_data = json.loads((await self.get('SELECT data FROM nekogram_users WHERE id = %s', user_id))['data'])
+        if data is None:
+            raw_user_data.pop(bot_token, None)
+        else:
+            if bot_token not in raw_user_data.keys():
+                raw_user_data[bot_token] = data
+            else:
+                raw_user_data[bot_token].update(data)
+
+        await self.apply('UPDATE nekogram_users SET data = %s WHERE id = %s', (json.dumps(raw_user_data), user_id))
+        return raw_user_data.get(bot_token, dict())
+
+    async def set_user_menu(self, user_id: int, menu: Optional[str] = None, bot_token: Optional[str] = None) -> str:
+        """
+        Set user menu.
+        :param user_id: Telegram ID of the user.
+        :param menu: User menu.
+        :param bot_token: Token of the Telegram bot obtained through @BotFather.
+        :return: User menu.
+        """
+        await self.set_user_data(user_id=user_id, data={'menu': menu}, bot_token=bot_token)
+        return menu
+
+    async def get_user_menu(self, user_id: int, bot_token: Optional[str] = None) -> Optional[str]:
+        """
+        Set user menu.
+        :param user_id: Telegram ID of the user.
+        :param bot_token: Token of the Telegram bot obtained through @BotFather.
+        :return: User menu if was set, otherwise None.
+        """
+        return (await self.get_user_data(user_id=user_id, bot_token=bot_token)).get('menu')
```

### Comparing `NekoGram-2.1.0/src/NekoGram/storages/mysql/tables.json` & `NekoGram-2.2.0/src/NekoGram/storages/mysql/tables.json`

 * *Files identical despite different names*

### Comparing `NekoGram-2.1.0/src/NekoGram/text_processors/json_processor.py` & `NekoGram-2.2.0/src/NekoGram/text_processors/json_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Union, Optional, Any, TextIO, Dict
-from .base_processor import BaseProcessor
 from os.path import isdir, isfile
 from io import TextIOWrapper
 from os import listdir
 
 try:
     import ujson as json
 except ImportError:
     import json
 
+from .base_processor import BaseProcessor
+
 
 class JSONProcessor(BaseProcessor):
     def __init__(self):
         super().__init__()
 
     def _verify(self):
         for lang, data in self.texts.items():
```

### Comparing `NekoGram-2.1.0/src/NekoGram/utils.py` & `NekoGram-2.2.0/src/NekoGram/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from aiogram.dispatcher.middlewares import BaseMiddleware
 from contextlib import suppress
-from .base_neko import BaseNeko
 from aiogram import types
 from typing import Union
 from io import BytesIO
 import aiohttp
+
 try:
     import ujson as json
 except ImportError:
     import json
 
+from .base_neko import BaseNeko
+
 
 class HandlerInjector(BaseMiddleware):
     """
     Neko injector middleware
     """
 
     def __init__(self, neko: BaseNeko):
         super().__init__()
         self.neko: BaseNeko = neko
 
-    async def on_process_message(self, message: types.Message, _: dict):
+    async def on_pre_process_message(self, message: types.Message, _: dict):
         """
         This handler is called when dispatcher receives a message
         """
         # Get current handler
         message.conf['neko'] = self.neko
         with suppress(Exception):
             message.conf['request_token'] = message.conf['parent']().conf['request_token']
```

### Comparing `NekoGram-2.1.0/src/NekoGram/webhook.py` & `NekoGram-2.2.0/src/NekoGram/webhook.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from aiogram.dispatcher.webhook import WebhookRequestHandler, web
-from .base_neko import BaseNeko
 from aiogram.utils.executor import Executor
 
+from .base_neko import BaseNeko
+
 
 class KittyExecutor(Executor):
     def __init__(self, neko: BaseNeko, skip_updates=None, check_ip=False, retry_after=None, loop=None):
         super().__init__(dispatcher=neko.dp, skip_updates=skip_updates, check_ip=check_ip, retry_after=retry_after,
                          loop=loop)
         self.neko: BaseNeko = neko
```

### Comparing `NekoGram-2.1.0/src/NekoGram/widgets/broadcast/formatters.py` & `NekoGram-2.2.0/src/NekoGram/widgets/broadcast/formatters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,49 @@
-from aiogram.types import User, InlineKeyboardMarkup, InlineKeyboardButton, Message
-from NekoGram import Neko, Menu, NekoRouter
-from typing import Dict, List
-try:
-    import ujson as json
-except ImportError:
-    import json
-
-ROUTER: NekoRouter = NekoRouter(name='broadcast')
-
-
-@ROUTER.formatter()
-async def widget_broadcast(data: Menu, user: User, neko: Neko):
-    if not await neko.storage.check('SELECT id FROM nekogram_users WHERE id != %s', user.id):
-        await data.obj.answer(text=data.extras['alt_text'], show_alert=True)
-        data.break_execution()
-
-
-@ROUTER.formatter()
-async def widget_broadcast_post_markup(data: Menu, user: User, neko: Neko):
-    user_data = await neko.storage.get_user_data(user_id=user.id)
-    raw_markup: List[List[Dict[str, str]]] = user_data.get('widget_broadcast_post_markup', [])
-    markup: InlineKeyboardMarkup = InlineKeyboardMarkup()
-    row_index: int = 0
-
-    for row in raw_markup:
-        row_buttons = []
-
-        button_index: int = 0
-        for button in row:
-            row_buttons.append(InlineKeyboardButton(text=button['text'], callback_data=f'widget_broadcast_remove_button'
-                                                                                       f'#{row_index}-{button_index}'))
-            button_index += 1
-        if button_index < 3:
-            row_buttons.append(InlineKeyboardButton(text='➕',
-                                                    callback_data=f'widget_broadcast_add_button_step_1#{row_index}'))
-        markup.add(*row_buttons)
-        row_index += 1
-
-    await data.build(markup=markup, markup_format={'row_index': row_index})
-
-
-@ROUTER.formatter()
-async def widget_broadcast_add_button_step_1(data: Menu, user: User, neko: Neko):
-    if isinstance(data.obj, Message):
-        return
-    await neko.storage.set_user_data(data={'widget_broadcast_post_row_index': data.call_data}, user_id=user.id)
+from aiogram.types import User, InlineKeyboardMarkup, InlineKeyboardButton, Message
+from typing import Dict, List
+try:
+    import ujson as json
+except ImportError:
+    import json
+
+from NekoGram import Neko, Menu, NekoRouter
+
+
+ROUTER: NekoRouter = NekoRouter(name='broadcast')
+
+
+@ROUTER.formatter()
+async def widget_broadcast(data: Menu, _: User, neko: Neko):
+    if await neko.storage.check('SELECT id FROM nekogram_users;') < 2:
+        await data.obj.answer(text=data.extras['alt_text'], show_alert=True)
+        data.break_execution()
+
+
+@ROUTER.formatter()
+async def widget_broadcast_post_markup(data: Menu, user: User, neko: Neko):
+    user_data = await neko.storage.get_user_data(user_id=user.id)
+    raw_markup: List[List[Dict[str, str]]] = user_data.get('widget_broadcast_post_markup', [])
+    markup: InlineKeyboardMarkup = InlineKeyboardMarkup()
+    row_index: int = 0
+
+    for row in raw_markup:
+        row_buttons = []
+
+        button_index: int = 0
+        for button in row:
+            row_buttons.append(InlineKeyboardButton(text=button['text'], callback_data=f'widget_broadcast_remove_button'
+                                                                                       f'#{row_index}-{button_index}'))
+            button_index += 1
+        if button_index < 3:
+            row_buttons.append(InlineKeyboardButton(text='➕',
+                                                    callback_data=f'widget_broadcast_add_button_step_1#{row_index}'))
+        markup.add(*row_buttons)
+        row_index += 1
+
+    await data.build(markup=markup, markup_format={'row_index': row_index})
+
+
+@ROUTER.formatter()
+async def widget_broadcast_add_button_step_1(data: Menu, user: User, neko: Neko):
+    if isinstance(data.obj, Message):
+        return
+    await neko.storage.set_user_data(data={'widget_broadcast_post_row_index': data.call_data}, user_id=user.id)
```

### Comparing `NekoGram-2.1.0/src/NekoGram/widgets/broadcast/translations/en.json` & `NekoGram-2.2.0/src/NekoGram/widgets/broadcast/translations/en.json`

 * *Files identical despite different names*

### Comparing `NekoGram-2.1.0/src/NekoGram/widgets/broadcast/translations/pl.json` & `NekoGram-2.2.0/src/NekoGram/widgets/broadcast/translations/pl.json`

 * *Files identical despite different names*

### Comparing `NekoGram-2.1.0/src/NekoGram/widgets/broadcast/translations/ru.json` & `NekoGram-2.2.0/src/NekoGram/widgets/broadcast/translations/ru.json`

 * *Files identical despite different names*

### Comparing `NekoGram-2.1.0/src/NekoGram/widgets/broadcast/translations/uk.json` & `NekoGram-2.2.0/src/NekoGram/widgets/broadcast/translations/uk.json`

 * *Files identical despite different names*

### Comparing `NekoGram-2.1.0/src/NekoGram/widgets/broadcast/utils.py` & `NekoGram-2.2.0/src/NekoGram/widgets/broadcast/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from aiogram.types import InlineKeyboardMarkup, InlineKeyboardButton
 from typing import List, Dict
+
 from ...base_neko import BaseNeko
 
 
 def assemble_markup(markup: List[List[Dict[str, str]]]) -> InlineKeyboardMarkup:
     final_markup = InlineKeyboardMarkup()
     for row in markup:
         row_buttons = []
```

### Comparing `NekoGram-2.1.0/src/NekoGram/widgets/languages/formatters.py` & `NekoGram-2.2.0/src/NekoGram/widgets/languages/formatters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from NekoGram import Neko, Menu, NekoRouter
 from aiogram import types
 
+from NekoGram import Neko, Menu, NekoRouter
+
+
 ROUTER: NekoRouter = NekoRouter(name='languages')
 
 
 @ROUTER.formatter()
 async def widget_languages(data: Menu, _: types.User, neko: Neko):
     markup: types.InlineKeyboardMarkup = types.InlineKeyboardMarkup()
     for lang in neko.text_processor.texts.keys():
```

### Comparing `NekoGram-2.1.0/src/NekoGram/widgets/stats/formatters.py` & `NekoGram-2.2.0/src/NekoGram/widgets/stats/formatters.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-from NekoGram import Neko, Menu, NekoRouter
 from aiogram import types
+
 try:
     import ujson as json
 except ImportError:
     import json
 
+from NekoGram import Neko, Menu, NekoRouter
+
+
 ROUTER: NekoRouter = NekoRouter(name='stats')
 
 
 @ROUTER.formatter()
 async def widget_stats(data: Menu, _: types.User, neko: Neko):
     total = await neko.storage.check('SELECT id FROM nekogram_stats')
     single_user = await neko.storage.get('SELECT user_id, COUNT(*) AS c, nu.full_name, nu.username '
```

### Comparing `NekoGram-2.1.0/src/NekoGram/widgets/stats/sql/tables.json` & `NekoGram-2.2.0/src/NekoGram/widgets/stats/sql/tables.json`

 * *Files identical despite different names*

### Comparing `NekoGram-2.1.0/src/NekoGram/widgets/stats/util.py` & `NekoGram-2.2.0/src/NekoGram/widgets/stats/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from aiogram.dispatcher.middlewares import BaseMiddleware
-from ...base_neko import BaseNeko
 from aiogram import types
 import os
+
 try:
     import ujson as json
 except ImportError:
     import json
 
+from ...base_neko import BaseNeko
+
 
 class StatsInjector(BaseMiddleware):
     """
     Neko injector middleware
     """
 
     def __init__(self, neko: BaseNeko):
```

### Comparing `NekoGram-2.1.0/src/NekoGram.egg-info/PKG-INFO` & `NekoGram-2.2.0/src/NekoGram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NekoGram
-Version: 2.1.0
+Version: 2.2.0
 Summary: Creating bots has never been simpler.
 Author-email: lyteloli <me@lyteloli.space>
 License: MIT License
         
         Copyright (c) 2020 lyteloli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `NekoGram-2.1.0/src/NekoGram.egg-info/SOURCES.txt` & `NekoGram-2.2.0/src/NekoGram.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,20 +16,21 @@
 src/NekoGram.egg-info/requires.txt
 src/NekoGram.egg-info/top_level.txt
 src/NekoGram/handlers/__init__.py
 src/NekoGram/handlers/callback.py
 src/NekoGram/handlers/message.py
 src/NekoGram/storages/__init__.py
 src/NekoGram/storages/base_storage.py
-src/NekoGram/storages/memory_storage.py
 src/NekoGram/storages/mysql/__init__.py
 src/NekoGram/storages/mysql/mysql.py
 src/NekoGram/storages/mysql/tables.json
 src/NekoGram/storages/pg/__init__.py
 src/NekoGram/storages/pg/pg.py
+src/NekoGram/storages/sqlite/__init__.py
+src/NekoGram/storages/sqlite/sqlite.py
 src/NekoGram/text_processors/__init__.py
 src/NekoGram/text_processors/base_processor.py
 src/NekoGram/text_processors/json_processor.py
 src/NekoGram/widgets/__init__.py
 src/NekoGram/widgets/broadcast/__init__.py
 src/NekoGram/widgets/broadcast/formatters.py
 src/NekoGram/widgets/broadcast/functions.py
```

