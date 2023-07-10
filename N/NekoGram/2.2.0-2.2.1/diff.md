# Comparing `tmp/NekoGram-2.2.0.tar.gz` & `tmp/NekoGram-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NekoGram-2.2.0.tar", last modified: Mon Jul 10 09:47:25 2023, max compression
+gzip compressed data, was "NekoGram-2.2.1.tar", last modified: Mon Jul 10 10:19:22 2023, max compression
```

## Comparing `NekoGram-2.2.0.tar` & `NekoGram-2.2.1.tar`

### file list

```diff
@@ -1,78 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.148330 NekoGram-2.2.0/
--rw-rw-rw-   0        0        0     1086 2021-07-29 12:59:10.000000 NekoGram-2.2.0/LICENSE
--rw-rw-rw-   0        0        0    17999 2023-07-10 09:47:25.147329 NekoGram-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    16128 2022-11-11 15:21:46.000000 NekoGram-2.2.0/README.md
--rw-rw-rw-   0        0        0      966 2023-07-10 09:47:18.000000 NekoGram-2.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-10 09:47:25.148330 NekoGram-2.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.082633 NekoGram-2.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.099134 NekoGram-2.2.0/src/NekoGram/
--rw-rw-rw-   0        0        0       78 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/__init__.py
--rw-rw-rw-   0        0        0     6752 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/base_neko.py
--rw-rw-rw-   0        0        0     8274 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/filters.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.114417 NekoGram-2.2.0/src/NekoGram/handlers/
--rw-rw-rw-   0        0        0       92 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/handlers/__init__.py
--rw-rw-rw-   0        0        0     1919 2023-06-18 11:48:30.000000 NekoGram-2.2.0/src/NekoGram/handlers/callback.py
--rw-rw-rw-   0        0        0     5421 2023-06-18 11:48:30.000000 NekoGram-2.2.0/src/NekoGram/handlers/message.py
--rw-rw-rw-   0        0        0       72 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/logger.py
--rw-rw-rw-   0        0        0    11418 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/menus.py
--rw-rw-rw-   0        0        0    16959 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/neko.py
--rw-rw-rw-   0        0        0     4373 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/router.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.115924 NekoGram-2.2.0/src/NekoGram/storages/
--rw-rw-rw-   0        0        0       39 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/storages/__init__.py
--rw-rw-rw-   0        0        0     3460 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/storages/base_storage.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.118475 NekoGram-2.2.0/src/NekoGram/storages/mysql/
--rw-rw-rw-   0        0        0       51 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/storages/mysql/__init__.py
--rw-rw-rw-   0        0        0    16032 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/storages/mysql/mysql.py
--rw-rw-rw-   0        0        0     1114 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/storages/mysql/tables.json
-drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.119978 NekoGram-2.2.0/src/NekoGram/storages/pg/
--rw-rw-rw-   0        0        0       43 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/storages/pg/__init__.py
--rw-rw-rw-   0        0        0    11705 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/storages/pg/pg.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.121986 NekoGram-2.2.0/src/NekoGram/storages/sqlite/
--rw-rw-rw-   0        0        0       55 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/storages/sqlite/__init__.py
--rw-rw-rw-   0        0        0    11324 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/storages/sqlite/sqlite.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.123491 NekoGram-2.2.0/src/NekoGram/text_processors/
--rw-rw-rw-   0        0        0       84 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/text_processors/__init__.py
--rw-rw-rw-   0        0        0      437 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/text_processors/base_processor.py
--rw-rw-rw-   0        0        0     3183 2023-06-18 11:48:30.000000 NekoGram-2.2.0/src/NekoGram/text_processors/json_processor.py
--rw-rw-rw-   0        0        0     2710 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/utils.py
--rw-rw-rw-   0        0        0     1311 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/webhook.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.124498 NekoGram-2.2.0/src/NekoGram/widgets/
--rw-rw-rw-   0        0        0       42 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.128873 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/
--rw-rw-rw-   0        0        0      128 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/__init__.py
--rw-rw-rw-   0        0        0     1923 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/formatters.py
--rw-rw-rw-   0        0        0     5410 2023-07-10 09:39:14.000000 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/functions.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.131986 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/translations/
--rw-rw-rw-   0        0        0     2058 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/translations/en.json
--rw-rw-rw-   0        0        0     2134 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/translations/pl.json
--rw-rw-rw-   0        0        0     2390 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/translations/ru.json
--rw-rw-rw-   0        0        0     2380 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/translations/uk.json
--rw-rw-rw-   0        0        0       77 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/util.py
--rw-rw-rw-   0        0        0     1804 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/widgets/broadcast/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.136942 NekoGram-2.2.0/src/NekoGram/widgets/languages/
--rw-rw-rw-   0        0        0      128 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/languages/__init__.py
--rw-rw-rw-   0        0        0      648 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/widgets/languages/formatters.py
--rw-rw-rw-   0        0        0      449 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/widgets/languages/functions.py
--rw-rw-rw-   0        0        0       44 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/languages/replacements.json
-drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.140500 NekoGram-2.2.0/src/NekoGram/widgets/languages/translations/
--rw-rw-rw-   0        0        0      262 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/languages/translations/en.json
--rw-rw-rw-   0        0        0      272 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/languages/translations/he.json
--rw-rw-rw-   0        0        0      260 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/languages/translations/pl.json
--rw-rw-rw-   0        0        0      284 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/languages/translations/ru.json
--rw-rw-rw-   0        0        0      280 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/languages/translations/uk.json
--rw-rw-rw-   0        0        0      373 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/widgets/languages/util.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.144308 NekoGram-2.2.0/src/NekoGram/widgets/stats/
--rw-rw-rw-   0        0        0      128 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/stats/__init__.py
--rw-rw-rw-   0        0        0      905 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/widgets/stats/formatters.py
--rw-rw-rw-   0        0        0       80 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/widgets/stats/functions.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.145819 NekoGram-2.2.0/src/NekoGram/widgets/stats/sql/
--rw-rw-rw-   0        0        0     1003 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/stats/sql/tables.json
-drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.146323 NekoGram-2.2.0/src/NekoGram/widgets/stats/translations/
--rw-rw-rw-   0        0        0      223 2023-03-04 12:20:43.000000 NekoGram-2.2.0/src/NekoGram/widgets/stats/translations/en.json
--rw-rw-rw-   0        0        0     2540 2023-06-18 12:16:45.000000 NekoGram-2.2.0/src/NekoGram/widgets/stats/util.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:47:25.110903 NekoGram-2.2.0/src/NekoGram.egg-info/
--rw-rw-rw-   0        0        0    17999 2023-07-10 09:47:25.000000 NekoGram-2.2.0/src/NekoGram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2023-07-10 09:47:25.000000 NekoGram-2.2.0/src/NekoGram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 09:47:25.000000 NekoGram-2.2.0/src/NekoGram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-10 09:47:25.000000 NekoGram-2.2.0/src/NekoGram.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-10 09:47:25.000000 NekoGram-2.2.0/src/NekoGram.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 10:19:22.437000 NekoGram-2.2.1/
+-rw-rw-rw-   0        0        0     1086 2021-07-29 12:59:10.000000 NekoGram-2.2.1/LICENSE
+-rw-rw-rw-   0        0        0    17999 2023-07-10 10:19:22.435994 NekoGram-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    16128 2022-11-11 15:21:46.000000 NekoGram-2.2.1/README.md
+-rw-rw-rw-   0        0        0      987 2023-07-10 10:19:14.000000 NekoGram-2.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-10 10:19:22.437000 NekoGram-2.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-10 10:19:22.367538 NekoGram-2.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-10 10:19:22.381647 NekoGram-2.2.1/src/NekoGram/
+-rw-rw-rw-   0        0        0       78 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/__init__.py
+-rw-rw-rw-   0        0        0     6752 2023-07-10 09:39:14.000000 NekoGram-2.2.1/src/NekoGram/base_neko.py
+-rw-rw-rw-   0        0        0     8274 2023-06-18 12:16:45.000000 NekoGram-2.2.1/src/NekoGram/filters.py
+drwxrwxrwx   0        0        0        0 2023-07-10 10:19:22.400954 NekoGram-2.2.1/src/NekoGram/handlers/
+-rw-rw-rw-   0        0        0       92 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/handlers/__init__.py
+-rw-rw-rw-   0        0        0     1919 2023-06-18 11:48:30.000000 NekoGram-2.2.1/src/NekoGram/handlers/callback.py
+-rw-rw-rw-   0        0        0     5421 2023-06-18 11:48:30.000000 NekoGram-2.2.1/src/NekoGram/handlers/message.py
+-rw-rw-rw-   0        0        0       72 2023-06-18 12:16:45.000000 NekoGram-2.2.1/src/NekoGram/logger.py
+-rw-rw-rw-   0        0        0    11418 2023-06-18 12:16:45.000000 NekoGram-2.2.1/src/NekoGram/menus.py
+-rw-rw-rw-   0        0        0    16959 2023-07-10 09:39:14.000000 NekoGram-2.2.1/src/NekoGram/neko.py
+-rw-rw-rw-   0        0        0     4373 2023-06-18 12:16:45.000000 NekoGram-2.2.1/src/NekoGram/router.py
+drwxrwxrwx   0        0        0        0 2023-07-10 10:19:22.402608 NekoGram-2.2.1/src/NekoGram/storages/
+-rw-rw-rw-   0        0        0       39 2023-07-10 09:39:14.000000 NekoGram-2.2.1/src/NekoGram/storages/__init__.py
+-rw-rw-rw-   0        0        0     3460 2023-07-10 09:39:14.000000 NekoGram-2.2.1/src/NekoGram/storages/base_storage.py
+drwxrwxrwx   0        0        0        0 2023-07-10 10:19:22.405117 NekoGram-2.2.1/src/NekoGram/storages/mysql/
+-rw-rw-rw-   0        0        0       51 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/storages/mysql/__init__.py
+-rw-rw-rw-   0        0        0    16032 2023-07-10 09:39:14.000000 NekoGram-2.2.1/src/NekoGram/storages/mysql/mysql.py
+-rw-rw-rw-   0        0        0     1114 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/storages/mysql/tables.json
+drwxrwxrwx   0        0        0        0 2023-07-10 10:19:22.407272 NekoGram-2.2.1/src/NekoGram/storages/pg/
+-rw-rw-rw-   0        0        0       43 2023-07-10 09:39:14.000000 NekoGram-2.2.1/src/NekoGram/storages/pg/__init__.py
+-rw-rw-rw-   0        0        0    11705 2023-07-10 09:39:14.000000 NekoGram-2.2.1/src/NekoGram/storages/pg/pg.py
+-rw-rw-rw-   0        0        0      296 2023-07-10 09:39:14.000000 NekoGram-2.2.1/src/NekoGram/storages/pg/tables.sql
+drwxrwxrwx   0        0        0        0 2023-07-10 10:19:22.410378 NekoGram-2.2.1/src/NekoGram/storages/sqlite/
+-rw-rw-rw-   0        0        0       55 2023-07-10 09:39:14.000000 NekoGram-2.2.1/src/NekoGram/storages/sqlite/__init__.py
+-rw-rw-rw-   0        0        0    11324 2023-07-10 09:39:14.000000 NekoGram-2.2.1/src/NekoGram/storages/sqlite/sqlite.py
+-rw-rw-rw-   0        0        0      306 2023-07-10 09:39:14.000000 NekoGram-2.2.1/src/NekoGram/storages/sqlite/tables.sql
+drwxrwxrwx   0        0        0        0 2023-07-10 10:19:22.412383 NekoGram-2.2.1/src/NekoGram/text_processors/
+-rw-rw-rw-   0        0        0       84 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/text_processors/__init__.py
+-rw-rw-rw-   0        0        0      437 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/text_processors/base_processor.py
+-rw-rw-rw-   0        0        0     3183 2023-06-18 11:48:30.000000 NekoGram-2.2.1/src/NekoGram/text_processors/json_processor.py
+-rw-rw-rw-   0        0        0     2710 2023-06-18 12:16:45.000000 NekoGram-2.2.1/src/NekoGram/utils.py
+-rw-rw-rw-   0        0        0     1311 2023-06-18 12:16:45.000000 NekoGram-2.2.1/src/NekoGram/webhook.py
+drwxrwxrwx   0        0        0        0 2023-07-10 10:19:22.413385 NekoGram-2.2.1/src/NekoGram/widgets/
+-rw-rw-rw-   0        0        0       42 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 10:19:22.417895 NekoGram-2.2.1/src/NekoGram/widgets/broadcast/
+-rw-rw-rw-   0        0        0      128 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/widgets/broadcast/__init__.py
+-rw-rw-rw-   0        0        0     1923 2023-07-10 09:39:14.000000 NekoGram-2.2.1/src/NekoGram/widgets/broadcast/formatters.py
+-rw-rw-rw-   0        0        0     5410 2023-07-10 09:39:14.000000 NekoGram-2.2.1/src/NekoGram/widgets/broadcast/functions.py
+drwxrwxrwx   0        0        0        0 2023-07-10 10:19:22.420742 NekoGram-2.2.1/src/NekoGram/widgets/broadcast/translations/
+-rw-rw-rw-   0        0        0     2058 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/widgets/broadcast/translations/en.json
+-rw-rw-rw-   0        0        0     2134 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/widgets/broadcast/translations/pl.json
+-rw-rw-rw-   0        0        0     2390 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/widgets/broadcast/translations/ru.json
+-rw-rw-rw-   0        0        0     2380 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/widgets/broadcast/translations/uk.json
+-rw-rw-rw-   0        0        0       77 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/widgets/broadcast/util.py
+-rw-rw-rw-   0        0        0     1804 2023-06-18 12:16:45.000000 NekoGram-2.2.1/src/NekoGram/widgets/broadcast/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-10 10:19:22.426264 NekoGram-2.2.1/src/NekoGram/widgets/languages/
+-rw-rw-rw-   0        0        0      128 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/widgets/languages/__init__.py
+-rw-rw-rw-   0        0        0      648 2023-06-18 12:16:45.000000 NekoGram-2.2.1/src/NekoGram/widgets/languages/formatters.py
+-rw-rw-rw-   0        0        0      449 2023-06-18 12:16:45.000000 NekoGram-2.2.1/src/NekoGram/widgets/languages/functions.py
+-rw-rw-rw-   0        0        0       44 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/widgets/languages/replacements.json
+drwxrwxrwx   0        0        0        0 2023-07-10 10:19:22.430474 NekoGram-2.2.1/src/NekoGram/widgets/languages/translations/
+-rw-rw-rw-   0        0        0      262 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/widgets/languages/translations/en.json
+-rw-rw-rw-   0        0        0      272 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/widgets/languages/translations/he.json
+-rw-rw-rw-   0        0        0      260 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/widgets/languages/translations/pl.json
+-rw-rw-rw-   0        0        0      284 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/widgets/languages/translations/ru.json
+-rw-rw-rw-   0        0        0      280 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/widgets/languages/translations/uk.json
+-rw-rw-rw-   0        0        0      373 2023-06-18 12:16:45.000000 NekoGram-2.2.1/src/NekoGram/widgets/languages/util.py
+drwxrwxrwx   0        0        0        0 2023-07-10 10:19:22.433204 NekoGram-2.2.1/src/NekoGram/widgets/stats/
+-rw-rw-rw-   0        0        0      128 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/widgets/stats/__init__.py
+-rw-rw-rw-   0        0        0      905 2023-06-18 12:16:45.000000 NekoGram-2.2.1/src/NekoGram/widgets/stats/formatters.py
+-rw-rw-rw-   0        0        0       80 2023-06-18 12:16:45.000000 NekoGram-2.2.1/src/NekoGram/widgets/stats/functions.py
+drwxrwxrwx   0        0        0        0 2023-07-10 10:19:22.434209 NekoGram-2.2.1/src/NekoGram/widgets/stats/sql/
+-rw-rw-rw-   0        0        0     1003 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/widgets/stats/sql/tables.json
+drwxrwxrwx   0        0        0        0 2023-07-10 10:19:22.435209 NekoGram-2.2.1/src/NekoGram/widgets/stats/translations/
+-rw-rw-rw-   0        0        0      223 2023-03-04 12:20:43.000000 NekoGram-2.2.1/src/NekoGram/widgets/stats/translations/en.json
+-rw-rw-rw-   0        0        0     2540 2023-06-18 12:16:45.000000 NekoGram-2.2.1/src/NekoGram/widgets/stats/util.py
+drwxrwxrwx   0        0        0        0 2023-07-10 10:19:22.398831 NekoGram-2.2.1/src/NekoGram.egg-info/
+-rw-rw-rw-   0        0        0    17999 2023-07-10 10:19:22.000000 NekoGram-2.2.1/src/NekoGram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2248 2023-07-10 10:19:22.000000 NekoGram-2.2.1/src/NekoGram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 10:19:22.000000 NekoGram-2.2.1/src/NekoGram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-10 10:19:22.000000 NekoGram-2.2.1/src/NekoGram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-10 10:19:22.000000 NekoGram-2.2.1/src/NekoGram.egg-info/top_level.txt
```

### Comparing `NekoGram-2.2.0/LICENSE` & `NekoGram-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/PKG-INFO` & `NekoGram-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NekoGram
-Version: 2.2.0
+Version: 2.2.1
 Summary: Creating bots has never been simpler.
 Author-email: lyteloli <me@lyteloli.space>
 License: MIT License
         
         Copyright (c) 2020 lyteloli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `NekoGram-2.2.0/README.md` & `NekoGram-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/pyproject.toml` & `NekoGram-2.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NekoGram"
-version = "2.2.0"
+version = "2.2.1"
 authors = [
   { name="lyteloli", email="me@lyteloli.space" },
 ]
 description = "Creating bots has never been simpler."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
@@ -20,13 +20,13 @@
     "Topic :: Software Development"
 ]
 dependencies = [
     "aiogram~=2.23.1",
     "importlib-resources~=5.10.0"
 ]
 [tool.setuptools.package-data]
-NekoGram = ["storages/mysql/tables.json", "widgets/languages/replacements.json", "widgets/*/translations/*.json",
+NekoGram = ["storages/*/tables.json", "storages/*/tables.sql", "widgets/languages/replacements.json", "widgets/*/translations/*.json",
     "widgets/*/sql/tables.json"]
 
 [project.urls]
 "Homepage" = "https://github.com/lyteloli/NekoGram"
 "Bug Tracker" = "https://github.com/lyteloli/NekoGram/issues"
```

### Comparing `NekoGram-2.2.0/src/NekoGram/base_neko.py` & `NekoGram-2.2.1/src/NekoGram/base_neko.py`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/filters.py` & `NekoGram-2.2.1/src/NekoGram/filters.py`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/handlers/callback.py` & `NekoGram-2.2.1/src/NekoGram/handlers/callback.py`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/handlers/message.py` & `NekoGram-2.2.1/src/NekoGram/handlers/message.py`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/menus.py` & `NekoGram-2.2.1/src/NekoGram/menus.py`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/neko.py` & `NekoGram-2.2.1/src/NekoGram/neko.py`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/router.py` & `NekoGram-2.2.1/src/NekoGram/router.py`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/storages/base_storage.py` & `NekoGram-2.2.1/src/NekoGram/storages/base_storage.py`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/storages/mysql/mysql.py` & `NekoGram-2.2.1/src/NekoGram/storages/mysql/mysql.py`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/storages/mysql/tables.json` & `NekoGram-2.2.1/src/NekoGram/storages/mysql/tables.json`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/storages/pg/pg.py` & `NekoGram-2.2.1/src/NekoGram/storages/pg/pg.py`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/storages/sqlite/sqlite.py` & `NekoGram-2.2.1/src/NekoGram/storages/sqlite/sqlite.py`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/text_processors/json_processor.py` & `NekoGram-2.2.1/src/NekoGram/text_processors/json_processor.py`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/utils.py` & `NekoGram-2.2.1/src/NekoGram/utils.py`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/webhook.py` & `NekoGram-2.2.1/src/NekoGram/webhook.py`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/widgets/broadcast/formatters.py` & `NekoGram-2.2.1/src/NekoGram/widgets/broadcast/formatters.py`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/widgets/broadcast/functions.py` & `NekoGram-2.2.1/src/NekoGram/widgets/broadcast/functions.py`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/widgets/broadcast/translations/en.json` & `NekoGram-2.2.1/src/NekoGram/widgets/broadcast/translations/en.json`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/widgets/broadcast/translations/pl.json` & `NekoGram-2.2.1/src/NekoGram/widgets/broadcast/translations/pl.json`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/widgets/broadcast/translations/ru.json` & `NekoGram-2.2.1/src/NekoGram/widgets/broadcast/translations/ru.json`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/widgets/broadcast/translations/uk.json` & `NekoGram-2.2.1/src/NekoGram/widgets/broadcast/translations/uk.json`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/widgets/broadcast/utils.py` & `NekoGram-2.2.1/src/NekoGram/widgets/broadcast/utils.py`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/widgets/languages/formatters.py` & `NekoGram-2.2.1/src/NekoGram/widgets/languages/formatters.py`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/widgets/stats/formatters.py` & `NekoGram-2.2.1/src/NekoGram/widgets/stats/formatters.py`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/widgets/stats/sql/tables.json` & `NekoGram-2.2.1/src/NekoGram/widgets/stats/sql/tables.json`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram/widgets/stats/util.py` & `NekoGram-2.2.1/src/NekoGram/widgets/stats/util.py`

 * *Files identical despite different names*

### Comparing `NekoGram-2.2.0/src/NekoGram.egg-info/PKG-INFO` & `NekoGram-2.2.1/src/NekoGram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NekoGram
-Version: 2.2.0
+Version: 2.2.1
 Summary: Creating bots has never been simpler.
 Author-email: lyteloli <me@lyteloli.space>
 License: MIT License
         
         Copyright (c) 2020 lyteloli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `NekoGram-2.2.0/src/NekoGram.egg-info/SOURCES.txt` & `NekoGram-2.2.1/src/NekoGram.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,18 @@
 src/NekoGram/storages/__init__.py
 src/NekoGram/storages/base_storage.py
 src/NekoGram/storages/mysql/__init__.py
 src/NekoGram/storages/mysql/mysql.py
 src/NekoGram/storages/mysql/tables.json
 src/NekoGram/storages/pg/__init__.py
 src/NekoGram/storages/pg/pg.py
+src/NekoGram/storages/pg/tables.sql
 src/NekoGram/storages/sqlite/__init__.py
 src/NekoGram/storages/sqlite/sqlite.py
+src/NekoGram/storages/sqlite/tables.sql
 src/NekoGram/text_processors/__init__.py
 src/NekoGram/text_processors/base_processor.py
 src/NekoGram/text_processors/json_processor.py
 src/NekoGram/widgets/__init__.py
 src/NekoGram/widgets/broadcast/__init__.py
 src/NekoGram/widgets/broadcast/formatters.py
 src/NekoGram/widgets/broadcast/functions.py
```

